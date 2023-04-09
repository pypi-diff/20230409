# Comparing `tmp/CustomGPT-0.1.3.tar.gz` & `tmp/CustomGPT-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomGPT-0.1.3.tar", last modified: Sun Apr  9 06:47:12 2023, max compression
+gzip compressed data, was "CustomGPT-0.1.4.tar", last modified: Sun Apr  9 07:03:52 2023, max compression
```

## Comparing `CustomGPT-0.1.3.tar` & `CustomGPT-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 06:47:12.263093 CustomGPT-0.1.3/
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 06:47:12.261791 CustomGPT-0.1.3/CustomGPT/
--rw-r--r--   0 lymengnaret   (501) staff       (20)       34 2023-04-09 06:46:21.000000 CustomGPT-0.1.3/CustomGPT/__init__.py
--rw-r--r--   0 lymengnaret   (501) staff       (20)     4202 2023-04-09 06:26:37.000000 CustomGPT-0.1.3/CustomGPT/custom_gpt.py
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 06:47:12.262624 CustomGPT-0.1.3/CustomGPT.egg-info/
--rw-r--r--   0 lymengnaret   (501) staff       (20)      762 2023-04-09 06:47:12.000000 CustomGPT-0.1.3/CustomGPT.egg-info/PKG-INFO
--rw-r--r--   0 lymengnaret   (501) staff       (20)      236 2023-04-09 06:47:12.000000 CustomGPT-0.1.3/CustomGPT.egg-info/SOURCES.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)        1 2023-04-09 06:47:12.000000 CustomGPT-0.1.3/CustomGPT.egg-info/dependency_links.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)       23 2023-04-09 06:47:12.000000 CustomGPT-0.1.3/CustomGPT.egg-info/requires.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)       10 2023-04-09 06:47:12.000000 CustomGPT-0.1.3/CustomGPT.egg-info/top_level.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)     1063 2023-04-09 05:26:04.000000 CustomGPT-0.1.3/LICENSE
--rw-r--r--   0 lymengnaret   (501) staff       (20)      762 2023-04-09 06:47:12.262841 CustomGPT-0.1.3/PKG-INFO
--rw-r--r--   0 lymengnaret   (501) staff       (20)      957 2023-04-09 05:57:50.000000 CustomGPT-0.1.3/README.md
--rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-09 06:47:12.263128 CustomGPT-0.1.3/setup.cfg
--rw-r--r--   0 lymengnaret   (501) staff       (20)      926 2023-04-09 06:47:03.000000 CustomGPT-0.1.3/setup.py
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 07:03:52.341856 CustomGPT-0.1.4/
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 07:03:52.340776 CustomGPT-0.1.4/CustomGPT/
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       34 2023-04-09 06:46:21.000000 CustomGPT-0.1.4/CustomGPT/__init__.py
+-rw-r--r--   0 lymengnaret   (501) staff       (20)     4383 2023-04-09 07:02:42.000000 CustomGPT-0.1.4/CustomGPT/custom_gpt.py
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 07:03:52.341534 CustomGPT-0.1.4/CustomGPT.egg-info/
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      762 2023-04-09 07:03:52.000000 CustomGPT-0.1.4/CustomGPT.egg-info/PKG-INFO
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      236 2023-04-09 07:03:52.000000 CustomGPT-0.1.4/CustomGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)        1 2023-04-09 07:03:52.000000 CustomGPT-0.1.4/CustomGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       23 2023-04-09 07:03:52.000000 CustomGPT-0.1.4/CustomGPT.egg-info/requires.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       10 2023-04-09 07:03:52.000000 CustomGPT-0.1.4/CustomGPT.egg-info/top_level.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)     1063 2023-04-09 05:26:04.000000 CustomGPT-0.1.4/LICENSE
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      762 2023-04-09 07:03:52.341709 CustomGPT-0.1.4/PKG-INFO
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      957 2023-04-09 05:57:50.000000 CustomGPT-0.1.4/README.md
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-09 07:03:52.341892 CustomGPT-0.1.4/setup.cfg
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      926 2023-04-09 07:03:45.000000 CustomGPT-0.1.4/setup.py
```

### Comparing `CustomGPT-0.1.3/CustomGPT/custom_gpt.py` & `CustomGPT-0.1.4/CustomGPT/custom_gpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,19 @@
         """
         res = self.session.get(
             "https://chat.openai.com/backend-api/models",
             headers={
                 "key": "value",
             },
         )
-        self.session.cookies.set("_puid", res.cookies["_puid"])
+        # Check if '_puid' exists in the response cookies
+        if "_puid" in res.cookies:
+            self.session.cookies.set("_puid", res.cookies["_puid"])
+        else:
+            print("Warning: _puid cookie not found in the response.")
 
     def filter_response(self, res):
         """
         Filter the API response to extract the relevant data.
 
         :param res: The raw API response
         :type res: requests.Response
```

### Comparing `CustomGPT-0.1.3/CustomGPT.egg-info/PKG-INFO` & `CustomGPT-0.1.4/CustomGPT.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomGPT
-Version: 0.1.3
+Version: 0.1.4
 Summary: A custom GPT package for interacting with GPT-4 models without using the OpenAI API.
 Home-page: https://github.com/NLmeng/CustomGPT
 Author: Lymeng Naret
 Author-email: lymengnaret@yahoo.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CustomGPT-0.1.3/LICENSE` & `CustomGPT-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CustomGPT-0.1.3/PKG-INFO` & `CustomGPT-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomGPT
-Version: 0.1.3
+Version: 0.1.4
 Summary: A custom GPT package for interacting with GPT-4 models without using the OpenAI API.
 Home-page: https://github.com/NLmeng/CustomGPT
 Author: Lymeng Naret
 Author-email: lymengnaret@yahoo.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CustomGPT-0.1.3/README.md` & `CustomGPT-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `CustomGPT-0.1.3/setup.py` & `CustomGPT-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="CustomGPT",
-    version="0.1.3",
+    version="0.1.4",
     description="A custom GPT package for interacting with GPT-4 models without using the OpenAI API.",
     author="Lymeng Naret",
     author_email="lymengnaret@yahoo.com",
     url="https://github.com/NLmeng/CustomGPT",
     packages=find_packages(),
     install_requires=[
         "requests",
```

