# Comparing `tmp/rtd-bin-server-1.3.0.tar.gz` & `tmp/rtd-bin-server-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtd-bin-server-1.3.0.tar", last modified: Fri Nov 19 16:47:41 2021, max compression
+gzip compressed data, was "rtd-bin-server-1.4.0.tar", last modified: Sun Apr  9 11:05:26 2023, max compression
```

## Comparing `rtd-bin-server-1.3.0.tar` & `rtd-bin-server-1.4.0.tar`

### file list

```diff
@@ -1,41 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 16:47:41.731680 rtd-bin-server-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5577 2021-11-19 16:47:41.731680 rtd-bin-server-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4275 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 16:47:41.727680 rtd-bin-server-1.3.0/bin/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 16:47:41.727680 rtd-bin-server-1.3.0/bin/assets/
--rw-r--r--   0 runner    (1001) docker     (121)    16958 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 16:47:41.731680 rtd-bin-server-1.3.0/bin/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/assets/scripts/loc.js
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/assets/scripts/newform.js
--rw-r--r--   0 runner    (1001) docker     (121)      431 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/assets/scripts/report.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 16:47:41.731680 rtd-bin-server-1.3.0/bin/assets/styles/
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/assets/styles/monokai.css
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/assets/styles/report.css
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/assets/styles/style.css
--rw-r--r--   0 runner    (1001) docker     (121)     3635 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8607 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     2600 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/highlight.py
--rw-r--r--   0 runner    (1001) docker     (121)     3344 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 16:47:41.731680 rtd-bin-server-1.3.0/bin/views/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/views/blank.html
--rw-r--r--   0 runner    (1001) docker     (121)      570 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/views/head.html
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/views/highlight.html
--rw-r--r--   0 runner    (1001) docker     (121)      251 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/views/howto.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/bin/views/newform.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 16:47:41.731680 rtd-bin-server-1.3.0/rtd_bin_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5577 2021-11-19 16:47:41.000000 rtd-bin-server-1.3.0/rtd_bin_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      715 2021-11-19 16:47:41.000000 rtd-bin-server-1.3.0/rtd_bin_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-19 16:47:41.000000 rtd-bin-server-1.3.0/rtd_bin_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-11-19 16:47:41.000000 rtd-bin-server-1.3.0/rtd_bin_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-11-19 16:47:41.000000 rtd-bin-server-1.3.0/rtd_bin_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      857 2021-11-19 16:47:41.731680 rtd-bin-server-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 16:47:41.731680 rtd-bin-server-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9354 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/tests/test_highlight.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-19 16:47:37.000000 rtd-bin-server-1.3.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:05:26.782057 rtd-bin-server-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-04-09 11:05:26.782057 rtd-bin-server-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:05:26.774057 rtd-bin-server-1.4.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:05:26.774057 rtd-bin-server-1.4.0/bin/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:05:26.778057 rtd-bin-server-1.4.0/bin/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/icons/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/icons/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/icons/history.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/icons/new.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/icons/report.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:05:26.778057 rtd-bin-server-1.4.0/bin/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/scripts/change-lang.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/scripts/loc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/scripts/newform.js
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/scripts/report.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:05:26.778057 rtd-bin-server-1.4.0/bin/assets/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/styles/monokai.css
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/styles/report.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/assets/styles/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:05:26.778057 rtd-bin-server-1.4.0/bin/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/views/blank.html
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/views/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/views/highlight.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/views/howto.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/views/newform.html
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/bin/views/svg.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:05:26.782057 rtd-bin-server-1.4.0/rtd_bin_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-04-09 11:05:26.000000 rtd-bin-server-1.4.0/rtd_bin_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-09 11:05:26.000000 rtd-bin-server-1.4.0/rtd_bin_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:05:26.000000 rtd-bin-server-1.4.0/rtd_bin_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 11:05:26.000000 rtd-bin-server-1.4.0/rtd_bin_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-09 11:05:26.000000 rtd-bin-server-1.4.0/rtd_bin_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-09 11:05:26.782057 rtd-bin-server-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:05:26.782057 rtd-bin-server-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/tests/fake_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/tests/html_sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/tests/test_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 11:05:17.000000 rtd-bin-server-1.4.0/version.txt
```

### Comparing `rtd-bin-server-1.3.0/LICENSE` & `rtd-bin-server-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtd-bin-server-1.3.0/PKG-INFO` & `rtd-bin-server-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtd-bin-server
-Version: 1.3.0
+Version: 1.4.0
 Summary: A pastebin for Read The Docs discord community
 Home-page: https://github.com/readthedocs-fr/bin-server
 Author: Read The Docs
 Author-email: opensource@readthedocs.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/readthedocs-fr/bin-server/issues
 Project-URL: Documentation, https://rtd-bin-server.readthedocs.io/en/latest/
@@ -39,14 +39,16 @@
             RTDBIN_MAXSIZE=16kiB
             RTDBIN_DEFAULT_LANGUAGE=text
             RTDBIN_DEFAULT_MAXUSAGE=0
             RTDBIN_DEFAULT_LIFETIME=0
             REDIS_HOST=localhost
             REDIS_PORT=6379
             REDIS_DB=0
+            REDIS_PASSWORD=
+            REDIS_USERNAME=
         
         Par défaut, le service utilise le serveur web `wsgiref` disponible dans la bibliothèque standard de Python pour traiter les requêtes. Ce serveur est propice dans un environnement de développement ou lorsque le volume d'utilisateur est réduit. Pour de meilleures performances, [un serveur tiers compatible wsgi](https://wsgi.readthedocs.io/en/latest/servers.html) peut être utilisé à la place.
         
         	$ pip install gunicorn
         	$ gunicorn bin:app
         
         Des fichiers de configuration d'exemples pour `nginx`, `systemd` et `gunicorn` sont disponibles dans le [wiki](https://github.com/readthedocs-fr/bin/wiki/systemd-nginx-gunicorn).
```

### Comparing `rtd-bin-server-1.3.0/README.md` & `rtd-bin-server-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     RTDBIN_MAXSIZE=16kiB
     RTDBIN_DEFAULT_LANGUAGE=text
     RTDBIN_DEFAULT_MAXUSAGE=0
     RTDBIN_DEFAULT_LIFETIME=0
     REDIS_HOST=localhost
     REDIS_PORT=6379
     REDIS_DB=0
+    REDIS_PASSWORD=
+    REDIS_USERNAME=
 
 Par défaut, le service utilise le serveur web `wsgiref` disponible dans la bibliothèque standard de Python pour traiter les requêtes. Ce serveur est propice dans un environnement de développement ou lorsque le volume d'utilisateur est réduit. Pour de meilleures performances, [un serveur tiers compatible wsgi](https://wsgi.readthedocs.io/en/latest/servers.html) peut être utilisé à la place.
 
 	$ pip install gunicorn
 	$ gunicorn bin:app
 
 Des fichiers de configuration d'exemples pour `nginx`, `systemd` et `gunicorn` sont disponibles dans le [wiki](https://github.com/readthedocs-fr/bin/wiki/systemd-nginx-gunicorn).
```

### Comparing `rtd-bin-server-1.3.0/bin/assets/favicon.ico` & `rtd-bin-server-1.4.0/bin/assets/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `rtd-bin-server-1.3.0/bin/assets/scripts/loc.js` & `rtd-bin-server-1.4.0/bin/assets/scripts/loc.js`

 * *Files identical despite different names*

### Comparing `rtd-bin-server-1.3.0/bin/assets/scripts/newform.js` & `rtd-bin-server-1.4.0/bin/assets/scripts/newform.js`

 * *Files identical despite different names*

### Comparing `rtd-bin-server-1.3.0/bin/assets/styles/monokai.css` & `rtd-bin-server-1.4.0/bin/assets/styles/monokai.css`

 * *Files identical despite different names*

### Comparing `rtd-bin-server-1.3.0/bin/assets/styles/style.css` & `rtd-bin-server-1.4.0/bin/assets/styles/style.css`

 * *Files identical despite different names*

### Comparing `rtd-bin-server-1.3.0/bin/config.py` & `rtd-bin-server-1.4.0/bin/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,40 +16,50 @@
 * ``RTDBIN_IDENTSIZE``: The length of generated unique identifier for new snippets (default: 6)
 * ``RTDBIN_DEFAULT_LANGUAGE``: The default language selected in the new snippet form
 * ``RTDBIN_DEFAULT_MAXUSAGE``: The default maximum usages before a snippet is automatically removed, 0 means no maximum (default: 0)
 * ``RTDBIN_DEFAULT_LIFETIME``: The default time before a snippet is automatically removed, 0 means no limit (default: 0)
 * ``REDIS_HOST``: The Redis host adress to connect to
 * ``REDIS_PORT``: The Redis port to connect to
 * ``REDIS_DB``: The Redis database to connect to
+* ``REDIS_PASSWORD``: The password of the Redis database to connect to
+* ``REDIS_USERNAME``: The username of the Redis database to connect to
 """
 
 
 import logging
 import os
 from argparse import ArgumentParser
 from dotenv import load_dotenv
 from metrics import Byte, Time
+from pprint import pformat
 
 
 logger = logging.getLogger(__name__)
 bin_logger = logging.getLogger(__package__)
 
 
 def strtobool(s):
     try:
         s = s.lower()
     except AttributeError:
         pass
     return s not in {False, "0", "false", "no"}
 
 
+def asdict():
+    return {
+        key: value for key, value in globals().items()
+        if key.isupper() and not key.startswith('__')
+    }
+
+
 def _setup():
     global HOST, PORT, MAXSIZE, IDENTSIZE
     global DEFAULT_LANGUAGE, DEFAULT_MAXUSAGE, DEFAULT_LIFETIME
-    global REDIS_HOST, REDIS_PORT, REDIS_DB
+    global REDIS_HOST, REDIS_PORT, REDIS_DB, REDIS_PASSWORD, REDIS_USERNAME
 
     cli = ArgumentParser()
     cli.add_argument('--rtdbin-port', metavar="PORT", type=int, help="builtin server port")
     cli.add_argument('--rtdbin-config', metavar="PATH", help="dotenv config file")
     options = cli.parse_known_args()[0]
     load_dotenv(options.rtdbin_config)  # use a sensitive default when omitted
 
@@ -63,14 +73,16 @@
     IDENTSIZE = int(os.getenv('RTDBIN_IDENTSIZE', 6))
     DEFAULT_LANGUAGE = os.getenv('RTDBIN_DEFAULT_LANGUAGE', 'text')
     DEFAULT_MAXUSAGE = int(os.getenv('RTDBIN_DEFAULT_MAXUSAGE', 0))
     DEFAULT_LIFETIME = Time(os.getenv('RTDBIN_DEFAULT_LIFETIME', 0))
     REDIS_HOST = os.getenv('REDIS_HOST', 'localhost')
     REDIS_PORT = int(os.getenv('REDIS_PORT', 6379))
     REDIS_DB = int(os.getenv('REDIS_DB', 0))
+    REDIS_PASSWORD = os.getenv('REDIS_PASSWORD') or None
+    REDIS_USERNAME = os.getenv('REDIS_USERNAME') or None
 
     # Configure logging
     if "gunicorn" in server_software:
         gunicorn_logger = logging.getLogger('gunicorn.error')
         bin_logger.handlers = gunicorn_logger.handlers
         bin_logger.setLevel(gunicorn_logger.level)
     elif server_software == "":
@@ -82,14 +94,10 @@
         )
 
     # Report config
     logger.debug(
         "Detected WSGI server: %s.",
         server_software or 'builtin wsgiref (unsafe for production)'
     )
-    logger.debug(
-        "Runtime configuration:\n  %s", "\n  ".join([
-        f"{key}: {val}" for key, val in globals().items()
-        if key.isupper() and not key.startswith('__')
-    ]))
+    logger.debug("Runtime configuration:\n%s", pformat(asdict()))
 
 _setup()
```

### Comparing `rtd-bin-server-1.3.0/bin/controller.py` & `rtd-bin-server-1.4.0/bin/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 Various HTTP routes the external world uses to communicate with the application.
 """
 
 import bottle as bt
 import cgi
 import logging
 import re
+import os.path
 import secrets
-from pathlib import Path
 from metrics import Time
 from bin import root, config, models
-from bin.highlight import highlight, parse_language, parse_extension, languages
+from bin.highlight import highlight, languages, langtoext, exttolang
 
 
 logger = logging.getLogger(__name__)
 BOTUARE = re.compile(r'|'.join([
     re.escape('Mozilla/5.0 (compatible; Discordbot/2.0; +https://discordapp.com)'),
     re.escape('facebookexternalhit/1.1 (+http://www.facebook.com/externalhit_uatext.php)'),
 ]))
@@ -80,45 +80,60 @@
     :param token: (form) optional the "admin" token allows you to delete your snippet
 
     :raises HTTPError: code 411 when the ``Content-Length`` http header is missing
     :raises HTTPError: code 413 when the http request is too large (mostly because the snippet is too long)
     :raises HTTPError: code 400 with a sensible status when the form processing fails
     """
     content_length = bt.request.get_header('Content-Length')
-    if content_length is None:
+    if not content_length:
         raise bt.HTTPError(411, "Content-Length required")
     if int(content_length) > config.MAXSIZE:
         raise bt.HTTPError(413, f"Payload too large, we accept maximum {config.MAXSIZE}")
 
     files = bt.request.files
     forms = bt.request.forms
 
     token = None
     code = None
-    lang = config.DEFAULT_LANGUAGE
+    lang = None
+    ext = None
     maxusage = config.DEFAULT_MAXUSAGE
     lifetime = config.DEFAULT_LIFETIME
     parentid = ''
 
     try:
+        # Form extraction
         if files:
             part = next(files.values())
             charset = cgi.parse_header(part.content_type)[1].get('charset', 'utf-8')
             code = part.file.read(config.MAXSIZE).decode(charset)
-            lang = parse_extension(Path(part.filename).suffix.lstrip('.')) or lang
+            ext = os.path.splitext(part.filename)[1][1:] or langtoext[config.DEFAULT_LANGUAGE]
         if forms:
             # WSGI forces latin-1 decoding, this is wrong, we recode it in utf-8
             code = forms.get('code', '').encode('latin-1').decode() or code
-            lang = forms.get('lang') or lang
+            lang = forms.get('lang') or config.DEFAULT_LANGUAGE
             maxusage = int(forms.get('maxusage') or maxusage)
             lifetime = Time(forms.get('lifetime') or lifetime)
             parentid = forms.get('parentid', '')
             token = forms.get('token')
 
-        ext = parse_language(lang)
+        # Form validation
+        if lang:
+            ext = langtoext.get(lang)
+            if ext is None:
+                logger.warning('Unknown lang %r, using %r.', lang, config.DEFAULT_LANGUAGE)
+                lang = config.DEFAULT_LANGUAGE
+                ext = langtoext[config.DEFAULT_LANGUAGE]
+
+        if ext:
+            lang = exttolang.get(ext)
+            if lang is None:
+                logger.warning('Unknown file extension %r, using %r.', ext, langtoext[config.DEFAULT_LANGUAGE])
+                lang = config.DEFAULT_LANGUAGE
+                ext = langtoext[config.DEFAULT_LANGUAGE]
         if not code:
             raise ValueError("Code is missing")
         if maxusage < 0:
             raise ValueError("Maximum usage must be positive")
         if lifetime < 0:
             raise ValueError("Lifetime must be positive")
         if parentid:
@@ -151,18 +166,22 @@
     if BOTUARE.match(bt.request.headers.get('User-Agent', '')):
         return bt.template('blank.html')
 
     try:
         snippet = models.Snippet.get_by_id(snippetid)
     except KeyError:
         raise bt.HTTPError(404, "Snippet not found")
-    lang = parse_extension(ext) or config.DEFAULT_LANGUAGE
+
+    lang = langtoext.get(ext, config.DEFAULT_LANGUAGE)
+    ext = langtoext[lang]  # always use the prefered extension for that lang
     codehl = highlight(snippet.code, lang)
+
     return bt.template(
         'highlight.html',
+        languages=languages,
         codehl=codehl,
         lang=lang,
         ext=ext,
         snippetid=snippetid,
         parentid=snippet.parentid,
         token=bt.request.query.token,
     )
@@ -230,13 +249,13 @@
     snippetid = bt.request.forms.get("snippetid")
     if not name:
         raise bt.HTTPError(400, "Missing name")
     if not snippetid:
         raise bt.HTTPError(400, "Missing snippetid")
 
     try:
-        snippet = models.Snippet.get_by_id(snippetid)
+        models.Snippet.get_by_id(snippetid)
     except KeyError:
         raise bt.HTTPError(404, "Snippet not found")
     logger.warning("The snippet %s got reported by %s", snippetid, name)
 
     return bt.HTTPResponse("The snippet have been reported.")
```

### Comparing `rtd-bin-server-1.3.0/bin/highlight.py` & `rtd-bin-server-1.4.0/bin/highlight.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 """ HTML highlighted code export and language tools """
 
-
+import os.path
 import pygments
-from pygments.lexers import get_lexer_by_name
+from pygments.lexers import get_all_lexers, get_lexer_by_name
 from pygments.formatters.html import HtmlFormatter
 
 
+# ==================================================================== #
+#                     Supported langages database                      #
+# ==================================================================== #
+
 languages = [
     # (ext, lang)
     ('c', 'c'),
     ('cpp', 'cpp'),
     ('cs', 'csharp'),
     ('css', 'css'),
+    ('dart', 'dart'),
     ('diff', 'diff'),
     ('erl', 'erlang'),
     ('ex', 'elixir'),
     ('go', 'go'),
     ('h', 'objectivec'),
     ('hs', 'haskell'),
     ('html', 'html'),
     ('ini', 'ini'),
     ('java', 'java'),
     ('js', 'javascript'),
     ('json', 'json'),
+    ('jl', 'julia'),
     ('kt', 'kotlin'),
     ('less', 'less'),
     ('lisp', 'lisp'),
     ('lua', 'lua'),
     ('md', 'markdown'),
     ('php', 'php'),
     ('pl', 'perl'),
@@ -44,43 +50,47 @@
     ('txt', 'text'),
     ('xml', 'xml'),
     ('yml', 'yaml'),
 ]
 exttolang = {ext: lang for ext, lang in languages}
 langtoext = {lang: ext for ext, lang in languages}
 
-
-def parse_extension(ext):
-    """ From a language extension, get a language """
-    ext = (ext or '').casefold()
-    if ext in langtoext:
-        return ext  # this is a lang already
-    return exttolang.get(ext)
-
-
-def parse_language(lang):
-    """ From a language name, get an extension """
-    lang = (lang or '').casefold()
-    if lang in exttolang:
-        return lang  # this is an ext already
-    return langtoext.get(lang)
-
-
+def _load_more_languages():
+    """ Save more langs to the ``exttolang`` and ``langtoext`` maps """
+    for name, aliases, globs, _mimetypes in get_all_lexers():
+        if not globs:
+           continue
+        name = name.lower()
+        for glob in globs:
+            ext = os.path.splitext(glob)[1][1:]
+            langtoext.setdefault(name, ext)
+            exttolang.setdefault(ext, name)
+        for alias in aliases:
+            ext = langtoext[name]
+            langtoext.setdefault(alias, ext)
+            exttolang.setdefault(ext, alias)
+
+_load_more_languages()
+del _load_more_languages
+
+# ==================================================================== #
+#                 Plaintext to stylized HTML utilities                 #
+# ==================================================================== #
 
 class _TableHtmlFormatter(HtmlFormatter):
     """
     Extension to the default pygment HtmlFormatter to control the html
     skeleton output, class names and line numbering.
     """
     def __init__(self, **options):
         super().__init__(**options)
         if options.get('linenos', False) == 'bin-table':
             self.linenos = 3
 
-    def wrap(self, source, outfile):
+    def wrap(self, source, outfile=None):
         if self.linenos == 3:
             source = self._wrap_table(source)
         yield from source
 
     def _wrap_table(self, inner):
         yield 0, '<table class="highlight"><tbody>'
         for i, (t, l) in enumerate([*inner, (1, '')]):
```

### Comparing `rtd-bin-server-1.3.0/bin/models.py` & `rtd-bin-server-1.4.0/bin/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from bin import config
 
 
 # We always connect to Redis
 database = Redis(
     host=config.REDIS_HOST,
     port=config.REDIS_PORT,
-    db=config.REDIS_DB
+    db=config.REDIS_DB,
+    password=config.REDIS_PASSWORD,
+    username=config.REDIS_USERNAME,
 )
 
 
 class Snippet:
     """
     A snippet is a immuable text that have been saved in the database
     and that is retrivable via an unique URL.
```

### Comparing `rtd-bin-server-1.3.0/bin/views/head.html` & `rtd-bin-server-1.4.0/bin/views/head.html`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 <meta name=viewport content="width=device-width, initial-scale=1.0">
 <meta name=author content="ReadTheDocs">
 <meta name=title content="ReadTheDocs Bin">
 <meta name=description content="https://github.com/readthedocs-fr/bin-server">
 <meta name=theme-color content="#1e282d">
 <meta name=color-scheme content="only light">
 
-<link rel="shortcut icon" href="/assets/favicon.ico" type="image/x-icon">
+<link rel="shortcut icon" href="/assets/icons/favicon.ico" type="image/x-icon">
 <link rel=stylesheet href="/assets/styles/style.css">
```

### Comparing `rtd-bin-server-1.3.0/rtd_bin_server.egg-info/PKG-INFO` & `rtd-bin-server-1.4.0/rtd_bin_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtd-bin-server
-Version: 1.3.0
+Version: 1.4.0
 Summary: A pastebin for Read The Docs discord community
 Home-page: https://github.com/readthedocs-fr/bin-server
 Author: Read The Docs
 Author-email: opensource@readthedocs.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/readthedocs-fr/bin-server/issues
 Project-URL: Documentation, https://rtd-bin-server.readthedocs.io/en/latest/
@@ -39,14 +39,16 @@
             RTDBIN_MAXSIZE=16kiB
             RTDBIN_DEFAULT_LANGUAGE=text
             RTDBIN_DEFAULT_MAXUSAGE=0
             RTDBIN_DEFAULT_LIFETIME=0
             REDIS_HOST=localhost
             REDIS_PORT=6379
             REDIS_DB=0
+            REDIS_PASSWORD=
+            REDIS_USERNAME=
         
         Par défaut, le service utilise le serveur web `wsgiref` disponible dans la bibliothèque standard de Python pour traiter les requêtes. Ce serveur est propice dans un environnement de développement ou lorsque le volume d'utilisateur est réduit. Pour de meilleures performances, [un serveur tiers compatible wsgi](https://wsgi.readthedocs.io/en/latest/servers.html) peut être utilisé à la place.
         
         	$ pip install gunicorn
         	$ gunicorn bin:app
         
         Des fichiers de configuration d'exemples pour `nginx`, `systemd` et `gunicorn` sont disponibles dans le [wiki](https://github.com/readthedocs-fr/bin/wiki/systemd-nginx-gunicorn).
```

### Comparing `rtd-bin-server-1.3.0/setup.cfg` & `rtd-bin-server-1.4.0/setup.cfg`

 * *Files identical despite different names*

