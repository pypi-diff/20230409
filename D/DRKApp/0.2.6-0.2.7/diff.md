# Comparing `tmp/DRKApp-0.2.6.tar.gz` & `tmp/DRKApp-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DRKApp-0.2.6.tar", last modified: Sat Mar 11 18:36:09 2023, max compression
+gzip compressed data, was "dist/DRKApp-0.2.7.tar", last modified: Sun Apr  9 12:33:38 2023, max compression
```

## Comparing `DRKApp-0.2.6.tar` & `DRKApp-0.2.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 rahulraj   (501) staff       (20)        0 2023-03-11 18:36:09.000000 DRKApp-0.2.6/
--rw-r--r--   0 rahulraj   (501) staff       (20)      613 2023-03-11 18:36:09.000000 DRKApp-0.2.6/PKG-INFO
--rw-r--r--   0 rahulraj   (501) staff       (20)      806 2023-03-11 18:36:03.000000 DRKApp-0.2.6/setup.py
-drwxr-xr-x   0 rahulraj   (501) staff       (20)        0 2023-03-11 18:36:09.000000 DRKApp-0.2.6/DRKApp.egg-info/
--rw-r--r--   0 rahulraj   (501) staff       (20)      613 2023-03-11 18:36:09.000000 DRKApp-0.2.6/DRKApp.egg-info/PKG-INFO
--rw-r--r--   0 rahulraj   (501) staff       (20)      176 2023-03-11 18:36:09.000000 DRKApp-0.2.6/DRKApp.egg-info/SOURCES.txt
--rw-r--r--   0 rahulraj   (501) staff       (20)       22 2023-03-11 18:36:09.000000 DRKApp-0.2.6/DRKApp.egg-info/requires.txt
--rw-r--r--   0 rahulraj   (501) staff       (20)        7 2023-03-11 18:36:09.000000 DRKApp-0.2.6/DRKApp.egg-info/top_level.txt
--rw-r--r--   0 rahulraj   (501) staff       (20)        1 2023-03-11 18:36:09.000000 DRKApp-0.2.6/DRKApp.egg-info/dependency_links.txt
-drwxr-xr-x   0 rahulraj   (501) staff       (20)        0 2023-03-11 18:36:09.000000 DRKApp-0.2.6/DRKApp/
--rw-r--r--   0 rahulraj   (501) staff       (20)     6180 2023-03-11 18:35:56.000000 DRKApp-0.2.6/DRKApp/__init__.py
--rw-r--r--   0 rahulraj   (501) staff       (20)       38 2023-03-11 18:36:09.000000 DRKApp-0.2.6/setup.cfg
+drwxr-xr-x   0 rahulraj   (501) staff       (20)        0 2023-04-09 12:33:38.000000 DRKApp-0.2.7/
+-rw-r--r--   0 rahulraj   (501) staff       (20)      613 2023-04-09 12:33:38.000000 DRKApp-0.2.7/PKG-INFO
+-rw-r--r--   0 rahulraj   (501) staff       (20)      806 2023-04-09 12:33:10.000000 DRKApp-0.2.7/setup.py
+drwxr-xr-x   0 rahulraj   (501) staff       (20)        0 2023-04-09 12:33:38.000000 DRKApp-0.2.7/DRKApp.egg-info/
+-rw-r--r--   0 rahulraj   (501) staff       (20)      613 2023-04-09 12:33:38.000000 DRKApp-0.2.7/DRKApp.egg-info/PKG-INFO
+-rw-r--r--   0 rahulraj   (501) staff       (20)      176 2023-04-09 12:33:38.000000 DRKApp-0.2.7/DRKApp.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulraj   (501) staff       (20)       22 2023-04-09 12:33:38.000000 DRKApp-0.2.7/DRKApp.egg-info/requires.txt
+-rw-r--r--   0 rahulraj   (501) staff       (20)        7 2023-04-09 12:33:38.000000 DRKApp-0.2.7/DRKApp.egg-info/top_level.txt
+-rw-r--r--   0 rahulraj   (501) staff       (20)        1 2023-04-09 12:33:38.000000 DRKApp-0.2.7/DRKApp.egg-info/dependency_links.txt
+drwxr-xr-x   0 rahulraj   (501) staff       (20)        0 2023-04-09 12:33:38.000000 DRKApp-0.2.7/DRKApp/
+-rw-r--r--   0 rahulraj   (501) staff       (20)     7141 2023-04-09 12:32:02.000000 DRKApp-0.2.7/DRKApp/__init__.py
+-rw-r--r--   0 rahulraj   (501) staff       (20)       38 2023-04-09 12:33:38.000000 DRKApp-0.2.7/setup.cfg
```

### Comparing `DRKApp-0.2.6/PKG-INFO` & `DRKApp-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: DRKApp
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python package to access the DRK APP API
 Home-page: https://github.com/iamrraj/Mattr_lib
 Author: Rahul Raj
 Author-email: rajr97333@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: DRK APP API
```

### Comparing `DRKApp-0.2.6/setup.py` & `DRKApp-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Create a setup.py file for the drkApp package
 
 from setuptools import setup
 
 
 setup(
     name='DRKApp',
-    version='0.2.6',
+    version='0.2.7',
     description="A Python package to access the DRK APP API",
     url='https://github.com/iamrraj/Mattr_lib',
     author="Rahul Raj",
     author_email="rajr97333@gmail.com",
     license='MIT',
     packages=['DRKApp'],
     install_requires=[
```

### Comparing `DRKApp-0.2.6/DRKApp.egg-info/PKG-INFO` & `DRKApp-0.2.7/DRKApp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: DRKApp
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python package to access the DRK APP API
 Home-page: https://github.com/iamrraj/Mattr_lib
 Author: Rahul Raj
 Author-email: rajr97333@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: DRK APP API
```

### Comparing `DRKApp-0.2.6/DRKApp/__init__.py` & `DRKApp-0.2.7/DRKApp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         """
         return {
             "partner_list": "users/partner-list/",
             "vulnerabilities": "case/vulnerabilities/",
             "dropdowns": "case/dropdown/",
             "case_list": "case/all-case/",
             "third-party": "case/third-party-case-details/",
+            "threat-data": "case/threat-data/",
         }
 
     def check_required_params(self):
         """
         Checks whether all the required parameters are provided.
         """
         if not self.token:
@@ -174,7 +175,36 @@
 
         if response.status_code == 200 or response.status_code == 201:
             data = response.json()
             return {"data": data, "status": response.status_code}
         else:
             raise Exception(
                 f"Failed to fetch data from API with status code {response.status_code} and message {response.text}")
+
+    def get_threat_data(self, threat=None):
+        if threat is None:
+            raise ValueError("Threat is required")
+
+        api = self.api
+        self.check_required_params()
+
+        api_url = self.get_api_url()
+
+        final_api = self.all_api_list().get(api, None)
+
+        headers = {
+            "Authorization": f"Bearer {self.token}",
+            "Content-Type": "application/json",
+            "origin": api_url
+        }
+
+        response = requests.get(
+            f"{api_url}{final_api}{threat}/?api-key={self.token}",
+            headers=headers
+        )
+
+        if response.status_code == 200 or response.status_code == 201:
+            data = response.json()
+            return {"data": data, "status": response.status_code}
+        else:
+            raise Exception(
+                f"Failed to fetch data from API with status code {response.status_code} and message {response.text}")
```

