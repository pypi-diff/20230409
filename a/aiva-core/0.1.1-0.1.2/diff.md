# Comparing `tmp/aiva_core-0.1.1.tar.gz` & `tmp/aiva_core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiva_core-0.1.1.tar", max compression
+gzip compressed data, was "aiva_core-0.1.2.tar", max compression
```

## Comparing `aiva_core-0.1.1.tar` & `aiva_core-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0     1069 2023-03-18 09:34:43.339523 aiva_core-0.1.1/LICENSE
--rw-r--r--   0        0        0       79 2023-03-18 09:34:43.339523 aiva_core-0.1.1/README.md
--rw-r--r--   0        0        0      610 2023-03-22 15:19:31.213879 aiva_core-0.1.1/aiva/__init__.py
--rw-r--r--   0        0        0      610 2023-03-22 15:18:07.064106 aiva_core-0.1.1/aiva/core/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 08:39:46.743960 aiva_core-0.1.1/aiva/core/assistants/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 08:39:16.675922 aiva_core-0.1.1/aiva/core/assistants/classes/__init__.py
--rw-r--r--   0        0        0     2009 2023-04-04 16:24:17.903807 aiva_core-0.1.1/aiva/core/assistants/classes/aiva.py
--rw-r--r--   0        0        0        0 2023-03-18 10:44:39.271607 aiva_core-0.1.1/aiva/core/chatbots/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 16:17:19.925412 aiva_core-0.1.1/aiva/core/chatbots/classes/__init__.py
--rw-r--r--   0        0        0    13334 2023-04-04 15:29:22.675746 aiva_core-0.1.1/aiva/core/chatbots/classes/chat_gpt.py
--rw-r--r--   0        0        0     2668 2023-04-02 15:18:04.651397 aiva_core-0.1.1/aiva/core/exceptions/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-04 14:18:24.368586 aiva_core-0.1.1/aiva/core/types/__init__.py
--rw-r--r--   0        0        0        0 2023-03-18 11:37:48.145434 aiva_core-0.1.1/aiva/core/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-03-18 11:37:57.725395 aiva_core-0.1.1/aiva/core/utils/classes/__init__.py
--rw-r--r--   0        0        0     5033 2023-04-03 16:06:31.679079 aiva_core-0.1.1/aiva/core/utils/classes/assistant.py
--rw-r--r--   0        0        0     6124 2023-04-03 16:06:49.230862 aiva_core-0.1.1/aiva/core/utils/classes/chat.py
--rw-r--r--   0        0        0     1301 2023-03-30 15:13:51.662471 aiva_core-0.1.1/aiva/core/utils/classes/chat_instances.py
--rw-r--r--   0        0        0     6437 2023-04-03 16:27:04.447773 aiva_core-0.1.1/aiva/core/utils/classes/chatbot.py
--rw-r--r--   0        0        0     6946 2023-03-28 15:32:51.466758 aiva_core-0.1.1/aiva/core/utils/classes/chatbot_classes.py
--rw-r--r--   0        0        0     4438 2023-04-03 16:52:11.488365 aiva_core-0.1.1/aiva/core/utils/classes/message.py
--rw-r--r--   0        0        0     5738 2023-04-03 16:43:37.452314 aiva_core-0.1.1/aiva/core/utils/classes/message_instances.py
--rw-r--r--   0        0        0     6307 2023-04-03 16:08:13.661857 aiva_core-0.1.1/aiva/core/utils/classes/payload.py
--rw-r--r--   0        0        0     8678 2023-04-04 15:27:29.375830 aiva_core-0.1.1/aiva/core/utils/classes/request.py
--rw-r--r--   0        0        0     7454 2023-04-04 15:15:52.280460 aiva_core-0.1.1/aiva/core/utils/classes/response.py
--rw-r--r--   0        0        0     5699 2023-04-04 14:56:50.247959 aiva_core-0.1.1/aiva/core/utils/classes/transaction.py
--rw-r--r--   0        0        0     1343 2023-03-30 15:14:18.631042 aiva_core-0.1.1/aiva/core/utils/classes/transaction_instances.py
--rw-r--r--   0        0        0        0 2023-04-02 10:05:33.083934 aiva_core-0.1.1/aiva/core/utils/enums/__init__.py
--rw-r--r--   0        0        0     1340 2023-04-02 10:08:51.819591 aiva_core-0.1.1/aiva/core/utils/enums/role.py
--rw-r--r--   0        0        0        0 2023-03-30 15:12:26.840766 aiva_core-0.1.1/aiva/core/utils/mixins/__init__.py
--rw-r--r--   0        0        0     5545 2023-04-03 16:45:32.259434 aiva_core-0.1.1/aiva/core/utils/mixins/instances.py
--rw-r--r--   0        0        0     1050 2023-04-09 14:43:52.533923 aiva_core-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 aiva_core-0.1.1/setup.py
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 aiva_core-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-18 09:34:43.339523 aiva_core-0.1.2/LICENSE
+-rw-r--r--   0        0        0       79 2023-03-18 09:34:43.339523 aiva_core-0.1.2/README.md
+-rw-r--r--   0        0        0      610 2023-03-22 15:18:07.064106 aiva_core-0.1.2/aiva/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-19 08:39:46.743960 aiva_core-0.1.2/aiva/core/assistants/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-19 08:39:16.675922 aiva_core-0.1.2/aiva/core/assistants/classes/__init__.py
+-rw-r--r--   0        0        0     2009 2023-04-04 16:24:17.903807 aiva_core-0.1.2/aiva/core/assistants/classes/aiva.py
+-rw-r--r--   0        0        0        0 2023-03-18 10:44:39.271607 aiva_core-0.1.2/aiva/core/chatbots/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 16:17:19.925412 aiva_core-0.1.2/aiva/core/chatbots/classes/__init__.py
+-rw-r--r--   0        0        0    13334 2023-04-04 15:29:22.675746 aiva_core-0.1.2/aiva/core/chatbots/classes/chat_gpt.py
+-rw-r--r--   0        0        0     2668 2023-04-02 15:18:04.651397 aiva_core-0.1.2/aiva/core/exceptions/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-04 14:18:24.368586 aiva_core-0.1.2/aiva/core/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-18 11:37:48.145434 aiva_core-0.1.2/aiva/core/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-18 11:37:57.725395 aiva_core-0.1.2/aiva/core/utils/classes/__init__.py
+-rw-r--r--   0        0        0     5033 2023-04-03 16:06:31.679079 aiva_core-0.1.2/aiva/core/utils/classes/assistant.py
+-rw-r--r--   0        0        0     6124 2023-04-03 16:06:49.230862 aiva_core-0.1.2/aiva/core/utils/classes/chat.py
+-rw-r--r--   0        0        0     1301 2023-03-30 15:13:51.662471 aiva_core-0.1.2/aiva/core/utils/classes/chat_instances.py
+-rw-r--r--   0        0        0     6437 2023-04-03 16:27:04.447773 aiva_core-0.1.2/aiva/core/utils/classes/chatbot.py
+-rw-r--r--   0        0        0     6946 2023-03-28 15:32:51.466758 aiva_core-0.1.2/aiva/core/utils/classes/chatbot_classes.py
+-rw-r--r--   0        0        0     4438 2023-04-03 16:52:11.488365 aiva_core-0.1.2/aiva/core/utils/classes/message.py
+-rw-r--r--   0        0        0     5738 2023-04-03 16:43:37.452314 aiva_core-0.1.2/aiva/core/utils/classes/message_instances.py
+-rw-r--r--   0        0        0     6307 2023-04-03 16:08:13.661857 aiva_core-0.1.2/aiva/core/utils/classes/payload.py
+-rw-r--r--   0        0        0     8678 2023-04-04 15:27:29.375830 aiva_core-0.1.2/aiva/core/utils/classes/request.py
+-rw-r--r--   0        0        0     7454 2023-04-04 15:15:52.280460 aiva_core-0.1.2/aiva/core/utils/classes/response.py
+-rw-r--r--   0        0        0     5699 2023-04-04 14:56:50.247959 aiva_core-0.1.2/aiva/core/utils/classes/transaction.py
+-rw-r--r--   0        0        0     1343 2023-03-30 15:14:18.631042 aiva_core-0.1.2/aiva/core/utils/classes/transaction_instances.py
+-rw-r--r--   0        0        0        0 2023-04-02 10:05:33.083934 aiva_core-0.1.2/aiva/core/utils/enums/__init__.py
+-rw-r--r--   0        0        0     1340 2023-04-02 10:08:51.819591 aiva_core-0.1.2/aiva/core/utils/enums/role.py
+-rw-r--r--   0        0        0        0 2023-03-30 15:12:26.840766 aiva_core-0.1.2/aiva/core/utils/mixins/__init__.py
+-rw-r--r--   0        0        0     5545 2023-04-03 16:45:32.259434 aiva_core-0.1.2/aiva/core/utils/mixins/instances.py
+-rw-r--r--   0        0        0     1050 2023-04-09 14:54:56.711693 aiva_core-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 aiva_core-0.1.2/setup.py
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 aiva_core-0.1.2/PKG-INFO
```

### Comparing `aiva_core-0.1.1/LICENSE` & `aiva_core-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/__init__.py` & `aiva_core-0.1.2/aiva/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/assistants/classes/aiva.py` & `aiva_core-0.1.2/aiva/core/assistants/classes/aiva.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/chatbots/classes/chat_gpt.py` & `aiva_core-0.1.2/aiva/core/chatbots/classes/chat_gpt.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/exceptions/__init__.py` & `aiva_core-0.1.2/aiva/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/types/__init__.py` & `aiva_core-0.1.2/aiva/core/types/__init__.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/assistant.py` & `aiva_core-0.1.2/aiva/core/utils/classes/assistant.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/chat.py` & `aiva_core-0.1.2/aiva/core/utils/classes/chat.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/chat_instances.py` & `aiva_core-0.1.2/aiva/core/utils/classes/chat_instances.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/chatbot.py` & `aiva_core-0.1.2/aiva/core/utils/classes/chatbot.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/chatbot_classes.py` & `aiva_core-0.1.2/aiva/core/utils/classes/chatbot_classes.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/message.py` & `aiva_core-0.1.2/aiva/core/utils/classes/message.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/message_instances.py` & `aiva_core-0.1.2/aiva/core/utils/classes/message_instances.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/payload.py` & `aiva_core-0.1.2/aiva/core/utils/classes/payload.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/request.py` & `aiva_core-0.1.2/aiva/core/utils/classes/request.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/response.py` & `aiva_core-0.1.2/aiva/core/utils/classes/response.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/transaction.py` & `aiva_core-0.1.2/aiva/core/utils/classes/transaction.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/classes/transaction_instances.py` & `aiva_core-0.1.2/aiva/core/utils/classes/transaction_instances.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/enums/role.py` & `aiva_core-0.1.2/aiva/core/utils/enums/role.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/aiva/core/utils/mixins/instances.py` & `aiva_core-0.1.2/aiva/core/utils/mixins/instances.py`

 * *Files identical despite different names*

### Comparing `aiva_core-0.1.1/pyproject.toml` & `aiva_core-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ┌─────────────────────────────────────────────────────────────────────────────────────
 # │ PROJECT
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 [tool.poetry]
-name = "aiva.core"
-version = "0.1.1"
+name = "aiva-core"
+version = "0.1.2"
 description = "A repository for AIVA, the AI Virtual Assistant written in Python."
 authors = ["Sean O'Leary <seamicole@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aiva"}]
 
 [tool.poetry.dependencies]
```

### Comparing `aiva_core-0.1.1/setup.py` & `aiva_core-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 {'': ['*']}
 
 install_requires = \
 ['openai>=0.27.2,<0.28.0', 'tiktoken>=0.3.2,<0.4.0']
 
 setup_kwargs = {
     'name': 'aiva-core',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A repository for AIVA, the AI Virtual Assistant written in Python.',
     'long_description': '# aiva-core\nA repository for AIVA, the AI Virtual Assistant written in Python.\n',
     'author': "Sean O'Leary",
     'author_email': 'seamicole@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aiva_core-0.1.1/PKG-INFO` & `aiva_core-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiva-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: A repository for AIVA, the AI Virtual Assistant written in Python.
 License: MIT
 Author: Sean O'Leary
 Author-email: seamicole@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

