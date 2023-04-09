# Comparing `tmp/lastfm-cli-scrobbler-0.1.0.tar.gz` & `tmp/lastfm-cli-scrobbler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastfm-cli-scrobbler-0.1.0.tar", last modified: Sat Mar  6 18:05:08 2021, max compression
+gzip compressed data, was "lastfm-cli-scrobbler-0.1.1.tar", last modified: Sun Apr  9 20:13:12 2023, max compression
```

## Comparing `lastfm-cli-scrobbler-0.1.0.tar` & `lastfm-cli-scrobbler-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,11 @@
-drwxr-xr-x   0 maxim     (1000) maxim     (1000)        0 2021-03-06 18:05:08.396697 lastfm-cli-scrobbler-0.1.0/
--rw-r--r--   0 maxim     (1000) maxim     (1000)     1075 2020-07-07 17:25:06.000000 lastfm-cli-scrobbler-0.1.0/LICENSE
--rw-r--r--   0 maxim     (1000) maxim     (1000)       15 2021-03-06 18:02:09.000000 lastfm-cli-scrobbler-0.1.0/MANIFEST.in
--rw-r--r--   0 maxim     (1000) maxim     (1000)     2396 2021-03-06 18:05:08.396697 lastfm-cli-scrobbler-0.1.0/PKG-INFO
--rw-r--r--   0 maxim     (1000) maxim     (1000)     1144 2020-10-14 20:15:11.000000 lastfm-cli-scrobbler-0.1.0/README.md
-drwxr-xr-x   0 maxim     (1000) maxim     (1000)        0 2021-03-06 18:05:08.393363 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler/
--rw-r--r--   0 maxim     (1000) maxim     (1000)        0 2021-03-06 18:04:47.000000 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler/__init__.py
--rwxr--r--   0 maxim     (1000) maxim     (1000)     5927 2021-03-06 18:01:44.000000 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler/last_my.py
--rwxr--r--   0 maxim     (1000) maxim     (1000)     3137 2021-03-06 18:01:46.000000 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler/last_pylast.py
-drwxr-xr-x   0 maxim     (1000) maxim     (1000)        0 2021-03-06 18:05:08.396697 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler.egg-info/
--rw-r--r--   0 maxim     (1000) maxim     (1000)     2396 2021-03-06 18:05:08.000000 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler.egg-info/PKG-INFO
--rw-r--r--   0 maxim     (1000) maxim     (1000)      415 2021-03-06 18:05:08.000000 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler.egg-info/SOURCES.txt
--rw-r--r--   0 maxim     (1000) maxim     (1000)        1 2021-03-06 18:05:08.000000 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler.egg-info/dependency_links.txt
--rw-r--r--   0 maxim     (1000) maxim     (1000)      114 2021-03-06 18:05:08.000000 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler.egg-info/entry_points.txt
--rw-r--r--   0 maxim     (1000) maxim     (1000)       24 2021-03-06 18:05:08.000000 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler.egg-info/requires.txt
--rw-r--r--   0 maxim     (1000) maxim     (1000)       21 2021-03-06 18:05:08.000000 lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler.egg-info/top_level.txt
--rw-r--r--   0 maxim     (1000) maxim     (1000)     1059 2021-03-06 18:05:08.396697 lastfm-cli-scrobbler-0.1.0/setup.cfg
--rw-r--r--   0 maxim     (1000) maxim     (1000)       38 2021-03-06 18:00:12.000000 lastfm-cli-scrobbler-0.1.0/setup.py
+drwxr-xr-x   0 maxim     (1000) maxim     (1000)        0 2023-04-09 20:13:12.445291 lastfm-cli-scrobbler-0.1.1/
+-rw-r--r--   0 maxim     (1000) maxim     (1000)     1075 2023-04-09 19:41:11.000000 lastfm-cli-scrobbler-0.1.1/LICENSE
+-rw-r--r--   0 maxim     (1000) maxim     (1000)       16 2023-04-09 20:01:11.000000 lastfm-cli-scrobbler-0.1.1/MANIFEST.in
+-rw-r--r--   0 maxim     (1000) maxim     (1000)     2254 2023-04-09 20:13:12.445291 lastfm-cli-scrobbler-0.1.1/PKG-INFO
+-rw-r--r--   0 maxim     (1000) maxim     (1000)     1297 2023-04-09 19:41:11.000000 lastfm-cli-scrobbler-0.1.1/README.md
+drwxr-xr-x   0 maxim     (1000) maxim     (1000)        0 2023-04-09 20:13:12.445291 lastfm-cli-scrobbler-0.1.1/lastfm_cli_scrobbler/
+-rw-r--r--   0 maxim     (1000) maxim     (1000)        0 2021-03-06 18:04:47.000000 lastfm-cli-scrobbler-0.1.1/lastfm_cli_scrobbler/__init__.py
+-rwxr-xr-x   0 maxim     (1000) maxim     (1000)     6172 2023-04-09 19:41:11.000000 lastfm-cli-scrobbler-0.1.1/lastfm_cli_scrobbler/last_my.py
+-rwxr-xr-x   0 maxim     (1000) maxim     (1000)     3319 2023-04-09 19:41:11.000000 lastfm-cli-scrobbler-0.1.1/lastfm_cli_scrobbler/last_pylast.py
+-rw-r--r--   0 maxim     (1000) maxim     (1000)     1115 2023-04-09 20:13:12.445291 lastfm-cli-scrobbler-0.1.1/setup.cfg
+-rw-r--r--   0 maxim     (1000) maxim     (1000)       37 2021-03-06 18:13:16.000000 lastfm-cli-scrobbler-0.1.1/setup.py
```

### Comparing `lastfm-cli-scrobbler-0.1.0/LICENSE` & `lastfm-cli-scrobbler-0.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Maksim Terpilowski
+Copyright (c) 2023 Maksim Terpilowski
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `lastfm-cli-scrobbler-0.1.0/README.md` & `lastfm-cli-scrobbler-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Last.fm CLI Scrobbler
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/2ef30d84737c4e509dd16a45e63b8d98)](https://www.codacy.com/gh/maximtrp/lastfm-cli-scrobbler/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=maximtrp/lastfm-cli-scrobbler&amp;utm_campaign=Badge_Grade)
+![PyPI](https://img.shields.io/pypi/v/lastfm-cli-scrobbler)
+[![Downloads](https://pepy.tech/badge/lastfm-cli-scrobbler)](https://pepy.tech/project/lastfm-cli-scrobbler)
 
 This is a simple Last.fm command-line scrobbler written in Python.
 
 ## Installation
 
+### PyPi
+
 ```bash
-$ pip install git+https://github.com/maximtrp/lastfm-cli-scrobbler.git
+pip install lastfm-cli-scrobbler
 ```
 
-Or you may clone this repo and install it using:
+### GitHub repo
 
 ```bash
-$ pip install .
+pip install git+https://github.com/maximtrp/lastfm-cli-scrobbler.git
 ```
 
 ## Usage 
 
 After the installation, two commands will be available: `scrobble` (my own API implementation) and `scrobble2` (`pylast` API implementation).
 
 ```bash
@@ -29,12 +33,12 @@
 ```
 
 Pylast-based version is probably more stable, but my own implementation of Last.fm API returns the full log (and shows a cross instead of a check if a track was ignored):
 
 ```bash
 $ scrobble {01..04}*.flac
 Scrobbling report:
-[✔] Shuttle358 - Ash
-[✔] Shuttle358 - Chessa
-[✔] Shuttle358 - Blast
-[✔] Shuttle358 - Duh
+[v] Shuttle358 - Ash
+[v] Shuttle358 - Chessa
+[v] Shuttle358 - Blast
+[v] Shuttle358 - Duh
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler/last_my.py` & `lastfm-cli-scrobbler-0.1.1/lastfm_cli_scrobbler/last_my.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,106 +1,111 @@
 #!/usr/bin/python
+"""Last.fm CLI scrobbler implementation"""
 
-from yaml import safe_load as yaml_load, dump as yaml_dump
-from glob import glob
 from os.path import exists, isdir, expanduser
-from requests import post
+from glob import glob
 from getpass import getpass
 from time import time
 from hashlib import md5
 from optparse import OptionParser
+from yaml import safe_load as yaml_load, dump as yaml_dump
+from requests import post
 from mutagen import File as MutagenFile
 
 
-# Signature strings and url paramaters dicts
 def make_string(lst, prefix):
-    n = len(lst)
+    """Signature strings and url paramaters dicts"""
+    lst_len = len(lst)
     prefixed_lst = sorted(list(zip(
-        ['%s[%d]' % (prefix, i) for i in range(n)],
+        [f'{prefix}[{i}]' for i in range(lst_len)],
         lst
     )))
     prefixed_lst_filtered = list(filter(lambda x: x[1], prefixed_lst))
     prefixed_dict = dict(prefixed_lst_filtered)
     return (
         "".join(map("".join, prefixed_lst_filtered)),
         prefixed_dict
     )
 
 
 def main():
+    """CLI entrypoint function"""
 
     # Parsing command-line arguments
     parser = OptionParser(usage="Usage: %prog [FILES]")
     _, args = parser.parse_args()
 
     # Checking credentials and loading data if exists
     credentials_fn = expanduser('~/.lastfm_scrobbler')
     logged_in = False
 
     if exists(credentials_fn):
-        with open(credentials_fn) as file:
+        with open(credentials_fn, encoding='utf8') as file:
             creds = yaml_load(file) or {}
     else:
         creds = {}
 
     creds_ready = set([
         'username', 'secret', 'api_key', 'session_key'
     ]).issubset(creds)
 
     if not creds_ready:
 
         print('[x] Auth keys not found')
         while not logged_in:
             username = input('[?] Enter your username: ')
             password = getpass('[?] Enter your password: ')
-            print('[!] Please create an API account: https://www.last.fm/api/account/create')
+            print(
+                '[!] Please create an API account: '
+                'https://www.last.fm/api/account/create')
             api_key = getpass('[?] Enter your API key: ')
             secret = getpass('[?] Enter your API secret: ')
 
             api_sig = md5(bytes(
-                'api_key{}methodauth.getmobilesessionpassword{}username{}{}'
-                .format(api_key, password, username, secret), encoding='utf8')
+                f'api_key{api_key}'
+                f'methodauth.getmobilesessionpassword{password}'
+                f'username{username}{secret}', encoding='utf8')
             ).hexdigest()
             session_url = 'https://ws.audioscrobbler.com/2.0/'
             params = {
                 'method': 'auth.getmobilesession', 'format': 'json',
                 'api_key': api_key, 'api_sig': api_sig, 'password': password,
                 'username': username
             }
-            response = post(session_url, data=params).json()
+            response = post(session_url, data=params, timeout=30).json()
 
             if 'error' in response:
                 print('[x] Error:', response['message'])
                 print('[!] Making another attempt...')
             else:
                 logged_in = True
                 session_key = response['session']['key']
                 creds['api_key'] = api_key
                 creds['secret'] = secret
                 creds['session_key'] = session_key
-                with open(credentials_fn, 'wt') as file:
+                with open(credentials_fn, 'wt', encoding='utf8') as file:
                     yaml_dump(creds, file)
                 print('[v] Session key was obtained successfully\n')
 
     items = args if args else glob('*')
     files = filter(lambda x: not isdir(x), items)
     tracks_info = {}
     cum_length = 0
     timestamp_now = int(time())
 
     for file in files:
-        ft = MutagenFile(file, easy=True)
-        if not ft:
+        filetype = MutagenFile(file, easy=True)
+        if not filetype:
             continue
 
-        artist, albumartist, track, album = ft.get('artist', [None])[0],\
-            ft.get('albumartist', [None])[0],\
-            ft.get('title', [None])[0],\
-            ft.get('album', [None])[0]
-        length = int(ft.info.length)
+        artist, albumartist, track, album = filetype.get('artist', [None])[0],\
+            filetype.get('albumartist', [None])[0],\
+            filetype.get('title', [None])[0],\
+            filetype.get('album', [None])[0]
+        length = int(filetype.info.length)
         cum_length += length
         timestamp = str(timestamp_now - cum_length)
         tracks_info.update({
             timestamp: {
                 'file': file, 'album': album, 'track': track,
                 'artist': artist, 'albumartist': albumartist
             }
@@ -130,46 +135,49 @@
         albumartists.append(albumartist)
         albums.append(album)
         timestamps.append(timestamp)
 
     artists_sig, artists_url = make_string(artists, 'artist')
     tracks_sig, tracks_url = make_string(tracks, 'track')
     albums_sig, albums_url = make_string(albums, 'album')
-    albumartists_sig, albumartists_url = make_string(albumartists, 'albumartist')
+    albumartists_sig, albumartists_url = make_string(
+        albumartists, 'albumartist')
     timestamps_sig, timestamps_url = make_string(timestamps, 'timestamp')
 
-    api_sig = md5(bytes('{}{}api_key{}{}methodtrack.scrobblesk{}{}{}{}'.format(
-        albums_sig, albumartists_sig, creds['api_key'], artists_sig, creds['session_key'],
-        timestamps_sig, tracks_sig, creds['secret']), encoding='utf8')
+    api_sig = md5(bytes(''.join([
+        albums_sig, albumartists_sig, "api_key", creds[
+            'api_key'], artists_sig, "methodtrack.scrobblesk", creds['session_key'],
+        timestamps_sig, tracks_sig, creds['secret']]), encoding='utf8')
     ).hexdigest()
 
     # Parameters init and scrobbling
     params = {
         'api_key': creds['api_key'], 'api_sig': api_sig, 'sk': creds['session_key'],
         'method': 'track.scrobble', 'format': 'json'
     }
     params.update(albums_url)
     params.update(artists_url)
     params.update(albumartists_url)
     params.update(timestamps_url)
     params.update(tracks_url)
 
-    response = post('https://ws.audioscrobbler.com/2.0/', data=params)
+    response = post('https://ws.audioscrobbler.com/2.0/',
+                    data=params, timeout=30)
     result = response.json()
 
     if 'scrobbles' in result:
         print('Scrobbling report:')
         scrobbles = result['scrobbles']['scrobble']
         if not isinstance(scrobbles, list):
             scrobbles = [scrobbles]
 
         for scrobble in scrobbles:
             track = tracks_info[str(scrobble['timestamp'])]
-            status = '[{}]'.format('x' if scrobble['ignoredMessage']['code'] == '1' else '✔')
-            print('{} {} - {}'.format(status, track['artist'], track['track']))
+            status = 'x' if scrobble['ignoredMessage']['code'] == '1' else '✔'
+            print(f'[{status}] {track["artist"]} - {track["track"]}')
 
     elif 'error' in result:
         print('Error:', result['message'])
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `lastfm-cli-scrobbler-0.1.0/lastfm_cli_scrobbler/last_pylast.py` & `lastfm-cli-scrobbler-0.1.1/lastfm_cli_scrobbler/last_pylast.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/usr/bin/python
+"""Last.fm CLI scrobbler implementation based on pylast"""
 
-from yaml import safe_load as yaml_load, dump as yaml_dump
 from glob import glob
 from os.path import exists, isdir, expanduser
-from getpass import getpass
 from time import time
-from pylast import LastFMNetwork, md5
 from optparse import OptionParser
+from getpass import getpass
+from yaml import safe_load as yaml_load, dump as yaml_dump
 from mutagen import File as MutagenFile
+from pylast import LastFMNetwork, md5
 
 
 def main():
+    """CLI entrypoint function"""
 
     # Parsing command-line arguments
     parser = OptionParser(usage="Usage: %prog [FILES]")
     _, args = parser.parse_args()
 
     # Checking credentials and loading data if exists
     credentials_fn = expanduser('~/.lastfm_scrobbler')
 
     if exists(credentials_fn):
-        with open(credentials_fn) as file:
+        with open(credentials_fn, encoding='utf8') as file:
             creds = yaml_load(file) or {}
     else:
         creds = {}
 
     creds_ready = set([
         'username', 'secret', 'api_key', 'session_key'
     ]).issubset(creds)
@@ -50,62 +52,63 @@
 
     try:
         network = LastFMNetwork(
             api_key=api_key, api_secret=secret,
             username=username, session_key=session_key,
             password_hash=password_hash
         )
-    except Exception as e:
-        print('[x] Auth unsuccessful:', str(e))
+
+    except Exception as exc:
+        print('[x] Auth unsuccessful:', str(exc))
         exit(1)
 
     creds['api_key'] = api_key
     creds['secret'] = secret
     creds['session_key'] = network.session_key
     creds['username'] = username
 
-    with open(credentials_fn, 'wt') as file:
+    with open(credentials_fn, 'wt', encoding='utf8') as file:
         yaml_dump(creds, file)
 
-    print('[v] Auth successful')
+    print('[✔] Auth successful')
 
     items = args if args else glob('*')
     files = filter(lambda x: not isdir(x), items)
     tracks = []
     cum_length = 0
     timestamp_now = int(time())
 
     for file in files:
-        ft = MutagenFile(file, easy=True)
-        if not ft:
+        filetype = MutagenFile(file, easy=True)
+        if not filetype:
             continue
 
-        artist = ft.get('artist', [None])[0]
-        album_artist = ft.get('albumartist', [None])[0]
-        title = ft.get('title', [None])[0]
-        album = ft.get('album', [None])[0]
+        artist = filetype.get('artist', [None])[0]
+        album_artist = filetype.get('albumartist', [None])[0]
+        title = filetype.get('title', [None])[0]
+        album = filetype.get('album', [None])[0]
 
         if not artist or not title:
             print('[x] Skipping file:', file)
             continue
 
-        duration = int(ft.info.length)
+        duration = int(filetype.info.length)
         cum_length += duration
         timestamp = str(timestamp_now - cum_length)
         tracks.append({
             'artist': artist,
             'album_artist': album_artist,
             'title': title,
             'album': album,
             'duration': duration,
             'timestamp': timestamp
         })
 
     try:
         network.scrobble_many(tracks)
-        print('[v] Scrobbling successful')
-    except Exception as e:
-        print('[x] Scrobbling unsuccessful:', str(e))
+        print('[✔] Scrobbling successful')
+    except Exception as exc:
+        print('[x] Scrobbling unsuccessful:', str(exc))
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lastfm-cli-scrobbler-0.1.0/setup.cfg` & `lastfm-cli-scrobbler-0.1.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lastfm-cli-scrobbler
-version = 0.1.0
+version = 0.1.1
 description = Last.fm CLI Scrobbler
 url = https://github.com/maximtrp/lastfm-cli-scrobbler
 author = Maksim Terpilowski
 author_email = maximtrp@gmail.com
 keywords = python, lastfm, cli, scrobbler
 classifiers = 
 	Development Status :: 3 - Alpha
@@ -15,14 +15,15 @@
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 python_requires = >=3.5
 packages = find:
 install_requires = 
@@ -32,10 +33,11 @@
 
 [options.entry_points]
 console_scripts = 
 	scrobble = lastfm_cli_scrobbler.last_my:main
 	scrobble2 = lastfm_cli_scrobbler.last_pylast:main
 
 [egg_info]
+egg_base = /tmp
 tag_build = 
 tag_date = 0
```

