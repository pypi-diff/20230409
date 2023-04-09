# Comparing `tmp/spotify_to_ytmusic-0.1.1.tar.gz` & `tmp/spotify_to_ytmusic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_to_ytmusic-0.1.1.tar", last modified: Sat Apr  8 18:53:20 2023, max compression
+gzip compressed data, was "spotify_to_ytmusic-0.1.2.tar", last modified: Sun Apr  9 19:29:00 2023, max compression
```

## Comparing `spotify_to_ytmusic-0.1.1.tar` & `spotify_to_ytmusic-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.520875 spotify_to_ytmusic-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.508875 spotify_to_ytmusic-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.512875 spotify_to_ytmusic-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-08 18:53:20.516875 spotify_to_ytmusic-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 18:53:20.520875 spotify_to_ytmusic-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.516875 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/match.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/settings.ini.example
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.516875 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.516875 spotify_to_ytmusic-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/tests/test_spotipy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/tests/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.662665 spotify_to_ytmusic-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.658666 spotify_to_ytmusic-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.658666 spotify_to_ytmusic-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-09 19:29:00.662665 spotify_to_ytmusic-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:29:00.662665 spotify_to_ytmusic-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.658666 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/settings.ini.example
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.662665 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.662665 spotify_to_ytmusic-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/tests/test_spotipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/tests/test_youtube.py
```

### Comparing `spotify_to_ytmusic-0.1.1/.github/workflows/coverage.yml` & `spotify_to_ytmusic-0.1.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.1/.github/workflows/pythonpublish.yml` & `spotify_to_ytmusic-0.1.2/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.1/.gitignore` & `spotify_to_ytmusic-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.1/LICENSE` & `spotify_to_ytmusic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.1/PKG-INFO` & `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spotify_to_ytmusic
-Version: 0.1.1
+Name: spotify-to-ytmusic
+Version: 0.1.2
 Summary: Transfer Spotify playlists to YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -86,38 +86,40 @@
 1. Generate a new app at https://developer.spotify.com/dashboard
 2. Run
 
 .. code-block::
 
     spotify_to_ytmusic setup
 
-For backwards compatibility you can also create your own file and pass it using `--file settings.ini`.
+For backwards compatibility you can also create your own file and pass it using ``--file settings.ini``.
 
 Usage
 ------
 
 After you've completed setup, you can simply run the script from the command line using:
+
 .. code-block::
 
     spotify_to_ytmusic create <spotifylink>
 
-where `<spotifylink>` is a link like https://open.spotify.com/playlist/0S0cuX8pnvmF7gA47Eu63M
+where ``<spotifylink>`` is a link like https://open.spotify.com/playlist/0S0cuX8pnvmF7gA47Eu63M
 
 The script will log its progress and output songs that were not found in YouTube Music to **noresults.txt**.
 
 Transfer all playlists of a Spotify user
 ----------------------------------------
 
 For migration purposes, it is possible to transfer all public playlists of a user by using the Spotify user's ID (unique username).
 
 .. code-block::
 
     spotify_to_ytmusic all <spotifyuserid>
 
-## Command line options
+Command line options
+---------------------
 
 There are some additional command line options for setting the playlist name and determining whether it's public or not. To view them, run
 
 .. code::
 
     spotify_to_ytmusic -h
```

### Comparing `spotify_to_ytmusic-0.1.1/README.rst` & `spotify_to_ytmusic-0.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -46,38 +46,40 @@
 1. Generate a new app at https://developer.spotify.com/dashboard
 2. Run
 
 .. code-block::
 
     spotify_to_ytmusic setup
 
-For backwards compatibility you can also create your own file and pass it using `--file settings.ini`.
+For backwards compatibility you can also create your own file and pass it using ``--file settings.ini``.
 
 Usage
 ------
 
 After you've completed setup, you can simply run the script from the command line using:
+
 .. code-block::
 
     spotify_to_ytmusic create <spotifylink>
 
-where `<spotifylink>` is a link like https://open.spotify.com/playlist/0S0cuX8pnvmF7gA47Eu63M
+where ``<spotifylink>`` is a link like https://open.spotify.com/playlist/0S0cuX8pnvmF7gA47Eu63M
 
 The script will log its progress and output songs that were not found in YouTube Music to **noresults.txt**.
 
 Transfer all playlists of a Spotify user
 ----------------------------------------
 
 For migration purposes, it is possible to transfer all public playlists of a user by using the Spotify user's ID (unique username).
 
 .. code-block::
 
     spotify_to_ytmusic all <spotifyuserid>
 
-## Command line options
+Command line options
+---------------------
 
 There are some additional command line options for setting the playlist name and determining whether it's public or not. To view them, run
 
 .. code::
 
     spotify_to_ytmusic -h
```

### Comparing `spotify_to_ytmusic-0.1.1/pyproject.toml` & `spotify_to_ytmusic-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/controllers.py` & `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/controllers.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         count = count + 1
         try:
             playlist = spotify.getSpotifyPlaylist(p["external_urls"]["spotify"])
             videoIds = ytmusic.search_songs(playlist["tracks"])
             playlist_id = ytmusic.create_playlist(
                 p["name"],
                 p["description"],
-                "PUBLIC" if p['public'] else "PRIVATE",
+                "PUBLIC" if p["public"] else "PRIVATE",
                 videoIds,
             )
             print(playlist_id)
         except Exception as ex:
             print(f"Could not transfer playlist {p['name']}. {str(ex)}")
```

### Comparing `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/main.py` & `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,20 +62,17 @@
     remove_parser = subparsers.add_parser(
         "remove", help="Remove playlists with specified regex pattern."
     )
     remove_parser.set_defaults(func=controllers.remove)
     remove_parser.add_argument("pattern", help="regex pattern")
 
     all_parser = subparsers.add_parser(
-        "all",
-        help="Transfer all public playlists of the specified user (Spotify User ID)."
-    )
-    all_parser.add_argument(
-        "user", type=str, help="Spotify userid of the specified user."
+        "all", help="Transfer all public playlists of the specified user (Spotify User ID)."
     )
+    all_parser.add_argument("user", type=str, help="Spotify userid of the specified user.")
     all_parser.set_defaults(func=controllers.all)
 
     return parser.parse_args(args)
 
 
 def main():
     args = get_args()
```

### Comparing `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/match.py` & `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/match.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/settings.py` & `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/settings.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/setup.py` & `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import shutil
 import sys
 from pathlib import Path
 from typing import Optional
 
 import ytmusicapi
 
@@ -25,15 +26,15 @@
     elif choice == choices[2]:
         setup_spotify()
         setup_youtube()
 
 
 def setup_youtube():
     settings = Settings()
-    settings["youtube"]["headers"] = ytmusicapi.setup_oauth()
+    settings["youtube"]["headers"] = json.dumps(ytmusicapi.setup_oauth())
     settings.save()
 
 
 def setup_spotify():
     settings = Settings()
     credentials = {
         "client_credentials": input(
```

### Comparing `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/spotify.py` & `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/spotify.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,27 +49,14 @@
             results = self.api.user_playlists(user, offset=count * 50)["items"]
             pl.extend(results)
             more = len(results) == 50
             count = count + 1
 
         return [p for p in pl if p["owner"]["id"] == user and p["tracks"]["total"] > 0]
 
-    def get_tracks(self, url):
-        tracks = []
-        url_parts = parse_url(url)
-        path = url_parts.path.split("/")
-        id = path[2]
-        if "album" == path[1]:
-            album = self.api.album(id)
-            tracks.extend(build_results(album["tracks"]["items"], album["name"]))
-        elif "track" == path[1]:
-            track = self.api.track(id)
-            tracks.extend(build_results([track]))
-        return tracks
-
 
 def build_results(tracks, album=None):
     results = []
     for track in tracks:
         if "track" in track:
             track = track["track"]
         if not track or track["duration_ms"] == 0:
```

### Comparing `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/ytmusic.py` & `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/ytmusic.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/PKG-INFO` & `spotify_to_ytmusic-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spotify-to-ytmusic
-Version: 0.1.1
+Name: spotify_to_ytmusic
+Version: 0.1.2
 Summary: Transfer Spotify playlists to YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -86,38 +86,40 @@
 1. Generate a new app at https://developer.spotify.com/dashboard
 2. Run
 
 .. code-block::
 
     spotify_to_ytmusic setup
 
-For backwards compatibility you can also create your own file and pass it using `--file settings.ini`.
+For backwards compatibility you can also create your own file and pass it using ``--file settings.ini``.
 
 Usage
 ------
 
 After you've completed setup, you can simply run the script from the command line using:
+
 .. code-block::
 
     spotify_to_ytmusic create <spotifylink>
 
-where `<spotifylink>` is a link like https://open.spotify.com/playlist/0S0cuX8pnvmF7gA47Eu63M
+where ``<spotifylink>`` is a link like https://open.spotify.com/playlist/0S0cuX8pnvmF7gA47Eu63M
 
 The script will log its progress and output songs that were not found in YouTube Music to **noresults.txt**.
 
 Transfer all playlists of a Spotify user
 ----------------------------------------
 
 For migration purposes, it is possible to transfer all public playlists of a user by using the Spotify user's ID (unique username).
 
 .. code-block::
 
     spotify_to_ytmusic all <spotifyuserid>
 
-## Command line options
+Command line options
+---------------------
 
 There are some additional command line options for setting the playlist name and determining whether it's public or not. To view them, run
 
 .. code::
 
     spotify_to_ytmusic -h
```

### Comparing `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/SOURCES.txt` & `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

