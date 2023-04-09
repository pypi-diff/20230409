# Comparing `tmp/langchain_utils-0.1.1.tar.gz` & `tmp/langchain_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.1.1.tar", max compression
+gzip compressed data, was "langchain_utils-0.1.2.tar", max compression
```

## Comparing `langchain_utils-0.1.1.tar` & `langchain_utils-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-04-09 06:06:32.834472 langchain_utils-0.1.1/langchain_utils/__init__.py
--rwxr-xr-x   0        0        0     1285 2023-04-09 04:56:49.564631 langchain_utils-0.1.1/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0      132 2023-04-09 04:53:43.422829 langchain_utils-0.1.1/langchain_utils/prompts.py
--rw-r--r--   0        0        0     1054 2023-04-09 06:06:32.833953 langchain_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 langchain_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-04-09 14:42:52.744027 langchain_utils-0.1.2/langchain_utils/__init__.py
+-rwxr-xr-x   0        0        0     4023 2023-04-09 14:42:02.576415 langchain_utils-0.1.2/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0      449 2023-04-09 14:08:17.975001 langchain_utils-0.1.2/langchain_utils/prompts.py
+-rw-r--r--   0        0        0      534 2023-04-09 14:36:32.955521 langchain_utils-0.1.2/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1119 2023-04-09 14:42:52.743161 langchain_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 langchain_utils-0.1.2/PKG-INFO
```

### Comparing `langchain_utils-0.1.1/pyproject.toml` & `langchain_utils-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
@@ -19,19 +19,22 @@
 "Bug Tracker" = "https://github.com/tddschn/langchain-utils/issues"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 langchain = "^0.0.135"
 youtube-transcript-api = "^0.5.0"
 pytube = "^12.1.3"
+pyperclip = "^1.8.2"
+tiktoken = "^0.3.3"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 better-exceptions = "^0.3.3"
 ipython = "^8.12.0"
 ipykernel = "^6.22.0"
 rich = "^13.3.3"
+pyinstrument = "^4.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `langchain_utils-0.1.1/PKG-INFO` & `langchain_utils-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: langchain (>=0.0.135,<0.0.136)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pytube (>=12.1.3,<13.0.0)
+Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: youtube-transcript-api (>=0.5.0,<0.6.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/langchain-utils/issues
 Project-URL: Repository, https://github.com/tddschn/langchain-utils
 Description-Content-Type: text/markdown
```

