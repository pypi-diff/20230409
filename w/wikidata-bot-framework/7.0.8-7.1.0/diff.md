# Comparing `tmp/wikidata-bot-framework-7.0.8.tar.gz` & `tmp/wikidata-bot-framework-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikidata-bot-framework-7.0.8.tar", last modified: Fri Apr  7 13:07:44 2023, max compression
+gzip compressed data, was "wikidata-bot-framework-7.1.0.tar", last modified: Sat Apr  8 22:59:49 2023, max compression
```

## Comparing `wikidata-bot-framework-7.0.8.tar` & `wikidata-bot-framework-7.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-07 13:07:44.743328 wikidata-bot-framework-7.0.8/
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1070 2023-01-08 17:41:08.000000 wikidata-bot-framework-7.0.8/LICENSE
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1186 2023-04-07 13:07:44.743140 wikidata-bot-framework-7.0.8/PKG-INFO
--rw-r--r--   0 aoyansarkar   (501) staff       (20)      146 2023-01-08 17:41:08.000000 wikidata-bot-framework-7.0.8/README.md
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1382 2023-04-07 13:07:33.000000 wikidata-bot-framework-7.0.8/pyproject.toml
--rw-r--r--   0 aoyansarkar   (501) staff       (20)       38 2023-04-07 13:07:44.743383 wikidata-bot-framework-7.0.8/setup.cfg
--rw-r--r--   0 aoyansarkar   (501) staff       (20)       38 2023-01-08 18:32:42.000000 wikidata-bot-framework-7.0.8/setup.py
-drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-07 13:07:44.741459 wikidata-bot-framework-7.0.8/wikidata_bot_framework/
--rw-r--r--   0 aoyansarkar   (501) staff       (20)    35594 2023-04-07 13:07:33.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework/__init__.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)      705 2023-02-04 22:38:43.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework/constants.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)    12102 2023-03-04 17:24:25.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework/dataclasses.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     4782 2023-02-03 21:36:54.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework/process_reason.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1327 2023-01-23 02:06:05.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework/sentry.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1659 2023-02-04 17:10:17.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework/transformers.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     8626 2023-02-20 01:04:13.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework/utils.py
-drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-07 13:07:44.742738 wikidata-bot-framework-7.0.8/wikidata_bot_framework.egg-info/
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1186 2023-04-07 13:07:44.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework.egg-info/PKG-INFO
--rw-r--r--   0 aoyansarkar   (501) staff       (20)      565 2023-04-07 13:07:44.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework.egg-info/SOURCES.txt
--rw-r--r--   0 aoyansarkar   (501) staff       (20)        1 2023-04-07 13:07:44.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework.egg-info/dependency_links.txt
--rw-r--r--   0 aoyansarkar   (501) staff       (20)      102 2023-04-07 13:07:44.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework.egg-info/requires.txt
--rw-r--r--   0 aoyansarkar   (501) staff       (20)       23 2023-04-07 13:07:44.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework.egg-info/top_level.txt
--rw-r--r--   0 aoyansarkar   (501) staff       (20)        1 2023-01-08 18:38:56.000000 wikidata-bot-framework-7.0.8/wikidata_bot_framework.egg-info/zip-safe
+drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-08 22:59:49.033688 wikidata-bot-framework-7.1.0/
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1070 2023-01-08 17:41:08.000000 wikidata-bot-framework-7.1.0/LICENSE
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1186 2023-04-08 22:59:49.033325 wikidata-bot-framework-7.1.0/PKG-INFO
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)      146 2023-01-08 17:41:08.000000 wikidata-bot-framework-7.1.0/README.md
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1382 2023-04-08 22:59:05.000000 wikidata-bot-framework-7.1.0/pyproject.toml
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)       38 2023-04-08 22:59:49.033779 wikidata-bot-framework-7.1.0/setup.cfg
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)       38 2023-01-08 18:32:42.000000 wikidata-bot-framework-7.1.0/setup.py
+drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-08 22:59:49.028634 wikidata-bot-framework-7.1.0/wikidata_bot_framework/
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)    35556 2023-04-08 22:57:57.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/__init__.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)      743 2023-04-08 22:52:06.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/constants.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)    12102 2023-03-04 17:24:25.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/dataclasses.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     4782 2023-02-03 21:36:54.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/process_reason.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1327 2023-01-23 02:06:05.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/sentry.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1659 2023-02-04 17:10:17.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/transformers.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     9920 2023-04-08 22:57:57.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/utils.py
+drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-08 22:59:49.032671 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1186 2023-04-08 22:59:49.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/PKG-INFO
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)      565 2023-04-08 22:59:49.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)        1 2023-04-08 22:59:49.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)      102 2023-04-08 22:59:49.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/requires.txt
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)       23 2023-04-08 22:59:49.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/top_level.txt
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)        1 2023-01-08 18:38:56.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/zip-safe
```

### Comparing `wikidata-bot-framework-7.0.8/LICENSE` & `wikidata-bot-framework-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.0.8/PKG-INFO` & `wikidata-bot-framework-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidata-bot-framework
-Version: 7.0.8
+Version: 7.1.0
 Summary: A framework for making Wikidata bots.
 License: MIT License
 Project-URL: repository, https://github.com/PythonCoderAS/wikidata-bot-framework
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `wikidata-bot-framework-7.0.8/pyproject.toml` & `wikidata-bot-framework-7.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wikidata-bot-framework"
-version = "7.0.8"
+version = "7.1.0"
 description = "A framework for making Wikidata bots."
 readme = "README.md"
 dependencies = [
     "pywikibot",
     "mwparserfromhell",
     "python-dotenv",
     "sentry-sdk",
```

### Comparing `wikidata-bot-framework-7.0.8/wikidata_bot_framework/__init__.py` & `wikidata-bot-framework-7.1.0/wikidata_bot_framework/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,17 +701,15 @@
                                 new_claim, *extra_reference.new_reference_props.values()
                             )
                             acted = True
         with start_span(
             op="post_output_process", description="Post Output Process Hook"
         ):
             if self.post_output_process_hook(output, item):
-                re_cycle |= self.processed_hook(
-                    item, ProcessReason.post_output
-                )
+                re_cycle |= self.processed_hook(item, ProcessReason.post_output)
                 if not acted:
                     acted = True
         if acted:
             with start_span(op="pre_edit_process", description="Pre Edit Process Hook"):
                 self.pre_edit_process_hook(output, item)
             with start_span(op="edit_entity", description="Edit Entity"):
                 retries = 3
```

### Comparing `wikidata-bot-framework-7.0.8/wikidata_bot_framework/constants.py` & `wikidata-bot-framework-7.1.0/wikidata_bot_framework/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,10 +16,12 @@
 
 url_prop = "P854"
 retrieved_prop = "P813"
 archive_url_prop = "P1065"
 archive_date_prop = "P2960"
 deprecated_reason_prop = "P2241"
 link_rot_id = "Q1193907"
+preferred_rank_reason_prop = "P7452"
+
 site: pywikibot.DataSite = pywikibot.Site("wikidata", "wikidata")
 
 EntityPage = Union[pywikibot.ItemPage, pywikibot.PropertyPage, pywikibot.LexemePage]
```

### Comparing `wikidata-bot-framework-7.0.8/wikidata_bot_framework/dataclasses.py` & `wikidata-bot-framework-7.1.0/wikidata_bot_framework/dataclasses.py`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.0.8/wikidata_bot_framework/process_reason.py` & `wikidata-bot-framework-7.1.0/wikidata_bot_framework/process_reason.py`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.0.8/wikidata_bot_framework/sentry.py` & `wikidata-bot-framework-7.1.0/wikidata_bot_framework/sentry.py`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.0.8/wikidata_bot_framework/transformers.py` & `wikidata-bot-framework-7.1.0/wikidata_bot_framework/transformers.py`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.0.8/wikidata_bot_framework/utils.py` & `wikidata-bot-framework-7.1.0/wikidata_bot_framework/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import secrets
 from collections import defaultdict
 from copy import copy
-from typing import Any, Literal, Mapping, MutableMapping, Union, overload
+from typing import Literal, Mapping, MutableMapping, Union, overload
 
 import pywikibot
 
-from .constants import session
+from .constants import session, preferred_rank_reason_prop, site
 from .dataclasses import ExtraProperty, PossibleValueType
 
 
 def add_claim_locally(item: pywikibot.ItemPage, claim: pywikibot.Claim):
     item.claims.setdefault(claim.getID(), []).append(claim)
 
 
@@ -261,7 +261,35 @@
 def get_random_hex(num_chars: int = 32):
     """Generate a random hex suitable for EditGrouos.
 
     :param num_chars: The number of hexadecimal digits wanted, defaults to 32
     :return: A random hex string.
     """
     return secrets.token_hex(num_chars // 2)
+
+
+def mark_claim_as_preferred(
+    claim: Union[pywikibot.Claim, list[pywikibot.Claim]],
+    claim_list: list[pywikibot.Claim],
+    reason_for_preferred_rank_item: Union[pywikibot.ItemPage, None] = None,
+):
+    """Mark a claim as preferred.
+
+    :param claim: The claim or list of claims to mark as preferred.
+    :param claim_list: The list of claims that have the same property as the target claim The target claim(s) will be marked preferred while all other claims will be unmarked.
+    :param reason_for_preferred_rank_item: The item to use as the value for the qualifer "reason for preferred rank". Leave blank to not include the qualifier.
+    """
+    if not isinstance(claim, list):
+        claim = [claim]
+    for c in claim_list:
+        if c in claim:
+            c.rank = "preferred"
+            if reason_for_preferred_rank_item:
+                qual = pywikibot.Claim(
+                    site, preferred_rank_reason_prop, is_qualifier=True
+                )
+                qual.setTarget(reason_for_preferred_rank_item)
+                c.qualifiers[preferred_rank_reason_prop] = [qual]
+        else:
+            c.rank = "normal"
+            if preferred_rank_reason_prop in c.qualifiers:
+                del c.qualifiers[preferred_rank_reason_prop]
```

### Comparing `wikidata-bot-framework-7.0.8/wikidata_bot_framework.egg-info/PKG-INFO` & `wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidata-bot-framework
-Version: 7.0.8
+Version: 7.1.0
 Summary: A framework for making Wikidata bots.
 License: MIT License
 Project-URL: repository, https://github.com/PythonCoderAS/wikidata-bot-framework
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `wikidata-bot-framework-7.0.8/wikidata_bot_framework.egg-info/SOURCES.txt` & `wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

