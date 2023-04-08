# Comparing `tmp/nonebot-plugin-SDGPT-0.0.3.tar.gz` & `tmp/nonebot-plugin-SDGPT-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-SDGPT-0.0.3.tar", last modified: Sat Apr  8 21:06:19 2023, max compression
+gzip compressed data, was "nonebot-plugin-SDGPT-0.0.4.tar", last modified: Sat Apr  8 22:22:07 2023, max compression
```

## Comparing `nonebot-plugin-SDGPT-0.0.3.tar` & `nonebot-plugin-SDGPT-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 21:06:19.928209 nonebot-plugin-SDGPT-0.0.3/
--rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      137 2023-04-08 21:06:19.910193 nonebot-plugin-SDGPT-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-04-08 20:35:51.000000 nonebot-plugin-SDGPT-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 21:06:19.900183 nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT/
--rw-rw-rw-   0        0        0     3522 2023-04-08 19:41:45.000000 nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT/__init__.py
--rw-rw-rw-   0        0        0     8905 2023-04-08 20:30:32.000000 nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT/bot.py
-drwxrwxrwx   0        0        0        0 2023-04-08 21:06:19.909192 nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT.egg-info/
--rw-rw-rw-   0        0        0      137 2023-04-08 21:06:19.000000 nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-04-08 21:06:19.000000 nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 21:06:19.000000 nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-08 21:06:19.000000 nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-08 21:06:19.000000 nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      244 2023-04-08 21:06:04.000000 nonebot-plugin-SDGPT-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 21:06:19.928209 nonebot-plugin-SDGPT-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-08 22:22:07.836964 nonebot-plugin-SDGPT-0.0.4/
+-rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      137 2023-04-08 22:22:07.835963 nonebot-plugin-SDGPT-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-04-08 20:35:51.000000 nonebot-plugin-SDGPT-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 22:22:07.825954 nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT/
+-rw-rw-rw-   0        0        0     3522 2023-04-08 19:41:45.000000 nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT/__init__.py
+-rw-rw-rw-   0        0        0     8905 2023-04-08 20:30:32.000000 nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT/bot.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:22:07.834961 nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT.egg-info/
+-rw-rw-rw-   0        0        0      137 2023-04-08 22:22:07.000000 nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-08 22:22:07.000000 nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 22:22:07.000000 nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-04-08 22:22:07.000000 nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-08 22:22:07.000000 nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      301 2023-04-08 22:10:31.000000 nonebot-plugin-SDGPT-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-08 22:22:07.836964 nonebot-plugin-SDGPT-0.0.4/setup.cfg
```

### Comparing `nonebot-plugin-SDGPT-0.0.3/LICENSE` & `nonebot-plugin-SDGPT-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT/__init__.py` & `nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.0.3/nonebot_plugin_SDGPT/bot.py` & `nonebot-plugin-SDGPT-0.0.4/nonebot_plugin_SDGPT/bot.py`

 * *Files identical despite different names*

