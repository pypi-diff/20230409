# Comparing `tmp/cpcloud-0.0.2-py3-none-any.whl.zip` & `tmp/cpcloud-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6967 bytes, number of entries: 7
--rwxr-xr-x  2.0 unx     7809 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.data/scripts/cpcloud
--rwxr-xr-x  2.0 unx     7809 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.data/scripts/cpcloud.py
--rw-r--r--  2.0 unx     1077 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      574 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      569 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.dist-info/RECORD
-7 files, 17931 bytes uncompressed, 5953 bytes compressed:  66.8%
+Zip file size: 6997 bytes, number of entries: 7
+-rwxr-xr-x  2.0 unx     7900 b- defN 23-Apr-09 18:55 cpcloud-0.0.3.data/scripts/cpcloud
+-rwxr-xr-x  2.0 unx     7900 b- defN 23-Apr-09 18:55 cpcloud-0.0.3.data/scripts/cpcloud.py
+-rw-r--r--  2.0 unx     1077 b- defN 23-Apr-09 18:55 cpcloud-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      574 b- defN 23-Apr-09 18:55 cpcloud-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 18:55 cpcloud-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-09 18:55 cpcloud-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      569 b- defN 23-Apr-09 18:55 cpcloud-0.0.3.dist-info/RECORD
+7 files, 18113 bytes uncompressed, 5983 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: cpcloud-0.0.2.data/scripts/cpcloud
+Filename: cpcloud-0.0.3.data/scripts/cpcloud
 Comment: 
 
-Filename: cpcloud-0.0.2.data/scripts/cpcloud.py
+Filename: cpcloud-0.0.3.data/scripts/cpcloud.py
 Comment: 
 
-Filename: cpcloud-0.0.2.dist-info/LICENSE
+Filename: cpcloud-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: cpcloud-0.0.2.dist-info/METADATA
+Filename: cpcloud-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: cpcloud-0.0.2.dist-info/WHEEL
+Filename: cpcloud-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: cpcloud-0.0.2.dist-info/top_level.txt
+Filename: cpcloud-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cpcloud-0.0.2.dist-info/RECORD
+Filename: cpcloud-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cpcloud-0.0.2.data/scripts/cpcloud` & `cpcloud-0.0.3.data/scripts/cpcloud`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaFileUpload
 from googleapiclient.http import MediaIoBaseDownload
 
 from mimetypes import guess_type
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 SCOPES = [
     "https://www.googleapis.com/auth/drive",
     "https://www.googleapis.com/auth/drive.appdata",
     "https://www.googleapis.com/auth/drive.file",
 ]
 
@@ -45,15 +45,17 @@
     if not creds or not creds.valid:
         if creds and creds.expired and creds.refresh_token:
             creds.refresh(Request())
         else:
             flow = InstalledAppFlow.from_client_config(credentials, SCOPES)
             creds = flow.run_local_server(port=0)
         # Save the credentials for the next run
-        os.makedirs(os.path.dirname(TOKEN_FILE))
+        directory_path = os.path.dirname(TOKEN_FILE)
+        if not os.path.exists(directory_path):
+            os.makedirs(directory_path)
         with open(TOKEN_FILE, "w") as token:
             token.write(creds.to_json())
     return creds
 
 
 def upload_file(source_path, directory_id, service):
     try:
```

## Comparing `cpcloud-0.0.2.data/scripts/cpcloud.py` & `cpcloud-0.0.3.data/scripts/cpcloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaFileUpload
 from googleapiclient.http import MediaIoBaseDownload
 
 from mimetypes import guess_type
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 SCOPES = [
     "https://www.googleapis.com/auth/drive",
     "https://www.googleapis.com/auth/drive.appdata",
     "https://www.googleapis.com/auth/drive.file",
 ]
 
@@ -45,15 +45,17 @@
     if not creds or not creds.valid:
         if creds and creds.expired and creds.refresh_token:
             creds.refresh(Request())
         else:
             flow = InstalledAppFlow.from_client_config(credentials, SCOPES)
             creds = flow.run_local_server(port=0)
         # Save the credentials for the next run
-        os.makedirs(os.path.dirname(TOKEN_FILE))
+        directory_path = os.path.dirname(TOKEN_FILE)
+        if not os.path.exists(directory_path):
+            os.makedirs(directory_path)
         with open(TOKEN_FILE, "w") as token:
             token.write(creds.to_json())
     return creds
 
 
 def upload_file(source_path, directory_id, service):
     try:
```

## Comparing `cpcloud-0.0.2.dist-info/LICENSE` & `cpcloud-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cpcloud-0.0.2.dist-info/METADATA` & `cpcloud-0.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpcloud
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple tool to copy files using Google Drive.
 Author: Edzon Sanchez
 Author-email: edzon.sanchez@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

