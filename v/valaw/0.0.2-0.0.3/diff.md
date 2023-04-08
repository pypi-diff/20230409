# Comparing `tmp/valaw-0.0.2.tar.gz` & `tmp/valaw-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valaw-0.0.2.tar", last modified: Sat Apr  8 01:45:55 2023, max compression
+gzip compressed data, was "valaw-0.0.3.tar", last modified: Sat Apr  8 23:19:37 2023, max compression
```

## Comparing `valaw-0.0.2.tar` & `valaw-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 01:45:55.440105 valaw-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-04-04 04:45:45.000000 valaw-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1383 2023-04-08 01:45:55.438105 valaw-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      725 2023-04-06 23:58:20.000000 valaw-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 01:45:55.441099 valaw-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1118 2023-04-08 01:44:20.000000 valaw-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 01:45:55.334276 valaw-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 01:45:55.391097 valaw-0.0.2/src/valaw/
--rw-rw-rw-   0        0        0       73 2023-04-04 05:08:42.000000 valaw-0.0.2/src/valaw/__init__.py
--rw-rw-rw-   0        0        0    11124 2023-04-08 01:43:49.000000 valaw-0.0.2/src/valaw/client.py
-drwxrwxrwx   0        0        0        0 2023-04-08 01:45:55.434091 valaw-0.0.2/src/valaw.egg-info/
--rw-rw-rw-   0        0        0     1383 2023-04-08 01:45:55.000000 valaw-0.0.2/src/valaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-04-08 01:45:55.000000 valaw-0.0.2/src/valaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 01:45:55.000000 valaw-0.0.2/src/valaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-08 01:45:55.000000 valaw-0.0.2/src/valaw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 01:45:55.000000 valaw-0.0.2/src/valaw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 23:19:37.254421 valaw-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-04 04:45:45.000000 valaw-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1383 2023-04-08 23:19:37.251030 valaw-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2023-04-06 23:58:20.000000 valaw-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 23:19:37.254421 valaw-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1118 2023-04-08 23:18:41.000000 valaw-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 23:19:37.157648 valaw-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 23:19:37.197668 valaw-0.0.3/src/valaw/
+-rw-rw-rw-   0        0        0       73 2023-04-04 05:08:42.000000 valaw-0.0.3/src/valaw/__init__.py
+-rw-rw-rw-   0        0        0    11240 2023-04-08 23:17:11.000000 valaw-0.0.3/src/valaw/client.py
+drwxrwxrwx   0        0        0        0 2023-04-08 23:19:37.246770 valaw-0.0.3/src/valaw.egg-info/
+-rw-rw-rw-   0        0        0     1383 2023-04-08 23:19:37.000000 valaw-0.0.3/src/valaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-04-08 23:19:37.000000 valaw-0.0.3/src/valaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 23:19:37.000000 valaw-0.0.3/src/valaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-08 23:19:37.000000 valaw-0.0.3/src/valaw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-08 23:19:37.000000 valaw-0.0.3/src/valaw.egg-info/top_level.txt
```

### Comparing `valaw-0.0.2/LICENSE` & `valaw-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `valaw-0.0.2/PKG-INFO` & `valaw-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valaw
-Version: 0.0.2
+Version: 0.0.3
 Summary: An asynchronous API wrapper for VALORANT's API
 Home-page: https://github.com/Jet612/valaw
 Author: Jet612
 Project-URL: Documentation, https://github.com/Jet612/valaw/tree/main/docs
 Project-URL: Issue Tracker, https://github.com/Jet612/valaw/issues
 Project-URL: Chat/Support, https://discord.gg/mVXpvunBbF
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `valaw-0.0.2/README.md` & `valaw-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `valaw-0.0.2/setup.py` & `valaw-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r") as readme:
     long_desc = readme.read()
 
 setup(
     name="valaw",
-    version="0.0.2",
+    version="0.0.3",
     author="Jet612",
     description="An asynchronous API wrapper for VALORANT's API",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/Jet612/valaw",
     project_urls={
         "Documentation": "https://github.com/Jet612/valaw/tree/main/docs",
```

### Comparing `valaw-0.0.2/src/valaw/client.py` & `valaw-0.0.3/src/valaw/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
             raise Exceptions.InvalidCluster(f"Invalid cluster, valid clusters are: {clusters}.")
         
         self.token = token
         self.cluster = cluster
 
         # Subclasses
         self.account = Account(token, cluster)
+        self.content = Content(token, cluster)
+        self.match = Match(token, cluster)
 
         # Beta/Development message
         print("valaw: This library is still in development, please report any bugs to https://github.com/Jet612/valaw/issues.")
 
 class Account:
     def __init__(self, token: str, cluster: str):
         self.token = token
@@ -159,15 +161,15 @@
                 return await verify_content(resp)
             
 class Match:
     def __init__(self, token: str, cluster: str):
         self.token = token
         self.cluster = cluster
 
-    async def GET_getMatch(self, matchId: str, region: str):
+    async def GET_getMatch(self, matchId: str, region: str) -> dict:
         """Get match by id."""
 
         if region.lower() not in regions:
             raise Exceptions.InvalidRegion(f"Invalid region, valid regions are: {regions}.")
 
         async with aiohttp.ClientSession() as session:
             headers = {
@@ -176,15 +178,15 @@
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{region}.api.riotgames.com/val/match/v1/matches/{matchId}", headers=headers) as resp:
                 return await verify_content(resp)
             
-    async def GET_getMatchlist(self, puuid: str, region: str):
+    async def GET_getMatchlist(self, puuid: str, region: str) -> dict:
         """Get matchlist for games played by puuid."""
 
         if region.lower() not in regions:
             raise Exceptions.InvalidRegion(f"Invalid region, valid regions are: {regions}.")
 
         async with aiohttp.ClientSession() as session:
             headers = {
@@ -193,15 +195,15 @@
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{region}.api.riotgames.com/val/match/v1/matchlists/by-puuid/{puuid}", headers=headers) as resp:
                 return await verify_content(resp)
             
-    async def GET_getRecent(self, queue: str, region: str):
+    async def GET_getRecent(self, queue: str, region: str) -> dict:
         """
         Get recent matches.
 
         Returns a list of match ids that have completed 
         in the last 10 minutes for live regions and 12 hours 
         for the esports routing value. NA/LATAM/BR share a 
         match history deployment. As such, recent matches
```

### Comparing `valaw-0.0.2/src/valaw.egg-info/PKG-INFO` & `valaw-0.0.3/src/valaw.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valaw
-Version: 0.0.2
+Version: 0.0.3
 Summary: An asynchronous API wrapper for VALORANT's API
 Home-page: https://github.com/Jet612/valaw
 Author: Jet612
 Project-URL: Documentation, https://github.com/Jet612/valaw/tree/main/docs
 Project-URL: Issue Tracker, https://github.com/Jet612/valaw/issues
 Project-URL: Chat/Support, https://discord.gg/mVXpvunBbF
 Classifier: Programming Language :: Python :: 3.8
```

