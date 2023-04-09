# Comparing `tmp/ofscraper-1.74.tar.gz` & `tmp/ofscraper-1.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.74.tar", max compression
+gzip compressed data, was "ofscraper-1.75.tar", max compression
```

## Comparing `ofscraper-1.74.tar` & `ofscraper-1.75.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1073 2023-04-06 15:33:38.736121 ofscraper-1.74/LICENSE
--rw-r--r--   0        0        0     4532 2023-04-09 14:34:07.560077 ofscraper-1.74/README.md
--rw-r--r--   0        0        0      822 2023-04-09 14:41:13.463244 ofscraper-1.74/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.74/src/__init__.py
--rw-r--r--   0        0        0      751 2023-04-09 14:41:13.463244 ofscraper-1.74/src/__version__.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.74/src/api/__init__.py
--rw-r--r--   0        0        0     3418 2023-04-07 18:59:01.727222 ofscraper-1.74/src/api/highlights.py
--rw-r--r--   0        0        0      755 2023-04-06 15:33:38.742121 ofscraper-1.74/src/api/init.py
--rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.74/src/api/me.py
--rw-r--r--   0        0        0     4276 2023-04-08 02:39:37.314542 ofscraper-1.74/src/api/messages.py
--rw-r--r--   0        0        0     2286 2023-04-07 21:33:04.201250 ofscraper-1.74/src/api/paid.py
--rw-r--r--   0        0        0     6006 2023-04-08 02:39:58.242747 ofscraper-1.74/src/api/posts.py
--rw-r--r--   0        0        0     3166 2023-04-06 15:33:38.742121 ofscraper-1.74/src/api/profile.py
--rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.74/src/api/subscriptions.py
--rw-r--r--   0        0        0     4069 2023-04-08 17:31:23.478866 ofscraper-1.74/src/constants.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.74/src/db/__init__.py
--rw-r--r--   0        0        0    11481 2023-04-06 19:59:30.276880 ofscraper-1.74/src/db/operations.py
--rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.74/src/db/queries.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.74/src/interaction/__init__.py
--rw-r--r--   0        0        0     3246 2023-04-07 16:11:58.382914 ofscraper-1.74/src/interaction/like.py
--rwxr-xr-x   0        0        0    21195 2023-04-09 03:15:43.984031 ofscraper-1.74/src/scraper.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.74/src/utils/__init__.py
--rw-r--r--   0        0        0     8902 2023-04-07 07:23:51.927470 ofscraper-1.74/src/utils/auth.py
--rw-r--r--   0        0        0      694 2023-04-06 15:33:38.742121 ofscraper-1.74/src/utils/browser.py
--rw-r--r--   0        0        0     5025 2023-04-09 12:25:36.153843 ofscraper-1.74/src/utils/config.py
--rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.74/src/utils/dates.py
--rw-r--r--   0        0        0      372 2023-04-06 15:33:38.742121 ofscraper-1.74/src/utils/decorators.py
--rw-r--r--   0        0        0    17418 2023-04-09 14:34:48.797480 ofscraper-1.74/src/utils/download.py
--rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.74/src/utils/encoding.py
--rw-r--r--   0        0        0       28 2023-04-06 15:33:38.743121 ofscraper-1.74/src/utils/login.py
--rw-r--r--   0        0        0      418 2023-04-06 15:33:38.743121 ofscraper-1.74/src/utils/nap.py
--rw-r--r--   0        0        0     3160 2023-04-06 15:33:38.743121 ofscraper-1.74/src/utils/old_nap.py
--rw-r--r--   0        0        0     1901 2023-04-06 20:01:03.901832 ofscraper-1.74/src/utils/paths.py
--rw-r--r--   0        0        0     3891 2023-04-07 04:32:57.160701 ofscraper-1.74/src/utils/profiles.py
--rw-r--r--   0        0        0    16171 2023-04-09 12:26:19.702268 ofscraper-1.74/src/utils/prompts.py
--rw-r--r--   0        0        0      750 2023-04-06 15:33:38.743121 ofscraper-1.74/src/utils/separate.py
--rw-r--r--   0        0        0     5675 1970-01-01 00:00:00.000000 ofscraper-1.74/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-06 15:33:38.736121 ofscraper-1.75/LICENSE
+-rw-r--r--   0        0        0     4533 2023-04-09 16:26:59.278005 ofscraper-1.75/README.md
+-rw-r--r--   0        0        0      822 2023-04-09 16:28:46.830053 ofscraper-1.75/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.75/src/__init__.py
+-rw-r--r--   0        0        0      751 2023-04-09 16:28:46.830053 ofscraper-1.75/src/__version__.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.75/src/api/__init__.py
+-rw-r--r--   0        0        0     3418 2023-04-07 18:59:01.727222 ofscraper-1.75/src/api/highlights.py
+-rw-r--r--   0        0        0      755 2023-04-06 15:33:38.742121 ofscraper-1.75/src/api/init.py
+-rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.75/src/api/me.py
+-rw-r--r--   0        0        0     4276 2023-04-08 02:39:37.314542 ofscraper-1.75/src/api/messages.py
+-rw-r--r--   0        0        0     2286 2023-04-07 21:33:04.201250 ofscraper-1.75/src/api/paid.py
+-rw-r--r--   0        0        0     6006 2023-04-08 02:39:58.242747 ofscraper-1.75/src/api/posts.py
+-rw-r--r--   0        0        0     3166 2023-04-06 15:33:38.742121 ofscraper-1.75/src/api/profile.py
+-rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.75/src/api/subscriptions.py
+-rw-r--r--   0        0        0     4069 2023-04-08 17:31:23.478866 ofscraper-1.75/src/constants.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.75/src/db/__init__.py
+-rw-r--r--   0        0        0    11481 2023-04-06 19:59:30.276880 ofscraper-1.75/src/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.75/src/db/queries.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.75/src/interaction/__init__.py
+-rw-r--r--   0        0        0     3246 2023-04-07 16:11:58.382914 ofscraper-1.75/src/interaction/like.py
+-rwxr-xr-x   0        0        0    21163 2023-04-09 15:49:18.249866 ofscraper-1.75/src/scraper.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.75/src/utils/__init__.py
+-rw-r--r--   0        0        0     8902 2023-04-07 07:23:51.927470 ofscraper-1.75/src/utils/auth.py
+-rw-r--r--   0        0        0      694 2023-04-06 15:33:38.742121 ofscraper-1.75/src/utils/browser.py
+-rw-r--r--   0        0        0     5025 2023-04-09 12:25:36.153843 ofscraper-1.75/src/utils/config.py
+-rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.75/src/utils/dates.py
+-rw-r--r--   0        0        0      372 2023-04-06 15:33:38.742121 ofscraper-1.75/src/utils/decorators.py
+-rw-r--r--   0        0        0    17435 2023-04-09 16:19:51.649835 ofscraper-1.75/src/utils/download.py
+-rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.75/src/utils/encoding.py
+-rw-r--r--   0        0        0       28 2023-04-06 15:33:38.743121 ofscraper-1.75/src/utils/login.py
+-rw-r--r--   0        0        0      418 2023-04-06 15:33:38.743121 ofscraper-1.75/src/utils/nap.py
+-rw-r--r--   0        0        0     3160 2023-04-06 15:33:38.743121 ofscraper-1.75/src/utils/old_nap.py
+-rw-r--r--   0        0        0     1901 2023-04-06 20:01:03.901832 ofscraper-1.75/src/utils/paths.py
+-rw-r--r--   0        0        0     3891 2023-04-07 04:32:57.160701 ofscraper-1.75/src/utils/profiles.py
+-rw-r--r--   0        0        0    16171 2023-04-09 12:26:19.702268 ofscraper-1.75/src/utils/prompts.py
+-rw-r--r--   0        0        0      750 2023-04-06 15:33:38.743121 ofscraper-1.75/src/utils/separate.py
+-rw-r--r--   0        0        0     5676 1970-01-01 00:00:00.000000 ofscraper-1.75/PKG-INFO
```

### Comparing `ofscraper-1.74/LICENSE` & `ofscraper-1.75/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/README.md` & `ofscraper-1.75/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-A fork of onlyfans-scraper 
-It has been optimized to make it more feature complete with dc's onlyfans script
+A fork of onlyfans-scraper. It has been optimized to make it more feature complete with dc's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
 https://github.com/excludedBittern8/ofscraper/blob/main/CHANGES.md
 
 <h3>DISCLAIMERS:</h3>
 <ol>
```

### Comparing `ofscraper-1.74/pyproject.toml` & `ofscraper-1.75/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.74"
+version = "1.75"
 description = "automatically scrape onlyfans"
 authors = ["excludedBittern8 <excludedBittern8@riseup.net>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
```

### Comparing `ofscraper-1.74/src/__init__.py` & `ofscraper-1.75/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/__version__.py` & `ofscraper-1.75/src/__version__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,14 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/       
 """
 
 __title__ = 'ofscraper'
-__version__ = '1.74'
+__version__ = '1.75'
 __author__ = 'excludedBittern8'
 __author_email__ = 'excludedBittern8@riseup.net'
 __description__ = 'A command-line program to quickly download,like or unlike posts, and more'
 __url__ = 'https://github.com/excludedBittern8/ofscraper'
 __license__ = 'GNU General Public License v3 or later (GPLv3+)'
 __copyright__ = 'Copyright 2023'
```

### Comparing `ofscraper-1.74/src/api/highlights.py` & `ofscraper-1.75/src/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/api/init.py` & `ofscraper-1.75/src/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/api/me.py` & `ofscraper-1.75/src/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/api/messages.py` & `ofscraper-1.75/src/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/api/paid.py` & `ofscraper-1.75/src/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/api/posts.py` & `ofscraper-1.75/src/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/api/profile.py` & `ofscraper-1.75/src/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/api/subscriptions.py` & `ofscraper-1.75/src/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/constants.py` & `ofscraper-1.75/src/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/db/operations.py` & `ofscraper-1.75/src/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/db/queries.py` & `ofscraper-1.75/src/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/interaction/like.py` & `ofscraper-1.75/src/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/scraper.py` & `ofscraper-1.75/src/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,14 @@
             operations.write_profile_table(model_id,ele['name'])
             combined_urls=process_areas(headers, ele, model_id)
             asyncio.run(download.process_dicts(
             ele["name"],
             model_id,
             combined_urls,
             forced=args.dupe,
-            outpath=args.outpath
             ))
         except Exception as e:
             console.print("run failed with exception: ", e)
     
     
 
 def process_like():
@@ -383,15 +382,15 @@
             model_id = profile.get_id(headers, ele["name"])
             posts = like.get_posts(headers, model_id,ele['name'])
             favorited_posts = like.filter_for_favorited(posts)
             post_ids = like.get_post_ids(favorited_posts)
             like.unlike(headers, model_id, ele["name"], post_ids)
 
 @contextmanager
-def suppress_stdout():
+def asuppress_stdout():
     with open(os.devnull, "w") as devnull:
         old_stdout = sys.stdout
         old_stderr=sys.stderr
         sys.stdout = devnull
         sys.stderr = devnull
         try:  
             yield
```

### Comparing `ofscraper-1.74/src/utils/auth.py` & `ofscraper-1.75/src/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/utils/browser.py` & `ofscraper-1.75/src/utils/browser.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/utils/config.py` & `ofscraper-1.75/src/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/utils/dates.py` & `ofscraper-1.75/src/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/utils/download.py` & `ofscraper-1.75/src/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from ..utils.profiles import get_current_profile
 from .dates import convert_local_time
 
 
 config = read_config()['config']
 
 
-async def process_dicts(username, model_id, medialist,forced=False,outpath=None):
+async def process_dicts(username, model_id, medialist,forced=False):
     if medialist:
         if not forced:
             media_ids = set(operations.get_media_ids(model_id,username))
             medialist = separate_by_id(medialist, media_ids)
             console.print(f"Skipping previously downloaded\nMedia left for download {len(medialist)}")
         else:
             print("forcing all downloads")
@@ -342,17 +342,18 @@
 
 def getmediadir(ele,username,model_id):
     root= pathlib.Path((config.get('save_location') or pathlib.Path.home()/"ofscraper"))
     downloadDir=(config.get('dir_format') or "{model_username}/{responsetype}/{mediatype}").format(sitename="onlyfans",first_letter=username[0].capitalize(),model_id=model_id,model_username=username,responsetype=ele['responsetype'].capitalize(),mediatype=ele['mediatype'].capitalize(),value=ele['value'].capitalize(),date=arrow.get(ele['date']).format(config.get('date')))
     return root /downloadDir
 
 def trunicate(path):
+    path=pathlib.Path(path)
     ext=str(path.suffix)
     basepath=str(path.with_suffix(""))
     if platform.system() == 'Windows' and len(str(path))>256:
         return pathlib.Path(basepath[:256-len(ext)]).with_suffix(ext)
     elif platform.system() == 'Linux':
         dir=pathlib.Path(path).parent
-        file=pathlib.Path(basepath).name.encode("utf8")[:255-len(ext.encode('utf8'))].decode("utf8", "ignore")
+        file=pathlib.Path(basepath).name.encode("utf8")[:(255-len(ext.encode('utf8')))].decode("utf8", "ignore")
         return pathlib.Path(dir,file).with_suffix(ext)
     else:
         return path
```

### Comparing `ofscraper-1.74/src/utils/encoding.py` & `ofscraper-1.75/src/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/utils/old_nap.py` & `ofscraper-1.75/src/utils/old_nap.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/utils/paths.py` & `ofscraper-1.75/src/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/utils/profiles.py` & `ofscraper-1.75/src/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/utils/prompts.py` & `ofscraper-1.75/src/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/src/utils/separate.py` & `ofscraper-1.75/src/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.74/PKG-INFO` & `ofscraper-1.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.74
+Version: 1.75
 Summary: automatically scrape onlyfans
 Author: excludedBittern8
 Author-email: excludedBittern8@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -23,16 +23,15 @@
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0)
 Project-URL: Homepage, https://github.com/excludedBittern8/ofscraper
 Description-Content-Type: text/markdown
 
-A fork of onlyfans-scraper 
-It has been optimized to make it more feature complete with dc's onlyfans script
+A fork of onlyfans-scraper. It has been optimized to make it more feature complete with dc's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
 https://github.com/excludedBittern8/ofscraper/blob/main/CHANGES.md
 
 <h3>DISCLAIMERS:</h3>
 <ol>
```

