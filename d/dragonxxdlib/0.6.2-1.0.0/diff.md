# Comparing `tmp/dragonxxdlib-0.6.2.tar.gz` & `tmp/dragonxxdlib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonxxdlib-0.6.2.tar", last modified: Wed Sep 28 20:35:46 2022, max compression
+gzip compressed data, was "dragonxxdlib-1.0.0.tar", last modified: Sun Apr  9 19:38:40 2023, max compression
```

## Comparing `dragonxxdlib-0.6.2.tar` & `dragonxxdlib-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-09-28 20:35:46.521200 dragonxxdlib-0.6.2/
--rw-rw-rw-   0        0        0       82 2022-09-28 20:31:20.000000 dragonxxdlib-0.6.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2022-08-23 05:08:18.000000 dragonxxdlib-0.6.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2022-08-23 05:04:31.000000 dragonxxdlib-0.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0      727 2022-09-28 20:35:46.517945 dragonxxdlib-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0       60 2022-09-28 20:31:10.000000 dragonxxdlib-0.6.2/README.txt
-drwxrwxrwx   0        0        0        0 2022-09-28 20:35:46.481945 dragonxxdlib-0.6.2/dragonxxdlib/
--rw-rw-rw-   0        0        0     1487 2022-09-28 20:28:13.000000 dragonxxdlib-0.6.2/dragonxxdlib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-28 20:35:46.513944 dragonxxdlib-0.6.2/dragonxxdlib.egg-info/
--rw-rw-rw-   0        0        0      727 2022-09-28 20:35:46.000000 dragonxxdlib-0.6.2/dragonxxdlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2022-09-28 20:35:46.000000 dragonxxdlib-0.6.2/dragonxxdlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-28 20:35:46.000000 dragonxxdlib-0.6.2/dragonxxdlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-09-28 20:35:46.000000 dragonxxdlib-0.6.2/dragonxxdlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-28 20:35:46.521200 dragonxxdlib-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      747 2022-09-28 20:31:04.000000 dragonxxdlib-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:38:40.418256 dragonxxdlib-1.0.0/
+-rw-rw-rw-   0        0        0       81 2023-04-09 19:37:45.000000 dragonxxdlib-1.0.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2022-08-23 05:08:18.000000 dragonxxdlib-1.0.0/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2022-08-23 05:04:31.000000 dragonxxdlib-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      726 2023-04-09 19:38:40.417256 dragonxxdlib-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2022-09-28 20:31:10.000000 dragonxxdlib-1.0.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 19:38:40.378043 dragonxxdlib-1.0.0/dragonxxdlib/
+-rw-rw-rw-   0        0        0     1973 2023-04-09 19:35:31.000000 dragonxxdlib-1.0.0/dragonxxdlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:38:40.416262 dragonxxdlib-1.0.0/dragonxxdlib.egg-info/
+-rw-rw-rw-   0        0        0      726 2023-04-09 19:38:39.000000 dragonxxdlib-1.0.0/dragonxxdlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-09 19:38:39.000000 dragonxxdlib-1.0.0/dragonxxdlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 19:38:39.000000 dragonxxdlib-1.0.0/dragonxxdlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-09 19:38:39.000000 dragonxxdlib-1.0.0/dragonxxdlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 19:38:40.419257 dragonxxdlib-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      747 2023-04-09 19:36:09.000000 dragonxxdlib-1.0.0/setup.py
```

### Comparing `dragonxxdlib-0.6.2/LICENCE.txt` & `dragonxxdlib-1.0.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dragonxxdlib-0.6.2/PKG-INFO` & `dragonxxdlib-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonxxdlib
-Version: 0.6.2
+Version: 1.0.0
 Summary: Download from tik tok and youtube and facebook and other soon
 Home-page: UNKNOWN
 Author: yassen waly
 Author-email: 
 License: MIT
 Keywords: Download from tiktok and youtube and facebook
 Platform: UNKNOWN
@@ -16,11 +16,11 @@
 License-File: LICENCE.txt
 
 Download from tiktok and youtube and facebook and other soon
 
 Change Log
 ==========
 
-0.6.2 (28/9/2022)
+1.0.0 (9/4/2023)
 -------------------
 - second edition
```

### Comparing `dragonxxdlib-0.6.2/dragonxxdlib/__init__.py` & `dragonxxdlib-1.0.0/dragonxxdlib/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,17 +13,28 @@
     }
     r=requests.post(url,headers=head,data=data).json()
     json=r['url'][0]['url']
     return json
 
 
 def tiktok(urlt):
-    liba=requests.get(f"https://dev-ooooo2oo.pantheonsite.io/link.php?url={urlt}").json()
-    liba2=liba["result"]["download"]
-    return liba2
+    url2="https://api.onlinevideoconverter.pro/api/convert"
+    data2='{"url":"%s"}' %(urlt)
+    head2={
+'Host': 'api.onlinevideoconverter.pro',
+'accept': 'application/json, text/plain, */*',
+'content-type': 'application/json',
+'user-agent': 'Mozilla/5.0 (Linux; Android 9; CPH2083) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.0.0 Mobile Safari/537.36',
+'origin': 'https://en.onlinevideoconverter.pro',
+'referer': 'https://en.onlinevideoconverter.pro/',
+'content-length': '' + str(len(data2)) + '',
+    }
+    r2=requests.post(url2,headers=head2,data=data2).json()
+    json2=r2['url'][0]['url']
+    return json2
 
 def facebook(urlf):
     url2="https://api.onlinevideoconverter.pro/api/convert"
     data2='{"url":"%s"}' %(urlf)
     head2={
 'Host': 'api.onlinevideoconverter.pro',
 'accept': 'application/json, text/plain, */*',
```

### Comparing `dragonxxdlib-0.6.2/dragonxxdlib.egg-info/PKG-INFO` & `dragonxxdlib-1.0.0/dragonxxdlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonxxdlib
-Version: 0.6.2
+Version: 1.0.0
 Summary: Download from tik tok and youtube and facebook and other soon
 Home-page: UNKNOWN
 Author: yassen waly
 Author-email: 
 License: MIT
 Keywords: Download from tiktok and youtube and facebook
 Platform: UNKNOWN
@@ -16,11 +16,11 @@
 License-File: LICENCE.txt
 
 Download from tiktok and youtube and facebook and other soon
 
 Change Log
 ==========
 
-0.6.2 (28/9/2022)
+1.0.0 (9/4/2023)
 -------------------
 - second edition
```

### Comparing `dragonxxdlib-0.6.2/setup.py` & `dragonxxdlib-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='dragonxxdlib',
-  version='0.6.2',
+  version='1.0.0',
   description='Download from tik tok and youtube and facebook and other soon',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='yassen waly',
   author_email='',
   license='MIT', 
   classifiers=classifiers,
```

