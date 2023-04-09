# Comparing `tmp/CustomGPT-0.1.0.tar.gz` & `tmp/CustomGPT-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomGPT-0.1.0.tar", last modified: Sun Apr  9 06:00:17 2023, max compression
+gzip compressed data, was "CustomGPT-0.1.1.tar", last modified: Sun Apr  9 06:19:41 2023, max compression
```

## Comparing `CustomGPT-0.1.0.tar` & `CustomGPT-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 06:00:17.208581 CustomGPT-0.1.0/
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 06:00:17.206521 CustomGPT-0.1.0/CustomGPT.egg-info/
--rw-r--r--   0 lymengnaret   (501) staff       (20)      762 2023-04-09 06:00:17.000000 CustomGPT-0.1.0/CustomGPT.egg-info/PKG-INFO
--rw-r--r--   0 lymengnaret   (501) staff       (20)      238 2023-04-09 06:00:17.000000 CustomGPT-0.1.0/CustomGPT.egg-info/SOURCES.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)        1 2023-04-09 06:00:17.000000 CustomGPT-0.1.0/CustomGPT.egg-info/dependency_links.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)       23 2023-04-09 06:00:17.000000 CustomGPT-0.1.0/CustomGPT.egg-info/requires.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)       11 2023-04-09 06:00:17.000000 CustomGPT-0.1.0/CustomGPT.egg-info/top_level.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)     1063 2023-04-09 05:26:04.000000 CustomGPT-0.1.0/LICENSE
--rw-r--r--   0 lymengnaret   (501) staff       (20)      762 2023-04-09 06:00:17.208405 CustomGPT-0.1.0/PKG-INFO
--rw-r--r--   0 lymengnaret   (501) staff       (20)      957 2023-04-09 05:57:50.000000 CustomGPT-0.1.0/README.md
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 06:00:17.207490 CustomGPT-0.1.0/custom_gpt/
--rw-r--r--   0 lymengnaret   (501) staff       (20)        0 2023-04-09 05:26:37.000000 CustomGPT-0.1.0/custom_gpt/__init__.py
--rw-r--r--   0 lymengnaret   (501) staff       (20)     4202 2023-04-09 05:50:01.000000 CustomGPT-0.1.0/custom_gpt/custom_gpt.py
--rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-09 06:00:17.208637 CustomGPT-0.1.0/setup.cfg
--rw-r--r--   0 lymengnaret   (501) staff       (20)      926 2023-04-09 05:48:37.000000 CustomGPT-0.1.0/setup.py
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 06:19:41.731566 CustomGPT-0.1.1/
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 06:19:41.730761 CustomGPT-0.1.1/CustomGPT.egg-info/
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      762 2023-04-09 06:19:41.000000 CustomGPT-0.1.1/CustomGPT.egg-info/PKG-INFO
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      238 2023-04-09 06:19:41.000000 CustomGPT-0.1.1/CustomGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)        1 2023-04-09 06:19:41.000000 CustomGPT-0.1.1/CustomGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       23 2023-04-09 06:19:41.000000 CustomGPT-0.1.1/CustomGPT.egg-info/requires.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       11 2023-04-09 06:19:41.000000 CustomGPT-0.1.1/CustomGPT.egg-info/top_level.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)     1063 2023-04-09 05:26:04.000000 CustomGPT-0.1.1/LICENSE
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      762 2023-04-09 06:19:41.731431 CustomGPT-0.1.1/PKG-INFO
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      957 2023-04-09 05:57:50.000000 CustomGPT-0.1.1/README.md
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-09 06:19:41.731052 CustomGPT-0.1.1/custom_gpt/
+-rw-r--r--   0 lymengnaret   (501) staff       (20)        0 2023-04-09 05:26:37.000000 CustomGPT-0.1.1/custom_gpt/__init__.py
+-rw-r--r--   0 lymengnaret   (501) staff       (20)     3830 2023-04-09 06:14:26.000000 CustomGPT-0.1.1/custom_gpt/custom_gpt.py
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-09 06:19:41.731604 CustomGPT-0.1.1/setup.cfg
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      926 2023-04-09 06:07:08.000000 CustomGPT-0.1.1/setup.py
```

### Comparing `CustomGPT-0.1.0/CustomGPT.egg-info/PKG-INFO` & `CustomGPT-0.1.1/CustomGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomGPT
-Version: 0.1.0
+Version: 0.1.1
 Summary: A custom GPT package for interacting with GPT-4 models without using the OpenAI API.
 Home-page: https://github.com/NLmeng/CustomGPT
 Author: Lymeng Naret
 Author-email: lymengnaret@yahoo.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CustomGPT-0.1.0/LICENSE` & `CustomGPT-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CustomGPT-0.1.0/PKG-INFO` & `CustomGPT-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomGPT
-Version: 0.1.0
+Version: 0.1.1
 Summary: A custom GPT package for interacting with GPT-4 models without using the OpenAI API.
 Home-page: https://github.com/NLmeng/CustomGPT
 Author: Lymeng Naret
 Author-email: lymengnaret@yahoo.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CustomGPT-0.1.0/README.md` & `CustomGPT-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `CustomGPT-0.1.0/custom_gpt/custom_gpt.py` & `CustomGPT-0.1.1/custom_gpt/custom_gpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,14 @@
             "referer": "https://chat.openai.com/chat",
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-site",
         })
         self.session.cookies.set("_puid", os.getenv("_PUID"))
         self.prev_id = str(uuid.uuid4())
-        self.fetch_puid()
 
     def start_new_chat(self):
         """
         Start a new chat session and continuously prompt the user for input.
         Print the model's responses and continue until "exit" is entered.
         """
         res = self.session.post(
@@ -92,26 +91,14 @@
                     }
                 ],
                 "parent_message_id": session['message']['id'],
                 "conversation_id": session['conversation_id'],
             },
         )
         return self.filter_response(res)
-    
-    def fetch_puid(self):
-        """
-        Fetch and set the "_puid" cookie for the session.
-        """
-        res = self.session.get(
-            "https://chat.openai.com/backend-api/models",
-            headers={
-                "key": "value",
-            },
-        )
-        self.session.cookies.set("_puid", res.cookies["_puid"])
 
     def filter_response(self, res):
         """
         Filter the API response to extract the relevant data.
 
         :param res: The raw API response
         :type res: requests.Response
```

### Comparing `CustomGPT-0.1.0/setup.py` & `CustomGPT-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="CustomGPT",
-    version="0.1.0",
+    version="0.1.1",
     description="A custom GPT package for interacting with GPT-4 models without using the OpenAI API.",
     author="Lymeng Naret",
     author_email="lymengnaret@yahoo.com",
     url="https://github.com/NLmeng/CustomGPT",
     packages=find_packages(),
     install_requires=[
         "requests",
```

