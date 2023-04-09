# Comparing `tmp/qq_chat_history-1.1.2.tar.gz` & `tmp/qq_chat_history-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qq_chat_history-1.1.2.tar", max compression
+gzip compressed data, was "qq_chat_history-1.1.3.tar", max compression
```

## Comparing `qq_chat_history-1.1.2.tar` & `qq_chat_history-1.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-01-22 09:17:50.147457 qq_chat_history-1.1.2/LICENSE
--rw-r--r--   0        0        0      744 2023-03-19 03:17:34.950361 qq_chat_history-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      168 2023-03-18 07:36:17.870473 qq_chat_history-1.1.2/qq_chat_history/__init__.py
--rw-r--r--   0        0        0     5502 2023-03-19 02:59:50.357119 qq_chat_history-1.1.2/qq_chat_history/body.py
--rw-r--r--   0        0        0     1020 2023-03-19 03:14:07.609138 qq_chat_history-1.1.2/qq_chat_history/cli.py
--rw-r--r--   0        0        0      419 2023-03-17 15:22:57.736528 qq_chat_history-1.1.2/qq_chat_history/message.py
--rw-r--r--   0        0        0        0 2023-01-22 12:44:48.720506 qq_chat_history-1.1.2/qq_chat_history/py.typed
--rw-r--r--   0        0        0     2669 2023-03-19 03:17:24.426596 qq_chat_history-1.1.2/README.md
--rw-r--r--   0        0        0     3497 1970-01-01 00:00:00.000000 qq_chat_history-1.1.2/setup.py
--rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 qq_chat_history-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-01-22 09:17:50.147457 qq_chat_history-1.1.3/LICENSE
+-rw-r--r--   0        0        0      744 2023-04-09 14:58:02.590517 qq_chat_history-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-03-18 07:36:17.870473 qq_chat_history-1.1.3/qq_chat_history/__init__.py
+-rw-r--r--   0        0        0     5484 2023-04-09 14:55:58.142430 qq_chat_history-1.1.3/qq_chat_history/body.py
+-rw-r--r--   0        0        0     1011 2023-04-09 14:56:07.727793 qq_chat_history-1.1.3/qq_chat_history/cli.py
+-rw-r--r--   0        0        0      450 2023-04-09 14:56:46.627991 qq_chat_history-1.1.3/qq_chat_history/message.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:44:48.720506 qq_chat_history-1.1.3/qq_chat_history/py.typed
+-rw-r--r--   0        0        0     2669 2023-03-19 03:17:24.426596 qq_chat_history-1.1.3/README.md
+-rw-r--r--   0        0        0     3497 1970-01-01 00:00:00.000000 qq_chat_history-1.1.3/setup.py
+-rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 qq_chat_history-1.1.3/PKG-INFO
```

### Comparing `qq_chat_history-1.1.2/LICENSE` & `qq_chat_history-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qq_chat_history-1.1.2/pyproject.toml` & `qq_chat_history-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qq-chat-history"
-version = "1.1.2"
+version = "1.1.3"
 description = "A tool to extract QQ chat history."
 authors = ["kifuan <kifuan@foxmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "qq_chat_history"}]
 repository = "https://github.com/kifuan/qq-chat-history"
```

### Comparing `qq_chat_history-1.1.2/qq_chat_history/body.py` & `qq_chat_history-1.1.3/qq_chat_history/body.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 from .message import Message, MessageBuilder
 
 BRACKETS_REGEX = re.compile(r'[(<]([^()<>]*?)[>)]$')
 DATE_HEAD_REGEX = re.compile(r'^(\d{4}-\d{2}-\d{2}\s+\d\d?:\d{2}:\d{2})\s+')
 
 
 class Body:
-    """The parsed chat-history file body containing messages."""
+    """Chat history file body containing messages."""
 
     def __init__(self, messages: list[Message]) -> None:
         """Initializes the body with messages.
 
-        It is not recommended to construct a body directly.
-        Instead, you should use `from_xxx`, which are class methods.
+        Not recommended to construct a body directly.
+        Instead, using class methods `from_xxx` is recommended.
         """
         self._messages = messages
 
     @staticmethod
     def _make_builder_from_head(line: str) -> Optional[MessageBuilder]:
-        """Parses a message head, returns None if given line is not a message head."""
+        """Parses a message head. Returns None if the given line is invalid."""
         if (date_matcher := DATE_HEAD_REGEX.search(line)) is None:
             return None
         date = date_matcher.group().strip()
 
         if matcher := BRACKETS_REGEX.findall(line):
             group_user_id = cast(str, matcher[-1])
             name = DATE_HEAD_REGEX.sub('', BRACKETS_REGEX.sub('', line)).strip()
@@ -52,15 +52,15 @@
             '\n'.join(
                 content_lines.popleft() for _ in range(len(content_lines))
             ),
         )
 
     @classmethod
     def from_lines(cls, lines: Iterable[str]) -> 'Body':
-        """Creates a message group from lines."""
+        """Builds a body from lines."""
         messages: list[Message] = []
         builder: Optional[MessageBuilder] = None
         content_lines: deque[str] = deque()
 
         for line in dropwhile(lambda li: cls._make_builder_from_head(li) is None, lines):
             if next_builder := cls._make_builder_from_head(line):
                 messages.extend(cls._gen_from_builder(builder, content_lines))
@@ -70,21 +70,21 @@
                 content_lines.append(line)
 
         messages.extend(cls._gen_from_builder(builder, content_lines))
         return cls(messages)
 
     @classmethod
     def from_path(cls, path: Union[str, Path]) -> 'Body':
-        """Creates a message group from path to certain file."""
+        """Builds a body from path to certain file."""
         if isinstance(path, str):
             path = Path(path)
         return cls.from_lines(path.read_text('utf8').splitlines())
 
     def save(self, fp: TextIO, fmt: str, indent: int) -> None:
-        """Saves the body to file, supporting `yaml` and `json` files."""
+        """Saves to a file, supporting `yaml` and `json` formats."""
         data = [m.__dict__ for m in self._messages]
 
         if fmt == 'json':
             ujson.dump(
                 data, fp,
                 ensure_ascii=False,
                 indent=indent,
@@ -112,44 +112,44 @@
 
     def find_names(self, id_: str) -> list[str]:
         """Gets all names used by given id."""
         return [msg.name for msg in self._messages if msg.id == id_]
 
     @lru_cache()
     def find_latest_name(self, id_: str) -> Optional[str]:
-        """Gets the latest name used by given id."""
+        """Gets the latest name used by given id. Returns None when not found."""
         if names := self.find_names(id_):
             return names[-1]
         return None
 
     def find_messages_by_id(self, id_: str) -> list[Message]:
         """Finds all messages by given id."""
         return [msg for msg in self._messages if msg.id == id_]
 
     def find_messages_by_name(self, name: str) -> list[Message]:
         """Finds all messages by given name."""
         return [msg for msg in self._messages if msg.name == name]
 
     def find_first_message_by_id(self, id_: str) -> Optional[Message]:
-        """Finds first message by given id."""
+        """Finds the first message by given id."""
         for msg in self._messages:
             if msg.id == id_:
                 return msg
         return None
 
     def find_first_message_by_name(self, name: str) -> Optional[Message]:
-        """Finds first message by given name."""
+        """Finds the first message by given name."""
         for msg in self._messages:
             if msg.name == name:
                 return msg
         return None
 
 
 def parse(data: Union[Iterable[str], TextIOBase, str, Path]) -> Body:
-    """Parses given data in a message group."""
+    """Builds a message body by given data."""
     if isinstance(data, (str, Path)):
         return Body.from_path(data)
 
     if isinstance(data, TextIOBase):
         data = data.read().splitlines()
 
     return Body.from_lines(data)
```

### Comparing `qq_chat_history-1.1.2/qq_chat_history/cli.py` & `qq_chat_history-1.1.3/qq_chat_history/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 )
 @click.option(
     '--output-format', '-f', help='Output file format.',
     type=click.Choice(['json', 'yaml']), default='json', show_default=True,
 )
 @click.option('--indent', '-d', help='Output file indent.', type=int, default=2, show_default=True)
 def run(input_file: Path, output_file: Path, output_format: str, indent: int) -> None:
-    """Parse a chat history file in the command line."""
+    """Parse a chat history file in the CLI."""
     if output_file.suffix[1:] != output_format:
         output_file = output_file.with_suffix(f'.{output_format}')
 
     with output_file.open('w', encoding='utf8') as fp:
         parse(input_file).save(fp, output_format, indent)
```

### Comparing `qq_chat_history-1.1.2/README.md` & `qq_chat_history-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `qq_chat_history-1.1.2/setup.py` & `qq_chat_history-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'pyyaml>=6.0,<7.0', 'ujson>=5.7.0,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['qq-chat-history = qq_chat_history.cli:run']}
 
 setup_kwargs = {
     'name': 'qq-chat-history',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': 'A tool to extract QQ chat history.',
     'long_description': "# QQ 聊天记录提取器\n\n## 简介\n\n从 QQ 聊天记录文件中提取聊天信息，仅支持 `txt` 格式的聊天记录。\n\n\n## 安装\n\n使用 `pip` 安装，要求 `Python 3.9` 或以上版本。\n\n```bash\n> pip install -U qq-chat-history\n```\n\n## 使用\n\n最简单的启动方式如下，它会自动在当前目录下创建 `output.json` 进行输出（如果安装到虚拟环境请确保已激活）。\n\n```bash\n> qq-chat-history /path/to/file.txt\n```\n\n启动时输入 `--help` 参数查看更多配置项。\n\n```bash\n> qq-chat-history --help\n```\n\n或者，可以在代码中使用，如下：\n\n```python\nimport qq_chat_history\n\nlines = '''\n=========\n假装我是 QQ 自动生成的文件头\n=========\n\n1883-03-07 11:22:33 A<someone@example.com>\n关注永雏塔菲喵\n关注永雏塔菲谢谢喵\n\n1883-03-07 12:34:56 B(123123)\nTCG\n\n1883-03-07 13:24:36 C(456456)\nTCG\n\n1883-03-07 22:00:51 A<someone@example.com>\n塔菲怎么你了\n'''.strip().splitlines()\n\nfor msg in qq_chat_history.parse(lines):\n    print(msg.date, msg.id, msg.name, msg.content)\n```\n\n注意 `parse` 方法返回的是一个 `Body` 对象，一般以 `Iterable[Message]` 的形式使用。除外，`Body` 也提供了几个函数，~虽然一般也没什么用~。\n\n## Tips\n\n+ 在 `0.3.0+` 版本中，对于 `parse` 方法的实现进行了大调整，它将返回一个 `Body` 类，原先是 `Iterable[Message]`。但这并**不会导致兼容性问题**，因为 `Body` 也是一个 `Iterable[Message]`。\n\n  不同的是，`Body` 类相对于原先单纯的生成器**提供更多功能**，例如`find_xxx` 方法，可以从数据中查找指定 `id` 或 `name` 的消息；`save` 方法可以将数据以 `yaml` 或 `json` 格式保存到文件中，虽然这个工作一般都直接以 `CLI` 模式启动来完成。\n\n+ 在 `0.3.0+` 版本中，你可以向 `parse` 中传入多种多样的类型。\n\n  + `Iterable[str]`：迭代每行的可迭代对象，如 `list` 或 `tuple` 等。\n  + `TextIOBase`：文本文件对象，如用 `open` 打开的文本文件，或者 `io.StringIO` 都属于文本文件对象。\n  + `str`, `Path`：文件路径，如 `./data.txt`。\n\n  这些参数都将被调用合适的工厂方法来构造 `Body` 对象。\n\n+ 由于 `parse` 这个名字的含义比较不清晰，推荐与不推荐的使用方式如下：\n\n  ```python\n  # Not recommended 👎\n  from qq_chat_history import parse\n  parse(...)\n  \n  \n  # Recommended 👍\n  import qq_chat_history\n  qq_chat_history.parse(...)\n  \n  \n  from qq_chat_history import parse as parse_qq\n  parse_qq(...)\n  ```\n\n",
     'author': 'kifuan',
     'author_email': 'kifuan@foxmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kifuan/qq-chat-history',
```

### Comparing `qq_chat_history-1.1.2/PKG-INFO` & `qq_chat_history-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qq-chat-history
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool to extract QQ chat history.
 Home-page: https://github.com/kifuan/qq-chat-history
 License: MIT
 Author: kifuan
 Author-email: kifuan@foxmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

