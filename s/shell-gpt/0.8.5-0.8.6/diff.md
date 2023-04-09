# Comparing `tmp/shell_gpt-0.8.5.tar.gz` & `tmp/shell_gpt-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_gpt-0.8.5.tar", last modified: Fri Apr  7 21:58:59 2023, max compression
+gzip compressed data, was "shell_gpt-0.8.6.tar", last modified: Sun Apr  9 17:11:12 2023, max compression
```

## Comparing `shell_gpt-0.8.5.tar` & `shell_gpt-0.8.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 21:58:59.474375 shell_gpt-0.8.5/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.5/LICENSE
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14754 2023-04-07 21:58:59.474136 shell_gpt-0.8.5/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14406 2023-04-07 21:51:34.000000 shell_gpt-0.8.5/README.md
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-07 21:58:59.474411 shell_gpt-0.8.5/setup.cfg
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      829 2023-04-07 21:51:34.000000 shell_gpt-0.8.5/setup.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 21:58:59.471910 shell_gpt-0.8.5/sgpt/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      445 2023-04-04 16:16:05.000000 shell_gpt-0.8.5/sgpt/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.5/sgpt/__main__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4130 2023-04-07 18:29:19.000000 shell_gpt-0.8.5/sgpt/app.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.5/sgpt/cache.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3134 2023-04-02 15:59:57.000000 shell_gpt-0.8.5/sgpt/client.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2380 2023-04-04 16:16:05.000000 shell_gpt-0.8.5/sgpt/config.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 21:58:59.473046 shell_gpt-0.8.5/sgpt/handlers/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.5/sgpt/handlers/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-04 16:16:05.000000 shell_gpt-0.8.5/sgpt/handlers/chat_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.5/sgpt/handlers/default_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1121 2023-04-06 23:34:58.000000 shell_gpt-0.8.5/sgpt/handlers/handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1839 2023-04-07 18:29:19.000000 shell_gpt-0.8.5/sgpt/handlers/repl_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2092 2023-04-07 18:29:19.000000 shell_gpt-0.8.5/sgpt/make_prompt.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1771 2023-04-07 21:44:34.000000 shell_gpt-0.8.5/sgpt/utils.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 21:58:59.473919 shell_gpt-0.8.5/shell_gpt.egg-info/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14754 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/entry_points.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       97 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/requires.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-09 17:11:12.009149 shell_gpt-0.8.6/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.6/LICENSE
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15147 2023-04-09 17:11:12.008934 shell_gpt-0.8.6/PKG-INFO
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14799 2023-04-09 15:13:49.000000 shell_gpt-0.8.6/README.md
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-09 17:11:12.009186 shell_gpt-0.8.6/setup.cfg
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      829 2023-04-08 20:27:13.000000 shell_gpt-0.8.6/setup.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-09 17:11:12.007262 shell_gpt-0.8.6/sgpt/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      445 2023-04-04 16:16:05.000000 shell_gpt-0.8.6/sgpt/__init__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.6/sgpt/__main__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4398 2023-04-09 17:01:36.000000 shell_gpt-0.8.6/sgpt/app.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.6/sgpt/cache.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3069 2023-04-08 20:21:44.000000 shell_gpt-0.8.6/sgpt/client.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2726 2023-04-09 15:07:44.000000 shell_gpt-0.8.6/sgpt/config.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-09 17:11:12.008001 shell_gpt-0.8.6/sgpt/handlers/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.6/sgpt/handlers/__init__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-04 16:16:05.000000 shell_gpt-0.8.6/sgpt/handlers/chat_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.6/sgpt/handlers/default_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1121 2023-04-06 23:34:58.000000 shell_gpt-0.8.6/sgpt/handlers/handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1839 2023-04-07 18:29:19.000000 shell_gpt-0.8.6/sgpt/handlers/repl_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2092 2023-04-07 18:29:19.000000 shell_gpt-0.8.6/sgpt/make_prompt.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1877 2023-04-07 22:52:58.000000 shell_gpt-0.8.6/sgpt/utils.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-09 17:11:12.008752 shell_gpt-0.8.6/shell_gpt.egg-info/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15147 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       97 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/requires.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-09 17:11:11.000000 shell_gpt-0.8.6/shell_gpt.egg-info/top_level.txt
```

### Comparing `shell_gpt-0.8.5/LICENSE` & `shell_gpt-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.5/PKG-INFO` & `shell_gpt-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: shell_gpt
-Version: 0.8.5
+Version: 0.8.6
 Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
 Home-page: https://github.com/ther1d/shell_gpt
 Author: Farkhod Sadykov
 Author-email: farkhod@sadykov.dev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Shell GPT
-A command-line productivity tool powered by OpenAI's ChatGPT (GPT-3.5). As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
+A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.5
+pip install shell-gpt==0.8.6
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -255,37 +255,41 @@
 CHAT_CACHE_PATH=/tmp/shell_gpt/chat_cache
 # Request cache length (amount).
 CACHE_LENGTH=100
 # Request cache folder.
 CACHE_PATH=/tmp/shell_gpt/cache
 # Request timeout in seconds.
 REQUEST_TIMEOUT=60
+# Default OpenAI model to use.
+DEFAULT_MODEL=gpt-3.5-turbo
 ```
 
 ### Full list of arguments
-```shell
-╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────╮
-│   prompt      [PROMPT]  The prompt to generate completions for.                                         │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --temperature       FLOAT RANGE [0.0<=x<=1.0]  Randomness of generated output. [default: 0.1]           │
-│ --top-probability   FLOAT RANGE [0.1<=x<=1.0]  Limits highest probable tokens (words). [default: 1.0]   │
-│ --editor                                       Open $EDITOR to provide a prompt. [default: no-editor]   │
-│ --cache                                        Cache completion results. [default: cache]               │
-│ --help                                         Show this message and exit.                              │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Chat Options ──────────────────────────────────────────────────────────────────────────────────────────╮
-│ --chat           TEXT  Follow conversation with id (chat mode). [default: None]                         │
-│ --show-chat      TEXT  Show all messages from provided chat id. [default: None]                         │
-│ --list-chat            List all existing chat ids. [default: no-list-chat]                              │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────╮
-│ --shell  -s  Generate and execute shell commands.                                                       │
-│ --code       Generate only code. [default: no-code]                                                     │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```text
+╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   prompt      [PROMPT]  The prompt to generate completions for.                                            │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]      │
+│ --temperature      FLOAT RANGE [0.0<=x<=1.0]        Randomness of generated output. [default: 0.1]         │
+│ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0] │
+│ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor] │
+│ --cache                                             Cache completion results. [default: cache]             │
+│ --help                                              Show this message and exit.                            │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Assistance Options ───────────────────────────────────────────────────────────────────────────────────────╮
+│ --shell  -s                 Generate and execute shell commands.                                           │
+│ --code       --no-code      Generate only code. [default: no-code]                                         │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Chat Options ─────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --chat        TEXT  Follow conversation with id, use "temp" for quick session. [default: None]             │
+│ --repl        TEXT  Start a REPL (Read–eval–print loop) session. [default: None]                           │
+│ --show-chat   TEXT  Show all messages from provided chat id. [default: None]                               │
+│ --list-chat         List all existing chat ids. [default: no-list-chat]                                    │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Docker
 Run the container using the `OPENAI_API_KEY` environment variable, and a docker volume to store cache:
 ```shell
 docker run --rm \
            --env OPENAI_API_KEY="your OPENAI API key" \
```

### Comparing `shell_gpt-0.8.5/README.md` & `shell_gpt-0.8.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Shell GPT
-A command-line productivity tool powered by OpenAI's ChatGPT (GPT-3.5). As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
+A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.5
+pip install shell-gpt==0.8.6
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -245,37 +245,41 @@
 CHAT_CACHE_PATH=/tmp/shell_gpt/chat_cache
 # Request cache length (amount).
 CACHE_LENGTH=100
 # Request cache folder.
 CACHE_PATH=/tmp/shell_gpt/cache
 # Request timeout in seconds.
 REQUEST_TIMEOUT=60
+# Default OpenAI model to use.
+DEFAULT_MODEL=gpt-3.5-turbo
 ```
 
 ### Full list of arguments
-```shell
-╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────╮
-│   prompt      [PROMPT]  The prompt to generate completions for.                                         │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --temperature       FLOAT RANGE [0.0<=x<=1.0]  Randomness of generated output. [default: 0.1]           │
-│ --top-probability   FLOAT RANGE [0.1<=x<=1.0]  Limits highest probable tokens (words). [default: 1.0]   │
-│ --editor                                       Open $EDITOR to provide a prompt. [default: no-editor]   │
-│ --cache                                        Cache completion results. [default: cache]               │
-│ --help                                         Show this message and exit.                              │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Chat Options ──────────────────────────────────────────────────────────────────────────────────────────╮
-│ --chat           TEXT  Follow conversation with id (chat mode). [default: None]                         │
-│ --show-chat      TEXT  Show all messages from provided chat id. [default: None]                         │
-│ --list-chat            List all existing chat ids. [default: no-list-chat]                              │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────╮
-│ --shell  -s  Generate and execute shell commands.                                                       │
-│ --code       Generate only code. [default: no-code]                                                     │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```text
+╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   prompt      [PROMPT]  The prompt to generate completions for.                                            │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]      │
+│ --temperature      FLOAT RANGE [0.0<=x<=1.0]        Randomness of generated output. [default: 0.1]         │
+│ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0] │
+│ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor] │
+│ --cache                                             Cache completion results. [default: cache]             │
+│ --help                                              Show this message and exit.                            │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Assistance Options ───────────────────────────────────────────────────────────────────────────────────────╮
+│ --shell  -s                 Generate and execute shell commands.                                           │
+│ --code       --no-code      Generate only code. [default: no-code]                                         │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Chat Options ─────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --chat        TEXT  Follow conversation with id, use "temp" for quick session. [default: None]             │
+│ --repl        TEXT  Start a REPL (Read–eval–print loop) session. [default: None]                           │
+│ --show-chat   TEXT  Show all messages from provided chat id. [default: None]                               │
+│ --list-chat         List all existing chat ids. [default: no-list-chat]                                    │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Docker
 Run the container using the `OPENAI_API_KEY` environment variable, and a docker volume to store cache:
 ```shell
 docker run --rm \
            --env OPENAI_API_KEY="your OPENAI API key" \
```

### Comparing `shell_gpt-0.8.5/setup.py` & `shell_gpt-0.8.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # pylint: disable=consider-using-with
 setup(
     name="shell_gpt",
-    version="0.8.5",
+    version="0.8.6",
     packages=find_packages(),
     install_requires=[
         "typer~=0.7.0",
         "requests~=2.28.2",
         "rich==13.3.1",
         "distro~=1.8.0",
     ],
```

### Comparing `shell_gpt-0.8.5/sgpt/app.py` & `shell_gpt-0.8.6/sgpt/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,23 +15,27 @@
 import readline  # pylint: disable=unused-import
 
 import typer
 
 # Click is part of typer.
 from click import MissingParameter, BadArgumentUsage
 from sgpt import ChatHandler, DefaultHandler, ReplHandler, OpenAIClient, config
-from sgpt.utils import get_edited_prompt, run_command
+from sgpt.utils import get_edited_prompt, run_command, ModelOptions
 
 
-def main(  # pylint: disable=too-many-arguments
+def main(  # pylint: disable=too-many-arguments,too-many-locals
     prompt: str = typer.Argument(
         None,
         show_default=False,
         help="The prompt to generate completions for.",
     ),
+    model: ModelOptions = typer.Option(
+        ModelOptions(config.get("DEFAULT_MODEL")).value,
+        help="OpenAI GPT model to use.",
+    ),
     temperature: float = typer.Option(
         0.1,
         min=0.0,
         max=1.0,
         help="Randomness of generated output.",
     ),
     top_probability: float = typer.Option(
@@ -99,31 +103,34 @@
     api_key = config.get("OPENAI_API_KEY")
     client = OpenAIClient(api_host, api_key)
 
     if repl:
         # Will be in infinite loop here until user exits with Ctrl+C.
         ReplHandler(client, repl, shell, code).handle(
             prompt,
+            model=model.value,
             temperature=temperature,
             top_probability=top_probability,
             chat_id=repl,
             caching=cache,
         )
 
     if chat:
         full_completion = ChatHandler(client, chat, shell, code).handle(
             prompt,
+            model=model.value,
             temperature=temperature,
             top_probability=top_probability,
             chat_id=chat,
             caching=cache,
         )
     else:
         full_completion = DefaultHandler(client, shell, code).handle(
             prompt,
+            model=model.value,
             temperature=temperature,
             top_probability=top_probability,
             caching=cache,
         )
 
     if shell and typer.confirm("Execute shell command?"):
         run_command(full_completion)
```

### Comparing `shell_gpt-0.8.5/sgpt/cache.py` & `shell_gpt-0.8.6/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.5/sgpt/client.py` & `shell_gpt-0.8.6/sgpt/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 CACHE_LENGTH = int(config.get("CACHE_LENGTH"))
 CACHE_PATH = Path(config.get("CACHE_PATH"))
 REQUEST_TIMEOUT = int(config.get("REQUEST_TIMEOUT"))
 
 
 class OpenAIClient:
     cache = Cache(CACHE_LENGTH, CACHE_PATH)
-    # chat_cache = ChatCache(CHAT_CACHE_LENGTH, CHAT_CACHE_PATH)
 
     def __init__(self, api_host: str, api_key: str) -> None:
         self.api_key = api_key
         self.api_host = api_host
 
     @cache
     def _request(
```

### Comparing `shell_gpt-0.8.5/sgpt/config.py` & `shell_gpt-0.8.6/sgpt/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 import os
 from pathlib import Path
 from getpass import getpass
 from tempfile import gettempdir
 
 from click import UsageError
 
+from sgpt.utils import ModelOptions
+
 CONFIG_FOLDER = os.path.expanduser("~/.config")
 CONFIG_PATH = Path(CONFIG_FOLDER) / "shell_gpt" / ".sgptrc"
 # TODO: Refactor it to CHAT_STORAGE_PATH.
 CHAT_CACHE_PATH = Path(gettempdir()) / "shell_gpt" / "chat_cache"
 CACHE_PATH = Path(gettempdir()) / "shell_gpt" / "cache"
 CHAT_CACHE_LENGTH = 100
 CACHE_LENGTH = 100
 REQUEST_TIMEOUT = 60
-EXPECTED_KEYS = (
-    "OPENAI_API_HOST",
-    "OPENAI_API_KEY",
-    "CHAT_CACHE_LENGTH",
-    "CHAT_CACHE_PATH",
-    "CACHE_LENGTH",
-    "CACHE_PATH",
-    "REQUEST_TIMEOUT",
-)
+DEFAULT_MODEL = ModelOptions.GPT3.value
 config = {}
 
 
 def init() -> None:
     if not CONFIG_PATH.exists():
         CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
         # If user has ENV API key, don't write it to config file.
@@ -39,22 +33,34 @@
         config["CHAT_CACHE_LENGTH"] = os.getenv(
             "CHAT_CACHE_LENGTH", str(CHAT_CACHE_LENGTH)
         )
         config["CHAT_CACHE_PATH"] = os.getenv("CHAT_CACHE_PATH", str(CHAT_CACHE_PATH))
         config["CACHE_LENGTH"] = os.getenv("CACHE_LENGTH", str(CACHE_LENGTH))
         config["CACHE_PATH"] = os.getenv("CACHE_PATH", str(CACHE_PATH))
         config["REQUEST_TIMEOUT"] = os.getenv("REQUEST_TIMEOUT", str(REQUEST_TIMEOUT))
+        config["DEFAULT_MODEL"] = os.getenv("DEFAULT_MODEL", str(DEFAULT_MODEL))
         _write()
 
     with open(CONFIG_PATH, "r", encoding="utf-8") as file:
         for line in file:
             if "=" in line:
                 key, value = line.strip().split("=")
                 config[key] = value
 
+    # TODO: Refactor it this module to Config class.
+    # New features may add new keys to existing config.
+    if "DEFAULT_MODEL" not in config:
+        append("DEFAULT_MODEL", str(DEFAULT_MODEL))
+        init()
+
+
+def append(key: str, value: str) -> None:
+    with open(CONFIG_PATH, encoding="utf-8", mode="a") as file:
+        file.write(f"{key}={value}\n")
+
 
 def get(key: str) -> str:
     # Prioritize ENV variables.
     value = os.getenv(key) or config.get(key)
     assert value, UsageError(f"Config missing: {key}.")
     return value
```

### Comparing `shell_gpt-0.8.5/sgpt/handlers/chat_handler.py` & `shell_gpt-0.8.6/sgpt/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.5/sgpt/handlers/default_handler.py` & `shell_gpt-0.8.6/sgpt/handlers/default_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.5/sgpt/handlers/handler.py` & `shell_gpt-0.8.6/sgpt/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.5/sgpt/handlers/repl_handler.py` & `shell_gpt-0.8.6/sgpt/handlers/repl_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.5/sgpt/make_prompt.py` & `shell_gpt-0.8.6/sgpt/make_prompt.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.5/sgpt/utils.py` & `shell_gpt-0.8.6/sgpt/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 from tempfile import NamedTemporaryFile
 
 import platform
 
 from click import BadParameter
 
 
+class ModelOptions(str, Enum):
+    GPT3 = "gpt-3.5-turbo"
+    GPT4 = "gpt-4"
+    GPT4_32K = "gpt-4-32k"
+
+
 class CompletionModes(Enum):
     NORMAL = "normal"
     SHELL = "shell"
     CODE = "code"
 
     @classmethod
     def get_mode(cls, shell, code) -> "CompletionModes":
```

### Comparing `shell_gpt-0.8.5/shell_gpt.egg-info/PKG-INFO` & `shell_gpt-0.8.6/shell_gpt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: shell-gpt
-Version: 0.8.5
+Version: 0.8.6
 Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
 Home-page: https://github.com/ther1d/shell_gpt
 Author: Farkhod Sadykov
 Author-email: farkhod@sadykov.dev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Shell GPT
-A command-line productivity tool powered by OpenAI's ChatGPT (GPT-3.5). As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
+A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage ChatGPT capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.5
+pip install shell-gpt==0.8.6
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -255,37 +255,41 @@
 CHAT_CACHE_PATH=/tmp/shell_gpt/chat_cache
 # Request cache length (amount).
 CACHE_LENGTH=100
 # Request cache folder.
 CACHE_PATH=/tmp/shell_gpt/cache
 # Request timeout in seconds.
 REQUEST_TIMEOUT=60
+# Default OpenAI model to use.
+DEFAULT_MODEL=gpt-3.5-turbo
 ```
 
 ### Full list of arguments
-```shell
-╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────╮
-│   prompt      [PROMPT]  The prompt to generate completions for.                                         │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --temperature       FLOAT RANGE [0.0<=x<=1.0]  Randomness of generated output. [default: 0.1]           │
-│ --top-probability   FLOAT RANGE [0.1<=x<=1.0]  Limits highest probable tokens (words). [default: 1.0]   │
-│ --editor                                       Open $EDITOR to provide a prompt. [default: no-editor]   │
-│ --cache                                        Cache completion results. [default: cache]               │
-│ --help                                         Show this message and exit.                              │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Chat Options ──────────────────────────────────────────────────────────────────────────────────────────╮
-│ --chat           TEXT  Follow conversation with id (chat mode). [default: None]                         │
-│ --show-chat      TEXT  Show all messages from provided chat id. [default: None]                         │
-│ --list-chat            List all existing chat ids. [default: no-list-chat]                              │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────╮
-│ --shell  -s  Generate and execute shell commands.                                                       │
-│ --code       Generate only code. [default: no-code]                                                     │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```text
+╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   prompt      [PROMPT]  The prompt to generate completions for.                                            │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]      │
+│ --temperature      FLOAT RANGE [0.0<=x<=1.0]        Randomness of generated output. [default: 0.1]         │
+│ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0] │
+│ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor] │
+│ --cache                                             Cache completion results. [default: cache]             │
+│ --help                                              Show this message and exit.                            │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Assistance Options ───────────────────────────────────────────────────────────────────────────────────────╮
+│ --shell  -s                 Generate and execute shell commands.                                           │
+│ --code       --no-code      Generate only code. [default: no-code]                                         │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Chat Options ─────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --chat        TEXT  Follow conversation with id, use "temp" for quick session. [default: None]             │
+│ --repl        TEXT  Start a REPL (Read–eval–print loop) session. [default: None]                           │
+│ --show-chat   TEXT  Show all messages from provided chat id. [default: None]                               │
+│ --list-chat         List all existing chat ids. [default: no-list-chat]                                    │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Docker
 Run the container using the `OPENAI_API_KEY` environment variable, and a docker volume to store cache:
 ```shell
 docker run --rm \
            --env OPENAI_API_KEY="your OPENAI API key" \
```

