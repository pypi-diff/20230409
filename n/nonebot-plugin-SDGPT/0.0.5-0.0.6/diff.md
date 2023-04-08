# Comparing `tmp/nonebot-plugin-SDGPT-0.0.5.tar.gz` & `tmp/nonebot-plugin-SDGPT-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-SDGPT-0.0.5.tar", last modified: Sat Apr  8 22:31:31 2023, max compression
+gzip compressed data, was "nonebot-plugin-SDGPT-0.0.6.tar", last modified: Sat Apr  8 22:36:45 2023, max compression
```

## Comparing `nonebot-plugin-SDGPT-0.0.5.tar` & `nonebot-plugin-SDGPT-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 22:31:31.096123 nonebot-plugin-SDGPT-0.0.5/
--rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      137 2023-04-08 22:31:31.095122 nonebot-plugin-SDGPT-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-04-08 20:35:51.000000 nonebot-plugin-SDGPT-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 22:31:31.070701 nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT/
--rw-rw-rw-   0        0        0     3522 2023-04-08 19:41:45.000000 nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT/__init__.py
--rw-rw-rw-   0        0        0     8905 2023-04-08 20:30:32.000000 nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT/bot.py
-drwxrwxrwx   0        0        0        0 2023-04-08 22:31:31.093120 nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT.egg-info/
--rw-rw-rw-   0        0        0      137 2023-04-08 22:31:31.000000 nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-04-08 22:31:31.000000 nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 22:31:31.000000 nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2023-04-08 22:31:31.000000 nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-08 22:31:31.000000 nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      368 2023-04-08 22:31:02.000000 nonebot-plugin-SDGPT-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 22:31:31.096123 nonebot-plugin-SDGPT-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-08 22:36:45.160014 nonebot-plugin-SDGPT-0.0.6/
+-rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      137 2023-04-08 22:36:45.160014 nonebot-plugin-SDGPT-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-04-08 20:35:51.000000 nonebot-plugin-SDGPT-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 22:36:45.148004 nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT/
+-rw-rw-rw-   0        0        0     3522 2023-04-08 19:41:45.000000 nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT/__init__.py
+-rw-rw-rw-   0        0        0     8905 2023-04-08 20:30:32.000000 nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT/bot.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:36:45.158013 nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT.egg-info/
+-rw-rw-rw-   0        0        0      137 2023-04-08 22:36:45.000000 nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-08 22:36:45.000000 nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 22:36:45.000000 nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-04-08 22:36:45.000000 nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-08 22:36:45.000000 nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      336 2023-04-08 22:36:24.000000 nonebot-plugin-SDGPT-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-08 22:36:45.160014 nonebot-plugin-SDGPT-0.0.6/setup.cfg
```

### Comparing `nonebot-plugin-SDGPT-0.0.5/LICENSE` & `nonebot-plugin-SDGPT-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT/__init__.py` & `nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.0.5/nonebot_plugin_SDGPT/bot.py` & `nonebot-plugin-SDGPT-0.0.6/nonebot_plugin_SDGPT/bot.py`

 * *Files identical despite different names*

