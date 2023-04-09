# Comparing `tmp/tg_odesli_bot-0.3.0.tar.gz` & `tmp/tg_odesli_bot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_odesli_bot-0.3.0.tar", max compression
+gzip compressed data, was "tg_odesli_bot-0.3.1.tar", max compression
```

## Comparing `tg_odesli_bot-0.3.0.tar` & `tg_odesli_bot-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-03-04 20:28:34.213856 tg_odesli_bot-0.3.0/LICENSE
--rw-r--r--   0        0        0     5791 2023-03-04 20:28:34.213856 tg_odesli_bot-0.3.0/README.md
--rw-r--r--   0        0        0     2264 2023-03-04 20:28:34.213856 tg_odesli_bot-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       27 2023-03-04 20:28:34.213856 tg_odesli_bot-0.3.0/tg_odesli_bot/__init__.py
--rw-r--r--   0        0        0    30288 2023-03-04 20:28:34.213856 tg_odesli_bot-0.3.0/tg_odesli_bot/bot.py
--rw-r--r--   0        0        0     3231 2023-03-04 20:28:34.213856 tg_odesli_bot-0.3.0/tg_odesli_bot/platforms.py
--rw-r--r--   0        0        0     1229 2023-03-04 20:28:34.213856 tg_odesli_bot-0.3.0/tg_odesli_bot/schemas.py
--rw-r--r--   0        0        0     4680 2023-03-04 20:28:34.213856 tg_odesli_bot-0.3.0/tg_odesli_bot/settings.py
--rw-r--r--   0        0        0     6886 1970-01-01 00:00:00.000000 tg_odesli_bot-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 19:52:37.287616 tg_odesli_bot-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5791 2023-04-09 19:52:37.287616 tg_odesli_bot-0.3.1/README.md
+-rw-r--r--   0        0        0     2290 2023-04-09 19:52:37.287616 tg_odesli_bot-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-04-09 19:52:37.287616 tg_odesli_bot-0.3.1/tg_odesli_bot/__init__.py
+-rw-r--r--   0        0        0    30288 2023-04-09 19:52:37.287616 tg_odesli_bot-0.3.1/tg_odesli_bot/bot.py
+-rw-r--r--   0        0        0     3266 2023-04-09 19:52:37.287616 tg_odesli_bot-0.3.1/tg_odesli_bot/platforms.py
+-rw-r--r--   0        0        0     1229 2023-04-09 19:52:37.287616 tg_odesli_bot-0.3.1/tg_odesli_bot/schemas.py
+-rw-r--r--   0        0        0     4680 2023-04-09 19:52:37.287616 tg_odesli_bot-0.3.1/tg_odesli_bot/settings.py
+-rw-r--r--   0        0        0     6886 1970-01-01 00:00:00.000000 tg_odesli_bot-0.3.1/PKG-INFO
```

### Comparing `tg_odesli_bot-0.3.0/LICENSE` & `tg_odesli_bot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tg_odesli_bot-0.3.0/README.md` & `tg_odesli_bot-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tg_odesli_bot-0.3.0/pyproject.toml` & `tg_odesli_bot-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tg_odesli_bot"
-version = "0.3.0"
+version = "0.3.1"
 description = "Telegram Bot to share music with Odesli (former Songlink) service."
 repository = "https://github.com/9dogs/tg-odesli-bot"
 homepage = "https://github.com/9dogs/tg-odesli-bot"
 authors = ["Mikhail Knyazev <hellishbot@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
@@ -32,14 +32,15 @@
 ignore_missing_imports = true
 show_error_codes = true
 warn_unused_configs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 no_implicit_optional = true
 strict_equality = true
+plugins = "pydantic.mypy"
 
 [tool.coverage.run]
 branch = true
 
 [tool.pydocstyle]
 # D202: No blank lines allowed after function docstring
 # D203: 1 blank line required before class docstring
@@ -53,15 +54,15 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.12"
 aiocache = "^0.12.0"
 aiogram = "^2.0"
 marshmallow = "^3.17.0"
 python-dotenv = "^1.0.0"
 sentry-sdk = "^1.0.0"
-structlog = "^22.1.0"
+structlog = "^23.1.0"
 structlog-sentry = "^2.0.0"
 aiohttp = "^3.8.0"
 ujson = "^5.4.0"
 spotipy = "^2.22.1"
 pydantic = "^1.10.5"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `tg_odesli_bot-0.3.0/tg_odesli_bot/bot.py` & `tg_odesli_bot-0.3.1/tg_odesli_bot/bot.py`

 * *Files identical despite different names*

### Comparing `tg_odesli_bot-0.3.0/tg_odesli_bot/platforms.py` & `tg_odesli_bot-0.3.1/tg_odesli_bot/platforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,16 @@
 
 class SpotifyPlatform(PlatformABC):
     """Spotify platform."""
 
     key = 'spotify'
     url_re = (
         r'https?://([a-zA-Z\d-]+\.)*((spotify\.com/(album|track)/[^\s.,]*)'
-        r'|(tospotify\.com/[^\s.,]*))'
+        r'|(tospotify\.com/[^\s.,]*)'
+        r'|(spotify\.link/[^\s]*))'
     )
     name = 'Spotify'
     order = 3
 
 
 class YouTubeMusicPlatform(PlatformABC):
     """YouTube Music platform."""
```

### Comparing `tg_odesli_bot-0.3.0/tg_odesli_bot/schemas.py` & `tg_odesli_bot-0.3.1/tg_odesli_bot/schemas.py`

 * *Files identical despite different names*

### Comparing `tg_odesli_bot-0.3.0/tg_odesli_bot/settings.py` & `tg_odesli_bot-0.3.1/tg_odesli_bot/settings.py`

 * *Files identical despite different names*

### Comparing `tg_odesli_bot-0.3.0/PKG-INFO` & `tg_odesli_bot-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-odesli-bot
-Version: 0.3.0
+Version: 0.3.1
 Summary: Telegram Bot to share music with Odesli (former Songlink) service.
 Home-page: https://github.com/9dogs/tg-odesli-bot
 License: GPL-3.0-only
 Author: Mikhail Knyazev
 Author-email: hellishbot@gmail.com
 Requires-Python: >=3.10,<=3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,15 @@
 Requires-Dist: aiogram (>=2.0,<3.0)
 Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
 Requires-Dist: marshmallow (>=3.17.0,<4.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: sentry-sdk (>=1.0.0,<2.0.0)
 Requires-Dist: spotipy (>=2.22.1,<3.0.0)
-Requires-Dist: structlog (>=22.1.0,<23.0.0)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Requires-Dist: structlog-sentry (>=2.0.0,<3.0.0)
 Requires-Dist: ujson (>=5.4.0,<6.0.0)
 Project-URL: Repository, https://github.com/9dogs/tg-odesli-bot
 Description-Content-Type: text/markdown
 
 # Telegram Odesli Bot
```

