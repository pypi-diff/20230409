# Comparing `tmp/chatgpt_prompt_wrapper-0.0.1.tar.gz` & `tmp/chatgpt_prompt_wrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_prompt_wrapper-0.0.1.tar", max compression
+gzip compressed data, was "chatgpt_prompt_wrapper-0.0.2.tar", max compression
```

## Comparing `chatgpt_prompt_wrapper-0.0.1.tar` & `chatgpt_prompt_wrapper-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.1/LICENSE
--rw-r--r--   0        0        0     5202 2023-04-07 17:29:45.977249 chatgpt_prompt_wrapper-0.0.1/README.md
--rw-r--r--   0        0        0     2579 2023-04-08 00:40:12.640234 chatgpt_prompt_wrapper-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/__init__.py
--rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/__version__.py
--rw-r--r--   0        0        0     1882 2023-04-08 00:46:05.038083 chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/arg_parser.py
--rw-r--r--   0        0        0     5497 2023-04-08 00:46:02.245188 chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/chatgpt.py
--rw-r--r--   0        0        0     3043 2023-04-08 00:44:52.769039 chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
--rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
--rw-r--r--   0        0        0     1269 2023-04-08 00:45:02.387291 chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/config.py
--rw-r--r--   0        0        0      418 2023-04-08 00:46:29.766960 chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/init_cmd.py
--rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/log_formatter.py
--rw-r--r--   0        0        0     6454 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.2/LICENSE
+-rw-r--r--   0        0        0     7301 2023-04-09 12:37:14.786391 chatgpt_prompt_wrapper-0.0.2/README.md
+-rw-r--r--   0        0        0     2668 2023-04-09 12:04:28.101563 chatgpt_prompt_wrapper-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/__init__.py
+-rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/__version__.py
+-rw-r--r--   0        0        0     3025 2023-04-09 11:09:59.640753 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/arg_parser.py
+-rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
+-rw-r--r--   0        0        0     2256 2023-04-09 08:44:22.263306 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/ask.py
+-rw-r--r--   0        0        0     6484 2023-04-09 11:33:49.541432 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/chat.py
+-rw-r--r--   0        0        0     7010 2023-04-09 11:15:48.800476 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
+-rw-r--r--   0        0        0     5152 2023-04-09 12:04:28.101672 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
+-rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
+-rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/cmd/__init__.py
+-rw-r--r--   0        0        0      656 2023-04-08 13:10:04.933800 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/cmd/commands.py
+-rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/cmd/cost.py
+-rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/cmd/init.py
+-rw-r--r--   0        0        0     1596 2023-04-09 12:04:28.101755 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/config.py
+-rw-r--r--   0        0        0     1490 2023-04-09 08:44:22.264024 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/docstring.py
+-rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/log_formatter.py
+-rw-r--r--   0        0        0     8655 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.2/PKG-INFO
```

### Comparing `chatgpt_prompt_wrapper-0.0.1/LICENSE` & `chatgpt_prompt_wrapper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.1/pyproject.toml` & `chatgpt_prompt_wrapper-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "chatgpt-prompt-wrapper"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 homepage = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ["chat", "gpt", "openai", "cli"]
 classifiers = ["Development Status :: 3 - Alpha", "Environment :: Console", "Intended Audience :: Developers", "Intended Audience :: End Users/Desktop", "License :: OSI Approved :: Apache Software License", "Natural Language :: English", "Operating System :: OS Independent", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10", "Programming Language :: Python :: 3.11", "Topic :: Communications :: Chat", "Topic :: Utilities"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 tomli = { version = "2.0.1", python = "<3.11"}
 openai = "0.27.4"
 tiktoken = "0.3.3"
+docstring-inheritance = "^1.1.1"
+prompt-toolkit = "^3.0.38"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "7.2.2"
 pytest-cov = "4.0.0"
 pytest-xdist = "3.2.1"
 pytest-benchmark = "4.0.0"
 pyproject-pre-commit = "0.0.5"
@@ -66,11 +68,12 @@
 files = ["src/**/*.py"]
 strict = true
 warn_return_any = false
 ignore_missing_imports = true
 scripts_are_modules = true
 install_types = true
 non_interactive = true
+allow_subclassing_any = true
 
 [tool.poetry.scripts]
 cg = "chatgpt_prompt_wrapper:main"
 chatgpt_prompt_wrapper = "chatgpt_prompt_wrapper:main"
```

### Comparing `chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/arg_parser.py` & `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/arg_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 import os
 import sys
 from argparse import ArgumentParser, Namespace
 
-non_chatgpt_params = ["subcommand", "message", "conf", "key"]
+non_chatgpt_params = [
+    "subcommand",
+    "message",
+    "conf",
+    "show",
+    "hide",
+    "multiline",
+    "no_multiline",
+    "show_cost",
+]
 
 
 def get_arg_parser() -> ArgumentParser:
     arg_parser = ArgumentParser()
     arg_parser.add_argument(
-        "subcommand", help="Subcommand to run.", type=str, nargs=1
+        "subcommand",
+        help="Subcommand to run. Use 'commands' subcommand to list up available subcommands.",
+        type=str,
+        nargs=1,
     )
     arg_parser.add_argument(
         "message", help="Message to send to ChatGPT", type=str, nargs="*"
     )
     arg_parser.add_argument(
         "-k",
         "--key",
@@ -28,38 +40,71 @@
     )
     arg_parser.add_argument(
         "-t",
         "--tokens",
         help="The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model minus prompt tokens.",
         type=int,
     )
+    arg_parser.add_argument(
+        "--show",
+        help="Show prompt for ask command.",
+        action="store_true",
+    )
+    arg_parser.add_argument(
+        "--hide",
+        help="Hide prompt for ask command.",
+        action="store_true",
+    )
+    arg_parser.add_argument(
+        "--multiline",
+        help="Use multiline input for chat command.",
+        action="store_true",
+    )
+    arg_parser.add_argument(
+        "--no_multiline",
+        help="Use single line input for chat command.",
+        action="store_true",
+    )
+    arg_parser.add_argument(
+        "--show_cost",
+        help="Show cost used.",
+        action="store_true",
+    )
     return arg_parser
 
 
 def parse_arg() -> Namespace:
+    arg_parser = get_arg_parser()
+    optional_strings: dict[str, int] = {}
+    for action in arg_parser._actions:
+        for s in action.option_strings:
+            if isinstance(action.nargs, int):
+                optional_strings[s] = action.nargs
+            elif action.nargs is None:
+                optional_strings[s] = 1
+
     positional = []
     option = []
-    is_option = False
+    is_option = 0
     is_positional = False
     for arg in sys.argv[1:]:
         if is_positional:
             positional.append(arg)
         elif is_option:
             option.append(arg)
-            is_option = False
+            is_option -= 1
         elif arg == "--":
             is_positional = True
-        elif arg.startswith("-"):
+        elif arg in optional_strings:
             option.append(arg)
-            is_option = True
+            is_option = optional_strings[arg]
         else:
             positional.append(arg)
     subcommand = [positional[0]] if positional else []
     message = [" ".join(positional[1:])] if len(positional) > 1 else []
-    arg_parser = get_arg_parser()
     args = arg_parser.parse_args(subcommand + message + option)
     return args
 
 
 def cli_help() -> str:
     arg_parser = get_arg_parser()
     return arg_parser.format_help()
```

### Comparing `chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/chatgpt.py` & `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,25 @@
+from __future__ import annotations
+
 import logging
-from dataclasses import dataclass
+import sys
+from dataclasses import dataclass, field
+from typing import Any, Generator
 
 import openai
 import tiktoken
 
-from .chatgpt_prompt_wrapper_exception import ChatGPTPromptWrapperError
+from ..chatgpt_prompt_wrapper_exception import ChatGPTPromptWrapperError
+from ..docstring import NumpyModDocstringInheritanceInitMeta
 
 Messages = list[dict[str, str]]
 
 
-# Ref: https://platform.openai.com/docs/models/overview
-model_max_tokens = {
-    "gpt-4": 8192,
-    "gpt-4-0314": 8192,
-    "gpt-4-32k": 32768,
-    "gpt-4-32k-0314": 32768,
-    "gpt-3.5-turbo": 4096,
-    "gpt-3.5-turbo-0301": 4096,
-}
-
-
-# Ref: https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
-def num_tokens_from_messages(
-    messages: Messages, model: str = "gpt-3.5-turbo"
-) -> int:
-    encoding = tiktoken.encoding_for_model(model)
-    if "gpt-3.5" in model:
-        tokens_per_message = (
-            4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
-        )
-        tokens_per_name = -1  # if there's a name, the role is omitted
-    elif "gpt-4" in model:
-        tokens_per_message = 3
-        tokens_per_name = 1
-    else:
-        raise ChatGPTPromptWrapperError(f"Model: {model} is not supported.")
-    num_tokens = 0
-    for message in messages:
-        num_tokens += tokens_per_message
-        for key, value in message.items():
-            num_tokens += len(encoding.encode(value))
-            if key == "name":
-                num_tokens += tokens_per_name
-    num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
-    return num_tokens
-
-
 @dataclass
-class ChatGPT:
+class ChatGPT(metaclass=NumpyModDocstringInheritanceInitMeta):
     """ChatGPT class for interacting with OpenAI's API.
 
     Parameters
     ----------
     key : str
         OpenAI API key.
     model : str
@@ -62,89 +30,178 @@
         Sampling temperature (0 ~ 2).
     top_p: float
         Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time.
     presence_penalty: float
         The penalty for the model to return the same token (-2 ~ 2).
     frequency_penalty: float
         The penalty for the model to return the same token multiple times (-2 ~ 2).
+    colors: dict[str, str]
+        The colors to use for the different roles.
     """
 
     key: str
     model: str = "gpt-3.5-turbo"
     max_tokens: int = 0
     temperature: float = 1
     top_p: float = 1
     presence_penalty: float = 0
     frequency_penalty: float = 0
+    colors: dict[str, str] = field(
+        default_factory=lambda: {
+            "system": "blue",
+            "user": "green",
+            "assistant": "cyan",
+        }
+    )
 
     def __post_init__(self) -> None:
         self.log = logging.getLogger(__name__)
         openai.api_key = self.key
 
-    def get_max_tokens(self, messages: Messages) -> int:
-        prompt_tokens = num_tokens_from_messages(messages, self.model)
-        if prompt_tokens >= model_max_tokens[self.model]:
+        self.prepare_tokens_checker()
+
+        self.ansi_colors = {
+            "black": "30",
+            "red": "31",
+            "green": "32",
+            "yellow": "33",
+            "blue": "34",
+            "purple": "35",
+            "cyan": "36",
+            "gray": "37",
+        }
+
+        # Ref: https://platform.openai.com/docs/models/overview
+        self.model_max_tokens = {
+            "gpt-4": 8192,
+            "gpt-4-0314": 8192,
+            "gpt-4-32k": 32768,
+            "gpt-4-32k-0314": 32768,
+            "gpt-3.5-turbo": 4096,
+            "gpt-3.5-turbo-0301": 4096,
+        }
+
+        # prices / 1K tokens in USD, (Prompt, Completion)
+        # Ref: https://openai.com/pricing#language-models
+        self.prices = {
+            "gpt-4": (0.03, 0.06),
+            "gpt-4-0314": (0.03, 0.06),
+            "gpt-4-32k": (0.06, 0.12),
+            "gpt-4-32k-0314": (0.06, 0.12),
+            "gpt-3.5-turbo": (0.002, 0.002),
+            "gpt-3.5-turbo-0301": (0.002, 0.002),
+        }
+
+    def set_model(self, model: str) -> None:
+        self.model = self.model
+        self.prepare_tokens_checker()
+
+    def prepare_tokens_checker(self) -> None:
+        self.encoding = tiktoken.encoding_for_model(self.model)
+        if "gpt-3.5" in self.model:
+            # every message follows <|start|>{role/name}\n{content}<|end|>\n
+            self.tokens_per_message = 4
+            # if there's a name, the role is omitted
+            self.tokens_per_name = -1
+        elif "gpt-4" in self.model:
+            self.tokens_per_message = 3
+            self.tokens_per_name = 1
+        else:
+            raise ChatGPTPromptWrapperError(
+                f"Model: {self.model} is not supported."
+            )
+
+        # every reply is primed with <|start|>assistant<|message|>
+        self.reply_tokens = 3
+
+    def add_color(self, text: str, role: str, size: int = 0) -> str:
+        if (
+            sys.stdout.isatty()
+            and role in self.colors
+            and self.colors[role] in self.ansi_colors
+        ):
+            text = f"\033[{self.ansi_colors[self.colors[role]]};1m{text:>{size}}\033[m"
+        return text
+
+    def check_prompt_tokens(self, prompt_tokens: int) -> None:
+        if (
+            prompt_tokens
+            >= self.model_max_tokens[self.model] - self.max_tokens
+        ):
             raise ChatGPTPromptWrapperError(
-                f"Too much tokens: prompt tokens ({prompt_tokens}) >= model's max tokens ({model_max_tokens[self.model]})."
+                f"Too much tokens: prompt tokens ({prompt_tokens}) >= model's max tokens ({self.model_max_tokens[self.model]}) - max_tokens for completion ({self.max_tokens})."
             )
 
+    # Ref: https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
+    def num_tokens_from_message(
+        self, message: dict[str, str], only_content: bool = False
+    ) -> int:
+
+        if only_content:
+            return len(self.encoding.encode(message["content"]))
+
+        num_tokens = self.tokens_per_message
+        for key, value in message.items():
+            num_tokens += len(self.encoding.encode(value))
+            if key == "name":
+                num_tokens += self.tokens_per_name
+        return num_tokens
+
+    def num_total_tokens(self, prompt_tokens: int) -> int:
+        return prompt_tokens + self.reply_tokens
+
+    def num_tokens_from_messages(self, messages: Messages) -> int:
+        num_tokens = 0
+        for message in messages:
+            num_tokens += self.num_tokens_from_message(message)
+        return self.num_total_tokens(num_tokens)
+
+    def get_max_tokens(self, messages: Messages) -> int:
+        prompt_tokens = self.num_tokens_from_messages(messages)
+        self.check_prompt_tokens(prompt_tokens)
+
         if self.max_tokens == 0:
             # it must be maximum tokens for model - 1
-            max_tokens = model_max_tokens[self.model] - prompt_tokens - 1
+            max_tokens = self.model_max_tokens[self.model] - prompt_tokens - 1
         else:
             max_tokens = self.max_tokens
-            if max_tokens + prompt_tokens >= model_max_tokens[self.model]:
-                self.log.warning(
-                    f"Too much tokens: prompt tokens ({prompt_tokens}) + completion tokens (max_tokens) ({max_tokens}) >= model's max tokens ({model_max_tokens[self.model]})."
-                )
-                max_tokens = model_max_tokens[self.model] - prompt_tokens - 1
-                self.log.warning(f"Set max_tokens to {max_tokens}.")
         return max_tokens
 
     def fix_messages(self, messages: Messages) -> Messages:
         if "gpt-3.5" in self.model:
             for message in messages:
                 if message["role"] == "system":
                     message["role"] = "user"
         return messages
 
-    def chat(self, messages: Messages) -> str:
-        """Chat with the model.
-
-        Parameters
-        ----------
-        messages : list[dict[str, str]]
-            The messages to use.
-        """
-        messages = self.fix_messages(messages)
+    def completion(
+        self, messages: Messages, stream: bool = False
+    ) -> Generator[dict[str, Any], None, None] | dict[str, Any]:
         max_tokens = self.get_max_tokens(messages)
 
         response = openai.ChatCompletion.create(
             model=self.model,
             messages=messages,
             max_tokens=max_tokens,
             temperature=self.temperature,
             top_p=self.top_p,
             presence_penalty=self.presence_penalty,
             frequency_penalty=self.frequency_penalty,
+            stream=stream,
         )
+        return response
 
-        finish_reason = response["choices"][0]["finish_reason"]
-        if finish_reason == "stop":
-            pass
-        elif finish_reason == "length":
-            usage = response["usage"]
-            usage["prompt_tokens"], usage["completion_tokens"]
-            self.log.warning(
-                f'Too much tokens: prompt tokens = {response["usage"]["prompt_tokens"]}, completion tokens = {response["usage"]["completion_tokens"]}, while max_tokens = {self.max_tokens}, model\'s max tokens is {model_max_tokens[self.model]}.'
-            )
-        elif finish_reason == "content_filter":
-            self.log.warning(
-                "Omitted content due to a flag from our content filters."
-            )
-        elif finish_reason is None:
-            self.log.warning("API response still in progress or incomplete")
-        else:
-            raise ChatGPTCliError(
-                f"Unknown finish_reason: {response['choices'][0]['finish_reason']}"
-            )
-        return response["choices"][0]["message"]["content"]
+    def get_name(self, message: dict[str, str]) -> str:
+        name = message["role"]
+        if "name" in message:
+            if "gpt-3.5" in self.model:
+                name = message["name"]
+            else:
+                name = f"{message['name']} ({message['role']})"
+        return name
+
+    def get_output(self, message: dict[str, str], size: int = 0) -> str:
+        name = self.add_color(self.get_name(message), message["role"], size)
+        return f"{name}> {message['content']}"
+
+    def run(self, messages: Messages) -> float:
+        return 0
```

### Comparing `chatgpt_prompt_wrapper-0.0.1/src/chatgpt_prompt_wrapper/log_formatter.py` & `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/log_formatter.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.1/PKG-INFO` & `chatgpt_prompt_wrapper-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-prompt-wrapper
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Home-page: https://github.com/rcmdnk/chatgpt-prompt-wrapper
 License: Apache-2.0
 Keywords: chat,gpt,openai,cli
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -20,125 +20,194 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Utilities
+Requires-Dist: docstring-inheritance (>=1.1.1,<2.0.0)
 Requires-Dist: openai (==0.27.4)
+Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: tiktoken (==0.3.3)
 Requires-Dist: tomli (==2.0.1) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/rcmdnk/chatgpt-prompt-wrapper
 Description-Content-Type: text/markdown
 
-# chatgpt-cli
+# chatgpt-prompt-wrapper
 
-[![test](https://github.com/rcmdnk/chatgpt-cli/actions/workflows/test.yml/badge.svg)](https://github.com/rcmdnk/chatgpt-cli/actions/workflows/test.yml)
-[![test coverage](https://img.shields.io/badge/coverage-check%20here-blue.svg)](https://github.com/rcmdnk/chatgpt-cli/tree/coverage)
+[![test](https://github.com/rcmdnk/chatgpt-prompt-wrapper/actions/workflows/test.yml/badge.svg)](https://github.com/rcmdnk/chatgpt-prompt-wrapper/actions/workflows/test.yml)
+[![test coverage](https://img.shields.io/badge/coverage-check%20here-blue.svg)](https://github.com/rcmdnk/chatgpt-prompt-wrapper/tree/coverage)
 
 Python CLI implementation for [ChatGPT](https://openai.com/blog/chatgpt).
 
 ## Requirement
 
 - Python 3.9, 3.10, 3.11
 - Poetry (For development)
 
 ## Installation
 
 ```
-$ pip install chatgpt-cli
+$ pip install chatgpt-prompt-wrapper
 ```
 
 ## Usage
 
 ### Command line interface
 
 ```
-usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t TOKENS] [-r RETURN_TOKENS] subcommand [message ...]
+$ cg help
+usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t TOKENS] [--show] [--hide] [--multiline]
+          [--no_multiline] [--show_cost]
+          subcommand [message ...]
 
 positional arguments:
-  subcommand            Subcommand to run.
+  subcommand            Subcommand to run. Use 'commands' subcommand to list up available subcommands.
   message               Message to send to ChatGPT
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -k KEY, --key KEY     OpenAI API key.
   -c CONF, --conf CONF  Path to the configuration toml file.
   -m MODEL, --model MODEL
                         ChatGPT Model to use.
   -t TOKENS, --tokens TOKENS
-                        The maximum number of tokens to generate in the chat completion. Set 0 to use the
-                        max values for the model.
-  -r RETURN_TOKENS, --return_tokens RETURN_TOKENS
-                        The reserved number of tokens for the return.
+                        The maximum number of tokens to generate in the chat completion. Set 0 to use
+                        the max values for the model minus prompt tokens.
+  --show                Show prompt for ask command.
+  --hide                Hide prompt for ask command.
+  --multiline           Use multiline input for chat command.
+  --no_multiline        Use single line input for chat command.
+  --show_cost           Show cost used.
+
+```
+
+```
+$ cg commands
+Available subcommands:
+  Reserved commands:
+    init      : Initialize config file with an example command.
+    cost      : Show estimated cost used until now.
+    commands  : List up subcommands (show this).
+    version   : Show version.
+    help      : Show help.
+  User commands:
+    test      : Example command to test the OpenAI API.
+    ...
 ```
 
 ### Configuration file
 
 #### File path
 
 The default path to the configuration file is **$XDG_CONFIG_HOME/cg/config.toml**.
 
 If **$XDG_CONFIG_HOME** is not defined, use **~/.config/cg/config.toml**.
 
-If it does not exist and **~/.cg/config.toml** or **~/.cg.toml** exists,
+If it does not exist and **~/.cg/config.toml** exists,
 the existing file is used.
 
 You can change the path by `-c <file>` (`--conf <file>`) option.
 
 #### How to write the configuration file
 
 The configuration file is written in the TOML format.
 
 Subcommand is defined as the top table name.
 
 The options for each table can be:
 
 - `description`: Description of the command.
+- `chat`: Set `true` to make the command chat mode (default is ask mode, only one exchange).
+- `show_cost`: Set `true` to show cost at the end of the command.
 - `model`: The model to use. (default: "gpt-3.5-turbo")
 - `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
 - `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
-- List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content`. You can optionally give `name`.
+- List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
+
+The options for ask mode:
+
+- `show`: Set `true` to show prompt for non chat command.
+- `hide`: Set `true` to hide prompt for non chat command (default).
+
+The options for chat mode:
+
+- `multiline`: Set `true` to hide prompt for non chat command (default).
+- `no_multiline`: Set `true` to hide prompt for non chat command.
+
+Here is a example configuration (if you execute `cg init` at the first time, this configuration file is created).
+
+```toml
+[ask]
+description = "Ask a question w/o predefined prompt."
+
+[test]
+# Example command to test the OpenAI API, taken from below.
+# [Chat completion - OpenAI API](https://platform.openai.com/docs/guides/chat/introduction)
 
-```
-[test_cmd]
 description = "Example command to test the OpenAI API."
+show = true
 
-[[test_cmd.messages]]
+[[test.messages]]
 role = "system"
 content = "You are a helpful assistant."
-[[test_cmd.messages]]
+[[test.messages]]
 role = "user"
 content = "Who won the world series in 2020?"
-[[test_cmd.messages]]
+[[test.messages]]
 role = "assistant"
 "content" = "The Los Angeles Dodgers won the World Series in 2020."
-[[test_cmd.messages]]
+[[test.messages]]
 role = "user"
 content = "Where was it played?"
 
-[shell]
+[sh]
 description = "Ask a shell scripting question."
-[[shell.messages]]
+[[sh.messages]]
 role = "user"
 content = "You are an expert of the shell scripting. Answer the following questions."
 
 [py]
 description = "Ask a python programming question."
 [[py.messages]]
 role = "user"
 content = "You are an expert python programmer. Answer the following questions."
+
+[chat]
+description = "Chat with the assistant."
+chat = true
+[[chat.messages]]
+role = "user"
+content = "Let's enjoy a chat."
 ```
 
 These messages will be sent as an prompt before your input message.
 
-You can give full questions and use `cg` w/o input messages like a first example `test_cmd`.
+You can give full questions and use `cg` w/o input messages like a first example `test` command.
+
+Command examples:
+
+- test
+
+![test command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_test.png)
+
+- sh
+
+![sh command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_sh.png)
+
+- py
+
+![py command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_py.png)
+
+- caht
+
+![chat command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_chat.gif)
 
 ## Development
 
 ### Poetry
 
 Use [Poetry](https://python-poetry.org/) to setup environment.
 
@@ -211,15 +280,15 @@
 
 If you push a repository to GitHub, GitHub Actions will run a test job
 by [GitHub Actions](https://github.co.jp/features/actions).
 
 The job runs at the Pull Request, too.
 
 It checks codes with `pre-commit` and runs tests with `pytest`.
-It also makes a test coverage report and uploads it to [the coverage branch](https://github.com/rcmdnk/chatgpt-cli/tree/coverage).
+It also makes a test coverage report and uploads it to [the coverage branch](https://github.com/rcmdnk/chatgpt-prompt-wrapper/tree/coverage).
 
 You can see the test status as a badge in the README.
 
 ### Renovate
 
 If you want to update dependencies automatically, [install Renovate into your repository](https://docs.renovatebot.com/getting-started/installing-onboarding/).
```

