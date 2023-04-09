# Comparing `tmp/m3u_to_pyradio_playlist-0.0.3.tar.gz` & `tmp/m3u_to_pyradio_playlist-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3u_to_pyradio_playlist-0.0.3.tar", last modified: Mon Mar 27 01:36:26 2023, max compression
+gzip compressed data, was "m3u_to_pyradio_playlist-0.0.4.tar", last modified: Sun Apr  9 18:13:56 2023, max compression
```

## Comparing `m3u_to_pyradio_playlist-0.0.3.tar` & `m3u_to_pyradio_playlist-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-03-27 01:36:26.363769 m3u_to_pyradio_playlist-0.0.3/
--rw-r--r--   0 rmj        (501) staff       (20)    18092 2023-03-21 20:35:50.000000 m3u_to_pyradio_playlist-0.0.3/LICENSE
--rw-r--r--   0 rmj        (501) staff       (20)     3882 2023-03-27 01:36:26.363551 m3u_to_pyradio_playlist-0.0.3/PKG-INFO
--rw-r--r--   0 rmj        (501) staff       (20)     3545 2023-03-27 00:56:04.000000 m3u_to_pyradio_playlist-0.0.3/README.md
-drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-03-27 01:36:26.360467 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/
--rw-r--r--   0 rmj        (501) staff       (20)      214 2023-03-27 01:22:18.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/__init__.py
--rw-r--r--   0 rmj        (501) staff       (20)     4918 2023-03-27 01:35:39.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/__main__.py
-drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-03-27 01:36:26.362056 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/converter/
--rw-r--r--   0 rmj        (501) staff       (20)       25 2023-03-27 01:21:19.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/converter/__init__.py
--rw-r--r--   0 rmj        (501) staff       (20)     1465 2023-03-27 00:56:09.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/converter/converter.py
-drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-03-27 01:36:26.362653 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/downloader/
--rw-r--r--   0 rmj        (501) staff       (20)       26 2023-03-27 01:21:20.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/downloader/__init__.py
--rw-r--r--   0 rmj        (501) staff       (20)      447 2023-03-25 01:28:07.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/downloader/downloader.py
-drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-03-27 01:36:26.363174 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/utils/
--rw-r--r--   0 rmj        (501) staff       (20)       21 2023-03-27 01:21:21.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/utils/__init__.py
--rw-r--r--   0 rmj        (501) staff       (20)      136 2023-03-22 01:10:16.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/utils/utils.py
-drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-03-27 01:36:26.361641 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist.egg-info/
--rw-r--r--   0 rmj        (501) staff       (20)     3882 2023-03-27 01:36:26.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist.egg-info/PKG-INFO
--rw-r--r--   0 rmj        (501) staff       (20)      652 2023-03-27 01:36:26.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist.egg-info/SOURCES.txt
--rw-r--r--   0 rmj        (501) staff       (20)        1 2023-03-27 01:36:26.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist.egg-info/dependency_links.txt
--rw-r--r--   0 rmj        (501) staff       (20)       73 2023-03-27 01:36:26.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist.egg-info/entry_points.txt
--rw-r--r--   0 rmj        (501) staff       (20)        9 2023-03-27 01:36:26.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist.egg-info/requires.txt
--rw-r--r--   0 rmj        (501) staff       (20)       24 2023-03-27 01:36:26.000000 m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist.egg-info/top_level.txt
--rw-r--r--   0 rmj        (501) staff       (20)       38 2023-03-27 01:36:26.363829 m3u_to_pyradio_playlist-0.0.3/setup.cfg
--rw-r--r--   0 rmj        (501) staff       (20)     1000 2023-03-27 01:11:18.000000 m3u_to_pyradio_playlist-0.0.3/setup.py
+drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-04-09 18:13:56.428012 m3u_to_pyradio_playlist-0.0.4/
+-rw-r--r--   0 rmj        (501) staff       (20)    18092 2023-03-21 20:35:50.000000 m3u_to_pyradio_playlist-0.0.4/LICENSE
+-rw-r--r--   0 rmj        (501) staff       (20)     3882 2023-04-09 18:13:56.427857 m3u_to_pyradio_playlist-0.0.4/PKG-INFO
+-rw-r--r--   0 rmj        (501) staff       (20)     3545 2023-03-27 00:56:04.000000 m3u_to_pyradio_playlist-0.0.4/README.md
+drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-04-09 18:13:56.424914 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/
+-rw-r--r--   0 rmj        (501) staff       (20)      214 2023-04-09 18:10:59.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/__init__.py
+-rw-r--r--   0 rmj        (501) staff       (20)     4918 2023-03-27 01:35:39.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/__main__.py
+drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-04-09 18:13:56.426412 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/converter/
+-rw-r--r--   0 rmj        (501) staff       (20)       25 2023-03-27 01:21:19.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/converter/__init__.py
+-rw-r--r--   0 rmj        (501) staff       (20)     1892 2023-04-09 18:04:19.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/converter/converter.py
+drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-04-09 18:13:56.426914 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/downloader/
+-rw-r--r--   0 rmj        (501) staff       (20)       26 2023-03-27 01:21:20.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/downloader/__init__.py
+-rw-r--r--   0 rmj        (501) staff       (20)      447 2023-03-25 01:28:07.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/downloader/downloader.py
+drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-04-09 18:13:56.427465 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/utils/
+-rw-r--r--   0 rmj        (501) staff       (20)       21 2023-03-27 01:21:21.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/utils/__init__.py
+-rw-r--r--   0 rmj        (501) staff       (20)      136 2023-03-22 01:10:16.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/utils/utils.py
+drwxr-xr-x   0 rmj        (501) staff       (20)        0 2023-04-09 18:13:56.425972 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist.egg-info/
+-rw-r--r--   0 rmj        (501) staff       (20)     3882 2023-04-09 18:13:56.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist.egg-info/PKG-INFO
+-rw-r--r--   0 rmj        (501) staff       (20)      652 2023-04-09 18:13:56.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist.egg-info/SOURCES.txt
+-rw-r--r--   0 rmj        (501) staff       (20)        1 2023-04-09 18:13:56.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist.egg-info/dependency_links.txt
+-rw-r--r--   0 rmj        (501) staff       (20)       73 2023-04-09 18:13:56.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist.egg-info/entry_points.txt
+-rw-r--r--   0 rmj        (501) staff       (20)        9 2023-04-09 18:13:56.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist.egg-info/requires.txt
+-rw-r--r--   0 rmj        (501) staff       (20)       24 2023-04-09 18:13:56.000000 m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist.egg-info/top_level.txt
+-rw-r--r--   0 rmj        (501) staff       (20)       38 2023-04-09 18:13:56.428058 m3u_to_pyradio_playlist-0.0.4/setup.cfg
+-rw-r--r--   0 rmj        (501) staff       (20)     1000 2023-03-27 01:11:18.000000 m3u_to_pyradio_playlist-0.0.4/setup.py
```

### Comparing `m3u_to_pyradio_playlist-0.0.3/LICENSE` & `m3u_to_pyradio_playlist-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `m3u_to_pyradio_playlist-0.0.3/PKG-INFO` & `m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: m3u_to_pyradio_playlist
-Version: 0.0.3
+Name: m3u-to-pyradio-playlist
+Version: 0.0.4
 Summary: Converts M3U playlists to pyradio format
 Home-page: https://github.com/LionyxML/pyradio-m3u-to-playlist
 Author: Rahul M. Juliato
 Author-email: rahul.juliato@gmail.com
 License: GPL-2.0
 Platform: Any
 Description-Content-Type: text/markdown
```

### Comparing `m3u_to_pyradio_playlist-0.0.3/README.md` & `m3u_to_pyradio_playlist-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/__main__.py` & `m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/__main__.py`

 * *Files identical despite different names*

### Comparing `m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist/converter/converter.py` & `m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist/converter/converter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 """Functions used to convert m3u to CSV."""
 
 last_group = ''
 
 def html_entities_to_unicode_chars(a_string: str) -> str:
+    """ replace HTML entities found in text
+        refer to doc/html-entities.md for more info
+
+        &quot; will be replaced by ” (U+201D)
+        instead of a regular " (U+0022)
+    """
     ent = {
         '&#039;': "'",
         '&#1110;': 'і',
         '&#225;': 'á',
         '&#227;': 'ã',
         '&#39;': "'",
         '&#47;': '/',
         '&#93;': ']',
         '&amp;': '&',
         '&apos;': "'",
         '&gt;': '>',
-        '&quot;': '"',
+        '&quot;': '”',
         '&#xe1;': 'á',
     }
     for n in ent.keys():
         a_string = a_string.replace(n, ent[n])
     return a_string
 
 def create_csv_line(index: int, line: str, fullList: list) -> str:
     """Format a CSV line from m3u."""
     global last_group
     if line.startswith("#"):
         return None
 
+    # just to be in the safe side
+    line = line.replace('"', '&quot;')
+
     try:
         group, title = fullList[index - 1].split('" group-title="')[1].split('", ')
     except IndexError:
         title = fullList[index - 1].split(",")[-1]
         group = ''
+    try:
+        logo = fullList[index - 1].split(' tvg-logo="')[1].split('", ')[0].split('" ')[0]
+    except IndexError:
+        logo = ''
 
     if group != last_group:
-        out = f'"{group}",-\n"{title}",{line}'
+        out = f'"{group}",-,,\n"{title}",{line},,{logo}'
         last_group = group
     else:
-        out = f'"{title}",{line}'
+        out = f'"{title}",{line},,{logo}'
     return html_entities_to_unicode_chars(out)
 
 def convert_m3u_to_csv(m3u_content: list) -> list:
     """Given the content of a m3u file, returns the contents for a CSV file."""
     if not isinstance(m3u_content, (list)):
         return []
```

### Comparing `m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist.egg-info/PKG-INFO` & `m3u_to_pyradio_playlist-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: m3u-to-pyradio-playlist
-Version: 0.0.3
+Name: m3u_to_pyradio_playlist
+Version: 0.0.4
 Summary: Converts M3U playlists to pyradio format
 Home-page: https://github.com/LionyxML/pyradio-m3u-to-playlist
 Author: Rahul M. Juliato
 Author-email: rahul.juliato@gmail.com
 License: GPL-2.0
 Platform: Any
 Description-Content-Type: text/markdown
```

### Comparing `m3u_to_pyradio_playlist-0.0.3/m3u_to_pyradio_playlist.egg-info/SOURCES.txt` & `m3u_to_pyradio_playlist-0.0.4/m3u_to_pyradio_playlist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m3u_to_pyradio_playlist-0.0.3/setup.py` & `m3u_to_pyradio_playlist-0.0.4/setup.py`

 * *Files identical despite different names*

