# Comparing `tmp/JarvisAI-4.6.tar.gz` & `tmp/JarvisAI-4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JarvisAI-4.6.tar", last modified: Mon Apr  3 21:46:35 2023, max compression
+gzip compressed data, was "JarvisAI-4.7.tar", last modified: Sun Apr  9 20:50:25 2023, max compression
```

## Comparing `JarvisAI-4.6.tar` & `JarvisAI-4.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 21:46:35.087928 JarvisAI-4.6/
-drwxrwxrwx   0        0        0        0 2023-04-03 21:46:35.050971 JarvisAI-4.6/JarvisAI/
--rw-rw-rw-   0        0        0    10957 2023-03-24 22:46:02.000000 JarvisAI-4.6/JarvisAI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 21:46:35.065009 JarvisAI-4.6/JarvisAI/brain/
--rw-rw-rw-   0        0        0        0 2023-01-28 22:07:15.000000 JarvisAI-4.6/JarvisAI/brain/__init__.py
--rw-rw-rw-   0        0        0      931 2023-03-23 20:58:20.000000 JarvisAI-4.6/JarvisAI/brain/auth.py
--rw-rw-rw-   0        0        0      588 2023-03-24 22:47:55.000000 JarvisAI-4.6/JarvisAI/brain/chatbot_premium.py
--rw-rw-rw-   0        0        0     1505 2023-03-23 21:12:29.000000 JarvisAI-4.6/JarvisAI/brain/intent_classification.py
--rw-rw-rw-   0        0        0      919 2023-02-07 20:01:05.000000 JarvisAI-4.6/JarvisAI/brain/ner.py
-drwxrwxrwx   0        0        0        0 2023-04-03 21:46:35.081735 JarvisAI-4.6/JarvisAI/features/
--rw-rw-rw-   0        0        0        0 2023-01-30 20:22:07.000000 JarvisAI-4.6/JarvisAI/features/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-02-07 18:50:21.000000 JarvisAI-4.6/JarvisAI/features/click_photo.py
--rw-rw-rw-   0        0        0     1280 2023-02-01 15:51:59.000000 JarvisAI-4.6/JarvisAI/features/covid_cases.py
--rw-rw-rw-   0        0        0      333 2023-01-30 20:25:31.000000 JarvisAI-4.6/JarvisAI/features/date_time.py
--rw-rw-rw-   0        0        0      363 2023-02-01 12:00:25.000000 JarvisAI-4.6/JarvisAI/features/games.py
--rw-rw-rw-   0        0        0      310 2023-01-31 20:51:42.000000 JarvisAI-4.6/JarvisAI/features/greet.py
--rw-rw-rw-   0        0        0      186 2022-09-07 20:52:45.000000 JarvisAI-4.6/JarvisAI/features/iambored.py
--rw-rw-rw-   0        0        0     1068 2023-02-18 06:02:00.000000 JarvisAI-4.6/JarvisAI/features/internet_speed_test.py
--rw-rw-rw-   0        0        0      364 2023-02-01 14:15:18.000000 JarvisAI-4.6/JarvisAI/features/joke.py
--rw-rw-rw-   0        0        0      867 2023-02-07 18:49:43.000000 JarvisAI-4.6/JarvisAI/features/news.py
--rw-rw-rw-   0        0        0      333 2023-02-01 12:06:47.000000 JarvisAI-4.6/JarvisAI/features/places_near_me.py
--rw-rw-rw-   0        0        0      625 2023-02-01 12:07:35.000000 JarvisAI-4.6/JarvisAI/features/screenshot.py
--rw-rw-rw-   0        0        0      895 2023-02-01 12:08:12.000000 JarvisAI-4.6/JarvisAI/features/send_email.py
--rw-rw-rw-   0        0        0      615 2023-02-04 21:00:42.000000 JarvisAI-4.6/JarvisAI/features/tell_me_about.py
--rw-rw-rw-   0        0        0     3923 2022-10-28 16:25:41.000000 JarvisAI-4.6/JarvisAI/features/volume_controller.py
--rw-rw-rw-   0        0        0      983 2023-02-07 18:52:14.000000 JarvisAI-4.6/JarvisAI/features/weather.py
--rw-rw-rw-   0        0        0      535 2023-02-01 12:11:48.000000 JarvisAI-4.6/JarvisAI/features/website_open.py
--rw-rw-rw-   0        0        0      449 2023-02-01 12:12:30.000000 JarvisAI-4.6/JarvisAI/features/whatsapp_message.py
--rw-rw-rw-   0        0        0      245 2023-02-01 12:13:22.000000 JarvisAI-4.6/JarvisAI/features/youtube_play.py
--rw-rw-rw-   0        0        0      492 2023-02-01 12:14:04.000000 JarvisAI-4.6/JarvisAI/features/youtube_video_downloader.py
--rw-rw-rw-   0        0        0     3215 2023-04-03 21:32:42.000000 JarvisAI-4.6/JarvisAI/features_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-03 21:46:35.082749 JarvisAI-4.6/JarvisAI/utils/
--rw-rw-rw-   0        0        0        0 2023-02-01 12:31:07.000000 JarvisAI-4.6/JarvisAI/utils/__init__.py
--rw-rw-rw-   0        0        0     3670 2023-03-22 10:09:12.000000 JarvisAI-4.6/JarvisAI/utils/input_output.py
-drwxrwxrwx   0        0        0        0 2023-04-03 21:46:35.084255 JarvisAI-4.6/JarvisAI/utils/speech_to_text/
--rw-rw-rw-   0        0        0        0 2022-04-15 22:21:43.000000 JarvisAI-4.6/JarvisAI/utils/speech_to_text/__init__.py
--rw-rw-rw-   0        0        0     2277 2023-02-18 05:09:23.000000 JarvisAI-4.6/JarvisAI/utils/speech_to_text/speech_to_text.py
--rw-rw-rw-   0        0        0      715 2023-02-18 05:28:03.000000 JarvisAI-4.6/JarvisAI/utils/speech_to_text/speech_to_text_whisper.py
-drwxrwxrwx   0        0        0        0 2023-04-03 21:46:35.085265 JarvisAI-4.6/JarvisAI/utils/text_to_speech/
--rw-rw-rw-   0        0        0        0 2022-02-14 22:10:32.000000 JarvisAI-4.6/JarvisAI/utils/text_to_speech/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-02-07 16:16:47.000000 JarvisAI-4.6/JarvisAI/utils/text_to_speech/text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-04-03 21:46:35.061503 JarvisAI-4.6/JarvisAI.egg-info/
--rw-rw-rw-   0        0        0    11289 2023-04-03 21:46:34.000000 JarvisAI-4.6/JarvisAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1350 2023-04-03 21:46:34.000000 JarvisAI-4.6/JarvisAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 21:46:34.000000 JarvisAI-4.6/JarvisAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      244 2023-04-03 21:46:34.000000 JarvisAI-4.6/JarvisAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-03 21:46:34.000000 JarvisAI-4.6/JarvisAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2021-12-14 06:46:58.000000 JarvisAI-4.6/License.txt
--rw-rw-rw-   0        0        0       45 2022-06-18 21:40:40.000000 JarvisAI-4.6/MANIFEST.in
--rw-rw-rw-   0        0        0    11289 2023-04-03 21:46:35.086650 JarvisAI-4.6/PKG-INFO
--rw-rw-rw-   0        0        0    10377 2023-03-23 21:34:13.000000 JarvisAI-4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-03 21:46:35.087928 JarvisAI-4.6/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-03 21:46:13.000000 JarvisAI-4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 20:50:25.057886 JarvisAI-4.7/
+drwxrwxrwx   0        0        0        0 2023-04-09 20:50:24.716306 JarvisAI-4.7/JarvisAI/
+-rw-rw-rw-   0        0        0    10957 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 20:50:24.799123 JarvisAI-4.7/JarvisAI/brain/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/brain/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/brain/auth.py
+-rw-rw-rw-   0        0        0     3401 2023-04-09 20:49:35.000000 JarvisAI-4.7/JarvisAI/brain/chatbot_premium.py
+-rw-rw-rw-   0        0        0     1505 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/brain/intent_classification.py
+-rw-rw-rw-   0        0        0      919 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/brain/ner.py
+drwxrwxrwx   0        0        0        0 2023-04-09 20:50:25.019455 JarvisAI-4.7/JarvisAI/features/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/click_photo.py
+-rw-rw-rw-   0        0        0     1280 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/covid_cases.py
+-rw-rw-rw-   0        0        0      333 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/date_time.py
+-rw-rw-rw-   0        0        0      363 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/games.py
+-rw-rw-rw-   0        0        0      310 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/greet.py
+-rw-rw-rw-   0        0        0      186 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/iambored.py
+-rw-rw-rw-   0        0        0     1068 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/internet_speed_test.py
+-rw-rw-rw-   0        0        0      364 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/joke.py
+-rw-rw-rw-   0        0        0      867 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/news.py
+-rw-rw-rw-   0        0        0      333 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/places_near_me.py
+-rw-rw-rw-   0        0        0      625 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/screenshot.py
+-rw-rw-rw-   0        0        0      895 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/send_email.py
+-rw-rw-rw-   0        0        0      615 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/tell_me_about.py
+-rw-rw-rw-   0        0        0     3923 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/volume_controller.py
+-rw-rw-rw-   0        0        0      983 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/weather.py
+-rw-rw-rw-   0        0        0      535 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/website_open.py
+-rw-rw-rw-   0        0        0      449 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/whatsapp_message.py
+-rw-rw-rw-   0        0        0      245 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/youtube_play.py
+-rw-rw-rw-   0        0        0      492 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/youtube_video_downloader.py
+-rw-rw-rw-   0        0        0     3215 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-09 20:50:25.026483 JarvisAI-4.7/JarvisAI/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/__init__.py
+-rw-rw-rw-   0        0        0     3670 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/input_output.py
+drwxrwxrwx   0        0        0        0 2023-04-09 20:50:25.045450 JarvisAI-4.7/JarvisAI/utils/speech_to_text/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/speech_to_text/__init__.py
+-rw-rw-rw-   0        0        0     2277 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/speech_to_text/speech_to_text.py
+-rw-rw-rw-   0        0        0      715 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/speech_to_text/speech_to_text_whisper.py
+drwxrwxrwx   0        0        0        0 2023-04-09 20:50:25.055973 JarvisAI-4.7/JarvisAI/utils/text_to_speech/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/text_to_speech/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/text_to_speech/text_to_speech.py
+drwxrwxrwx   0        0        0        0 2023-04-09 20:50:24.743871 JarvisAI-4.7/JarvisAI.egg-info/
+-rw-rw-rw-   0        0        0    12183 2023-04-09 20:50:24.000000 JarvisAI-4.7/JarvisAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1350 2023-04-09 20:50:24.000000 JarvisAI-4.7/JarvisAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 20:50:24.000000 JarvisAI-4.7/JarvisAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      354 2023-04-09 20:50:24.000000 JarvisAI-4.7/JarvisAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-09 20:50:24.000000 JarvisAI-4.7/JarvisAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-04-03 21:49:40.000000 JarvisAI-4.7/License.txt
+-rw-rw-rw-   0        0        0       45 2023-04-03 21:49:40.000000 JarvisAI-4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    12183 2023-04-09 20:50:25.057886 JarvisAI-4.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11271 2023-04-07 06:33:15.000000 JarvisAI-4.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 20:50:25.058902 JarvisAI-4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1856 2023-04-09 20:50:12.000000 JarvisAI-4.7/setup.py
```

### Comparing `JarvisAI-4.6/JarvisAI/__init__.py` & `JarvisAI-4.7/JarvisAI/__init__.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/brain/auth.py` & `JarvisAI-4.7/JarvisAI/brain/auth.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/brain/intent_classification.py` & `JarvisAI-4.7/JarvisAI/brain/intent_classification.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/brain/ner.py` & `JarvisAI-4.7/JarvisAI/brain/ner.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features/click_photo.py` & `JarvisAI-4.7/JarvisAI/features/click_photo.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features/covid_cases.py` & `JarvisAI-4.7/JarvisAI/features/covid_cases.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features/internet_speed_test.py` & `JarvisAI-4.7/JarvisAI/features/internet_speed_test.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features/news.py` & `JarvisAI-4.7/JarvisAI/features/news.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features/screenshot.py` & `JarvisAI-4.7/JarvisAI/features/screenshot.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features/send_email.py` & `JarvisAI-4.7/JarvisAI/features/send_email.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features/tell_me_about.py` & `JarvisAI-4.7/JarvisAI/features/tell_me_about.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features/volume_controller.py` & `JarvisAI-4.7/JarvisAI/features/volume_controller.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features/weather.py` & `JarvisAI-4.7/JarvisAI/features/weather.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features/website_open.py` & `JarvisAI-4.7/JarvisAI/features/website_open.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/features_manager.py` & `JarvisAI-4.7/JarvisAI/features_manager.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/utils/input_output.py` & `JarvisAI-4.7/JarvisAI/utils/input_output.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/utils/speech_to_text/speech_to_text.py` & `JarvisAI-4.7/JarvisAI/utils/speech_to_text/speech_to_text.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/utils/speech_to_text/speech_to_text_whisper.py` & `JarvisAI-4.7/JarvisAI/utils/speech_to_text/speech_to_text_whisper.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI/utils/text_to_speech/text_to_speech.py` & `JarvisAI-4.7/JarvisAI/utils/text_to_speech/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/JarvisAI.egg-info/PKG-INFO` & `JarvisAI-4.7/JarvisAI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JarvisAI
-Version: 4.6
+Version: 4.7
 Summary: JarvisAI is python library to build your own AI virtual assistant with natural language processing.
 Home-page: https://github.com/Dipeshpal/Jarvis_AI
 Author: Dipesh
 Author-email: dipeshpal17@gmail.com
 License: UNKNOWN
 Project-URL: Official Website, https://jarvisai.in
 Project-URL: Documentation, https://github.com/Dipeshpal/Jarvis_AI
@@ -36,14 +36,32 @@
 5. What it can do (Features it supports)    
 6. Future / Request Features    
 7. Contribute    
 8. Contact me    
 9. Donate    
 10. Thank me on-    
   
+## Premium Plan-
+
+What is our premium plan?
+
+- AI will be able to understand all your commands. It will answer all your questions apart from below basic intent.
+
+- It will be able to handle intent- 'others / Unknown Intent'. Free plan doesn't support this.
+
+- It will be automatically upgraded to use GPT-3 based model in the future. Currently, it uses other advance custom AI models to answer queries.
+
+- Currently unlimited API calls. Later we might change / limit.
+
+- Currently, it doesn't remember the previous context of the chat, but soon it will be. We don't store your
+        personal chat information.
+
+**Check out our plan: https://jarvisai.in/dashboard**
+
+
 ## YouTube Tutorial-  
   
 Click on the image below to watch the tutorial on YouTube-  
   
 **Tutorial 1-**  
   
 [![JarvisAI Tutorial 1](https://img.youtube.com/vi/p2hdqB11S-8/0.jpg)](https://www.youtube.com/watch?v=p2hdqB11S-8)  
@@ -185,15 +203,15 @@
  15. download youtube video 
  16. asking weather 
  17. take screenshot 
  18. open website 
  19. send whatsapp message 
  20. covid cases 
  21. check internet speed
- 22. others  / Unknown Intent  (IN PROGRESS)
+ 22. others  / Unknown Intent (Premium Feature)
 
   
 ### 5.2. Supported Input/Output Methods (Which option do I need to choose?)-    
 
 You can set below parameter while creating object of JarvisAI-
 
     jarvis = JarvisAI.Jarvis(input_mechanism='voice', output_mechanism='both',  
@@ -218,33 +236,38 @@
 	    output_mechanism='text'
 
 5. **For voice and text output-**    
 
 	    output_mechanism='both'
        
 ## 6. Future/Request Features-    
+
  **WIP**    
  **You tell me**    
+    at dipeshpal17@gmail.com or my social media.
     
  ## 7. Contribute-    
  **Instructions Coming Soon**    
  ## 8. Contact me-    
  - [Instagram](https://www.instagram.com/dipesh_pal17)    
         
 - [YouTube](https://www.youtube.com/dipeshpal17)    
         
     
     
 ## 9. Donate-    
- [Donate and Contribute to run me this project, and buy a domain](https://www.buymeacoffee.com/dipeshpal)    
+ 
+Consider donating to JarvisAI to support our mission of keeping our servers running 24/7. Your contribution will enable us to continue doing great things and providing valuable services. Every little bit helps!
+
+[Click Here to support](https://www.instamojo.com/@techport/?ref=preview)    
     
 **_Feel free to use my code, don't forget to mention credit. All the contributors will get credits in this repo._**    
  **_Mention below line for credits-_**    
  ***Credits-***    
- - [https://jarvis-ai-api.herokuapp.com](https://jarvis-ai-api.herokuapp.com/)    
+ - [https://jarvisai.in](https://jarvisai.in)    
         
 - [https://github.com/Dipeshpal/Jarvis_AI](https://github.com/Dipeshpal/Jarvis_AI)    
         
 - [https://www.youtube.com/dipeshpal17](https://www.youtube.com/dipeshpal17)    
         
 - [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/dipesh_pal17/)
```

### Comparing `JarvisAI-4.6/JarvisAI.egg-info/SOURCES.txt` & `JarvisAI-4.7/JarvisAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/License.txt` & `JarvisAI-4.7/License.txt`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.6/PKG-INFO` & `JarvisAI-4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JarvisAI
-Version: 4.6
+Version: 4.7
 Summary: JarvisAI is python library to build your own AI virtual assistant with natural language processing.
 Home-page: https://github.com/Dipeshpal/Jarvis_AI
 Author: Dipesh
 Author-email: dipeshpal17@gmail.com
 License: UNKNOWN
 Project-URL: Official Website, https://jarvisai.in
 Project-URL: Documentation, https://github.com/Dipeshpal/Jarvis_AI
@@ -36,14 +36,32 @@
 5. What it can do (Features it supports)    
 6. Future / Request Features    
 7. Contribute    
 8. Contact me    
 9. Donate    
 10. Thank me on-    
   
+## Premium Plan-
+
+What is our premium plan?
+
+- AI will be able to understand all your commands. It will answer all your questions apart from below basic intent.
+
+- It will be able to handle intent- 'others / Unknown Intent'. Free plan doesn't support this.
+
+- It will be automatically upgraded to use GPT-3 based model in the future. Currently, it uses other advance custom AI models to answer queries.
+
+- Currently unlimited API calls. Later we might change / limit.
+
+- Currently, it doesn't remember the previous context of the chat, but soon it will be. We don't store your
+        personal chat information.
+
+**Check out our plan: https://jarvisai.in/dashboard**
+
+
 ## YouTube Tutorial-  
   
 Click on the image below to watch the tutorial on YouTube-  
   
 **Tutorial 1-**  
   
 [![JarvisAI Tutorial 1](https://img.youtube.com/vi/p2hdqB11S-8/0.jpg)](https://www.youtube.com/watch?v=p2hdqB11S-8)  
@@ -185,15 +203,15 @@
  15. download youtube video 
  16. asking weather 
  17. take screenshot 
  18. open website 
  19. send whatsapp message 
  20. covid cases 
  21. check internet speed
- 22. others  / Unknown Intent  (IN PROGRESS)
+ 22. others  / Unknown Intent (Premium Feature)
 
   
 ### 5.2. Supported Input/Output Methods (Which option do I need to choose?)-    
 
 You can set below parameter while creating object of JarvisAI-
 
     jarvis = JarvisAI.Jarvis(input_mechanism='voice', output_mechanism='both',  
@@ -218,33 +236,38 @@
 	    output_mechanism='text'
 
 5. **For voice and text output-**    
 
 	    output_mechanism='both'
        
 ## 6. Future/Request Features-    
+
  **WIP**    
  **You tell me**    
+    at dipeshpal17@gmail.com or my social media.
     
  ## 7. Contribute-    
  **Instructions Coming Soon**    
  ## 8. Contact me-    
  - [Instagram](https://www.instagram.com/dipesh_pal17)    
         
 - [YouTube](https://www.youtube.com/dipeshpal17)    
         
     
     
 ## 9. Donate-    
- [Donate and Contribute to run me this project, and buy a domain](https://www.buymeacoffee.com/dipeshpal)    
+ 
+Consider donating to JarvisAI to support our mission of keeping our servers running 24/7. Your contribution will enable us to continue doing great things and providing valuable services. Every little bit helps!
+
+[Click Here to support](https://www.instamojo.com/@techport/?ref=preview)    
     
 **_Feel free to use my code, don't forget to mention credit. All the contributors will get credits in this repo._**    
  **_Mention below line for credits-_**    
  ***Credits-***    
- - [https://jarvis-ai-api.herokuapp.com](https://jarvis-ai-api.herokuapp.com/)    
+ - [https://jarvisai.in](https://jarvisai.in)    
         
 - [https://github.com/Dipeshpal/Jarvis_AI](https://github.com/Dipeshpal/Jarvis_AI)    
         
 - [https://www.youtube.com/dipeshpal17](https://www.youtube.com/dipeshpal17)    
         
 - [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/dipesh_pal17/)
```

### Comparing `JarvisAI-4.6/README.md` & `JarvisAI-4.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,32 @@
 5. What it can do (Features it supports)    
 6. Future / Request Features    
 7. Contribute    
 8. Contact me    
 9. Donate    
 10. Thank me on-    
   
+## Premium Plan-
+
+What is our premium plan?
+
+- AI will be able to understand all your commands. It will answer all your questions apart from below basic intent.
+
+- It will be able to handle intent- 'others / Unknown Intent'. Free plan doesn't support this.
+
+- It will be automatically upgraded to use GPT-3 based model in the future. Currently, it uses other advance custom AI models to answer queries.
+
+- Currently unlimited API calls. Later we might change / limit.
+
+- Currently, it doesn't remember the previous context of the chat, but soon it will be. We don't store your
+        personal chat information.
+
+**Check out our plan: https://jarvisai.in/dashboard**
+
+
 ## YouTube Tutorial-  
   
 Click on the image below to watch the tutorial on YouTube-  
   
 **Tutorial 1-**  
   
 [![JarvisAI Tutorial 1](https://img.youtube.com/vi/p2hdqB11S-8/0.jpg)](https://www.youtube.com/watch?v=p2hdqB11S-8)  
@@ -163,15 +181,15 @@
  15. download youtube video 
  16. asking weather 
  17. take screenshot 
  18. open website 
  19. send whatsapp message 
  20. covid cases 
  21. check internet speed
- 22. others  / Unknown Intent  (IN PROGRESS)
+ 22. others  / Unknown Intent (Premium Feature)
 
   
 ### 5.2. Supported Input/Output Methods (Which option do I need to choose?)-    
 
 You can set below parameter while creating object of JarvisAI-
 
     jarvis = JarvisAI.Jarvis(input_mechanism='voice', output_mechanism='both',  
@@ -196,33 +214,38 @@
 	    output_mechanism='text'
 
 5. **For voice and text output-**    
 
 	    output_mechanism='both'
        
 ## 6. Future/Request Features-    
+
  **WIP**    
  **You tell me**    
+    at dipeshpal17@gmail.com or my social media.
     
  ## 7. Contribute-    
  **Instructions Coming Soon**    
  ## 8. Contact me-    
  - [Instagram](https://www.instagram.com/dipesh_pal17)    
         
 - [YouTube](https://www.youtube.com/dipeshpal17)    
         
     
     
 ## 9. Donate-    
- [Donate and Contribute to run me this project, and buy a domain](https://www.buymeacoffee.com/dipeshpal)    
+ 
+Consider donating to JarvisAI to support our mission of keeping our servers running 24/7. Your contribution will enable us to continue doing great things and providing valuable services. Every little bit helps!
+
+[Click Here to support](https://www.instamojo.com/@techport/?ref=preview)    
     
 **_Feel free to use my code, don't forget to mention credit. All the contributors will get credits in this repo._**    
  **_Mention below line for credits-_**    
  ***Credits-***    
- - [https://jarvis-ai-api.herokuapp.com](https://jarvis-ai-api.herokuapp.com/)    
+ - [https://jarvisai.in](https://jarvisai.in)    
         
 - [https://github.com/Dipeshpal/Jarvis_AI](https://github.com/Dipeshpal/Jarvis_AI)    
         
 - [https://www.youtube.com/dipeshpal17](https://www.youtube.com/dipeshpal17)    
         
 - [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/dipesh_pal17/)
```

### Comparing `JarvisAI-4.6/setup.py` & `JarvisAI-4.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 from setuptools import find_namespace_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="JarvisAI",
-    version="4.6",
+    version="4.7",
     author="Dipesh",
     author_email="dipeshpal17@gmail.com",
     description="JarvisAI is python library to build your own AI virtual assistant with natural language processing.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Dipeshpal/Jarvis_AI",
     include_package_data=True,
     packages=find_namespace_packages(include=['JarvisAI.*', 'JarvisAI']),
     install_requires=['numpy', 'gtts', 'playsound', 'pyscreenshot', "opencv-python",
                       'SpeechRecognition', 'pyjokes', 'wikipedia', 'scipy', 'lazyme',
                       "requests", "pyttsx3", "spacy==3.5.0", 'pywhatkit', 'speedtest-cli',
                       'pytube', 'pycountry', 'playsound', 'pyaudio', 'mediapipe==0.8.11',
-                      'pycaw', 'openai-whisper', 'shutup', 'sounddevice'],
+                      'pycaw', 'openai-whisper', 'shutup', 'sounddevice', 'html2text==2020.1.16',
+                      'wikipedia==1.4.0', 'Markdown==3.4.1', 'markdown2==2.4.8',
+                      'lxml==4.9.2', 'googlesearch-python==1.2.3'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     project_urls={
```

