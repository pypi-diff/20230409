# Comparing `tmp/dmp3-0.0.6.tar.gz` & `tmp/dmp3-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmp3-0.0.6.tar", last modified: Fri Apr  7 16:30:48 2023, max compression
+gzip compressed data, was "dmp3-0.0.7.tar", last modified: Sun Apr  9 14:10:21 2023, max compression
```

## Comparing `dmp3-0.0.6.tar` & `dmp3-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-07 16:30:48.151547 dmp3-0.0.6/
--rw-r--r--   0 user      (1000) user      (1000)     3109 2023-04-07 04:09:35.000000 dmp3-0.0.6/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)     1064 2023-04-05 05:41:07.000000 dmp3-0.0.6/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     6227 2023-04-07 16:30:48.151547 dmp3-0.0.6/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     5382 2023-04-07 16:29:40.000000 dmp3-0.0.6/README.rst
--rw-r--r--   0 user      (1000) user      (1000)      980 2023-04-07 16:23:05.000000 dmp3-0.0.6/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-07 16:30:48.151547 dmp3-0.0.6/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-07 16:30:48.141547 dmp3-0.0.6/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-07 16:30:48.141547 dmp3-0.0.6/src/dmp3/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-04-06 08:28:30.000000 dmp3-0.0.6/src/dmp3/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     4271 2023-04-07 14:45:10.000000 dmp3-0.0.6/src/dmp3/_internal.py
--rw-r--r--   0 user      (1000) user      (1000)     4887 2023-04-07 16:27:58.000000 dmp3-0.0.6/src/dmp3/dmp3.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-07 16:30:48.141547 dmp3-0.0.6/src/dmp3.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     6227 2023-04-07 16:30:48.000000 dmp3-0.0.6/src/dmp3.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      352 2023-04-07 16:30:48.000000 dmp3-0.0.6/src/dmp3.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-07 16:30:48.000000 dmp3-0.0.6/src/dmp3.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       39 2023-04-07 16:30:48.000000 dmp3-0.0.6/src/dmp3.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       14 2023-04-07 16:30:48.000000 dmp3-0.0.6/src/dmp3.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        5 2023-04-07 16:30:48.000000 dmp3-0.0.6/src/dmp3.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-07 16:30:48.151547 dmp3-0.0.6/tests/
--rw-r--r--   0 user      (1000) user      (1000)      290 2023-04-06 04:40:16.000000 dmp3-0.0.6/tests/conftest.py
--rw-r--r--   0 user      (1000) user      (1000)      682 2023-04-06 04:40:16.000000 dmp3-0.0.6/tests/terminal.py
--rw-r--r--   0 user      (1000) user      (1000)     4530 2023-04-07 15:43:38.000000 dmp3-0.0.6/tests/test_wsl.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 14:10:21.476760 dmp3-0.0.7/
+-rw-r--r--   0 user      (1000) user      (1000)     3109 2023-04-07 04:09:35.000000 dmp3-0.0.7/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)     1064 2023-04-05 05:41:07.000000 dmp3-0.0.7/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     6326 2023-04-09 14:10:21.476760 dmp3-0.0.7/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     5442 2023-04-09 14:08:25.000000 dmp3-0.0.7/README.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1031 2023-04-09 14:08:32.000000 dmp3-0.0.7/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-09 14:10:21.476760 dmp3-0.0.7/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 14:10:21.476760 dmp3-0.0.7/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 14:10:21.476760 dmp3-0.0.7/src/dmp3/
+-rw-r--r--   0 user      (1000) user      (1000)       23 2023-04-09 14:08:25.000000 dmp3-0.0.7/src/dmp3/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     4271 2023-04-07 14:45:10.000000 dmp3-0.0.7/src/dmp3/_internal.py
+-rw-r--r--   0 user      (1000) user      (1000)     5509 2023-04-09 14:08:25.000000 dmp3-0.0.7/src/dmp3/dmp3.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 14:10:21.476760 dmp3-0.0.7/src/dmp3.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     6326 2023-04-09 14:10:21.000000 dmp3-0.0.7/src/dmp3.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      373 2023-04-09 14:10:21.000000 dmp3-0.0.7/src/dmp3.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-09 14:10:21.000000 dmp3-0.0.7/src/dmp3.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       39 2023-04-09 14:10:21.000000 dmp3-0.0.7/src/dmp3.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       21 2023-04-09 14:10:21.000000 dmp3-0.0.7/src/dmp3.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        5 2023-04-09 14:10:21.000000 dmp3-0.0.7/src/dmp3.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 14:10:21.476760 dmp3-0.0.7/tests/
+-rw-r--r--   0 user      (1000) user      (1000)      290 2023-04-06 04:40:16.000000 dmp3-0.0.7/tests/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)      682 2023-04-06 04:40:16.000000 dmp3-0.0.7/tests/terminal.py
+-rw-r--r--   0 user      (1000) user      (1000)     4541 2023-04-09 14:08:25.000000 dmp3-0.0.7/tests/test_cli.py
+-rw-r--r--   0 user      (1000) user      (1000)      985 2023-04-09 14:08:25.000000 dmp3-0.0.7/tests/test_direct.py
```

### Comparing `dmp3-0.0.6/.gitignore` & `dmp3-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dmp3-0.0.6/LICENSE` & `dmp3-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dmp3-0.0.6/PKG-INFO` & `dmp3-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dmp3
-Version: 0.0.6
-Summary: Download youtube video or playlist or channel, convert to mp3, store into a folder.
+Version: 0.0.7
+Summary: Download youtube video, playlist, channel. Convert to mp3, store into folder. Efficiently refresh mutiple storage folders.
 Author-email: 0xdomyz <septemberwhyms@gmail.com>
 Project-URL: homepage, https://github.com/0xdomyz/utube_playlist_mp3_downloader
 Project-URL: documentation, https://github.com/0xdomyz/utube_playlist_mp3_downloader
 Project-URL: Bug Tracker, https://github.com/0xdomyz/utube_playlist_mp3_downloader/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,28 +16,28 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===============================
 DMP3
 ===============================
 
-Download youtube video or playlist or channel, convert to mp3, store into a folder.
+Download youtube video, playlist, channel. Convert to mp3, store into folder. Efficiently refresh mutiple storage folders.
 
 Features:
 
 - Download all or subset of playlist
 - Download all or most recent n videos from channel
 - Download only additional items, once local storage folder is created
 - Refresh local storage folder with saved parameters
 - Refresh multiple local storage folders
 
 Installation
 ------------
 
-#. Install Python 3.9 or 3.10 or 3.11.
+#. Install Python >= 3.9.
 
 #. Install package from pypi.
 
     .. code-block:: console
 
         pip install -U dmp3
 
@@ -104,15 +104,15 @@
     cd /home/user/Projects/utube_playlist_mp3_downloader/tests/mp3_dir
     dmp3 . -r
 
 Usage in python script:
 
 .. code-block:: Python
 
-        from dmp3.dmp3 import dmp3
+        from dmp3 import dmp3
         from pathlib import Path
 
         folder = Path("/home/user/Projects/utube_playlist_mp3_downloader/tests/mp3_dir/starcraft_terran")
         webpath = "https://www.youtube.com/playlist?list=PLEtYTVnkBVuZWJ4Gsxtt80tWbiiyy1bcy"
 
         dmp3(folder=folder)
         dmp3(folder=folder, webpath=webpath, start=1, end=3, refresh_folder_mode=False, mp3=True)
@@ -120,15 +120,15 @@
 API
 -------
 
    .. code-block:: console
    
         usage: dmp3 [-h] [-w WEBPATH] [-s START] [-e END] [-r] [-m MP3] folder
 
-        Download youtube video or playlist or channel, convert to mp3, store into a folder.
+        Download youtube video, playlist, channel. Convert to mp3, store into folder. Efficiently refresh mutiple storage folders.
 
         Creates folder if not exists.
         Otherwise only download additional mp3 into the folder.
 
         If webpath is provided, creates a .dmp3 file in the folder to store parameters.
         If not provided, uses saved parameter.
```

### Comparing `dmp3-0.0.6/README.rst` & `dmp3-0.0.7/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ===============================
 DMP3
 ===============================
 
-Download youtube video or playlist or channel, convert to mp3, store into a folder.
+Download youtube video, playlist, channel. Convert to mp3, store into folder. Efficiently refresh mutiple storage folders.
 
 Features:
 
 - Download all or subset of playlist
 - Download all or most recent n videos from channel
 - Download only additional items, once local storage folder is created
 - Refresh local storage folder with saved parameters
 - Refresh multiple local storage folders
 
 Installation
 ------------
 
-#. Install Python 3.9 or 3.10 or 3.11.
+#. Install Python >= 3.9.
 
 #. Install package from pypi.
 
     .. code-block:: console
 
         pip install -U dmp3
 
@@ -86,15 +86,15 @@
     cd /home/user/Projects/utube_playlist_mp3_downloader/tests/mp3_dir
     dmp3 . -r
 
 Usage in python script:
 
 .. code-block:: Python
 
-        from dmp3.dmp3 import dmp3
+        from dmp3 import dmp3
         from pathlib import Path
 
         folder = Path("/home/user/Projects/utube_playlist_mp3_downloader/tests/mp3_dir/starcraft_terran")
         webpath = "https://www.youtube.com/playlist?list=PLEtYTVnkBVuZWJ4Gsxtt80tWbiiyy1bcy"
 
         dmp3(folder=folder)
         dmp3(folder=folder, webpath=webpath, start=1, end=3, refresh_folder_mode=False, mp3=True)
@@ -102,15 +102,15 @@
 API
 -------
 
    .. code-block:: console
    
         usage: dmp3 [-h] [-w WEBPATH] [-s START] [-e END] [-r] [-m MP3] folder
 
-        Download youtube video or playlist or channel, convert to mp3, store into a folder.
+        Download youtube video, playlist, channel. Convert to mp3, store into folder. Efficiently refresh mutiple storage folders.
 
         Creates folder if not exists.
         Otherwise only download additional mp3 into the folder.
 
         If webpath is provided, creates a .dmp3 file in the folder to store parameters.
         If not provided, uses saved parameter.
```

### Comparing `dmp3-0.0.6/pyproject.toml` & `dmp3-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmp3"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="0xdomyz", email="septemberwhyms@gmail.com" },
 ]
-description = "Download youtube video or playlist or channel, convert to mp3, store into a folder."
+description = "Download youtube video, playlist, channel. Convert to mp3, store into folder. Efficiently refresh mutiple storage folders."
 readme = "README.rst"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Operating System :: POSIX :: Linux",
 ]
 dependencies = [
   "pytube",
   "yt-dlp",
+  "pyyaml",
 ]
 
 [project.urls]
 homepage = "https://github.com/0xdomyz/utube_playlist_mp3_downloader"
 documentation = "https://github.com/0xdomyz/utube_playlist_mp3_downloader"
 "Bug Tracker" = "https://github.com/0xdomyz/utube_playlist_mp3_downloader/issues"
```

### Comparing `dmp3-0.0.6/src/dmp3/_internal.py` & `dmp3-0.0.7/src/dmp3/_internal.py`

 * *Files identical despite different names*

### Comparing `dmp3-0.0.6/src/dmp3/dmp3.py` & `dmp3-0.0.7/src/dmp3/dmp3.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "--mp3",
     type=bool,
     help="Convert video to mp3 files in the folder, default is True (WIP)",
     default=True,
 )
 
 description = """
-Download youtube video or playlist or channel, convert to mp3, store into a folder.
+Download youtube video, playlist, channel. Convert to mp3, store into folder. Efficiently refresh mutiple storage folders.
 
 Creates folder if not exists.
 Otherwise only download additional mp3 into the folder.
 
 If webpath is provided, creates a .dmp3 file in the folder to store parameters.
 If not provided, uses saved parameter.
 
@@ -90,48 +90,56 @@
     webpath = kwargs["webpath"]
     start = kwargs["start"]
     end = kwargs["end"]
     mp3 = kwargs["mp3"]
 
     # folder
     if not folder.exists():
+        print(f"Creating folder: {folder}")
         folder.mkdir(parents=True)
     existing_ids = already_downloaded_ids(folder)
+    print(f"No. of existing mp3 files: {len(existing_ids)}")
 
     # webpath
     if webpath is None:
         try:
+            print(f"Reading webpath from .dmp3 file in the folder: {folder}")
             info = read_saved_info(folder / ".dmp3")
             webpath = info["webpath"]
             start = info["start"] if "start" in info and start is None else start
             end = info["end"] if "end" in info and end is None else end
         except FileNotFoundError:
             raise Exception(
                 f"No webpath provided and no .dmp3 file found in the folder: {folder}"
             )
     else:
         info = kwargs.copy()
         info["folder"] = str(folder)
+        print(f"Saving webpath to .dmp3 file in the folder: {folder}")
         save_info(info=info, path=folder / ".dmp3")
 
     # logics
     webpath_type = parse_webpath(webpath)
+    print(f"Webpath type recognized as: {webpath_type}")
 
     if webpath_type == "video":
         id = id_from_video_webpath(webpath)
         if id not in existing_ids:
             download_ids_and_convert_to_mp3([id], folder)
     elif webpath_type in ["playlist", "channel"]:
         if len(existing_ids) > 0:
             if webpath_type == "playlist":
+                print(f"Fetcing playlist items: {webpath}")
                 target_urls = fetch_items_from_list(webpath, start, end)
             else:
+                print(f"Fetcing channel items: {webpath}")
                 target_urls = fetch_items_from_channel(webpath, start, end)
             target_ids = ids_from_list(target_urls)
             new_ids = list(set(target_ids) - set(existing_ids))
+            print(f"No. of new mp3 files to download: {len(new_ids)}")
             download_ids_and_convert_to_mp3(new_ids, folder)
         else:
             download_list_subset_and_convert_to_mp3(webpath, folder, start, end)
     else:
         raise ValueError(f"Unknown webpath type: {webpath_type}")
 
 
@@ -139,27 +147,28 @@
     folder: Path,
     webpath: str = None,
     start: int = None,
     end: int = None,
     refresh_folder_mode: bool = False,
     mp3: bool = True,
 ):
-    # refresh all folders mode
     if refresh_folder_mode:
+        print("Refresh all folders mode")
         for sub_folder in folder.iterdir():
             if sub_folder.is_dir() and (sub_folder / ".dmp3").exists():
+                print(f"Processing folder: {sub_folder}")
                 process_folder_and_webpath(
                     folder=sub_folder,
                     webpath=None,
                     start=None,
                     end=None,
                     mp3=mp3,
                 )
     else:
-        # vanilla mode
+        print("Single folder mode")
         process_folder_and_webpath(
             folder=folder,
             webpath=webpath,
             start=start,
             end=end,
             mp3=mp3,
         )
```

### Comparing `dmp3-0.0.6/src/dmp3.egg-info/PKG-INFO` & `dmp3-0.0.7/src/dmp3.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dmp3
-Version: 0.0.6
-Summary: Download youtube video or playlist or channel, convert to mp3, store into a folder.
+Version: 0.0.7
+Summary: Download youtube video, playlist, channel. Convert to mp3, store into folder. Efficiently refresh mutiple storage folders.
 Author-email: 0xdomyz <septemberwhyms@gmail.com>
 Project-URL: homepage, https://github.com/0xdomyz/utube_playlist_mp3_downloader
 Project-URL: documentation, https://github.com/0xdomyz/utube_playlist_mp3_downloader
 Project-URL: Bug Tracker, https://github.com/0xdomyz/utube_playlist_mp3_downloader/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,28 +16,28 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===============================
 DMP3
 ===============================
 
-Download youtube video or playlist or channel, convert to mp3, store into a folder.
+Download youtube video, playlist, channel. Convert to mp3, store into folder. Efficiently refresh mutiple storage folders.
 
 Features:
 
 - Download all or subset of playlist
 - Download all or most recent n videos from channel
 - Download only additional items, once local storage folder is created
 - Refresh local storage folder with saved parameters
 - Refresh multiple local storage folders
 
 Installation
 ------------
 
-#. Install Python 3.9 or 3.10 or 3.11.
+#. Install Python >= 3.9.
 
 #. Install package from pypi.
 
     .. code-block:: console
 
         pip install -U dmp3
 
@@ -104,15 +104,15 @@
     cd /home/user/Projects/utube_playlist_mp3_downloader/tests/mp3_dir
     dmp3 . -r
 
 Usage in python script:
 
 .. code-block:: Python
 
-        from dmp3.dmp3 import dmp3
+        from dmp3 import dmp3
         from pathlib import Path
 
         folder = Path("/home/user/Projects/utube_playlist_mp3_downloader/tests/mp3_dir/starcraft_terran")
         webpath = "https://www.youtube.com/playlist?list=PLEtYTVnkBVuZWJ4Gsxtt80tWbiiyy1bcy"
 
         dmp3(folder=folder)
         dmp3(folder=folder, webpath=webpath, start=1, end=3, refresh_folder_mode=False, mp3=True)
@@ -120,15 +120,15 @@
 API
 -------
 
    .. code-block:: console
    
         usage: dmp3 [-h] [-w WEBPATH] [-s START] [-e END] [-r] [-m MP3] folder
 
-        Download youtube video or playlist or channel, convert to mp3, store into a folder.
+        Download youtube video, playlist, channel. Convert to mp3, store into folder. Efficiently refresh mutiple storage folders.
 
         Creates folder if not exists.
         Otherwise only download additional mp3 into the folder.
 
         If webpath is provided, creates a .dmp3 file in the folder to store parameters.
         If not provided, uses saved parameter.
```

### Comparing `dmp3-0.0.6/tests/terminal.py` & `dmp3-0.0.7/tests/terminal.py`

 * *Files identical despite different names*

### Comparing `dmp3-0.0.6/tests/test_wsl.py` & `dmp3-0.0.7/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
 
 from terminal import run_cmd_on_path
 
-# from dmp3.dmp3 import dmp3
+# from dmp3 import dmp3
 
 # set up
 _dir = Path("/home/user/Projects/utube_playlist_mp3_downloader/tests/mp3_dir")
 
-_playlist = "https://www.youtube.com/playlist?list=PLEtYTVnkBVuZWJ4Gsxtt80tWbiiyy1bcy"
+_playlist = "https://www.youtube.com/playlist?list=PLmXDcu9yx4WCHiLoBFvaXqC9ytNfTxvki"
 _folder = Path(_dir / "starcraft_terran")
 
-_playlist2 = "https://www.youtube.com/playlist?list=PL4C4D2047A5B1423D"
+_playlist2 = "https://www.youtube.com/playlist?list=PLmXDcu9yx4WDVK_u65DLeqAzmLkqfdhA3"
 _folder2 = Path(_dir / "diablo1")
 
 _video = "https://www.youtube.com/watch?v=mD4GbGmvNRc&list=PLEtYTVnkBVuZWJ4Gsxtt80tWbiiyy1bcy&index=2&ab_channel=Katrulzin"
 _video2 = "https://www.youtube.com/watch?v=zAS8KivZX5s&ab_channel=nudl3r"
 _video_folder = Path(_dir / "various")
 
 _channel = "https://www.youtube.com/@Diablo/videos"
```

