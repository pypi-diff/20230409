# Comparing `tmp/ofscraper-1.73.tar.gz` & `tmp/ofscraper-1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.73.tar", max compression
+gzip compressed data, was "ofscraper-1.74.tar", max compression
```

## Comparing `ofscraper-1.73.tar` & `ofscraper-1.74.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1073 2023-04-06 15:33:38.736121 ofscraper-1.73/LICENSE
--rw-r--r--   0        0        0     9234 2023-04-06 15:33:38.736121 ofscraper-1.73/README.md
--rw-r--r--   0        0        0      822 2023-04-08 02:40:42.813182 ofscraper-1.73/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.73/src/__init__.py
--rw-r--r--   0        0        0      751 2023-04-08 02:40:42.813182 ofscraper-1.73/src/__version__.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.73/src/api/__init__.py
--rw-r--r--   0        0        0     3418 2023-04-07 18:59:01.727222 ofscraper-1.73/src/api/highlights.py
--rw-r--r--   0        0        0      755 2023-04-06 15:33:38.742121 ofscraper-1.73/src/api/init.py
--rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.73/src/api/me.py
--rw-r--r--   0        0        0     4276 2023-04-08 02:39:37.314542 ofscraper-1.73/src/api/messages.py
--rw-r--r--   0        0        0     2286 2023-04-07 21:33:04.201250 ofscraper-1.73/src/api/paid.py
--rw-r--r--   0        0        0     6006 2023-04-08 02:39:58.242747 ofscraper-1.73/src/api/posts.py
--rw-r--r--   0        0        0     3166 2023-04-06 15:33:38.742121 ofscraper-1.73/src/api/profile.py
--rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.73/src/api/subscriptions.py
--rw-r--r--   0        0        0     4073 2023-04-07 18:11:39.208331 ofscraper-1.73/src/constants.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.73/src/db/__init__.py
--rw-r--r--   0        0        0    11481 2023-04-06 19:59:30.276880 ofscraper-1.73/src/db/operations.py
--rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.73/src/db/queries.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.73/src/interaction/__init__.py
--rw-r--r--   0        0        0     3246 2023-04-07 16:11:58.382914 ofscraper-1.73/src/interaction/like.py
--rwxr-xr-x   0        0        0    21153 2023-04-08 00:50:54.482139 ofscraper-1.73/src/scraper.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.73/src/utils/__init__.py
--rw-r--r--   0        0        0     8902 2023-04-07 07:23:51.927470 ofscraper-1.73/src/utils/auth.py
--rw-r--r--   0        0        0      694 2023-04-06 15:33:38.742121 ofscraper-1.73/src/utils/browser.py
--rw-r--r--   0        0        0     4985 2023-04-07 17:15:32.629148 ofscraper-1.73/src/utils/config.py
--rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.73/src/utils/dates.py
--rw-r--r--   0        0        0      372 2023-04-06 15:33:38.742121 ofscraper-1.73/src/utils/decorators.py
--rw-r--r--   0        0        0    17271 2023-04-08 02:29:55.499842 ofscraper-1.73/src/utils/download.py
--rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.73/src/utils/encoding.py
--rw-r--r--   0        0        0       28 2023-04-06 15:33:38.743121 ofscraper-1.73/src/utils/login.py
--rw-r--r--   0        0        0      418 2023-04-06 15:33:38.743121 ofscraper-1.73/src/utils/nap.py
--rw-r--r--   0        0        0     3160 2023-04-06 15:33:38.743121 ofscraper-1.73/src/utils/old_nap.py
--rw-r--r--   0        0        0     1901 2023-04-06 20:01:03.901832 ofscraper-1.73/src/utils/paths.py
--rw-r--r--   0        0        0     3891 2023-04-07 04:32:57.160701 ofscraper-1.73/src/utils/profiles.py
--rw-r--r--   0        0        0    16284 2023-04-07 07:12:53.191219 ofscraper-1.73/src/utils/prompts.py
--rw-r--r--   0        0        0      750 2023-04-06 15:33:38.743121 ofscraper-1.73/src/utils/separate.py
--rw-r--r--   0        0        0    10377 1970-01-01 00:00:00.000000 ofscraper-1.73/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-06 15:33:38.736121 ofscraper-1.74/LICENSE
+-rw-r--r--   0        0        0     4532 2023-04-09 14:34:07.560077 ofscraper-1.74/README.md
+-rw-r--r--   0        0        0      822 2023-04-09 14:41:13.463244 ofscraper-1.74/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.74/src/__init__.py
+-rw-r--r--   0        0        0      751 2023-04-09 14:41:13.463244 ofscraper-1.74/src/__version__.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.74/src/api/__init__.py
+-rw-r--r--   0        0        0     3418 2023-04-07 18:59:01.727222 ofscraper-1.74/src/api/highlights.py
+-rw-r--r--   0        0        0      755 2023-04-06 15:33:38.742121 ofscraper-1.74/src/api/init.py
+-rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.74/src/api/me.py
+-rw-r--r--   0        0        0     4276 2023-04-08 02:39:37.314542 ofscraper-1.74/src/api/messages.py
+-rw-r--r--   0        0        0     2286 2023-04-07 21:33:04.201250 ofscraper-1.74/src/api/paid.py
+-rw-r--r--   0        0        0     6006 2023-04-08 02:39:58.242747 ofscraper-1.74/src/api/posts.py
+-rw-r--r--   0        0        0     3166 2023-04-06 15:33:38.742121 ofscraper-1.74/src/api/profile.py
+-rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.74/src/api/subscriptions.py
+-rw-r--r--   0        0        0     4069 2023-04-08 17:31:23.478866 ofscraper-1.74/src/constants.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.74/src/db/__init__.py
+-rw-r--r--   0        0        0    11481 2023-04-06 19:59:30.276880 ofscraper-1.74/src/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.74/src/db/queries.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.74/src/interaction/__init__.py
+-rw-r--r--   0        0        0     3246 2023-04-07 16:11:58.382914 ofscraper-1.74/src/interaction/like.py
+-rwxr-xr-x   0        0        0    21195 2023-04-09 03:15:43.984031 ofscraper-1.74/src/scraper.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.74/src/utils/__init__.py
+-rw-r--r--   0        0        0     8902 2023-04-07 07:23:51.927470 ofscraper-1.74/src/utils/auth.py
+-rw-r--r--   0        0        0      694 2023-04-06 15:33:38.742121 ofscraper-1.74/src/utils/browser.py
+-rw-r--r--   0        0        0     5025 2023-04-09 12:25:36.153843 ofscraper-1.74/src/utils/config.py
+-rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.74/src/utils/dates.py
+-rw-r--r--   0        0        0      372 2023-04-06 15:33:38.742121 ofscraper-1.74/src/utils/decorators.py
+-rw-r--r--   0        0        0    17418 2023-04-09 14:34:48.797480 ofscraper-1.74/src/utils/download.py
+-rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.74/src/utils/encoding.py
+-rw-r--r--   0        0        0       28 2023-04-06 15:33:38.743121 ofscraper-1.74/src/utils/login.py
+-rw-r--r--   0        0        0      418 2023-04-06 15:33:38.743121 ofscraper-1.74/src/utils/nap.py
+-rw-r--r--   0        0        0     3160 2023-04-06 15:33:38.743121 ofscraper-1.74/src/utils/old_nap.py
+-rw-r--r--   0        0        0     1901 2023-04-06 20:01:03.901832 ofscraper-1.74/src/utils/paths.py
+-rw-r--r--   0        0        0     3891 2023-04-07 04:32:57.160701 ofscraper-1.74/src/utils/profiles.py
+-rw-r--r--   0        0        0    16171 2023-04-09 12:26:19.702268 ofscraper-1.74/src/utils/prompts.py
+-rw-r--r--   0        0        0      750 2023-04-06 15:33:38.743121 ofscraper-1.74/src/utils/separate.py
+-rw-r--r--   0        0        0     5675 1970-01-01 00:00:00.000000 ofscraper-1.74/PKG-INFO
```

### Comparing `ofscraper-1.73/LICENSE` & `ofscraper-1.74/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/pyproject.toml` & `ofscraper-1.74/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.73"
+version = "1.74"
 description = "automatically scrape onlyfans"
 authors = ["excludedBittern8 <excludedBittern8@riseup.net>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
```

### Comparing `ofscraper-1.73/src/__init__.py` & `ofscraper-1.74/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/__version__.py` & `ofscraper-1.74/src/__version__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,14 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/       
 """
 
 __title__ = 'ofscraper'
-__version__ = '1.73'
+__version__ = '1.74'
 __author__ = 'excludedBittern8'
 __author_email__ = 'excludedBittern8@riseup.net'
 __description__ = 'A command-line program to quickly download,like or unlike posts, and more'
 __url__ = 'https://github.com/excludedBittern8/ofscraper'
 __license__ = 'GNU General Public License v3 or later (GPLv3+)'
 __copyright__ = 'Copyright 2023'
```

### Comparing `ofscraper-1.73/src/api/highlights.py` & `ofscraper-1.74/src/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/api/init.py` & `ofscraper-1.74/src/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/api/me.py` & `ofscraper-1.74/src/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/api/messages.py` & `ofscraper-1.74/src/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/api/paid.py` & `ofscraper-1.74/src/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/api/posts.py` & `ofscraper-1.74/src/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/api/profile.py` & `ofscraper-1.74/src/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/api/subscriptions.py` & `ofscraper-1.74/src/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/constants.py` & `ofscraper-1.74/src/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 
 purchased_contentEP = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}&user_id={}"
 
 mainPromptChoices = {
     'Download content from a user': 0,
     'Like all of a user\'s posts': 1,
     'Unlike all of a user\'s posts': 2,
-    'Edit `auth.json` file': 3,
-    'Edit `config.json` file': 4,
+    'Edit auth.json`file': 3,
+    'Edit config.json file': 4,
     'Edit Profile': 5,
 
 }
 usernameOrListChoices = {
     'Select from accounts on profile': 0,
     'Enter a username': 1,
     'Scrape all users that I\'m subscribed to': 2
```

### Comparing `ofscraper-1.73/src/db/operations.py` & `ofscraper-1.74/src/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/db/queries.py` & `ofscraper-1.74/src/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/interaction/like.py` & `ofscraper-1.74/src/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/scraper.py` & `ofscraper-1.74/src/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,25 +546,24 @@
     filters.add_argument(
         '-ss', '--sub-status', help = 'Filter by whether or not your subscription has expired or not',default=None,required=False,type = str.lower,choices=["active","expired"]
     )
 
      #Paths
     paths=parser.add_argument_group("paths",description="Change or forced paths in program")
 
-    paths.add_argument(
-        '-op', '--outpath', help = 'Force downloading media into this directory',default=None,required=False
-    )
     args = parser.parse_args()
     global selectedusers
     selectedusers=None
     read_config()
 
 
     
     if len(list(filter(lambda x:x!=None and x!=False,[args.action,args.purchased,args.posts])))==0:
+        if args.daemon:
+            console.print("You need to pass at least one scraping method\n--action\n--posts\n--purchase\nAre all valid options. Skipping and going to menu")
         process_prompts()
         sys.exit(0)
     
 
 
 
     if args.posts:
```

### Comparing `ofscraper-1.73/src/utils/auth.py` & `ofscraper-1.74/src/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/utils/browser.py` & `ofscraper-1.74/src/utils/browser.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/utils/config.py` & `ofscraper-1.74/src/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             'save_location': config.get('save_location') or str(pathlib.Path.home() /'Data/ofscraper'),
             'file_size_limit': config.get('file_size_limit') or '',
             'dir_format': config.get("dir_format") or '{model_username}/{responsetype}/{mediatype}/',
             'file_format': config.get('file_format') or '{filename}.{ext}',
             'textlength':config.get('textlength') or 0,
             'date': config.get('date') or  "MM-DD-YYYY",
             "metadata": config.get('metadata') or "{configpath}/{profile}/.data/{username}_{model_id}",
-            "filter":config.get('filter') or ""
+            "filter":config.get('filter') or "Images,Audios,Videos"
         }
     }
     return new_config
 
 
 def make_config(path, config=None):
     config = config or  {
@@ -79,15 +79,15 @@
             'save_location': str(pathlib.Path.home() /'Data/ofscraper'),
             'file_size_limit': '',
             'dir_format':'{model_username}/{responsetype}/{mediatype}/',
             'file_format': '{filename}.{ext}',
             'textlength':0,
             'date':"MM-DD-YYYY",
             'metadata':"{configpath}/{profile}/.data/{username}_{model_id}",
-            "filter":""
+            "filter":"Images,Audios,Videos"
         }
     }
     if isinstance(config,str):
         config=json.loads(config)
 
     with open(path / configFile, 'w') as f:
         f.write(json.dumps(config, indent=4))
```

### Comparing `ofscraper-1.73/src/utils/dates.py` & `ofscraper-1.74/src/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/utils/download.py` & `ofscraper-1.74/src/utils/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -342,14 +342,17 @@
 
 def getmediadir(ele,username,model_id):
     root= pathlib.Path((config.get('save_location') or pathlib.Path.home()/"ofscraper"))
     downloadDir=(config.get('dir_format') or "{model_username}/{responsetype}/{mediatype}").format(sitename="onlyfans",first_letter=username[0].capitalize(),model_id=model_id,model_username=username,responsetype=ele['responsetype'].capitalize(),mediatype=ele['mediatype'].capitalize(),value=ele['value'].capitalize(),date=arrow.get(ele['date']).format(config.get('date')))
     return root /downloadDir
 
 def trunicate(path):
+    ext=str(path.suffix)
+    basepath=str(path.with_suffix(""))
     if platform.system() == 'Windows' and len(str(path))>256:
-        return pathlib.Path(str(path)[0:256])
+        return pathlib.Path(basepath[:256-len(ext)]).with_suffix(ext)
     elif platform.system() == 'Linux':
         dir=pathlib.Path(path).parent
-        file=pathlib.Path(path).name.encode("utf8")[:255].decode("utf8", "ignore")
-        return pathlib.Path(dir,file)
-    return path
+        file=pathlib.Path(basepath).name.encode("utf8")[:255-len(ext.encode('utf8'))].decode("utf8", "ignore")
+        return pathlib.Path(dir,file).with_suffix(ext)
+    else:
+        return path
```

### Comparing `ofscraper-1.73/src/utils/encoding.py` & `ofscraper-1.74/src/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/utils/old_nap.py` & `ofscraper-1.74/src/utils/old_nap.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/utils/paths.py` & `ofscraper-1.74/src/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/utils/profiles.py` & `ofscraper-1.74/src/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.73/src/utils/prompts.py` & `ofscraper-1.74/src/utils/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from InquirerPy.base import Choice
 
 from ..constants import mainPromptChoices, usernameOrListChoices, profilesPromptChoices
 
 
 def main_prompt() -> int:
     main_prompt_choices = [*mainPromptChoices]
-    main_prompt_choices.insert(4, Separator())
+    main_prompt_choices.insert(3, Separator())
 
     name = 'action'
 
     questions = [
         {
             'type': 'list',
             'name': name,
@@ -345,18 +345,15 @@
         }
     ]
     answer = prompt(questions)
     profile = answer[name]
 
     return profile
 
-#    'config': {
 
-#             'metadata':"{configpath}/{profile}/.data/{username}_{model_id}"
-#         }
 def config_prompt(config) -> dict:
     questions = [
         {
             'type': 'input',
             'name': 'main_profile',
             'message': 'What would you like your main profile to be?',
             'default': config.get('main_profile','main_profile')
@@ -385,21 +382,21 @@
             'message': 'What format do you want for downloaded files',
             'default': config.get('file_format', '{filename}.{ext}')
         },
                      {
             'type': 'input',
             'name': 'textlength',
             'message': 'Enter the max length to extract for post text, 0 means unlimited',
-            'default': config.get('textlenght', '0')
+            'default': config.get('textlength', '0')
         },
                           {
             'type': 'input',
             'name': 'date',
             'message': 'Enter Date formatting',
-            'default': config.get('textlenght', 'MM-DD-YYYY')
+            'default': config.get('date', 'MM-DD-YYYY')
         },
                                {
             'type': 'input',
             'name': 'metadata',
             'message': 'Where should metadata files be saved',
             'default': config.get('metadata', '{configpath}/{profile}/.data/{username}_{model_id}')
         }
```

### Comparing `ofscraper-1.73/src/utils/separate.py` & `ofscraper-1.74/src/utils/separate.py`

 * *Files identical despite different names*

