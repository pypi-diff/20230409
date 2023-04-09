# Comparing `tmp/langchain_utils-0.1.2.tar.gz` & `tmp/langchain_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.1.2.tar", max compression
+gzip compressed data, was "langchain_utils-0.1.3.tar", max compression
```

## Comparing `langchain_utils-0.1.2.tar` & `langchain_utils-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-04-09 14:42:52.744027 langchain_utils-0.1.2/langchain_utils/__init__.py
--rwxr-xr-x   0        0        0     4023 2023-04-09 14:42:02.576415 langchain_utils-0.1.2/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0      449 2023-04-09 14:08:17.975001 langchain_utils-0.1.2/langchain_utils/prompts.py
--rw-r--r--   0        0        0      534 2023-04-09 14:36:32.955521 langchain_utils-0.1.2/langchain_utils/utils.py
--rw-r--r--   0        0        0     1119 2023-04-09 14:42:52.743161 langchain_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 langchain_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-09 04:40:45.952449 langchain_utils-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-04-09 14:47:07.372336 langchain_utils-0.1.3/langchain_utils/__init__.py
+-rwxr-xr-x   0        0        0     4309 2023-04-09 14:45:07.607836 langchain_utils-0.1.3/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0      449 2023-04-09 14:08:17.975001 langchain_utils-0.1.3/langchain_utils/prompts.py
+-rw-r--r--   0        0        0      534 2023-04-09 14:36:32.955521 langchain_utils-0.1.3/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1119 2023-04-09 14:47:07.371731 langchain_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 langchain_utils-0.1.3/PKG-INFO
```

### Comparing `langchain_utils-0.1.2/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.1.3/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -96,28 +96,34 @@
                 )
             else:
                 prompt = PromptTemplate.from_template(
                     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_CONTINUED
                 ).partial(x=str(i + 1))
             content = doc.page_content
             formatted_prompt = prompt.format(what=what, content=content)
-            input(f'Press Enter to copy prompt {i+1}/{num_chunks}: ')
+            input(
+                f'Press Enter to copy prompt {i+1}/{num_chunks}. Word Count: {get_word_count(formatted_prompt)}, Char count: {len(formatted_prompt)}: '
+            )
             import pyperclip
 
             pyperclip.copy(formatted_prompt)
 
         return
     transcript = docs[0].page_content
     prompt = PromptTemplate.from_template(REPLY_OK_IF_YOU_READ_TEMPLATE)
     content = transcript
     formatted_prompt = prompt.format(what=what, content=content)
     if args.copy:
         import pyperclip
 
+        print(
+            f'Word Count: {get_word_count(formatted_prompt)}, Char count: {len(formatted_prompt)}',
+            file=sys.stderr,
+        )
         pyperclip.copy(formatted_prompt)
-        print('Prompt copied to clipboard.')
+        print('Prompt copied to clipboard.', file=sys.stderr)
     else:
         print(formatted_prompt)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.1.2/langchain_utils/utils.py` & `langchain_utils-0.1.3/langchain_utils/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.1.2/pyproject.toml` & `langchain_utils-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.1.2/PKG-INFO` & `langchain_utils-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

