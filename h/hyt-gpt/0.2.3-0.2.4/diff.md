# Comparing `tmp/hyt-gpt-0.2.3.tar.gz` & `tmp/hyt-gpt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.2.3.tar", last modified: Mon Mar 27 19:53:02 2023, max compression
+gzip compressed data, was "hyt-gpt-0.2.4.tar", last modified: Sun Apr  9 17:30:28 2023, max compression
```

## Comparing `hyt-gpt-0.2.3.tar` & `hyt-gpt-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-03-27 19:53:02.565149 hyt-gpt-0.2.3/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      747 2023-03-27 19:53:02.565149 hyt-gpt-0.2.3/PKG-INFO
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-03-27 19:53:02.565149 hyt-gpt-0.2.3/hyt_gpt/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        0 2023-03-24 22:01:13.000000 hyt-gpt-0.2.3/hyt_gpt/__init__.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     1402 2023-03-27 18:40:58.000000 hyt-gpt-0.2.3/hyt_gpt/gpt.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     2886 2023-03-24 22:01:13.000000 hyt-gpt-0.2.3/hyt_gpt/notion.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     6280 2023-03-27 19:52:03.000000 hyt-gpt-0.2.3/hyt_gpt/youtube.py
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-03-27 19:53:02.565149 hyt-gpt-0.2.3/hyt_gpt.egg-info/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      747 2023-03-27 19:53:02.000000 hyt-gpt-0.2.3/hyt_gpt.egg-info/PKG-INFO
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      204 2023-03-27 19:53:02.000000 hyt-gpt-0.2.3/hyt_gpt.egg-info/SOURCES.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        1 2023-03-27 19:53:02.000000 hyt-gpt-0.2.3/hyt_gpt.egg-info/dependency_links.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        8 2023-03-27 19:53:02.000000 hyt-gpt-0.2.3/hyt_gpt.egg-info/top_level.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)       38 2023-03-27 19:53:02.565149 hyt-gpt-0.2.3/setup.cfg
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      837 2023-03-27 19:52:16.000000 hyt-gpt-0.2.3/setup.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-09 17:30:28.616542 hyt-gpt-0.2.4/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-09 17:30:28.616542 hyt-gpt-0.2.4/PKG-INFO
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-09 17:30:28.616542 hyt-gpt-0.2.4/hyt_gpt/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.2.4/hyt_gpt/__init__.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     3736 2023-04-09 17:29:47.000000 hyt-gpt-0.2.4/hyt_gpt/gpt.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.2.4/hyt_gpt/notion.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     6366 2023-04-09 15:45:37.000000 hyt-gpt-0.2.4/hyt_gpt/youtube.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-09 17:30:28.616542 hyt-gpt-0.2.4/hyt_gpt.egg-info/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-09 17:30:28.000000 hyt-gpt-0.2.4/hyt_gpt.egg-info/PKG-INFO
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-04-09 17:30:28.000000 hyt-gpt-0.2.4/hyt_gpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-04-09 17:30:28.000000 hyt-gpt-0.2.4/hyt_gpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-04-09 17:30:28.000000 hyt-gpt-0.2.4/hyt_gpt.egg-info/top_level.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-04-09 17:30:28.616542 hyt-gpt-0.2.4/setup.cfg
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-04-09 17:30:19.000000 hyt-gpt-0.2.4/setup.py
```

### Comparing `hyt-gpt-0.2.3/PKG-INFO` & `hyt-gpt-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-
-UNKNOWN
-
```

### Comparing `hyt-gpt-0.2.3/hyt_gpt/notion.py` & `hyt-gpt-0.2.4/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.2.3/hyt_gpt/youtube.py` & `hyt-gpt-0.2.4/hyt_gpt/youtube.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,21 +137,23 @@
         }        
         with yt_dlp.YoutubeDL(options) as ydl:
             result = ydl.extract_info(url, download=False)
 
         # Extract the subtitles
         subtitles = []
         if 'subtitles' in result:
+            print('Found subtitles.')
             for subtitle_list in result['subtitles'].values():
                 for subtitle in subtitle_list:
                     if subtitle.get('ext') == 'vtt':
                         text = self.__get_text_from_url(subtitle.get('url'))
                         subtitles.extend(self.__parse_subtitles(text))
         
         if 'requested_subtitles' in result:
+            print('Found requested subtitles.')
             requested_subtitles = result.get('requested_subtitles')
             if 'en' in requested_subtitles:
                 subtitle = requested_subtitles['en']
                 if subtitle.get('ext') == 'vtt':
                     print('No subtitles found, fetching requested subtitles.')
                     text = self.__get_text_from_url(subtitle.get('url'))
                     subtitles.extend(self.__parse_requested_subtitles(text))
```

### Comparing `hyt-gpt-0.2.3/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.2.4/hyt_gpt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-
-UNKNOWN
-
```

### Comparing `hyt-gpt-0.2.3/setup.py` & `hyt-gpt-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.2.3',
+    version='0.2.4',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

