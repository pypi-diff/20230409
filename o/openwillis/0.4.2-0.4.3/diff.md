# Comparing `tmp/openwillis-0.4.2.tar.gz` & `tmp/openwillis-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwillis-0.4.2.tar", last modified: Thu Apr  6 05:06:32 2023, max compression
+gzip compressed data, was "openwillis-0.4.3.tar", last modified: Sun Apr  9 12:20:21 2023, max compression
```

## Comparing `openwillis-0.4.2.tar` & `openwillis-0.4.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-06 05:06:32.697212 openwillis-0.4.2/
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)    13641 2023-04-05 21:12:43.000000 openwillis-0.4.2/LICENSE.txt
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      205 2023-04-05 21:12:43.000000 openwillis-0.4.2/MANIFEST.in
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1115 2023-04-06 05:06:32.697212 openwillis-0.4.2/PKG-INFO
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      814 2023-04-05 21:12:43.000000 openwillis-0.4.2/README.md
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-05 21:12:43.000000 openwillis-0.4.2/RELEASE.md
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-06 05:06:32.677212 openwillis-0.4.2/openwillis/
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      469 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/__init__.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-06 05:06:32.677212 openwillis-0.4.2/openwillis/features/
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/features/__init__.py
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      373 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/features/api.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-06 05:06:32.677212 openwillis-0.4.2/openwillis/features/audio/
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      103 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/features/audio/__init__.py
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)    10582 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/features/audio/acoustic.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-06 05:06:32.677212 openwillis-0.4.2/openwillis/features/audio/config/
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      706 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/features/audio/config/acoustic.json
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-06 05:06:32.687212 openwillis-0.4.2/openwillis/features/speech/
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      346 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/features/speech/__init__.py
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)     1778 2023-04-05 21:24:03.000000 openwillis-0.4.2/openwillis/features/speech/aws_transcribe.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-06 05:06:32.687212 openwillis-0.4.2/openwillis/features/speech/config/
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)     1593 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/features/speech/config/speech.json
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)     5349 2023-04-06 05:00:32.000000 openwillis-0.4.2/openwillis/features/speech/speech_attribute.py
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)     3498 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/features/speech/speech_separation.py
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)     5512 2023-04-05 21:18:23.000000 openwillis-0.4.2/openwillis/features/speech/speech_transcribe.py
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)    17145 2023-04-06 05:01:02.000000 openwillis-0.4.2/openwillis/features/speech/util.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-06 05:06:32.687212 openwillis-0.4.2/openwillis/features/video/
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/features/video/__init__.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-06 05:06:32.697212 openwillis-0.4.2/openwillis/features/video/config/
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      185 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/features/video/config/facial.json
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)    11731 2023-04-05 21:20:53.000000 openwillis-0.4.2/openwillis/features/video/face_landmark.py
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)     7426 2023-04-05 21:21:16.000000 openwillis-0.4.2/openwillis/features/video/facial_emotion.py
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      145 2023-04-05 21:12:43.000000 openwillis-0.4.2/openwillis/usability.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-06 05:06:32.677212 openwillis-0.4.2/openwillis.egg-info/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1115 2023-04-06 05:06:32.000000 openwillis-0.4.2/openwillis.egg-info/PKG-INFO
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      989 2023-04-06 05:06:32.000000 openwillis-0.4.2/openwillis.egg-info/SOURCES.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-06 05:06:32.000000 openwillis-0.4.2/openwillis.egg-info/dependency_links.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-06 05:06:32.000000 openwillis-0.4.2/openwillis.egg-info/not-zip-safe
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      372 2023-04-06 05:06:32.000000 openwillis-0.4.2/openwillis.egg-info/requires.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       11 2023-04-06 05:06:32.000000 openwillis-0.4.2/openwillis.egg-info/top_level.txt
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      385 2023-04-05 21:40:18.000000 openwillis-0.4.2/requirements.txt
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)       79 2023-04-06 05:06:32.697212 openwillis-0.4.2/setup.cfg
--rw-r--r--   0 ssm-user  (1001) ssm-user  (1001)      936 2023-04-06 05:05:24.000000 openwillis-0.4.2/setup.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.321899 openwillis-0.4.3/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    13641 2023-04-09 12:18:45.000000 openwillis-0.4.3/LICENSE.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      205 2023-04-09 12:18:45.000000 openwillis-0.4.3/MANIFEST.in
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1115 2023-04-09 12:20:21.321899 openwillis-0.4.3/PKG-INFO
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      814 2023-04-09 12:18:45.000000 openwillis-0.4.3/README.md
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-09 12:18:45.000000 openwillis-0.4.3/RELEASE.md
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.311899 openwillis-0.4.3/openwillis/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      469 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/__init__.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.311899 openwillis-0.4.3/openwillis/features/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/__init__.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      373 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/api.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.311899 openwillis-0.4.3/openwillis/features/audio/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      103 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/audio/__init__.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    15820 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/audio/acoustic.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.311899 openwillis-0.4.3/openwillis/features/audio/config/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      706 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/audio/config/acoustic.json
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.321899 openwillis-0.4.3/openwillis/features/speech/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      346 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/__init__.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     2388 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/aws_transcribe.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.321899 openwillis-0.4.3/openwillis/features/speech/config/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1593 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/config/speech.json
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     6061 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/speech_attribute.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     7234 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/speech_separation.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     9148 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/speech_transcribe.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    30695 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/util.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.321899 openwillis-0.4.3/openwillis/features/video/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/video/__init__.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.321899 openwillis-0.4.3/openwillis/features/video/config/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      185 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/video/config/facial.json
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    16067 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/video/face_landmark.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    10471 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/video/facial_emotion.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      145 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/usability.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.311899 openwillis-0.4.3/openwillis.egg-info/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1115 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/PKG-INFO
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      989 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/SOURCES.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/dependency_links.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/not-zip-safe
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      372 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/requires.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       11 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/top_level.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      385 2023-04-09 12:18:45.000000 openwillis-0.4.3/requirements.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       79 2023-04-09 12:20:21.321899 openwillis-0.4.3/setup.cfg
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      936 2023-04-09 12:19:12.000000 openwillis-0.4.3/setup.py
```

### Comparing `openwillis-0.4.2/LICENSE.txt` & `openwillis-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.2/PKG-INFO` & `openwillis-0.4.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 0.4.2
+Version: 0.4.3
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6.*
 Description-Content-Type: text/markdown
```

### Comparing `openwillis-0.4.2/README.md` & `openwillis-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.2/openwillis/features/audio/config/acoustic.json` & `openwillis-0.4.3/openwillis/features/audio/config/acoustic.json`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.2/openwillis/features/speech/aws_transcribe.py` & `openwillis-0.4.3/openwillis/features/speech/aws_transcribe.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,25 +10,39 @@
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger=logging.getLogger()
 
 def transcribe_audio(s3uri, region_name, job_name, language = 'en-US'):
     """
+    ------------------------------------------------------------------------------------------------------
+
     Transcribe an audio file using AWS Transcribe.
 
-    Args:
-        job_uri (str): The S3 URI of the input audio file.
-        output_bucket (str): The name of the S3 bucket where the output file should be saved.
+    Parameters:
+    ...........
+    s3uri : str
+        The S3 URI of the input audio file.
+    region_name : str
+        The region where the transcription should be done.
+    job_name : str
+        The name of the transcription job.
+    language : str, optional
+        The language used in the input audio file. Default is 'en-US'.
 
     Raises:
-        Exception: If the transcription job fails.
+    ...........
+    Exception: If the transcription job fails.
 
     Returns:
-        str: The transcript of the audio file.
+    ...........
+    tuple : Two strings, the first string is the response object in JSON format, and the second string is
+    the transcript of the audio file.
+
+    ------------------------------------------------------------------------------------------------------
     """
     response = "{}"
     transcript = ""
 
     try:
         transcribe = boto3.client('transcribe', region_name = region_name)
         settings = {'ShowSpeakerLabels': True, 'MaxSpeakerLabels': 2}
@@ -42,18 +56,20 @@
             Settings=settings
         )
 
         while True:
             status = transcribe.get_transcription_job(TranscriptionJobName=job_name)
             if status['TranscriptionJob']['TranscriptionJobStatus'] in ['COMPLETED', 'FAILED']:
                 break
-            logger.info("Not ready yet...")
+            #logger.info("Not ready yet...")
 
         if status['TranscriptionJob']['TranscriptionJobStatus'] == 'COMPLETED':
             read_data = urllib.request.urlopen(status['TranscriptionJob']['Transcript']['TranscriptFileUri'])
+            
             response = json.loads(read_data.read().decode('utf-8'))
+            transcript = response['results']['transcripts'][0]['transcript']
 
     except Exception as e:
-        logger.error("Transcription job failed with exception: {}".format(e))
+        logger.error(f"Transcription job failed with file: {s3uri} exception: {e}")
 
     finally:
         return response, transcript
```

### Comparing `openwillis-0.4.2/openwillis/features/speech/config/speech.json` & `openwillis-0.4.3/openwillis/features/speech/config/speech.json`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.2/openwillis/features/speech/speech_attribute.py` & `openwillis-0.4.3/openwillis/features/speech/speech_attribute.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,122 +10,152 @@
 from openwillis.features.speech import util as ut
 
 logging.basicConfig(level=logging.INFO)
 logger=logging.getLogger()
 
 def get_config():
     """
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
 
-    This function reads the configuration file containing the column names for the output dataframes, and returns the
-    contents of the file as a dictionary.
+    This function reads the configuration file containing the column names for the output dataframes,
+    and returns the contents of the file as a dictionary.
+
+    Parameters:
+    ...........
+    None
 
     Returns:
-        measures: A dictionary containing the names of the columns in the output dataframes.
+    ...........
+    measures: A dictionary containing the names of the columns in the output dataframes.
 
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
     """
     dir_name = os.path.dirname(os.path.abspath(__file__))
     measure_path = os.path.abspath(os.path.join(dir_name, 'config/speech.json'))
 
     file = open(measure_path)
     measures = json.load(file)
     return measures
 
 def create_empty_dataframes(measures):
     """
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
 
     Creating an empty measure dataframe
 
-    Args:
-        measures: config file object
+    Parameters:
+    ...........
+    measures: dict
+        config file object
 
-    Return:
-        empty pandas dataframe
+    Returns:
+    ...........
+    tag_df: pandas dataframe
+        an empty dataframe for the tags
+    summ_df: pandas dataframe
+        an empty dataframe for the summary
 
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
     """
     summ_df = pd.DataFrame(columns=[measures['tot_words'], measures['speech_verb'], measures['speech_adj'],
                                     measures['speech_pronoun'], measures['speech_noun'], measures['neg'], measures['neu'],
                                     measures['pos'], measures['compound'], measures['speech_mattr'], measures['rate_of_speech'],
                                     measures['pause_rate'], measures['pause_meandur'], measures['silence_ratio']])
 
     # Create an empty tag dataframe
     tag_df = pd.DataFrame(columns=[measures['word'], measures['tag']])
     return tag_df, summ_df
 
 def is_amazon_transcribe(json_conf):
     """
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
 
     This function checks if the json response object is from Amazon Transcribe.
 
-    Args:
-        json_conf: JSON response object.
+    Parameters:
+    ...........
+    json_conf: dict
+        JSON response object.
 
     Returns:
-        True if the json response object is from Amazon Transcribe, False otherwise.
+    ...........
+    bool: True if the json response object is from Amazon Transcribe, False otherwise.
 
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
     """
     return 'jobName' in json_conf and 'results' in json_conf
 
 def filter_transcribe(json_conf):
     """
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
 
     This function extracts the text and filters the JSON data for Amazon Transcribe json response objects.
 
-    Args:
-        json_conf: aws transcribe json response.
+    Parameters:
+    ...........
+    json_conf: dict
+        aws transcribe json response.
 
     Returns:
-        text: The text extracted from the JSON object.
-        filter_json: The filtered JSON object containing only the relevant data for processing.
+    ...........
+    text: str
+        The text extracted from the JSON object.
+    filter_json: list
+        The filtered JSON object containing only the relevant data for processing.
 
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
     """
     text = json_conf['results']['transcripts'][0].get('transcript', '')
     item_data = json_conf['results']['items']
     filter_json = [item for item in item_data if 'start_time' in item and 'end_time' in item]
     return text, filter_json
 
 def filter_vosk(json_conf):
     """
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
 
     This function extracts the text for json_conf objects from sources other than Amazon Transcribe.
 
-    Args:
-        json_conf: The input text in the form of a JSON object.
+    Parameters:
+    ...........
+    json_conf: dict
+        The input text in the form of a JSON object.
 
     Returns:
-        text: The input text extracted from the JSON object.
+    ...........
+    text: str
+        The input text extracted from the JSON object.
 
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
     """
     text_list = [word['word'] for word in json_conf if 'word' in word]
     text = " ".join(text_list)
     return text
 
 def speech_characteristics(json_conf, language='en-us'):
     """
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
 
     Speech Characteristics
 
-    Args:
-        json_conf: Transcribed json file
-        language: Language type
+    Parameters:
+    ...........
+    json_conf: dict
+        Transcribed json file
+    language: str
+        Language type
 
     Returns:
-        results: Speech Characteristics
+    ...........
+    tag_df: pandas dataframe
+        A dataframe containing speech tags
+    summ_df: pandas dataframe
+        A dataframe containing summary information on the speech
 
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
     """
     measures = get_config()
     tag_df, summ_df = create_empty_dataframes(measures)
 
     try:
         if bool(json_conf):
             ut.download_nltk_resources()
@@ -139,11 +169,11 @@
             else:
                 text = filter_vosk(json_conf)
                 if len(text) > 0:
                     tag_df, summ_df = ut.process_language_feature(json_conf, [tag_df, summ_df], text, language, measures,
                                                                ['start', 'end'])
 
     except Exception as e:
-        logger.info('Error in speech Characteristics {}'.format(e))
+        logger.error(f'Error in speech Characteristics {e}')
 
     finally:
         return tag_df, summ_df
```

### Comparing `openwillis-0.4.2/openwillis/features/video/facial_emotion.py` & `openwillis-0.4.3/openwillis/features/video/facial_emotion.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,24 +14,32 @@
 
 logging.basicConfig(level=logging.INFO)
 logger=logging.getLogger()
 
 
 def run_deepface(path, measures):
     """
-    -----------------------------------------------------------------------------------------
-    Calling deepface to fetch facial emotion
-
-    Args:
-        path: image path
-        measures: measures config object
+    ------------------------------------------------------------------------------------------------------
+    This function takes an image path and measures config object as input, and uses the DeepFace package to
+    fetch facial emotion for each frame of the video. It returns a list of dataframes, each containing facial
+    emotion data for one frame.
+
+    Parameters:
+    ..........
+    path: str
+        The path of the image file
+    measures: dict
+        A configuration object containing keys for different facial emotion measures
 
     Returns:
-        df_list: framewise facial emotion dataframe list
-    -----------------------------------------------------------------------------------------
+    ..........
+    df_list: list
+        A list of pandas dataframes where each dataframe contains facial emotion data for a single frame of
+        the video.
+    ------------------------------------------------------------------------------------------------------
     """
 
     df_list = []
     frame = 0
     cols = [measures['angry'], measures['disgust'], measures['fear'], measures['happy'], measures['sad'],
             measures['surprise'], measures['neutral']]
 
@@ -57,66 +65,105 @@
 
             except Exception as e:
                 df_emotion = get_undected_emotion(frame, cols)
                 df_list.append(df_emotion)
                 frame +=1
 
     except Exception as e:
-        logger.info('Face not detected by mediapipe')
+        logger.error(f'Face not detected by deepface for- file:{path} & Error: {e}')
+
+    finally:
+        #Empty dataframe in case of insufficient datapoints
+        if len(df_list)==0:
+            df_emotion = pd.DataFrame(columns = cols)
+
+            df_list.append(df_emotion)
+            logger.info(f'Face not detected by deepface in : {path}')
 
     return df_list
 
 def get_undected_emotion(frame, cols):
+    """
+    ------------------------------------------------------------------------------------------------------
+    This function returns a pandas dataframe with a single row of NaN values for the different facial emotion
+    measures. It is used to fill in missing values in cases where DeepFace is unable to detect facial emotion
+    for a particular frame.
+
+    Parameters:
+    ..........
+    frame: int
+        The frame number for which the dataframe is being created
+    cols: list
+        A list of column names for the facial emotion measures
+
+    Returns:
+    ..........
+    df_emotion: pandas dataframe
+        A dataframe with a single row of NaN values for the different facial emotion measures.
+    ------------------------------------------------------------------------------------------------------
+    """
     df_common = pd.DataFrame([[frame]], columns=['frame'])
     value = [np.nan] * len(cols)
 
     df = pd.DataFrame([value], columns = cols)
     df_emotion = pd.concat([df_common, df], axis=1)
     return df_emotion
 
 def get_emotion(path, error_info, measures):
     """
-    -----------------------------------------------------------------------------------------
-    Fetching facial emotion
-
-    Args:
-        path: image path
-        error_info: error location
-        measures: measures config object
+    ------------------------------------------------------------------------------------------------------
+    This function fetches facial emotion data for each frame of the input video. It calls the run_deepface()
+    function to get a list of dataframes containing facial emotion data for each frame and then concatenates
+    these dataframes into a single dataframe.
+
+    Parameters:
+    ..........
+    path: str
+        The path of the input video file
+    error_info: str
+        A string that specifies the type of error that occurred (e.g., 'input' or 'baseline')
+    measures: dict
+        A configuration object containing keys for different facial emotion measures.
 
     Returns:
-        df_emo: facial emotion dataframe
-    -----------------------------------------------------------------------------------------
+    ..........
+    df_emo: pandas dataframe
+        A dataframe containing facial emotion data for each frame of the input video.
+    ------------------------------------------------------------------------------------------------------
     """
 
     emotion_list = run_deepface(path, measures)
 
     if len(emotion_list)>0:
         df_emo = pd.concat(emotion_list).reset_index(drop=True)
 
-    else:
-        #Handle error in future
-        df_emo = pd.DataFrame()
-        logger.info('Face not detected by deepface in :'+ error_info)
-
     return df_emo
 
 def baseline(df, base_path, measures):
     """
-    -----------------------------------------------------------------------------------------
-    Normalize raw data
-
-    Args:
-        df: facial emotion dataframe
-        base_path: baseline input file path
-        measures: measures config object
+    ------------------------------------------------------------------------------------------------------
+    This function normalizes the facial emotion data in the input dataframe using the baseline video. If no
+    baseline video is provided, the function simply returns the input dataframe. If a baseline video is
+    provided, the function first calculates the mean of the facial emotion measures for the baseline video and
+    then normalizes the facial emotion measures in the input dataframe by dividing them by the baseline mean.
+
+    Parameters:
+    ..........
+    df: pandas dataframe
+        The input dataframe containing facial emotion data
+    base_path: str
+        The path to the baseline video
+    measures: dict
+        A configuration object containing keys for different facial emotion measures.
 
     Returns:
-        df_emotion: Normalized facial emotion dataframe
-    -----------------------------------------------------------------------------------------
+    ..........
+    df_emotion: pandas dataframe
+        The normalized facial emotion data.
+    ------------------------------------------------------------------------------------------------------
     """
 
     df_emo = df.copy()
 
     if not os.path.exists(base_path):
         return df_emo
 
@@ -134,64 +181,75 @@
         df_emo = df_emo.div(base_df.iloc[0])
 
     df_emotion = pd.concat([df_common, df_emo], axis=1)
     return df_emotion
 
 def get_summary(df):
     """
-    -----------------------------------------------------------------------------------------
-    Displacement summary
-
-    Args:
-        df: Framewise euclidean displacement dataframe
+    ------------------------------------------------------------------------------------------------------
+    This function calculates the summary statistics for the input dataframe containing the normalized facial
+    emotion data. It calculates the mean and standard deviation of each facial emotion measure and returns
+    them as a dataframe.
+
+    Parameters:
+    ..........
+    df: pandas dataframe
+        The input dataframe containing the normalized facial emotion data.
 
     Returns:
-        df_summ: stat summary dataframe
-    -----------------------------------------------------------------------------------------
+    ..........
+    df_summ: pandas dataframe
+        A dataframe containing the summary statistics for the normalized facial emotion data.
+    ------------------------------------------------------------------------------------------------------
     """
 
     df_summ = pd.DataFrame()
     if len(df)>0:
 
         df_summ = df.mean(axis=1)
         df_summ = pd.DataFrame({'mean': df.mean(), 'stdev': df.std()}).T
 
         df_summ = df_summ.reset_index().rename(columns={'index': 'stats'})
+        df_summ = df_summ.drop(columns=['frame'])
     return df_summ
 
 def emotional_expressivity(filepath, baseline_filepath=''):
     """
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
 
     Facial emotion detection and analysis
 
     This function uses serengil/deepface to quantify the framewise expressivity of facial emotions,
     specifically happiness, sadness, anger, fear, disgust, and surprise – in addition to measuring
     the absence of any emotion (neutral). The summary output provides overall measurements for the input.
 
     Parameters
-        filepath : str; path to video
-        baseline_filepath : str; optional path to baseline video. see openwillis research guidelines on github
-                   wiki to read case for baseline video use, particularly in clinical research contexts.
-                   (default is 0, meaning no baseline correction will be conducted).
+    ..........
+    filepath : str
+        path to video
+    baseline_filepath : str, optional
+        optional path to baseline video. see openwillis research guidelines on github wiki to read case
+        for baseline video use, particularly in clinical research contexts. (default is 0, meaning no
+        baseline correction will be conducted).
 
     Returns
-        framewise : data-type: dataframe with framewise output of facial emotion expressivity. first column
-                    is the frame number, second column is time in seconds, subsequent columns are emotional
-                    expressivity  measures, and last column is overall emotional expressivity i.e. a mean of
-                    all individual emotions except neutral. all values are between 0 and 1, as outputted by
-                    deepface.
-
-        summary: data-type: dataframe with summary measurements. first column is name of statistic, subsequent
-                 columns are facial emotions, last column is overall expressivity i.e. the mean of all emotions
-                 except neutral. first row contains mean expressivity and second row contains standard deviation.
-                 in case an optional baseline video was provided all measures are relative to baseline values
-                 calculated from baseline.
+    ..........
+    df_norm_emo : pandas dataframe
+        Dataframe with framewise output of facial emotion expressivity. first column is the frame number,
+        second column is time in seconds, subsequent columns are emotional expressivity  measures, and
+        last column is overall emotional expressivity i.e. a mean of all individual emotions except
+        neutral. all values are between 0 and 1, as outputted by deepface.
+
+    df_summ: pandas dataframe
+        Dataframe with summary measurements. first column is name of statistic, subsequent columns are
+        facial emotions, last column is overall expressivity i.e. the mean of all emotions except neutral.
+        first row contains mean expressivity and second row contains standard deviation. In case an optional
+        baseline video was provided all measures are relative to baseline values calculated from baseline.
 
-    -----------------------------------------------------------------------------------------
+    ------------------------------------------------------------------------------------------------------
     """
     try:
 
         #Loading json config
         dir_name = os.path.dirname(os.path.abspath(__file__))
         measure_path = os.path.abspath(os.path.join(dir_name, 'config/facial.json'))
 
@@ -211,8 +269,8 @@
             df_norm_emo = df_norm_emo - 1
             df_norm_emo['frame'] = df_norm_emo['frame'] + 1
 
         df_summ = get_summary(df_norm_emo)
         return df_norm_emo, df_summ
 
     except Exception as e:
-        logger.info('Error in facial emotion calculation')
+        logger.error(f'Error in facial emotion calculation- file: {filepath} & Error: {e}')
```

### Comparing `openwillis-0.4.2/openwillis.egg-info/PKG-INFO` & `openwillis-0.4.3/openwillis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 0.4.2
+Version: 0.4.3
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6.*
 Description-Content-Type: text/markdown
```

### Comparing `openwillis-0.4.2/openwillis.egg-info/SOURCES.txt` & `openwillis-0.4.3/openwillis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.2/setup.py` & `openwillis-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(name='openwillis',
-                 version='0.4.2',
+                 version='0.4.3',
                  description='digital health measurement',
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url='https://github.com/bklynhlth/openwillis',
                  author='bklynhlth',
                  python_requires='>=3.6.*',
                  install_requires=install_requires,
```

