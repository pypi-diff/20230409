# Comparing `tmp/ronbun-0.7.1.tar.gz` & `tmp/ronbun-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ronbun-0.7.1.tar", last modified: Fri Apr  7 01:58:07 2023, max compression
+gzip compressed data, was "ronbun-0.7.2.tar", last modified: Sun Apr  9 15:33:46 2023, max compression
```

## Comparing `ronbun-0.7.1.tar` & `ronbun-0.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:58:07.776715 ronbun-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-07 01:57:58.000000 ronbun-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-07 01:58:07.772715 ronbun-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-07 01:57:58.000000 ronbun-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:58:07.772715 ronbun-0.7.1/ronbun/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-07 01:57:58.000000 ronbun-0.7.1/ronbun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-04-07 01:57:58.000000 ronbun-0.7.1/ronbun/readme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:58:07.772715 ronbun-0.7.1/ronbun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-07 01:58:07.000000 ronbun-0.7.1/ronbun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-07 01:58:07.000000 ronbun-0.7.1/ronbun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 01:58:07.000000 ronbun-0.7.1/ronbun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 01:58:07.000000 ronbun-0.7.1/ronbun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-07 01:58:07.000000 ronbun-0.7.1/ronbun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-07 01:58:07.000000 ronbun-0.7.1/ronbun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 01:58:07.776715 ronbun-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-07 01:57:58.000000 ronbun-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:33:46.932200 ronbun-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 15:33:35.000000 ronbun-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-09 15:33:46.932200 ronbun-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-09 15:33:35.000000 ronbun-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:33:46.928200 ronbun-0.7.2/ronbun/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 15:33:35.000000 ronbun-0.7.2/ronbun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-04-09 15:33:35.000000 ronbun-0.7.2/ronbun/readme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:33:46.928200 ronbun-0.7.2/ronbun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 15:33:46.932200 ronbun-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-09 15:33:35.000000 ronbun-0.7.2/setup.py
```

### Comparing `ronbun-0.7.1/LICENSE` & `ronbun-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ronbun-0.7.1/PKG-INFO` & `ronbun-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ronbun
-Version: 0.7.1
+Version: 0.7.2
 Summary: The Sample Programs README Automation Tool
 Home-page: https://github.com/TheRenegadeCoder/sample-programs-readmes
 Author: The Renegade Coder
 Author-email: jeremy.grifski@therenegadecoder.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ronbun-0.7.1/ronbun/readme.py` & `ronbun-0.7.2/ronbun/readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import argparse
 import logging
 import ssl
+import urllib.parse
 
 from snakemd import Document, Inline, MDList, Paragraph
 from subete import LanguageCollection, Repo, Project
 
 
 logger = logging.getLogger(__name__)
 
 
 issue_url_template_base = "https://github.com/TheRenegadeCoder/sample-programs/issues/new"
-issue_url_template_query = "?assignees=&labels=enhancement&template=code-snippet-request.md&title=Add+{project}+in+{language}"
+issue_url_template_query = "?assignees=&labels=enhancement,{label}&template=code-snippet-request.md&title=Add+{project}+in+{language}"
 
 
 def main():
     ssl._create_default_https_context = ssl._create_unverified_context
     args = _get_args()
     numeric_level = getattr(logging, args[1].upper(), None)
     if not isinstance(numeric_level, int):
@@ -78,15 +79,19 @@
 def _generate_missing_program_list(language: LanguageCollection, missing_programs: list[str]):
     list_items = list()
     missing_programs.sort(key=lambda x: x.name())
     for program in missing_programs:
         program: Project
         program_name = program.name()
         program_query = "+".join(program_name.split())
-        url = issue_url_template_base + issue_url_template_query.format(project=program_query, language=language.pathlike_name())
+        url = issue_url_template_base + issue_url_template_query.format(
+            label=program_query.lower(),
+            project=program_query,
+            language=urllib.parse.quote(language.name())
+        )
         program_item = Paragraph([f":x: {program_name} [Requirements]"])\
             .insert_link(program_name, url)\
             .insert_link("Requirements", program.requirements_url())
         list_items.append(program_item)
     return list_items
```

### Comparing `ronbun-0.7.1/ronbun.egg-info/PKG-INFO` & `ronbun-0.7.2/ronbun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ronbun
-Version: 0.7.1
+Version: 0.7.2
 Summary: The Sample Programs README Automation Tool
 Home-page: https://github.com/TheRenegadeCoder/sample-programs-readmes
 Author: The Renegade Coder
 Author-email: jeremy.grifski@therenegadecoder.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ronbun-0.7.1/setup.py` & `ronbun-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ronbun",
-    version="0.7.1",
+    version="0.7.2",
     author="The Renegade Coder",
     author_email="jeremy.grifski@therenegadecoder.com",
     description="The Sample Programs README Automation Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheRenegadeCoder/sample-programs-readmes",
     packages=setuptools.find_packages(),
     install_requires=[
         "SnakeMD>=2.0.0b1",
-        "subete>=0.11"
+        "subete>=0.15.1"
     ],
     entry_points={
         "console_scripts": [
             'ronbun = ronbun.readme:main'
         ],
     },
     classifiers=(
```

