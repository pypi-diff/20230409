# Comparing `tmp/videobox-0.3.2.tar.gz` & `tmp/videobox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videobox-0.3.2.tar", last modified: Mon Feb  6 10:09:58 2023, max compression
+gzip compressed data, was "videobox-0.4.0.tar", last modified: Sat Apr  8 08:53:56 2023, max compression
```

## Comparing `videobox-0.3.2.tar` & `videobox-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        0 2023-02-06 10:09:58.184217 videobox-0.3.2/
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     1103 2023-01-27 09:36:41.000000 videobox-0.3.2/.gitignore
-drwxr-xr-x   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        0 2023-02-06 10:09:58.181612 videobox-0.3.2/.vscode/
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)      856 2023-01-27 09:32:09.000000 videobox-0.3.2/.vscode/launch.json
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       49 2023-01-19 15:12:32.000000 videobox-0.3.2/.vscode/settings.json
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     1516 2023-01-19 15:12:32.000000 videobox-0.3.2/LICENSE
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     4236 2023-02-06 10:09:58.184053 videobox-0.3.2/PKG-INFO
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     3636 2023-01-27 08:36:36.000000 videobox-0.3.2/README.md
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       70 2023-01-19 15:12:32.000000 videobox-0.3.2/Videobox.code-workspace
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)      143 2023-01-27 08:36:36.000000 videobox-0.3.2/debugger.py
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)      550 2023-01-27 09:32:59.000000 videobox-0.3.2/makefile
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)      916 2023-02-06 09:46:54.000000 videobox-0.3.2/pyproject.toml
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       48 2023-01-19 15:12:32.000000 videobox-0.3.2/requirements.txt
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       38 2023-02-06 10:09:58.184252 videobox-0.3.2/setup.cfg
-drwxr-xr-x   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        0 2023-02-06 10:09:58.183181 videobox-0.3.2/videobox/
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       64 2023-02-06 09:46:49.000000 videobox-0.3.2/videobox/__init__.py
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       40 2023-01-19 15:12:32.000000 videobox-0.3.2/videobox/__main__.py
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     1368 2023-01-27 10:18:29.000000 videobox-0.3.2/videobox/api.py
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)    13010 2023-01-27 16:25:50.000000 videobox-0.3.2/videobox/main.py
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     9817 2023-01-25 14:36:05.000000 videobox-0.3.2/videobox/model.py
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)    11239 2023-01-27 08:36:36.000000 videobox-0.3.2/videobox/sync.py
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     4436 2023-02-06 10:09:54.000000 videobox-0.3.2/videobox/trackers.txt
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     1124 2023-01-19 15:12:32.000000 videobox-0.3.2/videobox/utilities.py
-drwxr-xr-x   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        0 2023-02-06 10:09:58.183869 videobox-0.3.2/videobox.egg-info/
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)     4236 2023-02-06 10:09:58.000000 videobox-0.3.2/videobox.egg-info/PKG-INFO
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)      495 2023-02-06 10:09:58.000000 videobox-0.3.2/videobox.egg-info/SOURCES.txt
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        1 2023-02-06 10:09:58.000000 videobox-0.3.2/videobox.egg-info/dependency_links.txt
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       47 2023-02-06 10:09:58.000000 videobox-0.3.2/videobox.egg-info/entry_points.txt
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)       58 2023-02-06 10:09:58.000000 videobox-0.3.2/videobox.egg-info/requires.txt
--rw-r--r--   0 andrea.peltrin (1702769464) OMNYS\Domain Users (858591763)        9 2023-02-06 10:09:58.000000 videobox-0.3.2/videobox.egg-info/top_level.txt
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2023-04-08 08:53:56.508782 videobox-0.4.0/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1103 2023-02-15 11:35:53.000000 videobox-0.4.0/.gitignore
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2023-04-08 08:53:56.505488 videobox-0.4.0/.vscode/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      856 2023-02-08 10:49:32.000000 videobox-0.4.0/.vscode/launch.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       49 2023-01-19 15:12:32.000000 videobox-0.4.0/.vscode/settings.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1516 2023-01-19 15:12:32.000000 videobox-0.4.0/LICENSE
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4452 2023-04-08 08:53:56.508561 videobox-0.4.0/PKG-INFO
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3852 2023-04-08 08:43:41.000000 videobox-0.4.0/README.md
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       70 2023-01-19 15:12:32.000000 videobox-0.4.0/Videobox.code-workspace
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      158 2023-04-08 08:43:41.000000 videobox-0.4.0/debugger.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      550 2023-02-15 11:35:53.000000 videobox-0.4.0/makefile
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      916 2023-04-08 08:46:40.000000 videobox-0.4.0/pyproject.toml
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       48 2023-01-19 15:12:32.000000 videobox-0.4.0/requirements.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       38 2023-04-08 08:53:56.508826 videobox-0.4.0/setup.cfg
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2023-04-08 08:53:56.507307 videobox-0.4.0/videobox/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       64 2023-04-08 08:46:13.000000 videobox-0.4.0/videobox/__init__.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       40 2023-01-19 15:12:32.000000 videobox-0.4.0/videobox/__main__.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1644 2023-04-08 08:43:41.000000 videobox-0.4.0/videobox/api.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    14229 2023-04-08 08:43:41.000000 videobox-0.4.0/videobox/main.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     9802 2023-04-08 08:43:41.000000 videobox-0.4.0/videobox/model.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    13162 2023-04-08 08:43:41.000000 videobox-0.4.0/videobox/sync.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4153 2023-04-08 08:53:51.000000 videobox-0.4.0/videobox/trackers.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1124 2023-01-19 15:12:32.000000 videobox-0.4.0/videobox/utilities.py
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2023-04-08 08:53:56.508328 videobox-0.4.0/videobox.egg-info/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4452 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/PKG-INFO
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      495 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/SOURCES.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763        1 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/dependency_links.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       47 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/entry_points.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       58 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/requires.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763        9 2023-04-08 08:53:56.000000 videobox-0.4.0/videobox.egg-info/top_level.txt
```

### Comparing `videobox-0.3.2/.gitignore` & `videobox-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `videobox-0.3.2/.vscode/launch.json` & `videobox-0.4.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `videobox-0.3.2/LICENSE` & `videobox-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `videobox-0.3.2/PKG-INFO` & `videobox-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videobox
-Version: 0.3.2
+Version: 0.4.0
 Summary: Video download CLI utility
 Author: Andrea Peltrin
 Project-URL: Homepage, https://github.com/passiomatic/videobox
 Project-URL: Bug Tracker, https://github.com/passiomatic/videobox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -35,38 +35,40 @@
 
 ## Quick guide
 
 First, tell Videobox to update its local database:
 
 ```
 $ videobox update
-First run: import running series... 
+First run: import full database...
 (...)
 ```
 
+This will copy the full Videobox database to your machine. Currently database contains about 1 year of releases and tracks more than 1.000 series.
+
 **Note**: Videobox will auto-update itself if local database hasn't been refreshed for a while.
 
-Find out what series are running:
+Find out which series have been updated this week:
 
 ```
 $ videobox running -y7
 Found 84 series updated in the last 7 days:
 (...)
 N
- · NCIS  CBS
- · NCIS: Hawai'i  CBS
- · NCIS: Los Angeles  CBS
+ · NCIS  #20
+ · NCIS: Hawai'i  #45271
+ · NCIS: Los Angeles  #20420
 ```
 
 Find out more about a specific series:
 
 ```
 $ videobox search ncis los angeles
 ------------------------------
-NCIS: Los Angeles  CBS
+NCIS: Los Angeles  #45  CBS
 ------------------------------
 NCIS: Los Angeles is a drama about the high stakes world of
 undercover surveillance at the Office of Special Projects
 (...)
 #Action #Adventure #Crime #Drama
 
 Found 1 season with a total of 15 episodes and 92 releases:
@@ -81,15 +83,15 @@
 More series info at <https://thetvdb.com/series/ncis-los-angeles>
 ```
 
 Download a whole series season without headaches:
 
 ```
 $ videobox download ncis los angeles -s14 --dry-run
-Ready to download 10 releases for series 'NCIS: Los Angeles':
+Ready to download 10 releases for season 14 for series 'NCIS: Los Angeles' into /Users/Alice/Downloads:
 
 Seeds  Res. Size   Name
 --------------------------------------------------------------------------------
   128 1080p 2.15GB ncis.los.angeles.s14e01.1080p.web.h264-glhf[eztv.re].mkv
   198 1080p 2.15GB NCIS.Los.Angeles.S14E02.1080p.WEB.h264-GOSSIP[eztv.re].mkv
   209 1080p 2.15GB NCIS.Los.Angeles.S14E03.1080p.WEB.h264-GOSSIP[eztv.re].mkv
 (...)
```

### Comparing `videobox-0.3.2/README.md` & `videobox-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,38 +18,40 @@
 
 ## Quick guide
 
 First, tell Videobox to update its local database:
 
 ```
 $ videobox update
-First run: import running series... 
+First run: import full database...
 (...)
 ```
 
+This will copy the full Videobox database to your machine. Currently database contains about 1 year of releases and tracks more than 1.000 series.
+
 **Note**: Videobox will auto-update itself if local database hasn't been refreshed for a while.
 
-Find out what series are running:
+Find out which series have been updated this week:
 
 ```
 $ videobox running -y7
 Found 84 series updated in the last 7 days:
 (...)
 N
- · NCIS  CBS
- · NCIS: Hawai'i  CBS
- · NCIS: Los Angeles  CBS
+ · NCIS  #20
+ · NCIS: Hawai'i  #45271
+ · NCIS: Los Angeles  #20420
 ```
 
 Find out more about a specific series:
 
 ```
 $ videobox search ncis los angeles
 ------------------------------
-NCIS: Los Angeles  CBS
+NCIS: Los Angeles  #45  CBS
 ------------------------------
 NCIS: Los Angeles is a drama about the high stakes world of
 undercover surveillance at the Office of Special Projects
 (...)
 #Action #Adventure #Crime #Drama
 
 Found 1 season with a total of 15 episodes and 92 releases:
@@ -64,15 +66,15 @@
 More series info at <https://thetvdb.com/series/ncis-los-angeles>
 ```
 
 Download a whole series season without headaches:
 
 ```
 $ videobox download ncis los angeles -s14 --dry-run
-Ready to download 10 releases for series 'NCIS: Los Angeles':
+Ready to download 10 releases for season 14 for series 'NCIS: Los Angeles' into /Users/Alice/Downloads:
 
 Seeds  Res. Size   Name
 --------------------------------------------------------------------------------
   128 1080p 2.15GB ncis.los.angeles.s14e01.1080p.web.h264-glhf[eztv.re].mkv
   198 1080p 2.15GB NCIS.Los.Angeles.S14E02.1080p.WEB.h264-GOSSIP[eztv.re].mkv
   209 1080p 2.15GB NCIS.Los.Angeles.S14E03.1080p.WEB.h264-GOSSIP[eztv.re].mkv
 (...)
```

### Comparing `videobox-0.3.2/makefile` & `videobox-0.4.0/makefile`

 * *Files identical despite different names*

### Comparing `videobox-0.3.2/pyproject.toml` & `videobox-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "videobox"
-version = "0.3.2"
+version = "0.4.0"
 authors = [
   { name="Andrea Peltrin" },
 ]
 description = "Video download CLI utility"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
```

### Comparing `videobox-0.3.2/videobox/api.py` & `videobox-0.4.0/videobox/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,59 @@
 import requests
 import videobox
 import logging
 
 TIMEOUT = 10
-API_ENDPOINT_URL = "https://videobox.passiomatic.com/1"
-USER_AGENT = "Videobox/{0} <https://videobox.passiomatic.com/>".format(
-    videobox.__version__)
+API_VERSION = 2
+API_ENDPOINT_URL = f"https://videobox.passiomatic.com/{API_VERSION}"
+USER_AGENT = f"Videobox/{videobox.__version__} <https://videobox.passiomatic.com/>"
 
+# Full import
 
-def get_running_series(client_id):
-    return get_url("{0}/series/running?client={1}".format(API_ENDPOINT_URL, client_id))
+def get_all_series(client_id):
+    return get_url(f"{API_ENDPOINT_URL}/series/all?client={client_id}")
 
 
+def get_all_series_tags(client_id):
+    return get_url(f"{API_ENDPOINT_URL}/series-tags/all?client={client_id}")
+
+
+def get_all_episodes(client_id):
+    return get_url(f"{API_ENDPOINT_URL}/episodes/all?client={client_id}")
+
+
+def get_all_releases(client_id):
+    return get_url(f"{API_ENDPOINT_URL}/releases/all?client={client_id}")
+
+
+# Sync
+
 def get_updated_series(client_id, since):
-    return get_url("{0}/series/updated?since={1}&client={2}".format(API_ENDPOINT_URL, int(since.timestamp()), client_id))
+    return get_url(f"{API_ENDPOINT_URL}/series/updated?since={int(since.timestamp())}&client={client_id}")
 
 
 def get_series_with_ids(client_id, ids):
-    return get_url("{0}/series?ids={1}&client={2}".format(API_ENDPOINT_URL, make_ids(ids), client_id))
+    return get_url(f"{API_ENDPOINT_URL}/series?ids={make_ids(ids)}&client={client_id}")
 
 
 def get_series_tags_for_ids(client_id, ids):
-    return get_url("{0}/series-tags?ids={1}&client={2}".format(API_ENDPOINT_URL, make_ids(ids), client_id))
+    return get_url(f"{API_ENDPOINT_URL}/series-tags?ids={make_ids(ids)}&client={client_id}")
 
 
 def get_episodes_with_ids(client_id, ids):
-    return get_url("{0}/episodes?ids={1}&client={2}".format(API_ENDPOINT_URL, make_ids(ids), client_id))
+    return get_url(f"{API_ENDPOINT_URL}/episodes?ids={make_ids(ids)}&client={client_id}")
 
 
 def get_releases_with_ids(client_id, ids):
-    return get_url("{0}/releases?ids={1}&client={2}".format(API_ENDPOINT_URL, make_ids(ids), client_id))
+    return get_url(f"{API_ENDPOINT_URL}/releases?ids={make_ids(ids)}&client={client_id}")
 
 
 def make_ids(ids):
     return ",".join(map(str, ids))
 
 
 def get_url(url):
     request_headers = {
         'User-Agent': USER_AGENT
     }
     logging.debug(f"Quering API endpoint {url}...")
-    return requests.get(url, timeout=TIMEOUT, headers=request_headers)
+    return requests.get(url, timeout=TIMEOUT, headers=request_headers)
```

### Comparing `videobox-0.3.2/videobox/main.py` & `videobox-0.4.0/videobox/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 import videobox.sync as sync
 import videobox.model as model
 import videobox.utilities as utilities
 
 
 MIN_SEEDERS = 5
 SERIES_RUNNING_DAYS = 30
+AUTO_UPDATE_DAYS = 2
 
 package_dir = Path(__file__).parent
 
 
-def running_command(args, options):
-    results = model.get_running_series(options.days)
+def running_command(args, options):    
+    results = model.get_running_series(max(1, min(options.days, 60)))
     print(
         f"Found {len(results)} series updated in the last {options.days} days:")
     initials_series = itertools.groupby(results, key=get_initial)
     for initial, series in initials_series:
         cprint(f"\n{initial}", attrs=["bold"])
         for s in series:
             print(f" · {s.sort_name}  {colored(s.network,  'light_grey')}")
@@ -59,58 +60,68 @@
 def on_update_done(message, alert):
     print(f"{message:60}")
     if alert:
         cprint(alert, "yellow")
 
 
 def download_command(parser, args, options):
-    query = sanitize_query(" ".join(args))
+    query = " ".join(args)
     if not query:
-        parser.error("missing download query.")
+        parser.error("missing query.")
 
+    if query.startswith("#"):
+        series = get_series_by_id(parser, query)
+        best_releases = print_download_summary(parser, series, options)
+    else:
+        results = model.search_series(query)
+        if len(results) == 1:
+            # Single match from FTS
+            series = model.get_series(results[0].rowid)
+            best_releases = print_download_summary(parser, series, options)
+        elif results:
+            # Multiple matches
+            print(
+                f"Found {len(results)} series matching query '{query}':\n")
+            for r in results:
+                print(
+                    f" · {r.name}  {colored(f'#{r.rowid}', 'light_grey')}")
+            print("\nPlease restrict your query or specify a series #id.")
+            return
+        else:
+            print(
+                f"No series to download matching '{query}'. Perhaps try to relax your query a little?")
+            return
+
+    if not options.dry_run:
+        completed_process = run_aria2(
+            options.output_dir, [r.magnet_uri for _, r in best_releases])
+
+
+def print_download_summary(parser, series, options):
     try:
         max_resolution = int(options.max_resolution.replace("p", "", 1))
     except ValueError:
         parser.error(f"unrecognized resolution {options.max_resolution}")
 
-    download_dir = options.output_dir
-    logging.debug(f"Download dir is {download_dir}")
-    results = model.search_series(query)
-    if len(results) == 1:
-        # Single match
-        series = results[0]
-        releases = model.get_releases_for_series(
-            series.rowid, options.season, max_resolution)
-        best_releases = find_best_releases(releases)
-        if options.dry_run:
-            print(
-                f"Ready to download {len(best_releases)} releases for {f'season {options.season} of ' if options.season else ''}series '{series.name}' into {download_dir}:\n")
-        else:
-            print(
-                f"Start downloading {len(best_releases)} releases for {f'season {options.season} of ' if options.season else ''}series '{series.name}' into {download_dir} via aria2c...\n")
-
-        print("Seeds  Res.   Size Name")
-        cprint("-" * 80, "dark_grey")
-        for _, r in best_releases:
-            print_release(r)
-
-        if not options.dry_run:
-            completed_process = run_aria2(
-                download_dir, [r.magnet_uri for _, r in best_releases])
-    elif results:
-        # Multiple matches
+    releases = model.get_releases_for_series(
+        series.id, options.season, max_resolution)
+    best_releases = find_best_releases(releases)
+    if options.dry_run:
         print(
-            f"Found {len(results)} series matching query '{query}':\n")
-        for r in results:
-            print(
-                f" · {r.name}")
-        print("\nPlease restrict your query.")
+            f"Ready to download {len(best_releases)} releases for {f'season {options.season} of ' if options.season else ''}series '{series.name}' into {options.output_dir}:\n")
     else:
         print(
-            f"No series to download matching '{query}'.")
+            f"Start downloading {len(best_releases)} releases for {f'season {options.season} of ' if options.season else ''}series '{series.name}' into {options.output_dir} via aria2c...\n")
+
+    print("Seeds  Res.   Size Name")
+    cprint("-" * 80, "dark_grey")
+    for _, r in best_releases:
+        print_release(r)
+
+    return best_releases
 
 
 def run_aria2(download_dir, magnet_uris):
     try:
         with open(package_dir.joinpath("trackers.txt")) as f:
             trackers = f.read()
     except FileNotFoundError as ex:
@@ -171,53 +182,78 @@
     elif resolution == 480:
         return f"{resolution:4}p"
     else:
         return "-"*5
 
 
 def search_command(parser, args, options):
-    query = sanitize_query(" ".join(args))
+    query = " ".join(args)
     if not query:
-        parser.error("missing search query.")
-    results = model.search_series(query)
-    if len(results) == 1:
-        today = date.today()
-        # Single match
-        series = model.get_series(results[0].rowid)
-        tags = model.get_tags_for_series(series)
-        episodes = model.get_episodes_for_series(series)
-        episode_count = len(episodes)
-        seasons = set([episode.season for episode in episodes])
-        release_count = sum([episode.release_count for episode in episodes])
-        cprint("-" * 30, "dark_grey")
-        cprint(
-            f"{colored(f'{series.name}', attrs=['bold'])}  {colored(series.network, 'light_grey')}")
-        cprint("-" * 30, "dark_grey")
-        if series.overview:
-            print("\n".join(textwrap.wrap(series.overview, 60)))
-        print(" ".join([colored(f"#{t.name}", "light_grey") for t in tags]))
-        print(f"\nFound {len(seasons)} {plural('season', len(seasons))} with a total of {episode_count} {plural('episode', episode_count)} and {release_count} {plural('release', release_count)}:")
-        for season, episodes in itertools.groupby(episodes, key=lambda e: e.season):
-            cprint(f"\nSeason {season}", attrs=["bold"])
-            for e in episodes:
-                print_episode(e, today)
-        print(f"\nMore info:")
-        print(f" · {series.tvdb_url}")
-        if series.imdb_url:
-            print(f" · {series.imdb_url}")
-    elif results:
-        # Multiple matches
-        print(
-            f"Found {len(results)} series matching query '{query}':\n")
-        for search_result in results:
-            print(
-                f" · {search_result.name}")
+        parser.error("missing query.")
+    if query.startswith("#"):
+        series = get_series_by_id(parser, query)
+        print_series_info(series)
     else:
-        print(
-            f"No series found matching '{query}'. Perhaps try to relax the search query a little?")
+        results = model.search_series(sanitize_query(query))
+        if len(results) == 1:
+            # Single match from FTS
+            series = model.get_series(results[0].rowid)
+            print_series_info(series)
+        elif results:
+            # Multiple matches
+            print(
+                f"Found {len(results)} series matching query '{query}':\n")
+            for search_result in results:
+                print(
+                    f" · {search_result.name}  {colored(f'#{search_result.rowid}', 'light_grey')}")
+            print("\nPlease restrict your query or specify a series #id.")
+        else:
+            print(
+                f"No series found matching '{query}'. Perhaps try to relax your query a little?")
+
+
+def parse_series_id(parser, query):
+    try:
+        series_id = int(query[1:])
+    except ValueError:
+        parser.error(f"{query} isn't a valid series id")
+    return series_id
+
+
+def get_series_by_id(parser, query):
+    series_id = parse_series_id(parser, query)
+    series = model.get_series(series_id)
+    if series is None:
+        parser.error(f"no series found with id #{series_id}")
+    return series
+
+
+def print_series_info(series):
+    today = date.today()
+    tags = model.get_tags_for_series(series)
+    episodes = model.get_episodes_for_series(series)
+    episode_count = len(episodes)
+    seasons = set([episode.season for episode in episodes])
+    release_count = sum([episode.release_count for episode in episodes])
+    cprint("-" * 30, "dark_grey")
+    cprint(
+        f"{colored(f'{series.name}', attrs=['bold'])}  {colored(f'#{series.id}', 'light_grey')}  {colored(series.network, 'light_grey')}")
+    cprint("-" * 30, "dark_grey")
+    if series.overview:
+        print("\n".join(textwrap.wrap(series.overview, 60)))
+    print(" ".join([colored(f"#{t.name}", "light_grey") for t in tags]))
+    print(f"\nFound {len(seasons)} {plural('season', len(seasons))} with a total of {episode_count} {plural('episode', episode_count)} and {release_count} {plural('release', release_count)}:")
+    for season, episodes in itertools.groupby(episodes, key=lambda e: e.season):
+        cprint(f"\nSeason {season}", attrs=["bold"])
+        for e in episodes:
+            print_episode(e, today)
+    print(f"\nMore info:")
+    print(f" · {series.tvdb_url}")
+    if series.imdb_url:
+        print(f" · {series.imdb_url}")
 
 
 def print_episode(e, today):
     aired = ""
     if e.aired_on and e.aired_on < today:
         # Past
         aired = f"Aired {utilities.datetime_since(e.aired_on, today)}"
@@ -242,15 +278,15 @@
         else:
             sanitized_query += " "
     return sanitized_query
 
 
 def auto_update_if_stale(config):
     last_log = model.get_last_log()
-    if (not last_log) or (datetime.utcnow() - last_log.timestamp) > timedelta(days=1):
+    if (not last_log) or (datetime.utcnow() - last_log.timestamp) > timedelta(days=AUTO_UPDATE_DAYS):
         print("Local database is stale, performing auto-update...")
         update_command(config)
 
 
 def run_command(config, parser, name, args, options):
     if name == "update":
         update_command(config)
@@ -291,16 +327,17 @@
 
 class CommandNotFound(RuntimeError):
     pass
 
 
 COMMANDS = [
     ('download',    'Download all available series releases or a single season'),
-    ('running',     'List all series with new releases in the last 30 days'),
-    ('search',      'Search for a series by name'),
+    ('running',
+     f'List all series with new releases in the last {SERIES_RUNNING_DAYS} days'),
+    ('search',      'Search for a series by name or #id'),
     ('update',      'Update local database')
 ]
 
 EPILOG = ""
 USAGE = '%prog command [options] [query]\n\n\
 Available commands are:\n\n' + "\n".join(f"  {c}\t{help}" for c, help in COMMANDS)
 
@@ -319,18 +356,18 @@
                                 dest='output_dir', help='directory to save downloaded files (default: current working directory)', default=os.getcwd())
     download_options.add_option('--dry-run',
                                 dest='dry_run', help='do not download anything, just list what would be', action="store_true")
     download_options.add_option('-r', '--max-resolution',
                                 dest='max_resolution', help='limit downloads to 1080p, 720p, or 480p videos (default: 2160p or highest found)', default="2160p")
     parser.add_option_group(download_options)
 
-    search_options = OptionGroup(parser, "Search options")
-    search_options.add_option('-y', '--days',
-                              dest='days', type='int', help=f'show series updated since number of days (default: {SERIES_RUNNING_DAYS})', default=SERIES_RUNNING_DAYS)
-    parser.add_option_group(search_options)
+    listing_options = OptionGroup(parser, "Listing options")
+    listing_options.add_option('-y', '--days',
+                              dest='days', type='int', help=f'list series updated since number of days (default: {SERIES_RUNNING_DAYS})', default=SERIES_RUNNING_DAYS)
+    parser.add_option_group(listing_options)
 
     return parser
 
 
 def run():
 
     parser = make_parser()
```

### Comparing `videobox-0.3.2/videobox/model.py` & `videobox-0.4.0/videobox/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,20 +72,17 @@
 
 
 class SeriesTag(db.Model):
     series = ForeignKeyField(Series, on_delete="CASCADE")
     # We could change a tag slug, so update this FK accordingly
     tag = ForeignKeyField(Tag, column_name="tag_slug",
                           on_delete="CASCADE", on_update="CASCADE")
-
+    
     class Meta:
-        indexes = (
-            (('series', 'tag'), True),
-        )
-
+        primary_key = CompositeKey('series', 'tag')
 
 class Episode(db.Model):
     tvdb_id = IntegerField(unique=True)
     series = ForeignKeyField(Series, backref='episodes', on_delete="CASCADE")
     name = CharField()
     season = SmallIntegerField()
     number = SmallIntegerField()
@@ -215,15 +212,15 @@
 
 def search_series(query):
     # return SeriesIndex.search(query, weights={'name': 2.0, 'overview': 0.1, 'network': 0.1}, with_score=True, score_alias='search_score')
     return SeriesIndex.search(query, with_score=True, score_alias='search_score')
 
 
 def get_series(series_id):
-    return Series.get(Series.id == series_id)
+    return Series.get_or_none(Series.id == series_id)
 
 
 def get_episode(episode_id):
     return Episode.get(Episode.id == episode_id)
 
 
 def get_release(id):
@@ -292,15 +289,15 @@
 
 
 ###########
 # LOCAL DB SETUP
 ###########
 
 TAGS = {
-    "action": "Action", "adventure": "Adventure", "animation": "Animation", "anime": "Anime", "awards-show": "Awards Show", "children": "Children", "comedy": "Comedy", "crime": "Crime", "documentary": "Documentary", "drama": "Drama", "family": "Family", "fantasy": "Fantasy", "food": "Food", "game-show": "Game Show", "history": "History", "home-and-garden": "Home and Garden", "horror": "Horror", "indie": "Indie", "martial-arts": "Martial Arts", "mini-series": "Mini-Series", "musical": "Musical", "mystery": "Mystery", "news": "News", "podcast": "Podcast", "reality": "Reality", "romance": "Romance", "science-fiction": "Science Fiction", "soap": "Soap", "special-interest": "Special Interest", "sport": "Sport", "suspense": "Suspense", "talk Show": "Talk Show", "thriller": "Thriller", "travel": "Travel", "western": "Western", "war": "War"
+    "action": "Action", "adventure": "Adventure", "animation": "Animation", "anime": "Anime", "awards-show": "AwardsShow", "children": "Children", "comedy": "Comedy", "crime": "Crime", "documentary": "Documentary", "drama": "Drama", "family": "Family", "fantasy": "Fantasy", "food": "Food", "game-show": "GameShow", "history": "History", "home-and-garden": "HomeAndGarden", "horror": "Horror", "indie": "Indie", "martial-arts": "MartialArts", "mini-series": "MiniSeries", "musical": "Musical", "mystery": "Mystery", "news": "News", "podcast": "Podcast", "reality": "Reality", "romance": "Romance", "science-fiction": "ScienceFiction", "soap": "Soap", "special-interest": "SpecialInterest", "sport": "Sport", "suspense": "Suspense", "talk Show": "TalkShow", "thriller": "Thriller", "travel": "Travel", "western": "Western", "war": "War"
 }
 
 
 def setup():
     db.create_tables([
         Series,
         SeriesIndex,
```

### Comparing `videobox-0.3.2/videobox/sync.py` & `videobox-0.4.0/videobox/sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,262 +1,335 @@
 from peewee import chunked
 import time
-from datetime import datetime, timezone
+from datetime import datetime, timedelta, timezone
 from requests.exceptions import HTTPError, ReadTimeout
-from urllib3.exceptions import ReadTimeoutError
 import logging
 import videobox.api as api
 import videobox.model as model
 from videobox.model import SeriesTag, db, Series, SeriesIndex, Episode, EpisodeIndex, Release, SyncLog
 
 INSERT_CHUNK_SIZE = 90      # SQLite has a limit of total 999 max variables
 REQUEST_CHUNK_SIZE = 450    # Total URI must be < 4096
+TIMEOUT_BEFORE_RETRY = 5    # Seconds
+
+
+class SyncError(Exception):
+    pass
 
 
 class SyncWorker(object):
 
     def __init__(self, client_id, progress_callback=None, done_callback=None):
         self.client_id = client_id
         self.progress_callback = progress_callback
         self.done_callback = done_callback
 
     def run(self):
         last_log = model.get_last_log()
-        start = time.time()
+        start_time = time.time()
 
-        # Start log line
-        current_log = SyncLog.create(description="Started sync")
+        current_log = SyncLog.create(description="Started import/sync")
 
-        response = []
-        if last_log:
-            logging.info("Last update done at {0} UTC, requesting updates since then".format(
-                last_log.timestamp.isoformat()))
-            if self.progress_callback:
-                self.progress_callback("Getting updated series...")
-            # Ensure UTC tz
-            response = self.do_request(lambda: api.get_updated_series(
-                self.client_id, last_log.timestamp.replace(tzinfo=timezone.utc)), retries=3)
-        else:
-            logging.info("No local database found, starting import")
-            if self.progress_callback:
-                self.progress_callback("First run: import running series...")
-
-            response = self.do_request(
-                lambda: api.get_running_series(self.client_id), retries=3)
-
-        if not response:
-            # @@TODO pass any error to current_log
-            self.update_log(current_log, status="E",
-                            description="Unable to contact sync server")
+        alert = ""
+        try:
+            if last_log:
+                alert, series_count, episode_count, release_count = self.update_library(
+                    last_log)
+            else:
+                series_count, episode_count, release_count = self.import_library()
+        except SyncError as ex:
+            self.update_log(current_log, status="E", description=str(ex))
+            if self.done_callback:
+                self.done_callback(str(ex), alert)
             return
 
+        elapsed_time = time.time()-start_time
+        if any([series_count, episode_count, release_count]):
+            description = "Finished in {:.1f}s: added/updated {} series, {} episodes, and {} releases".format(
+                elapsed_time, series_count, episode_count, release_count
+            )
+        else:
+            description = "Finished in {:.1f}s: no updates were found".format(
+                elapsed_time)
+
+        # Mark import/sync successful
+        self.update_log(current_log, status="K", description=description)
+
+        logging.info(f"{description}")
+
+        if self.done_callback:
+            self.done_callback(description, alert)
+
+    def import_library(self):
+        series_count, episode_count, release_count = 0, 0, 0
+        instant = datetime.utcnow()
+
+        logging.info("No local database found, starting full import")
+        if self.progress_callback:
+            self.progress_callback("First run, importing all series...", 0)
+
+        json = self.do_json_request(
+            lambda: api.get_all_series(self.client_id), retries=3)
+        if json:
+            series_count = self.save_series(json, instant)
+
+        if self.progress_callback:
+            self.progress_callback("Importing all series tags...", 25)
+
+        json = self.do_json_request(
+            lambda: api.get_all_series_tags(self.client_id))
+        if json:
+            self.save_series_tags(json)
+
+        if self.progress_callback:
+            self.progress_callback("Importing all episodes...", 50)
+
+        json = self.do_json_request(
+            lambda: api.get_all_episodes(self.client_id))
+        if json:
+            episode_count = self.save_episodes(json, instant)
+
+        if self.progress_callback:
+            self.progress_callback("Importing all releases...", 75)
+
+        json = self.do_json_request(
+            lambda: api.get_all_releases(self.client_id))
+        if json:
+            release_count = self.save_releases(json, instant)
+
+        return series_count, episode_count, release_count
+
+    def update_library(self, last_log):
+        series_count, episode_count, release_count = 0, 0, 0
+
+        logging.info("Last update done at {0} UTC, requesting updates since then".format(
+            last_log.timestamp.isoformat()))
+        if self.progress_callback:
+            self.progress_callback("Getting updated series...")
+        # Ensure UTC tz
+        json = self.do_json_request(lambda: api.get_updated_series(
+            self.client_id, last_log.timestamp.replace(tzinfo=timezone.utc)), retries=3)
+
         # Save alert from server, if any
-        alert = response["alert"]
+        alert = json["alert"]
 
         # Grab series
-        series_ids = response['series']
+        series_ids = json['series']
         if series_ids:
             logging.debug(
                 "Got {0} series, starting update".format(len(series_ids)))
             series_count = self.sync_series(series_ids)
 
         # Grab episodes
-        episode_ids = response['episodes']
+        episode_ids = json['episodes']
         if episode_ids:
             logging.debug(
                 "Got {0} episodes, starting update".format(len(episode_ids)))
             episode_count = self.sync_episodes(episode_ids)
 
         # Grab releases
-        release_ids = response['releases']
+        release_ids = json['releases']
         if release_ids:
             release_count = self.sync_releases(release_ids)
 
-        elapsed_time = time.time()-start
-        if any([series_ids, episode_ids, release_ids]):
-            description = "Finished in {:.2f}s: updated {} series, {} episodes, and {} releases".format(
-                elapsed_time, series_count, episode_count, release_count
-            )
-        else:
-            description = "Finished in {:.2f}s: no updates were found".format(
-                elapsed_time)
-
-        # Mark sync successful
-        self.update_log(current_log, status="K", description=description)
-
-        logging.info(f"{description}")
-
-        if self.done_callback:
-            self.done_callback(description, alert)
+        return alert, series_count, episode_count, release_count
 
     def sync_series(self, remote_ids):
         instant = datetime.utcnow()
 
         local_ids = [s.id for s in Series.select(Series.id)]
-        new_ids = list(set(remote_ids) - set(local_ids))
-        new_ids_count = len(new_ids)
+        new_ids = set(remote_ids) - set(local_ids)
+        count = 0
 
         # Always request all remote ids so we have a change to update existing series
         if remote_ids:
             def callback(percent, remaining):
                 self.progress_callback(
                     f"Updating {remaining} series...", 25 + percent)
 
             logging.debug(
-                f"Found missing {new_ids_count} of {len(remote_ids)} series")
+                f"Found missing {len(new_ids)} of {len(remote_ids)} series")
             # Reuqest old and new series
             response = self.do_chunked_request(
                 api.get_series_with_ids, remote_ids, callback)
             if response:
-                with db.atomic():
-                    logging.debug("Saving series to database...")
-                    for batch in chunked(response, INSERT_CHUNK_SIZE):
-                        # Insert new series and attempt to update existing ones
-                        (Series.insert_many(batch)
-                         .on_conflict(
-                            conflict_target=[Series.id],
-                            # Pass down values from insert clause
-                            preserve=[Series.name, Series.overview, Series.network, Series.poster_url, Series.fanart_url],
-                            update={Series.last_updated_on: instant})
-                         .execute())
-                        for series in batch:
-                            (SeriesIndex.insert({
-                                SeriesIndex.rowid: series['id'],
-                                SeriesIndex.name: series['name']
-                            })
-                                # Just replace name edits
-                                .on_conflict_replace()
-                                .execute())
-                SeriesIndex.optimize()
+                count = self.save_series(response, instant)
 
             #  Series tags
             response = self.do_chunked_request(
                 api.get_series_tags_for_ids, remote_ids, callback)
             if response:
-                with db.atomic():
-                    logging.debug("Saving series tags to database...")
-                    for batch in chunked(response, INSERT_CHUNK_SIZE):
-                        (SeriesTag.insert_many(batch)
-                            .on_conflict(action="nothing", conflict_target=[SeriesTag.series, SeriesTag.tag])
-                         .execute())
+                self.save_series_tags(response)
 
-        return len(remote_ids)
+        return count
+
+    def save_series(self, response, instant):
+        """
+        Insert new series and attempt to update existing ones
+        """
+        count = 0
+        with db.atomic():
+            logging.debug("Saving series to database...")
+            for batch in chunked(response, INSERT_CHUNK_SIZE):
+                count += (Series.insert_many(batch)
+                          .on_conflict(
+                    conflict_target=[Series.id],
+                    preserve=[Series.name, Series.overview, Series.network,
+                              Series.poster_url, Series.fanart_url],
+                    update={Series.last_updated_on: instant})
+                    .as_rowcount()
+                    .execute())
+                for series in batch:
+                    # FTS5 insert_many cannot handle upserts
+                    (SeriesIndex.insert({
+                        SeriesIndex.rowid: series['id'],
+                        SeriesIndex.name: series['name']
+                    })
+                        # Just replace name edits
+                        .on_conflict_replace()
+                        .execute())
+        SeriesIndex.optimize()
+        return count
+
+    def save_series_tags(self, response):
+        with db.atomic():
+            logging.debug("Saving series tags to database...")
+            for batch in chunked(response, INSERT_CHUNK_SIZE):
+                (SeriesTag.insert_many(batch)
+                    .on_conflict(action="nothing", conflict_target=[SeriesTag.series, SeriesTag.tag])
+                    .execute())
 
     def sync_episodes(self, remote_ids):
         instant = datetime.utcnow()
 
         local_ids = [e.id for e in Episode.select(Episode.id)]
-        new_ids = list(set(remote_ids) - set(local_ids))
-        new_ids_count = len(new_ids)
+        new_ids = set(remote_ids) - set(local_ids)
+        count = 0
 
         # Always request all remote ids so we have a change to update existing episodes
         if remote_ids:
             def callback(percent, remaining):
                 self.progress_callback(
                     f"Updating {remaining} episodes...", 50 + percent)
 
             logging.debug(
-                f"Found missing {new_ids_count} of {len(remote_ids)} episodes")
+                f"Found missing {len(new_ids)} of {len(remote_ids)} episodes")
             # Request old and new episodes
             response = self.do_chunked_request(
                 api.get_episodes_with_ids, remote_ids, callback)
             if response:
-                with db.atomic():
-                    logging.debug("Saving episodes to database...")
-                    for batch in chunked(response, INSERT_CHUNK_SIZE):
-                        # We need to cope with the unique constraint for (series, season, number)
-                        #   index because we cannot rely on episodes id's,
-                        #   they are often changed when TVDB users update them
-                        (Episode
-                            .insert_many(batch)
-                            .on_conflict(
-                                conflict_target=[
-                                    Episode.series, Episode.season, Episode.number],
-                                # Pass down values from insert clause 
-                                preserve=[Episode.name, Episode.overview, Episode.aired_on, Episode.thumbnail_url],
-                                update={Episode.last_updated_on: instant})
-                            .execute())
-                        # EpisodeIndex.insert({
-                        #     EpisodeIndex.rowid: episode_id,
-                        #     EpisodeIndex.name: episode.name,
-                        #     EpisodeIndex.overview: episode.overview}).execute()
+                count = self.save_episodes(response, instant)
+
+        return count
 
-        return len(remote_ids)
+    def save_episodes(self, response, instant):
+        """
+        Insert new episodes and attempt to update existing ones
+        """
+        count = 0
+        with db.atomic():
+            logging.debug("Saving episodes to database...")
+            for batch in chunked(response, INSERT_CHUNK_SIZE):
+                # We need to cope with the unique constraint for (series, season, number)
+                #   index because we cannot rely on episodes id's,
+                #   they are often changed when TVDB users update them
+                count += (Episode
+                          .insert_many(batch)
+                          .on_conflict(
+                              conflict_target=[
+                                  Episode.series, Episode.season, Episode.number],
+                              # Pass down values from insert clause
+                              preserve=[Episode.name, Episode.overview,
+                                        Episode.aired_on, Episode.thumbnail_url],
+                              update={Episode.last_updated_on: instant})
+                          .as_rowcount()
+                          .execute())
+                # EpisodeIndex.insert({
+                #     EpisodeIndex.rowid: episode_id,
+                #     EpisodeIndex.name: episode.name,
+                #     EpisodeIndex.overview: episode.overview}).execute()
+        return count
 
     def sync_releases(self, remote_ids):
+        instant = datetime.utcnow()
 
         local_ids = [r.id for r in Release.select(Release.id)]
-        new_ids = list(set(remote_ids) - set(local_ids))
-        new_ids_count = len(new_ids)
+        new_ids = set(remote_ids) - set(local_ids)
+        count = 0
 
         # Always request all remote ids so we have a chance to update existing releases
         if remote_ids:
             def callback(percent, remaining):
                 self.progress_callback(
                     f"Updating {remaining} releases...", 75 + percent)
 
             logging.debug(
-                f"Found missing {new_ids_count} of {len(remote_ids)} releases")
+                f"Found missing {len(new_ids)} of {len(remote_ids)} releases")
             # Request old and new releases
             response = self.do_chunked_request(
                 api.get_releases_with_ids, remote_ids, callback)
             if response:
-                with db.atomic():
-                    logging.debug("Saving releases to database...")
-                    for batch in chunked(response, INSERT_CHUNK_SIZE):
-                        (Release
-                            .insert_many(batch)
-                            .on_conflict(
-                                conflict_target=[Release.id],
-                                # Pass down values from insert clause
-                                preserve=[Release.peers, Release.seeders, Release.last_updated_on])
-                            .execute())
+                count = self.save_releases(response, instant)
+
+        return count
 
-        return len(remote_ids)
+    def save_releases(self, response, instant):
+        """
+        Insert new releases and attempt to update existing ones
+        """
+        count = 0
+        with db.atomic():
+            logging.debug("Saving releases to database...")
+            for batch in chunked(response, INSERT_CHUNK_SIZE):
+                count += (Release
+                          .insert_many(batch)
+                          .on_conflict(
+                              conflict_target=[Release.id],
+                              # Pass down values from insert clause
+                              preserve=[Release.peers, Release.seeders, Release.last_updated_on])
+                          .as_rowcount()
+                          .execute())
+        return count
 
     def progress(self, value, min, max):
         return self.scale_between(value, 0, 25, min, max)
 
     def scale_between(self, value, min_allowed, max_allowed, min, max):
         return (max_allowed - min_allowed) * (value - min) / (max - min) + min_allowed
 
-    def update_log(self, log, status, description=""):
+    def update_log(self, log, status, description):
         log.status = status
         log.description = description
         log.save()
 
     def do_chunked_request(self, handler, ids, callback=None):
         result = []
         ids_count = len(ids)
         for index, chunked_ids in enumerate(chunked(ids, REQUEST_CHUNK_SIZE)):
             if callback:
                 percent = self.progress(index*REQUEST_CHUNK_SIZE, 0, ids_count)
                 callback(percent, ids_count -
                          index*REQUEST_CHUNK_SIZE)
             logging.debug(
                 f"Requesting {index + 1} of {ids_count // REQUEST_CHUNK_SIZE + 1} chunks")
-            result.extend(self.do_request(
-                lambda: handler(self.client_id, chunked_ids)))
+            json = self.do_json_request(
+                lambda: handler(self.client_id, chunked_ids))
+            result.extend(json)
         return result
 
-    def do_request(self, handler, retries=1):
+    def do_json_request(self, handler, retries=1):
         for index in reversed(range(retries)):
             try:
                 response = handler()
                 response.raise_for_status()  # Raise an exeption on HTTP errors
-            except Exception as ex:
-                self.log_network_error(ex, index)
-                time.sleep(2)
+            except ReadTimeout as ex:
+                message = f'Server timed out while handling the request, {"retrying" if index else "skipped"}'
+                logging.warn(message)
+                time.sleep(TIMEOUT_BEFORE_RETRY)
                 continue  # Next retry
+            except HTTPError as ex:
+                message = f'Server error {ex.response.status_code} occurred while handling the request, giving up'
+                logging.error(message)
+                raise SyncError(message)
             return response.json()
-        return []
-
-    def log_network_error(self, ex, retry):
-        if isinstance(ex, TimeoutError) or isinstance(ex, ReadTimeoutError) or isinstance(ex, ReadTimeout):
-            logging.warn(
-                f'Server timed out while handling the request {ex}, {"retrying" if retry else "skipped"}')
-        elif isinstance(ex, HTTPError):
-            logging.error(
-                f'A server error occured while handling the request {ex}, {"retrying" if retry else "skipped"}')
-        else:
-            # Cannot handle this
-            raise ex
+        # No more retries, giving up
+        raise SyncError("Server timed out while handling the request")
```

### Comparing `videobox-0.3.2/videobox/trackers.txt` & `videobox-0.4.0/videobox/trackers.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-http://00.xxtor.com:443/announce,http://1337.abcvg.info:80/announce,http://dht.dhtclub.com:666/announce,http://i-p-v-6.tk:6969/announce,http://ipv6.1337.cx:6969/announce,http://ipv6.govt.hu:6969/announce,http://nyaa.tracker.wf:7777/announce,http://open-v6.demonoid.ch:6969/announce,http://open.acgnxtracker.com:80/announce,http://p2p.0g.cx:6969/announce,http://share.camoe.cn:8080/announce,http://t.nyaatracker.com:80/announce,http://torrentsmd.com:8080/announce,http://tr.cili001.com:8070/announce,http://tracker.bt4g.com:2095/announce,http://tracker.files.fm:6969/announce,http://tracker.gbitt.info:80/announce,http://tracker.ipv6tracker.ru:80/announce,http://tracker.k.vu:6969/announce,http://tracker.mywaifu.best:6969/announce,http://trackers.ydns.eu:10036/announce,http://trackme.theom.nz:80/announce,http://v6-tracker.0g.cx:6969/announce,http://www.all4nothin.net:80/announce.php,http://www.wareztorrent.com:80/announce,https://1337.abcvg.info:443/announce,https://opentracker.i2p.rocks:443/announce,https://tr.abiir.top:443/announce,https://tr.abir.ga:443/announce,https://tr.burnabyhighstar.com:443/announce,https://tracker.foreverpirates.co:443/announce,https://tracker.gbitt.info:443/announce,https://tracker.imgoingto.icu:443/announce,https://tracker.jiesen.life:8443/announce,https://tracker.kuroy.me:443/announce,https://tracker.lilithraws.cf:443/announce,https://tracker.lilithraws.org:443/announce,https://tracker.loligirl.cn:443/announce,https://tracker.mlsub.net:443/announce,https://tracker.nitrix.me:443/announce,https://tracker.tamersunion.org:443/announce,https://tracker1.520.jp:443/announce,https://trackers.mlsub.net:443/announce,https://trackme.theom.nz:443/announce,udp://6ahddutb1ucc3cp.ru:6969/announce,udp://9.rarbg.com:2810/announce,udp://aarsen.me:6969/announce,udp://acxx.de:6969/announce,udp://aegir.sexy:6969/announce,udp://bedro.cloud:6969/announce,udp://boysbitte.be:6969/announce,udp://bt.ktrackers.com:6666/announce,udp://chihaya.de:6969/announce,udp://chouchou.top:8080/announce,udp://cutscloud.duckdns.org:6969/announce,udp://dht.bt251.com:6969/announce,udp://epider.me:6969/announce,udp://exodus.desync.com:6969/announce,udp://free.publictracker.xyz:6969/announce,udp://htz3.noho.st:6969/announce,udp://ipv6.69.mu:6969/announce,udp://ipv6.tracker.monitorit4.me:6969/announce,udp://laze.cc:6969/announce,udp://mail.artixlinux.org:6969/announce,udp://moonburrow.club:6969/announce,udp://movies.zsw.ca:6969/announce,udp://open.demonii.com:1337/announce,udp://open.dstud.io:6969/announce,udp://open.free-tracker.ga:6969/announce,udp://open.publictracker.xyz:6969/announce,udp://open.stealth.si:80/announce,udp://open.tracker.ink:6969/announce,udp://opentor.org:2710/announce,udp://opentracker.i2p.rocks:6969/announce,udp://p4p.arenabg.com:1337/announce,udp://private.anonseed.com:6969/announce,udp://psyco.fr:6969/announce,udp://run.publictracker.xyz:6969/announce,udp://slicie.icon256.com:8000/announce,udp://stargrave.org:6969/announce,udp://static.54.161.216.95.clients.your-server.de:6969/announce,udp://t.133335.xyz:6969/announce,udp://thagoat.rocks:6969/announce,udp://thetracker.org:80/announce,udp://thouvenin.cloud:6969/announce,udp://torrents.artixlinux.org:6969/announce,udp://tracker.4.babico.name.tr:3131/announce,udp://tracker.altrosky.nl:6969/announce,udp://tracker.artixlinux.org:6969/announce,udp://tracker.auctor.tv:6969/announce,udp://tracker.beeimg.com:6969/announce,udp://tracker.birkenwald.de:6969/announce,udp://tracker.bitsearch.to:1337/announce,udp://tracker.cyberia.is:6969/announce,udp://tracker.jonaslsa.com:6969/announce,udp://tracker.joybomb.tw:6969/announce,udp://tracker.leech.ie:1337/announce,udp://tracker.moeking.me:6969/announce,udp://tracker.monitorit4.me:6969/announce,udp://tracker.openbittorrent.com:6969/announce,udp://tracker.opentrackr.org:1337/announce,udp://tracker.qu.ax:6969/announce,udp://tracker.skynetcloud.site:6969/announce,udp://tracker.skyts.net:6969/announce,udp://tracker.theoks.net:6969/announce,udp://tracker.tiny-vps.com:6969/announce,udp://tracker.torrent.eu.org:451/announce,udp://tracker1.bt.moack.co.kr:80/announce,udp://tracker2.dler.com:80/announce,udp://tracker6.lelux.fi:6969/announce,udp://u4.trakx.crim.ist:1337/announce,udp://uploads.gamecoast.net:6969/announce,udp://v1046920.hosted-by-vdsina.ru:6969/announce,udp://www.peckservers.com:9000/announce,ws://hub.bugout.link:80/announce,wss://tracker.openwebtorrent.com:443/announce
+http://1337.abcvg.info:80/announce,http://bt.endpot.com:80/announce,http://bt.okmp3.ru:2710/announce,http://incine.ru:6969/announce,http://nyaa.tracker.wf:7777/announce,http://open.acgnxtracker.com:80/announce,http://open.tracker.ink:6969/announce,http://p2p.0g.cx:6969/announce,http://parag.rs:6969/announce,http://share.camoe.cn:8080/announce,http://torrentsmd.com:8080/announce,http://tr.cili001.com:8070/announce,http://tracker.bt4g.com:2095/announce,http://tracker.files.fm:6969/announce,http://tracker.gbitt.info:80/announce,http://tracker.mywaifu.best:6969/announce,http://tracker.openbittorrent.com:80/announce,http://tracker.renfei.net:8080/announce,http://tracker.skyts.net:6969/announce,http://tracker.tfile.co:80/announce,http://trackme.theom.nz:80/announce,http://v6-tracker.0g.cx:6969/announce,http://www.all4nothin.net:80/announce.php,http://www.wareztorrent.com:80/announce,https://1337.abcvg.info:443/announce,https://opentracker.i2p.rocks:443/announce,https://t1.hloli.org:443/announce,https://tr.abiir.top:443/announce,https://tr.burnabyhighstar.com:443/announce,https://tracker.foreverpirates.co:443/announce,https://tracker.gbitt.info:443/announce,https://tracker.imgoingto.icu:443/announce,https://tracker.kuroy.me:443/announce,https://tracker.lilithraws.cf:443/announce,https://tracker.loligirl.cn:443/announce,https://tracker.tamersunion.org:443/announce,https://tracker1.520.jp:443/announce,https://trackme.theom.nz:443/announce,udp://9.rarbg.com:2810/announce,udp://aarsen.me:6969/announce,udp://acxx.de:6969/announce,udp://aegir.sexy:6969/announce,udp://astrr.ru:6969/announce,udp://bedro.cloud:6969/announce,udp://boysbitte.be:6969/announce,udp://bt.ktrackers.com:6666/announce,udp://bt1.archive.org:6969/announce,udp://epider.me:6969/announce,udp://exodus.desync.com:6969/announce,udp://htz3.noho.st:6969/announce,udp://ipv6.tracker.monitorit4.me:6969/announce,udp://laze.cc:6969/announce,udp://linfan.moe:6969/announce,udp://mail.artixlinux.org:6969/announce,udp://moonburrow.club:6969/announce,udp://movies.zsw.ca:6969/announce,udp://open.4ever.tk:6969/announce,udp://open.demonii.com:1337/announce,udp://open.dstud.io:6969/announce,udp://open.publictracker.xyz:6969/announce,udp://open.stealth.si:80/announce,udp://open.tracker.cl:1337/announce,udp://open.tracker.ink:6969/announce,udp://opentor.org:2710/announce,udp://opentracker.i2p.rocks:6969/announce,udp://opentracker.io:6969/announce,udp://p4p.arenabg.com:1337/announce,udp://private.anonseed.com:6969/announce,udp://retracker01-msk-virt.corbina.net:80/announce,udp://run.publictracker.xyz:6969/announce,udp://sanincode.com:6969/announce,udp://static.54.161.216.95.clients.your-server.de:6969/announce,udp://t.133335.xyz:6969/announce,udp://thagoat.rocks:6969/announce,udp://thetracker.org:80/announce,udp://torrents.artixlinux.org:6969/announce,udp://tracker-udp.gbitt.info:80/announce,udp://tracker.4.babico.name.tr:3131/announce,udp://tracker.altrosky.nl:6969/announce,udp://tracker.artixlinux.org:6969/announce,udp://tracker.auctor.tv:6969/announce,udp://tracker.beeimg.com:6969/announce,udp://tracker.birkenwald.de:6969/announce,udp://tracker.bitsearch.to:1337/announce,udp://tracker.ccp.ovh:6969/announce,udp://tracker.cyberia.is:6969/announce,udp://tracker.dler.com:6969/announce,udp://tracker.doko.moe:6969/announce,udp://tracker.filemail.com:6969/announce,udp://tracker.jonaslsa.com:6969/announce,udp://tracker.leech.ie:1337/announce,udp://tracker.moeking.me:6969/announce,udp://tracker.monitorit4.me:6969/announce,udp://tracker.openbittorrent.com:6969/announce,udp://tracker.opentrackr.org:1337/announce,udp://tracker.skyts.net:6969/announce,udp://tracker.srv00.com:6969/announce,udp://tracker.theoks.net:6969/announce,udp://tracker.torrent.eu.org:451/announce,udp://tracker1.bt.moack.co.kr:80/announce,udp://tracker2.dler.com:80/announce,udp://tracker6.lelux.fi:6969/announce,udp://u4.trakx.crim.ist:1337/announce,udp://u6.trakx.crim.ist:1337/announce,udp://uploads.gamecoast.net:6969/announce,udp://v1046920.hosted-by-vdsina.ru:6969/announce,udp://wepzone.net:6969/announce,ws://hub.bugout.link:80/announce,wss://tracker.openwebtorrent.com:443/announce
```

### Comparing `videobox-0.3.2/videobox/utilities.py` & `videobox-0.4.0/videobox/utilities.py`

 * *Files identical despite different names*

### Comparing `videobox-0.3.2/videobox.egg-info/PKG-INFO` & `videobox-0.4.0/videobox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videobox
-Version: 0.3.2
+Version: 0.4.0
 Summary: Video download CLI utility
 Author: Andrea Peltrin
 Project-URL: Homepage, https://github.com/passiomatic/videobox
 Project-URL: Bug Tracker, https://github.com/passiomatic/videobox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -35,38 +35,40 @@
 
 ## Quick guide
 
 First, tell Videobox to update its local database:
 
 ```
 $ videobox update
-First run: import running series... 
+First run: import full database...
 (...)
 ```
 
+This will copy the full Videobox database to your machine. Currently database contains about 1 year of releases and tracks more than 1.000 series.
+
 **Note**: Videobox will auto-update itself if local database hasn't been refreshed for a while.
 
-Find out what series are running:
+Find out which series have been updated this week:
 
 ```
 $ videobox running -y7
 Found 84 series updated in the last 7 days:
 (...)
 N
- · NCIS  CBS
- · NCIS: Hawai'i  CBS
- · NCIS: Los Angeles  CBS
+ · NCIS  #20
+ · NCIS: Hawai'i  #45271
+ · NCIS: Los Angeles  #20420
 ```
 
 Find out more about a specific series:
 
 ```
 $ videobox search ncis los angeles
 ------------------------------
-NCIS: Los Angeles  CBS
+NCIS: Los Angeles  #45  CBS
 ------------------------------
 NCIS: Los Angeles is a drama about the high stakes world of
 undercover surveillance at the Office of Special Projects
 (...)
 #Action #Adventure #Crime #Drama
 
 Found 1 season with a total of 15 episodes and 92 releases:
@@ -81,15 +83,15 @@
 More series info at <https://thetvdb.com/series/ncis-los-angeles>
 ```
 
 Download a whole series season without headaches:
 
 ```
 $ videobox download ncis los angeles -s14 --dry-run
-Ready to download 10 releases for series 'NCIS: Los Angeles':
+Ready to download 10 releases for season 14 for series 'NCIS: Los Angeles' into /Users/Alice/Downloads:
 
 Seeds  Res. Size   Name
 --------------------------------------------------------------------------------
   128 1080p 2.15GB ncis.los.angeles.s14e01.1080p.web.h264-glhf[eztv.re].mkv
   198 1080p 2.15GB NCIS.Los.Angeles.S14E02.1080p.WEB.h264-GOSSIP[eztv.re].mkv
   209 1080p 2.15GB NCIS.Los.Angeles.S14E03.1080p.WEB.h264-GOSSIP[eztv.re].mkv
 (...)
```

