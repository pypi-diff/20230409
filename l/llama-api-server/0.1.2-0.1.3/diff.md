# Comparing `tmp/llama_api_server-0.1.2.tar.gz` & `tmp/llama_api_server-0.1.3.tar.gz`

## Comparing `llama_api_server-0.1.2.tar` & `llama_api_server-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/Makefile
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/requirements.txt
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/.github/workflows/release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/llama_api_server/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/llama_api_server/__main__.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/llama_api_server/app.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/llama_api_server/model_pool.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/llama_api_server/utils.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/llama_api_server/models/llama_cpp.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/LICENSE
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 llama_api_server-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.gitattributes
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/Makefile
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/SECURITY.md
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/version.txt
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/__main__.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/app.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/model_pool.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/utils.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/models/llama_cpp.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/README.md
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/PKG-INFO
```

### Comparing `llama_api_server-0.1.2/.github/workflows/release.yml` & `llama_api_server-0.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.1.2/llama_api_server/app.py` & `llama_api_server-0.1.3/llama_api_server/app.py`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.1.2/llama_api_server/models/llama_cpp.py` & `llama_api_server-0.1.3/llama_api_server/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.1.2/.gitignore` & `llama_api_server-0.1.3/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 /models
 *.swp
 /.idea
+.DS_Store
 /config.yml
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `llama_api_server-0.1.2/LICENSE` & `llama_api_server-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.1.2/README.md` & `llama_api_server-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         path: /absolute/path/to/your/7B/ggml-model-q4_0.bin
   embeddings:
     text-embedding-ada-002:
       type: llama_cpp
       params:
         path: /absolute/path/to/your/7B/ggml-model-q4_0.bin
 EOF
-python -m python -m llama_api_server
+
+# start web server
+python -m llama_api_server
 ```
 
 ### Call with openai-python
 ```
 export OPENAI_API_BASE=http://127.0.0.1:5000/v1
 openai api completions.create -e text-davinci-003 -p "hello?"
 ```
@@ -45,27 +47,27 @@
 #### Tested with
 - [X] openai-python
     - [X] OPENAI\_API\_TYPE=default
     - [X] OPENAI\_API\_TYPE=azure
 
 #### Supported APIs
 - [X] Completions
-    - [X] set `temperature`, `top\_p`, and `top\_k`
-    - [X] set `max\_tokens`
+    - [X] set `temperature`, `top_p`, and `top_k`
+    - [X] set `max_tokens`
     - [ ] set `stop`
     - [ ] set `stream`
     - [ ] set `n`
-    - [ ] set `presence\_penalty` and `frequency\_penalty`
-    - [ ] set `logit\_bias`
+    - [ ] set `presence_penalty` and `frequency_penalty`
+    - [ ] set `logit_bias`
 - [X] Embeddings
     - [X] batch process
 - [ ] Chat
 
 #### Supported backed
 - [X] [llama.cpp](https://github.com/ggerganov/llama.cpp) via [llamacpp-python](https://github.com/thomasantony/llamacpp-python)
 
 #### Others
+- [X] Performance parameters like `n_batch` and `n_thread`
 - [ ] Documents
 - [ ] Token auth
 - [ ] Intergration tests
-- [ ] Performance parameters like `n_batch` and `n_thread`
 - [ ] A tool to download/prepare pretrain model
```

### Comparing `llama_api_server-0.1.2/pyproject.toml` & `llama_api_server-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llama_api_server"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = [
     {name = "iaalm", email= "iaalmsimon@gmail.com"}
 ]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.7"
@@ -24,12 +24,13 @@
   "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
   "llamacpp>=0.1.11",
   "Flask>=2.0.0",
   "numpy",
+  "pyyaml",
 ]
 
 [project.urls]
 homepage = "https://github.com/iaalm/llama-api-server"
 repository = "https://github.com/iaalm/llama-api-server"
```

### Comparing `llama_api_server-0.1.2/PKG-INFO` & `llama_api_server-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_api_server
-Version: 0.1.2
+Version: 0.1.3
 Project-URL: homepage, https://github.com/iaalm/llama-api-server
 Project-URL: repository, https://github.com/iaalm/llama-api-server
 Author-email: iaalm <iaalmsimon@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: flask>=2.0.0
 Requires-Dist: llamacpp>=0.1.11
 Requires-Dist: numpy
+Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
 
 llama-api-server
 =======
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Release](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml/badge.svg)](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml)
@@ -49,15 +50,17 @@
         path: /absolute/path/to/your/7B/ggml-model-q4_0.bin
   embeddings:
     text-embedding-ada-002:
       type: llama_cpp
       params:
         path: /absolute/path/to/your/7B/ggml-model-q4_0.bin
 EOF
-python -m python -m llama_api_server
+
+# start web server
+python -m llama_api_server
 ```
 
 ### Call with openai-python
 ```
 export OPENAI_API_BASE=http://127.0.0.1:5000/v1
 openai api completions.create -e text-davinci-003 -p "hello?"
 ```
@@ -67,27 +70,27 @@
 #### Tested with
 - [X] openai-python
     - [X] OPENAI\_API\_TYPE=default
     - [X] OPENAI\_API\_TYPE=azure
 
 #### Supported APIs
 - [X] Completions
-    - [X] set `temperature`, `top\_p`, and `top\_k`
-    - [X] set `max\_tokens`
+    - [X] set `temperature`, `top_p`, and `top_k`
+    - [X] set `max_tokens`
     - [ ] set `stop`
     - [ ] set `stream`
     - [ ] set `n`
-    - [ ] set `presence\_penalty` and `frequency\_penalty`
-    - [ ] set `logit\_bias`
+    - [ ] set `presence_penalty` and `frequency_penalty`
+    - [ ] set `logit_bias`
 - [X] Embeddings
     - [X] batch process
 - [ ] Chat
 
 #### Supported backed
 - [X] [llama.cpp](https://github.com/ggerganov/llama.cpp) via [llamacpp-python](https://github.com/thomasantony/llamacpp-python)
 
 #### Others
+- [X] Performance parameters like `n_batch` and `n_thread`
 - [ ] Documents
 - [ ] Token auth
 - [ ] Intergration tests
-- [ ] Performance parameters like `n_batch` and `n_thread`
 - [ ] A tool to download/prepare pretrain model
```

