# Comparing `tmp/chatgdb-1.0.3.tar.gz` & `tmp/chatgdb-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgdb-1.0.3.tar", max compression
+gzip compressed data, was "chatgdb-1.0.4.tar", max compression
```

## Comparing `chatgdb-1.0.3.tar` & `chatgdb-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-03-31 21:54:58.877640 chatgdb-1.0.3/LICENSE
--rw-r--r--   0        0        0     2562 2023-04-07 15:31:50.523582 chatgdb-1.0.3/README.md
--rw-r--r--   0        0        0        0 2023-04-01 22:30:13.298149 chatgdb-1.0.3/chatgdb/__init__.py
--rw-r--r--   0        0        0      748 2023-04-05 01:57:44.066776 chatgdb-1.0.3/chatgdb/cli.py
--rw-r--r--   0        0        0     5325 2023-04-06 18:48:11.972972 chatgdb-1.0.3/chatgdb/core.py
--rw-r--r--   0        0        0      567 2023-04-07 15:33:00.998996 chatgdb-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3528 1970-01-01 00:00:00.000000 chatgdb-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-31 21:54:58.877640 chatgdb-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3364 2023-04-08 15:40:59.988687 chatgdb-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-01 22:30:13.298149 chatgdb-1.0.4/chatgdb/__init__.py
+-rw-r--r--   0        0        0     1159 2023-04-09 00:04:17.999150 chatgdb-1.0.4/chatgdb/cli.py
+-rw-r--r--   0        0        0     5325 2023-04-08 23:18:29.443556 chatgdb-1.0.4/chatgdb/core.py
+-rw-r--r--   0        0        0      567 2023-04-09 00:05:26.683568 chatgdb-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4330 1970-01-01 00:00:00.000000 chatgdb-1.0.4/PKG-INFO
```

### Comparing `chatgdb-1.0.3/LICENSE` & `chatgdb-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgdb-1.0.3/chatgdb/cli.py` & `chatgdb-1.0.4/chatgdb/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 import argparse
 from os.path import abspath, dirname
 from inspect import getfile, currentframe
+from urllib.request import Request, urlopen
+import json
 
 
 def set_key(key):
     """Set the api key for ChatGDB"""
     path = dirname(abspath(getfile(currentframe()))) + "/.secret.txt"
     with open(path, "w") as f:
         f.write("OPENAI_KEY=\"" + key + "\"")
 
 
+def version():
+    """Return version information"""
+    with urlopen(Request("https://pypi.org/pypi/chatgdb/json"), timeout=10) as f:
+        return json.load(f)["info"]["version"]
+
+
 def main():
     parser = argparse.ArgumentParser(
         description="Configure ChatGDB, the GDB chatbot",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument(
         '-k',
         "--key",
         type=str,
         help="Provide an api key for ChatGDB")
+    parser.add_argument(
+        '-v',
+        "--version",
+        action="version",
+        version="%(prog)s " + version(),
+        help="Print the version of ChatGDB")
 
     args = parser.parse_args()
     if args.key:
         set_key(args.key)
     else:
         parser.print_help()
```

### Comparing `chatgdb-1.0.3/chatgdb/core.py` & `chatgdb-1.0.4/chatgdb/core.py`

 * *Files identical despite different names*

### Comparing `chatgdb-1.0.3/pyproject.toml` & `chatgdb-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ChatGDB"
-version = "1.0.3"
+version = "1.0.4"
 authors = ["Pranay Gosar <gosarpranay@gmail.com>"]
 description = "Harness the power of ChatGPT directly inside the GDB debugger!"
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/pgosar/chatgdb"
 keywords = ["gdb", "debugger", "chatgpt"]
```

