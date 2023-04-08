# Comparing `tmp/IreneAPIWrapper-2.3.6.tar.gz` & `tmp/IreneAPIWrapper-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IreneAPIWrapper-2.3.6.tar", last modified: Fri Apr  7 22:44:41 2023, max compression
+gzip compressed data, was "IreneAPIWrapper-2.3.7.tar", last modified: Sat Apr  8 22:53:08 2023, max compression
```

## Comparing `IreneAPIWrapper-2.3.6.tar` & `IreneAPIWrapper-2.3.7.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.612279 IreneAPIWrapper-2.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.600279 IreneAPIWrapper-2.3.6/IreneAPIWrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.608279 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/affiliation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/automedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.608279 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/abstractmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/mediasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/biasgame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/bloodtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/company.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/difficulty.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/eightball.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/fandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/groupalias.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/guessinggame.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/personalias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/preloadcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/reactionrolemessages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/reminder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/social.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/statsupdater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tiktokaccount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tweet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/twitchaccount.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/twitteraccount.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/unscramblegame.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/urban.py
--rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/userstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/wolfram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.608279 IreneAPIWrapper-2.3.6/IreneAPIWrapper/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/sections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.600279 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 22:44:41.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-07 22:44:41.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:44:41.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-07 22:44:41.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-07 22:44:41.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 22:44:41.612279 IreneAPIWrapper-2.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 22:44:41.612279 IreneAPIWrapper-2.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:08.016209 IreneAPIWrapper-2.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:08.008210 IreneAPIWrapper-2.3.7/IreneAPIWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:08.016209 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/affiliation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/automedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/banphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:08.016209 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/abstractmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/mediasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/biasgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/bloodtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/difficulty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/eightball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/fandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/groupalias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/guessinggame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/personalias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/preloadcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/reactionrolemessages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/reminder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/social.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/statsupdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/tiktokaccount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/tweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/twitchaccount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/twitteraccount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/unscramblegame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/urban.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/userstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/wolfram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:08.016209 IreneAPIWrapper-2.3.7/IreneAPIWrapper/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper/sections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:08.008210 IreneAPIWrapper-2.3.7/IreneAPIWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-08 22:53:07.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-08 22:53:07.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 22:53:07.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-08 22:53:07.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-08 22:53:07.000000 IreneAPIWrapper-2.3.7/IreneAPIWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-08 22:53:08.016209 IreneAPIWrapper-2.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 22:53:08.016209 IreneAPIWrapper-2.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-08 22:52:53.000000 IreneAPIWrapper-2.3.7/setup.py
```

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/exceptions.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/__init__.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from .location import Location
 from .bloodtype import BloodType
 from .automedia import AutoMedia, AffiliationTime
 from .position import Position
 from .social import Social
 from .display import Display
 from .fandom import Fandom
+from .banphrase import BanPhrase
 from .notification import Notification
 from .name import Name
 from .group import Group
 from .person import Person
 from .affiliation import Affiliation
 from .media import Media
 from .user import User
```

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/affiliation.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/affiliation.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/automedia.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/automedia.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/abstractmodel.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/abstractmodel.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/alias.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/alias.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/mediasource.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/mediasource.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/receiver.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/base/receiver.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/biasgame.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/biasgame.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/bloodtype.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/bloodtype.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/callback.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/callback.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/channel.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/channel.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/client.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/client.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/company.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/company.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/date.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/date.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/difficulty.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/difficulty.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/display.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/display.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/eightball.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/eightball.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/fandom.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/fandom.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/group.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/group.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/groupalias.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/groupalias.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/guessinggame.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/guessinggame.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/guild.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/guild.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/interactions.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/interactions.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/language.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/language.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/location.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/location.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/media.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/media.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/name.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/name.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/notification.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/notification.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/person.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/person.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/personalias.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/personalias.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/position.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/position.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/preloadcache.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/preloadcache.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,24 +68,26 @@
         Whether to preload all auto media (Defaults to True)
     reaction_role_messages: bool
         Whether to preload all reaction role messages (Defaults to True)
     """
     tags = person_aliases = group_aliases = persons = groups = twitter_accounts = \
         affiliations = bloodtypes = media = displays = companies = dates = locations = \
         positions = socials = fandoms = languages = eight_ball_responses = notifications = interactions = names = \
-        auto_media = reminders = reaction_role_messages = True
-    users = guilds = channels = twitch_subscriptions = twitter_subscriptions = tiktok_subscriptions = False
+        auto_media = reminders = reaction_role_messages = banned_phrases = True
+    users = guilds = channels = twitch_subscriptions = twitter_subscriptions = \
+        tiktok_subscriptions = False
 
     force: bool = True
 
     def get_evaluation(self):
         from . import (
             Tag, PersonAlias, GroupAlias, Affiliation, BloodType, Media, Display, Company, Date, Location, Position,
             Social, Person, User, Channel, Group, Fandom, Guild, TwitchAccount, TwitterAccount, Language,
-            EightBallResponse, Notification, Interaction, Name, AutoMedia, Reminder, ReactionRoleMessage, TikTokAccount
+            EightBallResponse, Notification, Interaction, Name, AutoMedia, Reminder, ReactionRoleMessage, TikTokAccount,
+            BanPhrase
         )
 
         eval_dict = {
             Tag: self.tags,
             PersonAlias: self.person_aliases,
             GroupAlias: self.group_aliases,
             Affiliation: self.affiliations,
@@ -109,20 +111,21 @@
             EightBallResponse: self.eight_ball_responses,
             Notification: self.notifications,
             Interaction: self.interactions,
             Name: self.names,
             AutoMedia: self.auto_media,
             Reminder: self.reminders,
             ReactionRoleMessage: self.reaction_role_messages,
-            TikTokAccount: self.tiktok_subscriptions
+            TikTokAccount: self.tiktok_subscriptions,
+            BanPhrase: self.banned_phrases
         }
 
         eval_dict_only_true = {key: val for key, val in eval_dict.items() if key}
         return eval_dict_only_true
 
     def all_false(self):
         self.tags = self.person_aliases = self.group_aliases = self.persons = self.groups = self.twitter_accounts = \
             self.users = self.guilds = self.affiliations = self.bloodtypes = self.media = self.displays = \
             self.companies = self.dates = self.locations = self.positions = self.socials = self.fandoms = \
             self.channels = self.twitch_subscriptions = self.twitter_subscriptions = self.languages = \
             self.eight_ball_responses = self.notifications = self.interactions = self.names = self.auto_media = \
-            self.reminders = self.reaction_role_messages = self.tiktok_subscriptions = False
+            self.reminders = self.reaction_role_messages = self.tiktok_subscriptions = self.banned_phrases = False
```

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/reactionrolemessages.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/reactionrolemessages.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/reminder.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/reminder.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/social.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/social.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/subscription.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/subscription.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tag.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/tag.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tiktokaccount.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/tiktokaccount.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/timeline.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/timeline.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tweet.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/tweet.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/twitchaccount.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/twitchaccount.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/twitteraccount.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/twitteraccount.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/unscramblegame.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/unscramblegame.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/user.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/user.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/userstatus.py` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper/models/userstatus.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/PKG-INFO` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IreneAPIWrapper
-Version: 2.3.6
+Version: 2.3.7
 Summary: A wrapper for Irene's API and connects with a websocket connection.
 Home-page: https://github.com/MujyKun/IreneAPIWrapper
 Author: MujyKun
 Author-email: mujy@irenebot.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/SOURCES.txt` & `IreneAPIWrapper-2.3.7/IreneAPIWrapper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 IreneAPIWrapper.egg-info/dependency_links.txt
 IreneAPIWrapper.egg-info/requires.txt
 IreneAPIWrapper.egg-info/top_level.txt
 IreneAPIWrapper/models/__init__.py
 IreneAPIWrapper/models/access.py
 IreneAPIWrapper/models/affiliation.py
 IreneAPIWrapper/models/automedia.py
+IreneAPIWrapper/models/banphrase.py
 IreneAPIWrapper/models/biasgame.py
 IreneAPIWrapper/models/bloodtype.py
 IreneAPIWrapper/models/callback.py
 IreneAPIWrapper/models/channel.py
 IreneAPIWrapper/models/client.py
 IreneAPIWrapper/models/company.py
 IreneAPIWrapper/models/date.py
```

### Comparing `IreneAPIWrapper-2.3.6/PKG-INFO` & `IreneAPIWrapper-2.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IreneAPIWrapper
-Version: 2.3.6
+Version: 2.3.7
 Summary: A wrapper for Irene's API and connects with a websocket connection.
 Home-page: https://github.com/MujyKun/IreneAPIWrapper
 Author: MujyKun
 Author-email: mujy@irenebot.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IreneAPIWrapper-2.3.6/pyproject.toml` & `IreneAPIWrapper-2.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "IreneAPIWrapper"
-version = "2.3.6"
+version = "2.3.7"
 description = "The Wrapper for the Websocket and REST API of Irene."
 authors = ["MujyKun <mujy@irenebot.com>"]
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
 ]
```

### Comparing `IreneAPIWrapper-2.3.6/setup.py` & `IreneAPIWrapper-2.3.7/setup.py`

 * *Files identical despite different names*

