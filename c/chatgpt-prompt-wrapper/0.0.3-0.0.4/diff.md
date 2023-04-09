# Comparing `tmp/chatgpt_prompt_wrapper-0.0.3.tar.gz` & `tmp/chatgpt_prompt_wrapper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_prompt_wrapper-0.0.3.tar", max compression
+gzip compressed data, was "chatgpt_prompt_wrapper-0.0.4.tar", max compression
```

## Comparing `chatgpt_prompt_wrapper-0.0.3.tar` & `chatgpt_prompt_wrapper-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,35 @@
--rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.3/LICENSE
--rw-r--r--   0        0        0     7684 2023-04-09 14:01:07.860253 chatgpt_prompt_wrapper-0.0.3/README.md
--rw-r--r--   0        0        0     2668 2023-04-09 14:03:50.725531 chatgpt_prompt_wrapper-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/__init__.py
--rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/__version__.py
--rw-r--r--   0        0        0     3245 2023-04-09 14:09:52.825789 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/arg_parser.py
--rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
--rw-r--r--   0        0        0     2368 2023-04-09 14:43:45.635610 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/ask.py
--rw-r--r--   0        0        0     6514 2023-04-09 14:44:17.761892 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/chat.py
--rw-r--r--   0        0        0     7377 2023-04-09 14:44:04.768036 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
--rw-r--r--   0        0        0     5152 2023-04-09 14:08:23.038547 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
--rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
--rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/cmd/__init__.py
--rw-r--r--   0        0        0      656 2023-04-08 13:10:04.933800 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/cmd/commands.py
--rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/cmd/cost.py
--rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/cmd/init.py
--rw-r--r--   0        0        0     1596 2023-04-09 12:04:28.101755 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/config.py
--rw-r--r--   0        0        0     1490 2023-04-09 08:44:22.264024 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/docstring.py
--rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/log_formatter.py
--rw-r--r--   0        0        0     9038 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.4/LICENSE
+-rw-r--r--   0        0        0     8020 2023-04-09 15:52:54.237309 chatgpt_prompt_wrapper-0.0.4/README.md
+-rw-r--r--   0        0        0     2668 2023-04-09 15:53:09.174448 chatgpt_prompt_wrapper-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/__init__.py
+-rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/__version__.py
+-rw-r--r--   0        0        0     3422 2023-04-09 15:40:50.061149 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/arg_parser.py
+-rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
+-rw-r--r--   0        0        0      426 2023-04-09 15:40:56.568943 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      349 2023-04-09 10:56:55.641263 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4076 2023-04-09 15:40:56.570213 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/ask.cpython-311.pyc
+-rw-r--r--   0        0        0     2228 2023-04-09 15:36:48.300461 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/ask.cpython-39.pyc
+-rw-r--r--   0        0        0     5976 2023-04-09 15:44:36.384736 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/chat.cpython-39.pyc
+-rw-r--r--   0        0        0     9910 2023-04-09 15:40:56.572114 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/chatgpt.cpython-311.pyc
+-rw-r--r--   0        0        0     6628 2023-04-09 15:44:36.278719 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/__pycache__/chatgpt.cpython-39.pyc
+-rw-r--r--   0        0        0     2414 2023-04-09 15:31:06.479272 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/ask.py
+-rw-r--r--   0        0        0     6370 2023-04-09 15:44:22.102233 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/chat.py
+-rw-r--r--   0        0        0     7504 2023-04-09 15:43:30.852390 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
+-rw-r--r--   0        0        0     5324 2023-04-09 15:56:41.373142 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
+-rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
+-rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__init__.py
+-rw-r--r--   0        0        0      374 2023-04-08 12:08:10.316082 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      303 2023-04-09 08:16:02.965964 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1644 2023-04-08 12:08:30.203863 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/commands.cpython-311.pyc
+-rw-r--r--   0        0        0     1058 2023-04-09 15:44:36.414978 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/commands.cpython-39.pyc
+-rw-r--r--   0        0        0     1217 2023-04-08 12:08:30.204184 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/cost.cpython-311.pyc
+-rw-r--r--   0        0        0      642 2023-04-09 08:16:02.966921 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/cost.cpython-39.pyc
+-rw-r--r--   0        0        0     1199 2023-04-08 12:08:30.202279 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/init.cpython-311.pyc
+-rw-r--r--   0        0        0      688 2023-04-08 12:10:44.880831 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/__pycache__/init.cpython-39.pyc
+-rw-r--r--   0        0        0      854 2023-04-09 15:44:22.008830 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/commands.py
+-rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/cost.py
+-rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/init.py
+-rw-r--r--   0        0        0     1410 2023-04-09 15:52:54.238316 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/config.py
+-rw-r--r--   0        0        0     1490 2023-04-09 08:44:22.264024 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/docstring.py
+-rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/log_formatter.py
+-rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.4/PKG-INFO
```

### Comparing `chatgpt_prompt_wrapper-0.0.3/LICENSE` & `chatgpt_prompt_wrapper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.3/README.md` & `chatgpt_prompt_wrapper-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,52 +18,55 @@
 
 ## Usage
 
 ### Command line interface
 
 ```
 $ cg help
-usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t TOKENS] [-l LIMIT] [--show] [--hide] [--multiline]
-          [--no_multiline] [--show_cost]
+usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t MAX_TOKENS] [-T MIN_MAX_TOKENS] [-l TOKENS_LIMIT]
+          [--show] [--hide] [--multiline] [--no_multiline] [--show_cost]
           subcommand [message ...]
 
 positional arguments:
   subcommand            Subcommand to run. Use 'commands' subcommand to list up available subcommands.
   message               Message to send to ChatGPT
 
 optional arguments:
   -h, --help            show this help message and exit
   -k KEY, --key KEY     OpenAI API key.
   -c CONF, --conf CONF  Path to the configuration toml file.
   -m MODEL, --model MODEL
                         ChatGPT Model to use.
-  -t TOKENS, --tokens TOKENS
+  -t MAX_TOKENS, --max_tokens MAX_TOKENS
                         The maximum number of tokens to generate in the chat completion. Set 0 to use
                         the max values for the model minus prompt tokens.
-  -l LIMIT, --limit LIMIT
+  -T MIN_MAX_TOKENS, --min_max_tokens MIN_MAX_TOKENS
+                        The minimum of max_tokens for the completion when max_tokens = 0.
+  -l TOKENS_LIMIT, --tokens_limit TOKENS_LIMIT
                         The limit of the total tokens of the prompt and the completion. Set 0 to use
                         the max values for the model.
   --show                Show prompt for ask command.
   --hide                Hide prompt for ask command.
   --multiline           Use multiline input for chat command.
   --no_multiline        Use single line input for chat command.
   --show_cost           Show cost used.
 ```
 
 ```
 $ cg commands
 Available subcommands:
   Reserved commands:
+    ask       : Ask w/o predefined prompt.
+    chat      : Start chat w/o predefined prompt.
     init      : Initialize config file with an example command.
     cost      : Show estimated cost used until now.
     commands  : List up subcommands (show this).
     version   : Show version.
     help      : Show help.
   User commands:
-    ask       : Ask a question w/o predefined prompt.
     test      : Example command to test the OpenAI API.
     ...
 ```
 
 ### Configuration file
 
 #### File path
@@ -86,14 +89,15 @@
 The options for each table can be:
 
 - `description`: Description of the command.
 - `chat`: Set `true` to make the command chat mode (default is ask mode, only one exchange).
 - `show_cost`: Set `true` to show cost at the end of the command.
 - `model`: The model to use. (default: "gpt-3.5-turbo")
 - `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model. (default: 0)
+- `min_max_tokens`: The minimum of max_tokens for the completion when max_tokens = 0. (default: 200)
 - `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
 - `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
 - List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
 
@@ -103,19 +107,21 @@
 - `hide`: Set `true` to hide prompt for non chat command (default).
 
 The options for chat mode:
 
 - `multiline`: Set `true` to hide prompt for non chat command (default).
 - `no_multiline`: Set `true` to hide prompt for non chat command.
 
-Here is a example configuration (if you execute `cg init` at the first time, this configuration file is created).
+Here is a example configuration:
 
 ```toml
-[ask]
-description = "Ask a question w/o predefined prompt."
+[global]
+# Global configuration
+# `global` is special name and not a subcommand
+model = 'gpt-3.5-turbo'
 
 [test]
 # Example command to test the OpenAI API, taken from below.
 # [Chat completion - OpenAI API](https://platform.openai.com/docs/guides/chat/introduction)
 
 description = "Example command to test the OpenAI API."
 show = true
@@ -141,16 +147,16 @@
 
 [py]
 description = "Ask a python programming question."
 [[py.messages]]
 role = "user"
 content = "You are an expert python programmer. Answer the following questions."
 
-[chat]
-description = "Chat with the assistant."
+[enjoy_chat]
+description = "Chat example with a predefined prompt."
 chat = true
 [[chat.messages]]
 role = "user"
 content = "Let's enjoy a chat."
 ```
 
 These messages will be sent as an prompt before your input message.
@@ -167,15 +173,15 @@
 
 ![sh command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_sh.png)
 
 - py
 
 ![py command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_py.png)
 
-- caht
+- enjoy_chat
 
 ![chat command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_chat.gif)
 
 ## Development
 
 ### Poetry
```

### Comparing `chatgpt_prompt_wrapper-0.0.3/pyproject.toml` & `chatgpt_prompt_wrapper-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatgpt-prompt-wrapper"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 homepage = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ["chat", "gpt", "openai", "cli"]
```

### Comparing `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/arg_parser.py` & `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/arg_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,20 @@
     arg_parser.add_argument(
         "-t",
         "--max_tokens",
         help="The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model minus prompt tokens.",
         type=int,
     )
     arg_parser.add_argument(
+        "-T",
+        "--min_max_tokens",
+        help="The minimum of max_tokens for the completion when max_tokens = 0.",
+        type=int,
+    )
+    arg_parser.add_argument(
         "-l",
         "--tokens_limit",
         help="The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model.",
         type=int,
     )
     arg_parser.add_argument(
         "--show",
```

### Comparing `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/ask.py` & `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/ask.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             pass
         elif finish_reason == "length":
             usage = response["usage"]
             usage["prompt_tokens"], usage["completion_tokens"]
             if self.max_tokens:
                 reason = f"max_tokens for completion = {self.max_tokens}."
             else:
-                reason = f"max_tokens for completion = {self.get_max_tokens(messages)} (prompt tokens: {usage['prompt_tokens']}, tokens limit: {self.tokens_limit})."
+                reason = f"max_tokens for completion = {self.get_max_tokens(messages)} (prompt tokens: {usage['prompt_tokens']}, tokens limit: {self.tokens_limit}, minimum of max tokens: {self.min_max_tokens})."
             self.log.warning(
                 f"The reply was truncated due to the tokens limit: {reason}"
             )
         elif finish_reason == "content_filter":
             self.log.warning(
                 "The reply was omitted due to the content filters."
             )
```

### Comparing `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/chat.py` & `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,28 +118,25 @@
                 self.log.warning(
                     "The reply was omitted due to the content filters.\n"
                 )
         self.log.info("\n")
         return message
 
     def run(self, messages: Messages) -> float:
-        max_tokens_orig = self.max_tokens
-        if self.max_tokens == 0:
-            # Set minimum max_tokens for chat
-            self.max_tokens = 100
-
         messages = self.fix_messages(messages)
         tokens = [
             self.num_tokens_from_message(message) for message in messages
         ]
         prompt_tokens = self.num_total_tokens(sum(tokens))
         self.check_prompt_tokens(prompt_tokens)
 
-        max_size = max(
-            10, max(len(self.get_name(message)) for message in messages)
+        max_size = (
+            max(10, max(len(self.get_name(message)) for message in messages))
+            if messages
+            else 10
         )
         for message in messages:
             self.log.info(self.get_output(message, max_size))
 
         self.set_no_line_break_log()
         cost = 0.0
         self.finish_chat = False
@@ -150,23 +147,23 @@
                 break
             message = {"role": "user", "content": text}
             if message["content"].lower() in self.chat_exit_cmd:
                 break
             message_tokens = self.num_tokens_from_message(message)
             if (
                 self.num_total_tokens(message_tokens)
-                > self.tokens_limit - self.max_tokens
+                > self.tokens_limit - self.min_max_tokens
             ):
                 self.log.warning("Input is too long, try shorter.\n")
                 continue
             messages.append(message)
             tokens.append(message_tokens)
             while (
                 prompt_tokens := self.num_total_tokens(sum(tokens))
-            ) > self.tokens_limit - self.max_tokens:
+            ) > self.tokens_limit - self.min_max_tokens:
                 messages = messages[1:]
                 tokens = tokens[1:]
             cost += self.prices[self.model][0] * prompt_tokens / 1000.0
             response = cast(
                 Generator[dict[str, Any], None, None],
                 self.completion(messages, stream=True),
             )
@@ -179,9 +176,8 @@
             )
 
         message = {"role": "assistant", "content": "Bye!"}
         self.log.info(self.get_output(message, max_size))
         self.log.info("\n")
 
         self.reset_no_line_break_log()
-        self.max_tokens = max_tokens_orig
         return cost
```

### Comparing `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py` & `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     ----------
     key : str
         OpenAI API key.
     model : str
         The model to use.
     max_tokens : int
         The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model minus prompt tokens.
+    min_max_tokens: int
+        The minimum of max_tokens for the completion when max_tokens = 0.
     tokens_limit : int
         The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model.
     temperature: float
         Sampling temperature (0 ~ 2).
     top_p: float
         Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time.
     presence_penalty: float
@@ -39,14 +41,15 @@
     colors: dict[str, str]
         The colors to use for the different roles.
     """
 
     key: str
     model: str = "gpt-3.5-turbo"
     max_tokens: int = 0
+    min_max_tokens: int = 200
     tokens_limit: int = 0
     temperature: float = 1
     top_p: float = 1
     presence_penalty: float = 0
     frequency_penalty: float = 0
     colors: dict[str, str] = field(
         default_factory=lambda: {
@@ -55,16 +58,16 @@
             "assistant": "cyan",
         }
     )
 
     def __post_init__(self) -> None:
         self.log = logging.getLogger(__name__)
         openai.api_key = self.key
-
-        self.prepare_tokens_checker()
+        if self.max_tokens:
+            self.min_max_tokens = self.max_tokens
 
         self.ansi_colors = {
             "black": "30",
             "red": "31",
             "green": "32",
             "yellow": "33",
             "blue": "34",
@@ -130,17 +133,17 @@
             and role in self.colors
             and self.colors[role] in self.ansi_colors
         ):
             text = f"\033[{self.ansi_colors[self.colors[role]]};1m{text:>{size}}\033[m"
         return text
 
     def check_prompt_tokens(self, prompt_tokens: int) -> None:
-        if prompt_tokens + self.max_tokens > self.tokens_limit:
+        if prompt_tokens + self.min_max_tokens > self.tokens_limit:
             raise ChatGPTPromptWrapperError(
-                f"Too much tokens: prompt tokens ({prompt_tokens}) + completion tokens (max_tokens) ({self.max_tokens}) > tokens limit ({self.tokens_limit})."
+                f"Too much tokens: prompt tokens ({prompt_tokens}) + completion tokens ({self.min_max_tokens}) > tokens limit ({self.tokens_limit})."
             )
 
     # Ref: https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     def num_tokens_from_message(
         self, message: dict[str, str], only_content: bool = False
     ) -> int:
 
@@ -163,19 +166,17 @@
             num_tokens += self.num_tokens_from_message(message)
         return self.num_total_tokens(num_tokens)
 
     def get_max_tokens(self, messages: Messages) -> int:
         prompt_tokens = self.num_tokens_from_messages(messages)
         self.check_prompt_tokens(prompt_tokens)
 
-        if self.max_tokens == 0:
-            max_tokens = self.tokens_limit - prompt_tokens
-        else:
-            max_tokens = self.max_tokens
-        return max_tokens
+        if self.max_tokens:
+            return self.max_tokens
+        return max(self.min_max_tokens, self.tokens_limit - prompt_tokens)
 
     def fix_messages(self, messages: Messages) -> Messages:
         if "gpt-3.5" in self.model:
             for message in messages:
                 if message["role"] == "system":
                     message["role"] = "user"
         return messages
```

### Comparing `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py` & `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,18 +161,23 @@
     with open(config_file, "rb") as f:
         config = tomllib.load(f)
 
     if cmd == "commands":
         commands(config, log)
         return
 
-    if cmd not in config:
+    cmds = ["ask", "chat"] + list(config)
+    if cmd not in cmds or cmd == "global":
         raise ChatGPTPromptWrapperError(f"Subcommand: {cmd} is not defined.")
 
-    cmd_config = config[cmd]
+    cmd_config = config.get("global", {})
+    cmd_config.update(config.get(cmd, {}))
+    if cmd == "chat":
+        cmd_config["chat"] = True
+
     chatgpt_params, messages, chat, show_cost = check_args(cmd_config, args)
 
     cost_data_this = run_chatgpt(messages, chatgpt_params, chat)
 
     update_cost(cost_file, cost_data_this, show_cost)
```

### Comparing `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/cmd/commands.py` & `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/cmd/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import logging
 from typing import Any
 
 
 def commands(config: dict[str, Any], log: logging.Logger) -> None:
     log.info("Available subcommands:")
     log.info("  Reserved commands:")
+    log.info(f"    {'ask':<10s}: Ask w/o predefined prompt.")
+    log.info(f"    {'chat':<10s}: Start chat w/o predefined prompt.")
     log.info(
         f"    {'init':<10s}: Initialize config file with an example command."
     )
     log.info(f"    {'cost':<10s}: Show estimated cost used until now.")
     log.info(f"    {'commands':<10s}: List up subcommands (show this).")
     log.info(f"    {'version':<10s}: Show version.")
     log.info(f"    {'help':<10s}: Show help.")
     log.info("  User commands:")
     for cmd in config:
+        if cmd in ["global", "ask", "chat"]:
+            continue
         log.info(f"    {cmd:<10s}: {config[cmd].get('description', '')}")
```

### Comparing `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/config.py` & `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,15 @@
     elif Path(f"~/.{dir_name}").expanduser().is_dir():
         return Path(f"~/.{dir_name}").expanduser() / file_name
     else:
         return xdg_config_home / dir_name / file_name
 
 
 def example_config() -> str:
-    return """[ask]
-description = "Ask a question w/o predefined prompt."
-
-[test]
+    return """[test]
 # Example command to test the OpenAI API, taken from below.
 # [Chat completion - OpenAI API](https://platform.openai.com/docs/guides/chat/introduction)
 
 description = "Example command to test the OpenAI API."
 show = true
 
 [[test.messages]]
@@ -45,15 +42,8 @@
 content = "You are an expert of the shell scripting. Answer the following questions."
 
 [py]
 description = "Ask a python programming question."
 [[py.messages]]
 role = "user"
 content = "You are an expert python programmer. Answer the following questions."
-
-[chat]
-description = "Chat with the assistant."
-chat = true
-[[chat.messages]]
-role = "user"
-content = "Let's enjoy a chat."
 """
```

### Comparing `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/docstring.py` & `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/docstring.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.3/src/chatgpt_prompt_wrapper/log_formatter.py` & `chatgpt_prompt_wrapper-0.0.4/src/chatgpt_prompt_wrapper/log_formatter.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.3/PKG-INFO` & `chatgpt_prompt_wrapper-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-prompt-wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Home-page: https://github.com/rcmdnk/chatgpt-prompt-wrapper
 License: Apache-2.0
 Keywords: chat,gpt,openai,cli
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -52,52 +52,55 @@
 
 ## Usage
 
 ### Command line interface
 
 ```
 $ cg help
-usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t TOKENS] [-l LIMIT] [--show] [--hide] [--multiline]
-          [--no_multiline] [--show_cost]
+usage: cg [-h] [-k KEY] [-c CONF] [-m MODEL] [-t MAX_TOKENS] [-T MIN_MAX_TOKENS] [-l TOKENS_LIMIT]
+          [--show] [--hide] [--multiline] [--no_multiline] [--show_cost]
           subcommand [message ...]
 
 positional arguments:
   subcommand            Subcommand to run. Use 'commands' subcommand to list up available subcommands.
   message               Message to send to ChatGPT
 
 optional arguments:
   -h, --help            show this help message and exit
   -k KEY, --key KEY     OpenAI API key.
   -c CONF, --conf CONF  Path to the configuration toml file.
   -m MODEL, --model MODEL
                         ChatGPT Model to use.
-  -t TOKENS, --tokens TOKENS
+  -t MAX_TOKENS, --max_tokens MAX_TOKENS
                         The maximum number of tokens to generate in the chat completion. Set 0 to use
                         the max values for the model minus prompt tokens.
-  -l LIMIT, --limit LIMIT
+  -T MIN_MAX_TOKENS, --min_max_tokens MIN_MAX_TOKENS
+                        The minimum of max_tokens for the completion when max_tokens = 0.
+  -l TOKENS_LIMIT, --tokens_limit TOKENS_LIMIT
                         The limit of the total tokens of the prompt and the completion. Set 0 to use
                         the max values for the model.
   --show                Show prompt for ask command.
   --hide                Hide prompt for ask command.
   --multiline           Use multiline input for chat command.
   --no_multiline        Use single line input for chat command.
   --show_cost           Show cost used.
 ```
 
 ```
 $ cg commands
 Available subcommands:
   Reserved commands:
+    ask       : Ask w/o predefined prompt.
+    chat      : Start chat w/o predefined prompt.
     init      : Initialize config file with an example command.
     cost      : Show estimated cost used until now.
     commands  : List up subcommands (show this).
     version   : Show version.
     help      : Show help.
   User commands:
-    ask       : Ask a question w/o predefined prompt.
     test      : Example command to test the OpenAI API.
     ...
 ```
 
 ### Configuration file
 
 #### File path
@@ -120,14 +123,15 @@
 The options for each table can be:
 
 - `description`: Description of the command.
 - `chat`: Set `true` to make the command chat mode (default is ask mode, only one exchange).
 - `show_cost`: Set `true` to show cost at the end of the command.
 - `model`: The model to use. (default: "gpt-3.5-turbo")
 - `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the max values for the model. (default: 0)
+- `min_max_tokens`: The minimum of max_tokens for the completion when max_tokens = 0. (default: 200)
 - `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the max values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
 - `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
 - List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
 
@@ -137,19 +141,21 @@
 - `hide`: Set `true` to hide prompt for non chat command (default).
 
 The options for chat mode:
 
 - `multiline`: Set `true` to hide prompt for non chat command (default).
 - `no_multiline`: Set `true` to hide prompt for non chat command.
 
-Here is a example configuration (if you execute `cg init` at the first time, this configuration file is created).
+Here is a example configuration:
 
 ```toml
-[ask]
-description = "Ask a question w/o predefined prompt."
+[global]
+# Global configuration
+# `global` is special name and not a subcommand
+model = 'gpt-3.5-turbo'
 
 [test]
 # Example command to test the OpenAI API, taken from below.
 # [Chat completion - OpenAI API](https://platform.openai.com/docs/guides/chat/introduction)
 
 description = "Example command to test the OpenAI API."
 show = true
@@ -175,16 +181,16 @@
 
 [py]
 description = "Ask a python programming question."
 [[py.messages]]
 role = "user"
 content = "You are an expert python programmer. Answer the following questions."
 
-[chat]
-description = "Chat with the assistant."
+[enjoy_chat]
+description = "Chat example with a predefined prompt."
 chat = true
 [[chat.messages]]
 role = "user"
 content = "Let's enjoy a chat."
 ```
 
 These messages will be sent as an prompt before your input message.
@@ -201,15 +207,15 @@
 
 ![sh command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_sh.png)
 
 - py
 
 ![py command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_py.png)
 
-- caht
+- enjoy_chat
 
 ![chat command](https://raw.githubusercontent.com/rcmdnk/chatgpt-prompt-wrapper/main/fig/cg_chat.gif)
 
 ## Development
 
 ### Poetry
```

