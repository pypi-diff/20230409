# Comparing `tmp/chatgpt_prompt_wrapper-0.0.2.tar.gz` & `tmp/chatgpt_prompt_wrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_prompt_wrapper-0.0.2.tar", max compression
+gzip compressed data, was "chatgpt_prompt_wrapper-0.0.3.tar", max compression
```

## Comparing `chatgpt_prompt_wrapper-0.0.2.tar` & `chatgpt_prompt_wrapper-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.2/LICENSE
--rw-r--r--   0        0        0     7301 2023-04-09 12:37:14.786391 chatgpt_prompt_wrapper-0.0.2/README.md
--rw-r--r--   0        0        0     2668 2023-04-09 12:04:28.101563 chatgpt_prompt_wrapper-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/__init__.py
--rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/__version__.py
--rw-r--r--   0        0        0     3025 2023-04-09 11:09:59.640753 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/arg_parser.py
--rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
--rw-r--r--   0        0        0     2256 2023-04-09 08:44:22.263306 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/ask.py
--rw-r--r--   0        0        0     6484 2023-04-09 11:33:49.541432 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/chat.py
--rw-r--r--   0        0        0     7010 2023-04-09 11:15:48.800476 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
--rw-r--r--   0        0        0     5152 2023-04-09 12:04:28.101672 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
--rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
--rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/cmd/__init__.py
--rw-r--r--   0        0        0      656 2023-04-08 13:10:04.933800 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/cmd/commands.py
--rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/cmd/cost.py
--rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/cmd/init.py
--rw-r--r--   0        0        0     1596 2023-04-09 12:04:28.101755 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/config.py
--rw-r--r--   0        0        0     1490 2023-04-09 08:44:22.264024 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/docstring.py
--rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/log_formatter.py
--rw-r--r--   0        0        0     8655 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7684 2023-04-09 14:01:07.860253 chatgpt_prompt_wrapper-0.0.3/README.md
+-rw-r--r--   0        0        0     2668 2023-04-09 14:03:50.725531 chatgpt_prompt_wrapper-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/__init__.py
+-rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/__version__.py
+-rw-r--r--   0        0        0     3245 2023-04-09 14:09:52.825789 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/arg_parser.py
+-rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
+-rw-r--r--   0        0        0     2368 2023-04-09 14:43:45.635610 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/ask.py
+-rw-r--r--   0        0        0     6514 2023-04-09 14:44:17.761892 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/chat.py
+-rw-r--r--   0        0        0     7377 2023-04-09 14:44:04.768036 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
+-rw-r--r--   0        0        0     5152 2023-04-09 14:08:23.038547 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
+-rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
+-rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/cmd/__init__.py
+-rw-r--r--   0        0        0      656 2023-04-08 13:10:04.933800 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/cmd/commands.py
+-rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/cmd/cost.py
+-rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/cmd/init.py
+-rw-r--r--   0        0        0     1596 2023-04-09 12:04:28.101755 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/config.py
+-rw-r--r--   0        0        0     1490 2023-04-09 08:44:22.264024 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/docstring.py
+-rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/log_formatter.py
+-rw-r--r--   0        0        0     9038 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.3/PKG-INFO
```

### Comparing `chatgpt_prompt_wrapper-0.0.2/LICENSE` & `chatgpt_prompt_wrapper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.2/README.md` & `chatgpt_prompt_wrapper-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ## Usage
 
 ### Command line interface
 
 ```
 $ cg help
-usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t TOKENS] [--show] [--hide] [--multiline]
+usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t TOKENS] [-l LIMIT] [--show] [--hide] [--multiline]
           [--no_multiline] [--show_cost]
           subcommand [message ...]
 
 positional arguments:
   subcommand            Subcommand to run. Use 'commands' subcommand to list up available subcommands.
   message               Message to send to ChatGPT
 
@@ -35,32 +35,35 @@
   -k KEY, --key KEY     OpenAI API key.
   -c CONF, --conf CONF  Path to the configuration toml file.
   -m MODEL, --model MODEL
                         ChatGPT Model to use.
   -t TOKENS, --tokens TOKENS
                         The maximum number of tokens to generate in the chat completion. Set 0 to use
                         the max values for the model minus prompt tokens.
+  -l LIMIT, --limit LIMIT
+                        The limit of the total tokens of the prompt and the completion. Set 0 to use
+                        the max values for the model.
   --show                Show prompt for ask command.
   --hide                Hide prompt for ask command.
   --multiline           Use multiline input for chat command.
   --no_multiline        Use single line input for chat command.
   --show_cost           Show cost used.
-
 ```
 
 ```
 $ cg commands
 Available subcommands:
   Reserved commands:
     init      : Initialize config file with an example command.
     cost      : Show estimated cost used until now.
     commands  : List up subcommands (show this).
     version   : Show version.
     help      : Show help.
   User commands:
+    ask       : Ask a question w/o predefined prompt.
     test      : Example command to test the OpenAI API.
     ...
 ```
 
 ### Configuration file
 
 #### File path
@@ -83,14 +86,15 @@
 The options for each table can be:
 
 - `description`: Description of the command.
 - `chat`: Set `true` to make the command chat mode (default is ask mode, only one exchange).
 - `show_cost`: Set `true` to show cost at the end of the command.
 - `model`: The model to use. (default: "gpt-3.5-turbo")
 - `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model. (default: 0)
+- `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
 - `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
 - List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
 
 The options for ask mode:
```

### Comparing `chatgpt_prompt_wrapper-0.0.2/pyproject.toml` & `chatgpt_prompt_wrapper-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatgpt-prompt-wrapper"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 homepage = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ["chat", "gpt", "openai", "cli"]
```

### Comparing `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/arg_parser.py` & `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/arg_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,19 +36,25 @@
         "-c", "--conf", help="Path to the configuration toml file.", type=str
     )
     arg_parser.add_argument(
         "-m", "--model", help="ChatGPT Model to use.", type=str
     )
     arg_parser.add_argument(
         "-t",
-        "--tokens",
+        "--max_tokens",
         help="The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model minus prompt tokens.",
         type=int,
     )
     arg_parser.add_argument(
+        "-l",
+        "--tokens_limit",
+        help="The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model.",
+        type=int,
+    )
+    arg_parser.add_argument(
         "--show",
         help="Show prompt for ask command.",
         action="store_true",
     )
     arg_parser.add_argument(
         "--hide",
         help="Hide prompt for ask command.",
```

### Comparing `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/ask.py` & `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/ask.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,20 +31,24 @@
 
         finish_reason = response["choices"][0]["finish_reason"]
         if finish_reason == "stop":
             pass
         elif finish_reason == "length":
             usage = response["usage"]
             usage["prompt_tokens"], usage["completion_tokens"]
+            if self.max_tokens:
+                reason = f"max_tokens for completion = {self.max_tokens}."
+            else:
+                reason = f"max_tokens for completion = {self.get_max_tokens(messages)} (prompt tokens: {usage['prompt_tokens']}, tokens limit: {self.tokens_limit})."
             self.log.warning(
-                f'Too much tokens: prompt tokens = {response["usage"]["prompt_tokens"]}, completion tokens = {response["usage"]["completion_tokens"]}, while max_tokens = {self.max_tokens}, model\'s max tokens is {self.model_max_tokens[self.model]}.'
+                f"The reply was truncated due to the tokens limit: {reason}"
             )
         elif finish_reason == "content_filter":
             self.log.warning(
-                "Omitted content due to a flag from the content filters."
+                "The reply was omitted due to the content filters."
             )
         elif finish_reason is None:
             self.log.warning("API response is incomplete")
         else:
             raise ChatGPTPromptWrapperError(
                 f"Unknown finish_reason: {response['choices'][0]['finish_reason']}"
             )
```

### Comparing `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/chat.py` & `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,18 +107,20 @@
                 )
                 message["role"] = delta["role"]
             if "content" in delta:
                 self.log.info(delta["content"])
                 message["content"] += delta["content"]
             finish_reason = chunk["choices"][0]["finish_reason"]
             if finish_reason == "length":
-                self.log.warning("Too much tokens.\n")
+                self.log.warning(
+                    "The reply was truncated due to the tokens limit.\n"
+                )
             elif finish_reason == "content_filter":
                 self.log.warning(
-                    "Omitted content due to a flag from the content filters.\n"
+                    "The reply was omitted due to the content filters.\n"
                 )
         self.log.info("\n")
         return message
 
     def run(self, messages: Messages) -> float:
         max_tokens_orig = self.max_tokens
         if self.max_tokens == 0:
@@ -148,23 +150,23 @@
                 break
             message = {"role": "user", "content": text}
             if message["content"].lower() in self.chat_exit_cmd:
                 break
             message_tokens = self.num_tokens_from_message(message)
             if (
                 self.num_total_tokens(message_tokens)
-                >= self.model_max_tokens[self.model] - self.max_tokens
+                > self.tokens_limit - self.max_tokens
             ):
                 self.log.warning("Input is too long, try shorter.\n")
                 continue
             messages.append(message)
             tokens.append(message_tokens)
             while (
                 prompt_tokens := self.num_total_tokens(sum(tokens))
-            ) >= self.model_max_tokens[self.model] - self.max_tokens:
+            ) > self.tokens_limit - self.max_tokens:
                 messages = messages[1:]
                 tokens = tokens[1:]
             cost += self.prices[self.model][0] * prompt_tokens / 1000.0
             response = cast(
                 Generator[dict[str, Any], None, None],
                 self.completion(messages, stream=True),
             )
```

### Comparing `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py` & `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     ----------
     key : str
         OpenAI API key.
     model : str
         The model to use.
     max_tokens : int
         The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model minus prompt tokens.
+    tokens_limit : int
+        The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model.
     temperature: float
         Sampling temperature (0 ~ 2).
     top_p: float
         Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time.
     presence_penalty: float
         The penalty for the model to return the same token (-2 ~ 2).
     frequency_penalty: float
@@ -37,14 +39,15 @@
     colors: dict[str, str]
         The colors to use for the different roles.
     """
 
     key: str
     model: str = "gpt-3.5-turbo"
     max_tokens: int = 0
+    tokens_limit: int = 0
     temperature: float = 1
     top_p: float = 1
     presence_penalty: float = 0
     frequency_penalty: float = 0
     colors: dict[str, str] = field(
         default_factory=lambda: {
             "system": "blue",
@@ -86,17 +89,25 @@
             "gpt-4": (0.03, 0.06),
             "gpt-4-0314": (0.03, 0.06),
             "gpt-4-32k": (0.06, 0.12),
             "gpt-4-32k-0314": (0.06, 0.12),
             "gpt-3.5-turbo": (0.002, 0.002),
             "gpt-3.5-turbo-0301": (0.002, 0.002),
         }
+        self.set_model(self.model)
 
     def set_model(self, model: str) -> None:
         self.model = self.model
+        # Total number of tokens must be maximum tokens for model - 1
+        if self.tokens_limit == 0:
+            self.tokens_limit = self.model_max_tokens[self.model] - 1
+        else:
+            self.tokens_limit = min(
+                self.tokens_limit, self.model_max_tokens[self.model] - 1
+            )
         self.prepare_tokens_checker()
 
     def prepare_tokens_checker(self) -> None:
         self.encoding = tiktoken.encoding_for_model(self.model)
         if "gpt-3.5" in self.model:
             # every message follows <|start|>{role/name}\n{content}<|end|>\n
             self.tokens_per_message = 4
@@ -119,20 +130,17 @@
             and role in self.colors
             and self.colors[role] in self.ansi_colors
         ):
             text = f"\033[{self.ansi_colors[self.colors[role]]};1m{text:>{size}}\033[m"
         return text
 
     def check_prompt_tokens(self, prompt_tokens: int) -> None:
-        if (
-            prompt_tokens
-            >= self.model_max_tokens[self.model] - self.max_tokens
-        ):
+        if prompt_tokens + self.max_tokens > self.tokens_limit:
             raise ChatGPTPromptWrapperError(
-                f"Too much tokens: prompt tokens ({prompt_tokens}) >= model's max tokens ({self.model_max_tokens[self.model]}) - max_tokens for completion ({self.max_tokens})."
+                f"Too much tokens: prompt tokens ({prompt_tokens}) + completion tokens (max_tokens) ({self.max_tokens}) > tokens limit ({self.tokens_limit})."
             )
 
     # Ref: https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     def num_tokens_from_message(
         self, message: dict[str, str], only_content: bool = False
     ) -> int:
 
@@ -156,27 +164,39 @@
         return self.num_total_tokens(num_tokens)
 
     def get_max_tokens(self, messages: Messages) -> int:
         prompt_tokens = self.num_tokens_from_messages(messages)
         self.check_prompt_tokens(prompt_tokens)
 
         if self.max_tokens == 0:
-            # it must be maximum tokens for model - 1
-            max_tokens = self.model_max_tokens[self.model] - prompt_tokens - 1
+            max_tokens = self.tokens_limit - prompt_tokens
         else:
             max_tokens = self.max_tokens
         return max_tokens
 
     def fix_messages(self, messages: Messages) -> Messages:
         if "gpt-3.5" in self.model:
             for message in messages:
                 if message["role"] == "system":
                     message["role"] = "user"
         return messages
 
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
     def completion(
         self, messages: Messages, stream: bool = False
     ) -> Generator[dict[str, Any], None, None] | dict[str, Any]:
         max_tokens = self.get_max_tokens(messages)
 
         response = openai.ChatCompletion.create(
             model=self.model,
@@ -186,22 +206,9 @@
             top_p=self.top_p,
             presence_penalty=self.presence_penalty,
             frequency_penalty=self.frequency_penalty,
             stream=stream,
         )
         return response
 
-    def get_name(self, message: dict[str, str]) -> str:
-        name = message["role"]
-        if "name" in message:
-            if "gpt-3.5" in self.model:
-                name = message["name"]
-            else:
-                name = f"{message['name']} ({message['role']})"
-        return name
-
-    def get_output(self, message: dict[str, str], size: int = 0) -> str:
-        name = self.add_color(self.get_name(message), message["role"], size)
-        return f"{name}> {message['content']}"
-
     def run(self, messages: Messages) -> float:
         return 0
```

### Comparing `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py` & `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/cmd/commands.py` & `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/config.py` & `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/config.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/docstring.py` & `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/docstring.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.2/src/chatgpt_prompt_wrapper/log_formatter.py` & `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/log_formatter.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.2/PKG-INFO` & `chatgpt_prompt_wrapper-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-prompt-wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Home-page: https://github.com/rcmdnk/chatgpt-prompt-wrapper
 License: Apache-2.0
 Keywords: chat,gpt,openai,cli
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -52,15 +52,15 @@
 
 ## Usage
 
 ### Command line interface
 
 ```
 $ cg help
-usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t TOKENS] [--show] [--hide] [--multiline]
+usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t TOKENS] [-l LIMIT] [--show] [--hide] [--multiline]
           [--no_multiline] [--show_cost]
           subcommand [message ...]
 
 positional arguments:
   subcommand            Subcommand to run. Use 'commands' subcommand to list up available subcommands.
   message               Message to send to ChatGPT
 
@@ -69,32 +69,35 @@
   -k KEY, --key KEY     OpenAI API key.
   -c CONF, --conf CONF  Path to the configuration toml file.
   -m MODEL, --model MODEL
                         ChatGPT Model to use.
   -t TOKENS, --tokens TOKENS
                         The maximum number of tokens to generate in the chat completion. Set 0 to use
                         the max values for the model minus prompt tokens.
+  -l LIMIT, --limit LIMIT
+                        The limit of the total tokens of the prompt and the completion. Set 0 to use
+                        the max values for the model.
   --show                Show prompt for ask command.
   --hide                Hide prompt for ask command.
   --multiline           Use multiline input for chat command.
   --no_multiline        Use single line input for chat command.
   --show_cost           Show cost used.
-
 ```
 
 ```
 $ cg commands
 Available subcommands:
   Reserved commands:
     init      : Initialize config file with an example command.
     cost      : Show estimated cost used until now.
     commands  : List up subcommands (show this).
     version   : Show version.
     help      : Show help.
   User commands:
+    ask       : Ask a question w/o predefined prompt.
     test      : Example command to test the OpenAI API.
     ...
 ```
 
 ### Configuration file
 
 #### File path
@@ -117,14 +120,15 @@
 The options for each table can be:
 
 - `description`: Description of the command.
 - `chat`: Set `true` to make the command chat mode (default is ask mode, only one exchange).
 - `show_cost`: Set `true` to show cost at the end of the command.
 - `model`: The model to use. (default: "gpt-3.5-turbo")
 - `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model. (default: 0)
+- `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
 - `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
 - List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
 
 The options for ask mode:
```

