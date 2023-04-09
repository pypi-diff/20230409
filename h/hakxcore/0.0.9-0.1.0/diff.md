# Comparing `tmp/hakxcore-0.0.9.tar.gz` & `tmp/hakxcore-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hakxcore-0.0.9.tar", last modified: Sun Aug 28 12:23:48 2022, max compression
+gzip compressed data, was "hakxcore-0.1.0.tar", last modified: Sun Apr  9 14:56:40 2023, max compression
```

## Comparing `hakxcore-0.0.9.tar` & `hakxcore-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-28 12:23:48.199384 hakxcore-0.0.9/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2022-08-28 07:52:10.000000 hakxcore-0.0.9/LICENCE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      165 2022-08-28 11:12:13.000000 hakxcore-0.0.9/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8621 2022-08-28 12:23:48.199384 hakxcore-0.0.9/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7806 2022-08-27 19:38:49.000000 hakxcore-0.0.9/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-28 12:23:48.191384 hakxcore-0.0.9/hakxcore/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2022-08-28 12:22:24.000000 hakxcore-0.0.9/hakxcore/__init__.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1532 2022-08-28 12:23:23.000000 hakxcore-0.0.9/hakxcore/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-28 12:23:48.195384 hakxcore-0.0.9/hakxcore.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8621 2022-08-28 12:23:48.000000 hakxcore-0.0.9/hakxcore.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2022-08-28 12:23:48.000000 hakxcore-0.0.9/hakxcore.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-08-28 12:23:48.000000 hakxcore-0.0.9/hakxcore.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2022-08-28 12:23:48.000000 hakxcore-0.0.9/hakxcore.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-08-28 12:23:48.000000 hakxcore-0.0.9/hakxcore.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-08-28 12:23:48.000000 hakxcore-0.0.9/hakxcore.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-08-28 12:23:48.000000 hakxcore-0.0.9/hakxcore.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7126 2022-08-27 19:38:49.000000 hakxcore-0.0.9/index.html
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-28 12:23:48.195384 hakxcore-0.0.9/media/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   333365 2022-08-27 19:38:49.000000 hakxcore-0.0.9/media/aboutme.gif
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10196 2022-08-27 19:38:49.000000 hakxcore-0.0.9/media/animated-tree.gif
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   148640 2022-08-27 19:38:49.000000 hakxcore-0.0.9/media/butterfly.gif
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    84714 2022-08-27 19:38:49.000000 hakxcore-0.0.9/media/dog.gif
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   369993 2022-08-27 19:38:49.000000 hakxcore-0.0.9/media/hakxcore-logo.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   383869 2022-08-27 19:38:49.000000 hakxcore-0.0.9/media/hakxcore-logo1.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-08-28 12:23:48.199384 hakxcore-0.0.9/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1445 2022-08-28 12:10:18.000000 hakxcore-0.0.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 14:56:40.792720 hakxcore-0.1.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2023-04-09 14:40:39.000000 hakxcore-0.1.0/LICENCE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-09 14:40:39.000000 hakxcore-0.1.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8517 2023-04-09 14:56:40.792720 hakxcore-0.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7722 2023-04-09 14:40:39.000000 hakxcore-0.1.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 14:56:40.788720 hakxcore-0.1.0/hakxcore/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-04-09 14:56:25.000000 hakxcore-0.1.0/hakxcore/__init__.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1532 2023-04-09 14:46:31.000000 hakxcore-0.1.0/hakxcore/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 14:56:40.788720 hakxcore-0.1.0/hakxcore.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8517 2023-04-09 14:56:40.000000 hakxcore-0.1.0/hakxcore.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-04-09 14:56:40.000000 hakxcore-0.1.0/hakxcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-09 14:56:40.000000 hakxcore-0.1.0/hakxcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-04-09 14:56:40.000000 hakxcore-0.1.0/hakxcore.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-09 14:56:40.000000 hakxcore-0.1.0/hakxcore.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2023-04-09 14:56:40.000000 hakxcore-0.1.0/hakxcore.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-09 14:56:40.000000 hakxcore-0.1.0/hakxcore.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7126 2023-04-09 14:40:39.000000 hakxcore-0.1.0/index.html
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 14:56:40.792720 hakxcore-0.1.0/media/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   333365 2023-04-09 14:40:39.000000 hakxcore-0.1.0/media/aboutme.gif
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10196 2023-04-09 14:40:39.000000 hakxcore-0.1.0/media/animated-tree.gif
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   148640 2023-04-09 14:40:39.000000 hakxcore-0.1.0/media/butterfly.gif
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    84714 2023-04-09 14:40:39.000000 hakxcore-0.1.0/media/dog.gif
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   369993 2023-04-09 14:40:39.000000 hakxcore-0.1.0/media/hakxcore-logo.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   383869 2023-04-09 14:40:39.000000 hakxcore-0.1.0/media/hakxcore-logo1.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-09 14:56:40.792720 hakxcore-0.1.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1445 2023-04-09 14:40:39.000000 hakxcore-0.1.0/setup.py
```

### Comparing `hakxcore-0.0.9/LICENCE` & `hakxcore-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `hakxcore-0.0.9/PKG-INFO` & `hakxcore-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 Metadata-Version: 2.1
 Name: hakxcore
-Version: 0.0.9
+Version: 0.1.0
 Summary: Hakxcore personal Repo and python package
 Home-page: https://github.com/hakxcore/hakxcore
+Download-URL: https://github.com/hakxcore/hakxcore/archive/refs/heads/main.zip
 Author: Mukesh Kumar
 Author-email: mukeshkumarchark@gmail.com
 License: MIT Licence
-Download-URL: https://github.com/hakxcore/hakxcore/archive/refs/heads/main.zip
 Keywords: hakxcore,bug bounty,mukesh,pentesting,security,development,enterprenurship
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.4
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Hi 👋, I'm [Mukesh](https://github.com/hakxcore) <img src="media/butterfly.gif" alt="butterfly" width="150"/> <img src="media/dog.gif" alt="butterfly" width="200"/>
-<!--<h3 align="center"><img src="media/animated-tree.gif" alt="butterfly" width=15%/></h>-->
-</br>
+<!--<h3 align="center"><img src="media/animated-tree.gif" alt="butterfly" width=15%/></h>   width='700' height='200' style='margin-right: 1rem;'-->
 </br>
 </br>
 
-<table style="border: none;">
-  <tr style="border: none; padding: 0; margin: 0;">
-  <td style="border: none; padding: 0; margin: 0;"> 
-    <a href="https://github.com/ryo-ma/github-profile-trophy" target="_blank">
-      <img src="https://github-profile-trophy.vercel.app/?username=hakxcore" alt="hakxcore" width='700' height='200' style='margin-right: 1rem;'/>
-    </a>
-    </td>
-  </tr>
-  </table>
+`$ pip install hakxcore`
+[![Downloads](https://static.pepy.tech/badge/hakxcore)](https://pepy.tech/project/hakxcore)
+---
+
+<a href="https://github.com/ryo-ma/github-profile-trophy" target="_blank">
+  <img width=900 src="https://github-profile-trophy.vercel.app/?username=hakxcore&column=8&theme=algolia&no-frame=true"/>
+</a>
+
 <p align="left"> <img src="https://komarev.com/ghpvc/?username=hakxcore&label=Profile%20views&color=0e75b6&style=flat" alt="hakxcore" /> </p>
 
+<!--
 - 🔭 I’m currently working on [`fig`](https://github.com/hakxcore/fig) project
 
 - 🌱 I’m currently learning **`Go`**
 
 - 👯 I’m looking to collaborate on [`Termux-snippets`](https://github.com/hakxcore/Termux-snippets)
 
 - 🤝 I’m looking for help with [`TrackPhoneNumber`](https://github.com/hakxcore/TrackPhoneNumber)
 
 - 💬 Ask me about **`pentesting`**
 
-- 📫 How to find me **from 👇** 
+- 📫 How to find me **from 👇**  -->
 
 <h3 align="left">Connect with me:</h3>
 
 
 <table style="border: none;">
   <tr style="border: none; padding: 0; margin: 0;">
  
@@ -142,33 +140,36 @@
   <a href="https://www.python.org" target="_blank"> 
     <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width='40' height='40' style='margin-right: 1rem;'/> 
   </a>
    </td>
     </tr>
 </table>
 
+---
+
+<p align="center"><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=hakxcore&theme=github_dark&layout=compact" width="495"></p>
 
-<h3 align="left">Github Stats:</h3>
+---
 
-<p align="center"><img src="https://github-readme-stats.vercel.app/api?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true" width="495"></p>
+<p align="center"><img src="https://github-readme-stats.vercel.app/api/?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true" width="495"></p>
 
 ---
 
 <p align="center"><img src="http://github-readme-streak-stats.herokuapp.com?user=hakxcore&theme=github-dark-blue&hide_border=true" width="495"></p>
 
 ---
 
-<!-- <p align="center"><img src="https://wakatime.com/share/@f1da14aa-8bdd-4153-8929-e5d2a84c18fa/fbc86a23-f5c5-48b0-b0b1-f6067ceb44c4.svg" width="495"></p>
+<p align="center"><img src="https://wakatime.com/share/@hakxcore/03139443-2c41-4d41-8369-1648b3cb1046.svg" width="495"></p>
 
 ---
 
-<p align="center"><img src="https://wakatime.com/share/@f1da14aa-8bdd-4153-8929-e5d2a84c18fa/4e719e13-8af6-4cd7-9d6f-e0c68e0adb5e.svg" width="495"></p></p> -->
 
-[![Hakxcor's GitHub Activity Graph](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=xcode)](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=xcode)
-  <br/> <br/> 
+<!-- [![Hakxcor's GitHub Activity Graph](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=github-dark-blue)](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=xcode) 
+  
+  --- -->
 
 [comment]: <> (
 hakxcore
 resources
 investigator
 jktravels
 investigation
@@ -178,23 +179,20 @@
 sunrise
 aday
 morph
 audio
 Matrix
 glitch
 weather
-35.154.197.179
 idcard
 business
 links-sites
 nonprofit-org
 )
 
 <h3 align="left">Support:</h3>
 <p><a href="https://www.buymeacoffee.com/hakxcore"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="https://www.buymeacoffee.com/hakxcore" /></a></p><br/><br/>
 
 <h3 align="left">Badges:</h3>
 <a href='https://docs.github.com/en/developers'><img src='https://raw.githubusercontent.com/acervenky/animated-github-badges/master/assets/devbadge.gif' width='40' height='40'>
 </a> <a href='https://education.github.com/pack'><img src='https://raw.githubusercontent.com/acervenky/animated-github-badges/master/assets/pro.gif' width='40' height='40'></a>
 <br /> <br /> 
-
-
```

#### html2text {}

```diff
@@ -1,46 +1,42 @@
-Metadata-Version: 2.1 Name: hakxcore Version: 0.0.9 Summary: Hakxcore personal
-Repo and python package Home-page: https://github.com/hakxcore/hakxcore Author:
-Mukesh Kumar Author-email: mukeshkumarchark@gmail.com License: MIT Licence
+Metadata-Version: 2.1 Name: hakxcore Version: 0.1.0 Summary: Hakxcore personal
+Repo and python package Home-page: https://github.com/hakxcore/hakxcore
 Download-URL: https://github.com/hakxcore/hakxcore/archive/refs/heads/main.zip
-Keywords: hakxcore,bug
-bounty,mukesh,pentesting,security,development,enterprenurship Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Information Technology
-Classifier: Operating System :: OS Independent Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.4 Description-Content-Type: text/markdown License-File:
-LICENCE # Hi ð, I'm [Mukesh](https://github.com/hakxcore) [butterfly]
-[butterfly]
+Author: Mukesh Kumar Author-email: mukeshkumarchark@gmail.com License: MIT
+Licence Keywords: hakxcore,bug
+bounty,mukesh,pentesting,security,development,enterprenurship Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+Operating System :: OS Independent Classifier: Topic :: Security Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3.4 Description-Content-Type: text/markdown License-File: LICENCE #
+Hi ð, I'm [Mukesh](https://github.com/hakxcore) [butterfly] [butterfly]
+`$ pip install hakxcore` [![Downloads](https://static.pepy.tech/badge/
+hakxcore)](https://pepy.tech/project/hakxcore) --- [https://github-profile-
+trophy.vercel.app/?username=hakxcore&column=8&theme=algolia&no-frame=true]
 [hakxcore]
-[hakxcore]
-- ð­ Iâm currently working on [`fig`](https://github.com/hakxcore/fig)
-project - ð± Iâm currently learning **`Go`** - ð¯ Iâm looking to
-collaborate on [`Termux-snippets`](https://github.com/hakxcore/Termux-snippets)
-- ð¤ Iâm looking for help with [`TrackPhoneNumber`](https://github.com/
-hakxcore/TrackPhoneNumber) - ð¬ Ask me about **`pentesting`** - ð« How to
-find me **from ð**
 **** Connect with me: ****
 [Dev_hakxcore] [hakxcore [Mukesh_kumar's [Mukesh_kumar's [Youtube_Hakxcore]
                twitter]  facebook]       instagram]      /tr>
 **** Languages and Tools I Know: ****
 [bash] [c] [cplusplus] [figma] [firebase] [git] [javascript] [linux] [python]
-**** Github Stats: ****
-                   [https://github-readme-stats.vercel.app/
-api?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true]
+---
+            [https://github-readme-stats.vercel.app/api/top-langs/
+             ?username=hakxcore&theme=github_dark&layout=compact]
+---
+                 [https://github-readme-stats.vercel.app/api/
+?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true]
 ---
  [http://github-readme-streak-stats.herokuapp.com?user=hakxcore&theme=github-
                           dark-blue&hide_border=true]
----  [![Hakxcor's GitHub Activity Graph](https://activity-graph.herokuapp.com/
-graph?username=hakxcore&theme=xcode)](https://activity-graph.herokuapp.com/
-graph?username=hakxcore&theme=xcode)
-
-[comment]: <> ( hakxcore resources investigator jktravels investigation domain-
-investigation music clock sunrise aday morph audio Matrix glitch weather
-35.154.197.179 idcard business links-sites nonprofit-org )
+---
+[https://wakatime.com/share/@hakxcore/03139443-2c41-4d41-8369-1648b3cb1046.svg]
+---  [comment]: <> ( hakxcore resources investigator jktravels investigation
+domain-investigation music clock sunrise aday morph audio Matrix glitch weather
+idcard business links-sites nonprofit-org )
 **** Support: ****
 [https://www.buymeacoffee.com/hakxcore]
 
 
 **** Badges: ****
 [https://raw.githubusercontent.com/acervenky/animated-github-badges/master/
 assets/devbadge.gif]â[https://raw.githubusercontent.com/acervenky/animated-
```

### Comparing `hakxcore-0.0.9/README.md` & `hakxcore-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # Hi 👋, I'm [Mukesh](https://github.com/hakxcore) <img src="media/butterfly.gif" alt="butterfly" width="150"/> <img src="media/dog.gif" alt="butterfly" width="200"/>
-<!--<h3 align="center"><img src="media/animated-tree.gif" alt="butterfly" width=15%/></h>-->
-</br>
+<!--<h3 align="center"><img src="media/animated-tree.gif" alt="butterfly" width=15%/></h>   width='700' height='200' style='margin-right: 1rem;'-->
 </br>
 </br>
 
-<table style="border: none;">
-  <tr style="border: none; padding: 0; margin: 0;">
-  <td style="border: none; padding: 0; margin: 0;"> 
-    <a href="https://github.com/ryo-ma/github-profile-trophy" target="_blank">
-      <img src="https://github-profile-trophy.vercel.app/?username=hakxcore" alt="hakxcore" width='700' height='200' style='margin-right: 1rem;'/>
-    </a>
-    </td>
-  </tr>
-  </table>
+`$ pip install hakxcore`
+[![Downloads](https://static.pepy.tech/badge/hakxcore)](https://pepy.tech/project/hakxcore)
+---
+
+<a href="https://github.com/ryo-ma/github-profile-trophy" target="_blank">
+  <img width=900 src="https://github-profile-trophy.vercel.app/?username=hakxcore&column=8&theme=algolia&no-frame=true"/>
+</a>
+
 <p align="left"> <img src="https://komarev.com/ghpvc/?username=hakxcore&label=Profile%20views&color=0e75b6&style=flat" alt="hakxcore" /> </p>
 
+<!--
 - 🔭 I’m currently working on [`fig`](https://github.com/hakxcore/fig) project
 
 - 🌱 I’m currently learning **`Go`**
 
 - 👯 I’m looking to collaborate on [`Termux-snippets`](https://github.com/hakxcore/Termux-snippets)
 
 - 🤝 I’m looking for help with [`TrackPhoneNumber`](https://github.com/hakxcore/TrackPhoneNumber)
 
 - 💬 Ask me about **`pentesting`**
 
-- 📫 How to find me **from 👇** 
+- 📫 How to find me **from 👇**  -->
 
 <h3 align="left">Connect with me:</h3>
 
 
 <table style="border: none;">
   <tr style="border: none; padding: 0; margin: 0;">
  
@@ -121,33 +120,36 @@
   <a href="https://www.python.org" target="_blank"> 
     <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width='40' height='40' style='margin-right: 1rem;'/> 
   </a>
    </td>
     </tr>
 </table>
 
+---
+
+<p align="center"><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=hakxcore&theme=github_dark&layout=compact" width="495"></p>
 
-<h3 align="left">Github Stats:</h3>
+---
 
-<p align="center"><img src="https://github-readme-stats.vercel.app/api?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true" width="495"></p>
+<p align="center"><img src="https://github-readme-stats.vercel.app/api/?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true" width="495"></p>
 
 ---
 
 <p align="center"><img src="http://github-readme-streak-stats.herokuapp.com?user=hakxcore&theme=github-dark-blue&hide_border=true" width="495"></p>
 
 ---
 
-<!-- <p align="center"><img src="https://wakatime.com/share/@f1da14aa-8bdd-4153-8929-e5d2a84c18fa/fbc86a23-f5c5-48b0-b0b1-f6067ceb44c4.svg" width="495"></p>
+<p align="center"><img src="https://wakatime.com/share/@hakxcore/03139443-2c41-4d41-8369-1648b3cb1046.svg" width="495"></p>
 
 ---
 
-<p align="center"><img src="https://wakatime.com/share/@f1da14aa-8bdd-4153-8929-e5d2a84c18fa/4e719e13-8af6-4cd7-9d6f-e0c68e0adb5e.svg" width="495"></p></p> -->
 
-[![Hakxcor's GitHub Activity Graph](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=xcode)](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=xcode)
-  <br/> <br/> 
+<!-- [![Hakxcor's GitHub Activity Graph](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=github-dark-blue)](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=xcode) 
+  
+  --- -->
 
 [comment]: <> (
 hakxcore
 resources
 investigator
 jktravels
 investigation
@@ -157,15 +159,14 @@
 sunrise
 aday
 morph
 audio
 Matrix
 glitch
 weather
-35.154.197.179
 idcard
 business
 links-sites
 nonprofit-org
 )
 
 <h3 align="left">Support:</h3>
```

#### html2text {}

```diff
@@ -1,34 +1,31 @@
 # Hi ð, I'm [Mukesh](https://github.com/hakxcore) [butterfly] [butterfly]
+`$ pip install hakxcore` [![Downloads](https://static.pepy.tech/badge/
+hakxcore)](https://pepy.tech/project/hakxcore) --- [https://github-profile-
+trophy.vercel.app/?username=hakxcore&column=8&theme=algolia&no-frame=true]
 [hakxcore]
-[hakxcore]
-- ð­ Iâm currently working on [`fig`](https://github.com/hakxcore/fig)
-project - ð± Iâm currently learning **`Go`** - ð¯ Iâm looking to
-collaborate on [`Termux-snippets`](https://github.com/hakxcore/Termux-snippets)
-- ð¤ Iâm looking for help with [`TrackPhoneNumber`](https://github.com/
-hakxcore/TrackPhoneNumber) - ð¬ Ask me about **`pentesting`** - ð« How to
-find me **from ð**
 **** Connect with me: ****
 [Dev_hakxcore] [hakxcore [Mukesh_kumar's [Mukesh_kumar's [Youtube_Hakxcore]
                twitter]  facebook]       instagram]      /tr>
 **** Languages and Tools I Know: ****
 [bash] [c] [cplusplus] [figma] [firebase] [git] [javascript] [linux] [python]
-**** Github Stats: ****
-                   [https://github-readme-stats.vercel.app/
-api?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true]
+---
+            [https://github-readme-stats.vercel.app/api/top-langs/
+             ?username=hakxcore&theme=github_dark&layout=compact]
+---
+                 [https://github-readme-stats.vercel.app/api/
+?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true]
 ---
  [http://github-readme-streak-stats.herokuapp.com?user=hakxcore&theme=github-
                           dark-blue&hide_border=true]
----  [![Hakxcor's GitHub Activity Graph](https://activity-graph.herokuapp.com/
-graph?username=hakxcore&theme=xcode)](https://activity-graph.herokuapp.com/
-graph?username=hakxcore&theme=xcode)
-
-[comment]: <> ( hakxcore resources investigator jktravels investigation domain-
-investigation music clock sunrise aday morph audio Matrix glitch weather
-35.154.197.179 idcard business links-sites nonprofit-org )
+---
+[https://wakatime.com/share/@hakxcore/03139443-2c41-4d41-8369-1648b3cb1046.svg]
+---  [comment]: <> ( hakxcore resources investigator jktravels investigation
+domain-investigation music clock sunrise aday morph audio Matrix glitch weather
+idcard business links-sites nonprofit-org )
 **** Support: ****
 [https://www.buymeacoffee.com/hakxcore]
 
 
 **** Badges: ****
 [https://raw.githubusercontent.com/acervenky/animated-github-badges/master/
 assets/devbadge.gif]â[https://raw.githubusercontent.com/acervenky/animated-
```

### Comparing `hakxcore-0.0.9/hakxcore/__main__.py` & `hakxcore-0.1.0/hakxcore/__main__.py`

 * *Files identical despite different names*

### Comparing `hakxcore-0.0.9/hakxcore.egg-info/PKG-INFO` & `hakxcore-0.1.0/hakxcore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 Metadata-Version: 2.1
 Name: hakxcore
-Version: 0.0.9
+Version: 0.1.0
 Summary: Hakxcore personal Repo and python package
 Home-page: https://github.com/hakxcore/hakxcore
+Download-URL: https://github.com/hakxcore/hakxcore/archive/refs/heads/main.zip
 Author: Mukesh Kumar
 Author-email: mukeshkumarchark@gmail.com
 License: MIT Licence
-Download-URL: https://github.com/hakxcore/hakxcore/archive/refs/heads/main.zip
 Keywords: hakxcore,bug bounty,mukesh,pentesting,security,development,enterprenurship
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.4
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Hi 👋, I'm [Mukesh](https://github.com/hakxcore) <img src="media/butterfly.gif" alt="butterfly" width="150"/> <img src="media/dog.gif" alt="butterfly" width="200"/>
-<!--<h3 align="center"><img src="media/animated-tree.gif" alt="butterfly" width=15%/></h>-->
-</br>
+<!--<h3 align="center"><img src="media/animated-tree.gif" alt="butterfly" width=15%/></h>   width='700' height='200' style='margin-right: 1rem;'-->
 </br>
 </br>
 
-<table style="border: none;">
-  <tr style="border: none; padding: 0; margin: 0;">
-  <td style="border: none; padding: 0; margin: 0;"> 
-    <a href="https://github.com/ryo-ma/github-profile-trophy" target="_blank">
-      <img src="https://github-profile-trophy.vercel.app/?username=hakxcore" alt="hakxcore" width='700' height='200' style='margin-right: 1rem;'/>
-    </a>
-    </td>
-  </tr>
-  </table>
+`$ pip install hakxcore`
+[![Downloads](https://static.pepy.tech/badge/hakxcore)](https://pepy.tech/project/hakxcore)
+---
+
+<a href="https://github.com/ryo-ma/github-profile-trophy" target="_blank">
+  <img width=900 src="https://github-profile-trophy.vercel.app/?username=hakxcore&column=8&theme=algolia&no-frame=true"/>
+</a>
+
 <p align="left"> <img src="https://komarev.com/ghpvc/?username=hakxcore&label=Profile%20views&color=0e75b6&style=flat" alt="hakxcore" /> </p>
 
+<!--
 - 🔭 I’m currently working on [`fig`](https://github.com/hakxcore/fig) project
 
 - 🌱 I’m currently learning **`Go`**
 
 - 👯 I’m looking to collaborate on [`Termux-snippets`](https://github.com/hakxcore/Termux-snippets)
 
 - 🤝 I’m looking for help with [`TrackPhoneNumber`](https://github.com/hakxcore/TrackPhoneNumber)
 
 - 💬 Ask me about **`pentesting`**
 
-- 📫 How to find me **from 👇** 
+- 📫 How to find me **from 👇**  -->
 
 <h3 align="left">Connect with me:</h3>
 
 
 <table style="border: none;">
   <tr style="border: none; padding: 0; margin: 0;">
  
@@ -142,33 +140,36 @@
   <a href="https://www.python.org" target="_blank"> 
     <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width='40' height='40' style='margin-right: 1rem;'/> 
   </a>
    </td>
     </tr>
 </table>
 
+---
+
+<p align="center"><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=hakxcore&theme=github_dark&layout=compact" width="495"></p>
 
-<h3 align="left">Github Stats:</h3>
+---
 
-<p align="center"><img src="https://github-readme-stats.vercel.app/api?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true" width="495"></p>
+<p align="center"><img src="https://github-readme-stats.vercel.app/api/?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true" width="495"></p>
 
 ---
 
 <p align="center"><img src="http://github-readme-streak-stats.herokuapp.com?user=hakxcore&theme=github-dark-blue&hide_border=true" width="495"></p>
 
 ---
 
-<!-- <p align="center"><img src="https://wakatime.com/share/@f1da14aa-8bdd-4153-8929-e5d2a84c18fa/fbc86a23-f5c5-48b0-b0b1-f6067ceb44c4.svg" width="495"></p>
+<p align="center"><img src="https://wakatime.com/share/@hakxcore/03139443-2c41-4d41-8369-1648b3cb1046.svg" width="495"></p>
 
 ---
 
-<p align="center"><img src="https://wakatime.com/share/@f1da14aa-8bdd-4153-8929-e5d2a84c18fa/4e719e13-8af6-4cd7-9d6f-e0c68e0adb5e.svg" width="495"></p></p> -->
 
-[![Hakxcor's GitHub Activity Graph](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=xcode)](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=xcode)
-  <br/> <br/> 
+<!-- [![Hakxcor's GitHub Activity Graph](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=github-dark-blue)](https://activity-graph.herokuapp.com/graph?username=hakxcore&theme=xcode) 
+  
+  --- -->
 
 [comment]: <> (
 hakxcore
 resources
 investigator
 jktravels
 investigation
@@ -178,23 +179,20 @@
 sunrise
 aday
 morph
 audio
 Matrix
 glitch
 weather
-35.154.197.179
 idcard
 business
 links-sites
 nonprofit-org
 )
 
 <h3 align="left">Support:</h3>
 <p><a href="https://www.buymeacoffee.com/hakxcore"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="https://www.buymeacoffee.com/hakxcore" /></a></p><br/><br/>
 
 <h3 align="left">Badges:</h3>
 <a href='https://docs.github.com/en/developers'><img src='https://raw.githubusercontent.com/acervenky/animated-github-badges/master/assets/devbadge.gif' width='40' height='40'>
 </a> <a href='https://education.github.com/pack'><img src='https://raw.githubusercontent.com/acervenky/animated-github-badges/master/assets/pro.gif' width='40' height='40'></a>
 <br /> <br /> 
-
-
```

#### html2text {}

```diff
@@ -1,46 +1,42 @@
-Metadata-Version: 2.1 Name: hakxcore Version: 0.0.9 Summary: Hakxcore personal
-Repo and python package Home-page: https://github.com/hakxcore/hakxcore Author:
-Mukesh Kumar Author-email: mukeshkumarchark@gmail.com License: MIT Licence
+Metadata-Version: 2.1 Name: hakxcore Version: 0.1.0 Summary: Hakxcore personal
+Repo and python package Home-page: https://github.com/hakxcore/hakxcore
 Download-URL: https://github.com/hakxcore/hakxcore/archive/refs/heads/main.zip
-Keywords: hakxcore,bug
-bounty,mukesh,pentesting,security,development,enterprenurship Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Information Technology
-Classifier: Operating System :: OS Independent Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.4 Description-Content-Type: text/markdown License-File:
-LICENCE # Hi ð, I'm [Mukesh](https://github.com/hakxcore) [butterfly]
-[butterfly]
+Author: Mukesh Kumar Author-email: mukeshkumarchark@gmail.com License: MIT
+Licence Keywords: hakxcore,bug
+bounty,mukesh,pentesting,security,development,enterprenurship Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+Operating System :: OS Independent Classifier: Topic :: Security Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3.4 Description-Content-Type: text/markdown License-File: LICENCE #
+Hi ð, I'm [Mukesh](https://github.com/hakxcore) [butterfly] [butterfly]
+`$ pip install hakxcore` [![Downloads](https://static.pepy.tech/badge/
+hakxcore)](https://pepy.tech/project/hakxcore) --- [https://github-profile-
+trophy.vercel.app/?username=hakxcore&column=8&theme=algolia&no-frame=true]
 [hakxcore]
-[hakxcore]
-- ð­ Iâm currently working on [`fig`](https://github.com/hakxcore/fig)
-project - ð± Iâm currently learning **`Go`** - ð¯ Iâm looking to
-collaborate on [`Termux-snippets`](https://github.com/hakxcore/Termux-snippets)
-- ð¤ Iâm looking for help with [`TrackPhoneNumber`](https://github.com/
-hakxcore/TrackPhoneNumber) - ð¬ Ask me about **`pentesting`** - ð« How to
-find me **from ð**
 **** Connect with me: ****
 [Dev_hakxcore] [hakxcore [Mukesh_kumar's [Mukesh_kumar's [Youtube_Hakxcore]
                twitter]  facebook]       instagram]      /tr>
 **** Languages and Tools I Know: ****
 [bash] [c] [cplusplus] [figma] [firebase] [git] [javascript] [linux] [python]
-**** Github Stats: ****
-                   [https://github-readme-stats.vercel.app/
-api?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true]
+---
+            [https://github-readme-stats.vercel.app/api/top-langs/
+             ?username=hakxcore&theme=github_dark&layout=compact]
+---
+                 [https://github-readme-stats.vercel.app/api/
+?username=hakxcore&theme=github_dark&count_private=true&show_icons=true&include_all_commits=true&hide_border=true]
 ---
  [http://github-readme-streak-stats.herokuapp.com?user=hakxcore&theme=github-
                           dark-blue&hide_border=true]
----  [![Hakxcor's GitHub Activity Graph](https://activity-graph.herokuapp.com/
-graph?username=hakxcore&theme=xcode)](https://activity-graph.herokuapp.com/
-graph?username=hakxcore&theme=xcode)
-
-[comment]: <> ( hakxcore resources investigator jktravels investigation domain-
-investigation music clock sunrise aday morph audio Matrix glitch weather
-35.154.197.179 idcard business links-sites nonprofit-org )
+---
+[https://wakatime.com/share/@hakxcore/03139443-2c41-4d41-8369-1648b3cb1046.svg]
+---  [comment]: <> ( hakxcore resources investigator jktravels investigation
+domain-investigation music clock sunrise aday morph audio Matrix glitch weather
+idcard business links-sites nonprofit-org )
 **** Support: ****
 [https://www.buymeacoffee.com/hakxcore]
 
 
 **** Badges: ****
 [https://raw.githubusercontent.com/acervenky/animated-github-badges/master/
 assets/devbadge.gif]â[https://raw.githubusercontent.com/acervenky/animated-
```

### Comparing `hakxcore-0.0.9/index.html` & `hakxcore-0.1.0/index.html`

 * *Files identical despite different names*

### Comparing `hakxcore-0.0.9/media/aboutme.gif` & `hakxcore-0.1.0/media/aboutme.gif`

 * *Files identical despite different names*

### Comparing `hakxcore-0.0.9/media/animated-tree.gif` & `hakxcore-0.1.0/media/animated-tree.gif`

 * *Files identical despite different names*

### Comparing `hakxcore-0.0.9/media/butterfly.gif` & `hakxcore-0.1.0/media/butterfly.gif`

 * *Files identical despite different names*

### Comparing `hakxcore-0.0.9/media/dog.gif` & `hakxcore-0.1.0/media/dog.gif`

 * *Files identical despite different names*

### Comparing `hakxcore-0.0.9/media/hakxcore-logo.png` & `hakxcore-0.1.0/media/hakxcore-logo.png`

 * *Files identical despite different names*

### Comparing `hakxcore-0.0.9/media/hakxcore-logo1.png` & `hakxcore-0.1.0/media/hakxcore-logo1.png`

 * *Files identical despite different names*

### Comparing `hakxcore-0.0.9/setup.py` & `hakxcore-0.1.0/setup.py`

 * *Files identical despite different names*

