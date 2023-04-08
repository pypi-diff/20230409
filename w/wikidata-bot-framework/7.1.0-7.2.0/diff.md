# Comparing `tmp/wikidata-bot-framework-7.1.0.tar.gz` & `tmp/wikidata-bot-framework-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikidata-bot-framework-7.1.0.tar", last modified: Sat Apr  8 22:59:49 2023, max compression
+gzip compressed data, was "wikidata-bot-framework-7.2.0.tar", last modified: Sat Apr  8 23:34:49 2023, max compression
```

## Comparing `wikidata-bot-framework-7.1.0.tar` & `wikidata-bot-framework-7.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-08 22:59:49.033688 wikidata-bot-framework-7.1.0/
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1070 2023-01-08 17:41:08.000000 wikidata-bot-framework-7.1.0/LICENSE
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1186 2023-04-08 22:59:49.033325 wikidata-bot-framework-7.1.0/PKG-INFO
--rw-r--r--   0 aoyansarkar   (501) staff       (20)      146 2023-01-08 17:41:08.000000 wikidata-bot-framework-7.1.0/README.md
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1382 2023-04-08 22:59:05.000000 wikidata-bot-framework-7.1.0/pyproject.toml
--rw-r--r--   0 aoyansarkar   (501) staff       (20)       38 2023-04-08 22:59:49.033779 wikidata-bot-framework-7.1.0/setup.cfg
--rw-r--r--   0 aoyansarkar   (501) staff       (20)       38 2023-01-08 18:32:42.000000 wikidata-bot-framework-7.1.0/setup.py
-drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-08 22:59:49.028634 wikidata-bot-framework-7.1.0/wikidata_bot_framework/
--rw-r--r--   0 aoyansarkar   (501) staff       (20)    35556 2023-04-08 22:57:57.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/__init__.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)      743 2023-04-08 22:52:06.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/constants.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)    12102 2023-03-04 17:24:25.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/dataclasses.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     4782 2023-02-03 21:36:54.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/process_reason.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1327 2023-01-23 02:06:05.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/sentry.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1659 2023-02-04 17:10:17.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/transformers.py
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     9920 2023-04-08 22:57:57.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework/utils.py
-drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-08 22:59:49.032671 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/
--rw-r--r--   0 aoyansarkar   (501) staff       (20)     1186 2023-04-08 22:59:49.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/PKG-INFO
--rw-r--r--   0 aoyansarkar   (501) staff       (20)      565 2023-04-08 22:59:49.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/SOURCES.txt
--rw-r--r--   0 aoyansarkar   (501) staff       (20)        1 2023-04-08 22:59:49.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/dependency_links.txt
--rw-r--r--   0 aoyansarkar   (501) staff       (20)      102 2023-04-08 22:59:49.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/requires.txt
--rw-r--r--   0 aoyansarkar   (501) staff       (20)       23 2023-04-08 22:59:49.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/top_level.txt
--rw-r--r--   0 aoyansarkar   (501) staff       (20)        1 2023-01-08 18:38:56.000000 wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/zip-safe
+drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-08 23:34:49.565075 wikidata-bot-framework-7.2.0/
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1070 2023-01-08 17:41:08.000000 wikidata-bot-framework-7.2.0/LICENSE
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1186 2023-04-08 23:34:49.564853 wikidata-bot-framework-7.2.0/PKG-INFO
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)      146 2023-01-08 17:41:08.000000 wikidata-bot-framework-7.2.0/README.md
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1382 2023-04-08 23:31:56.000000 wikidata-bot-framework-7.2.0/pyproject.toml
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)       38 2023-04-08 23:34:49.565138 wikidata-bot-framework-7.2.0/setup.cfg
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)       38 2023-01-08 18:32:42.000000 wikidata-bot-framework-7.2.0/setup.py
+drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-08 23:34:49.562815 wikidata-bot-framework-7.2.0/wikidata_bot_framework/
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)    35556 2023-04-08 22:57:57.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework/__init__.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)      743 2023-04-08 22:52:06.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework/constants.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)    12102 2023-03-04 17:24:25.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework/dataclasses.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     4782 2023-02-03 21:36:54.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework/process_reason.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1327 2023-01-23 02:06:05.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework/sentry.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1659 2023-02-04 17:10:17.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework/transformers.py
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)    10326 2023-04-08 23:31:44.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework/utils.py
+drwxr-xr-x   0 aoyansarkar   (501) staff       (20)        0 2023-04-08 23:34:49.564417 wikidata-bot-framework-7.2.0/wikidata_bot_framework.egg-info/
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)     1186 2023-04-08 23:34:49.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework.egg-info/PKG-INFO
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)      565 2023-04-08 23:34:49.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)        1 2023-04-08 23:34:49.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)      102 2023-04-08 23:34:49.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework.egg-info/requires.txt
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)       23 2023-04-08 23:34:49.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework.egg-info/top_level.txt
+-rw-r--r--   0 aoyansarkar   (501) staff       (20)        1 2023-01-08 18:38:56.000000 wikidata-bot-framework-7.2.0/wikidata_bot_framework.egg-info/zip-safe
```

### Comparing `wikidata-bot-framework-7.1.0/LICENSE` & `wikidata-bot-framework-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.1.0/PKG-INFO` & `wikidata-bot-framework-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidata-bot-framework
-Version: 7.1.0
+Version: 7.2.0
 Summary: A framework for making Wikidata bots.
 License: MIT License
 Project-URL: repository, https://github.com/PythonCoderAS/wikidata-bot-framework
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `wikidata-bot-framework-7.1.0/pyproject.toml` & `wikidata-bot-framework-7.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wikidata-bot-framework"
-version = "7.1.0"
+version = "7.2.0"
 description = "A framework for making Wikidata bots."
 readme = "README.md"
 dependencies = [
     "pywikibot",
     "mwparserfromhell",
     "python-dotenv",
     "sentry-sdk",
```

### Comparing `wikidata-bot-framework-7.1.0/wikidata_bot_framework/__init__.py` & `wikidata-bot-framework-7.2.0/wikidata_bot_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.1.0/wikidata_bot_framework/constants.py` & `wikidata-bot-framework-7.2.0/wikidata_bot_framework/constants.py`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.1.0/wikidata_bot_framework/dataclasses.py` & `wikidata-bot-framework-7.2.0/wikidata_bot_framework/dataclasses.py`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.1.0/wikidata_bot_framework/process_reason.py` & `wikidata-bot-framework-7.2.0/wikidata_bot_framework/process_reason.py`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.1.0/wikidata_bot_framework/sentry.py` & `wikidata-bot-framework-7.2.0/wikidata_bot_framework/sentry.py`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.1.0/wikidata_bot_framework/transformers.py` & `wikidata-bot-framework-7.2.0/wikidata_bot_framework/transformers.py`

 * *Files identical despite different names*

### Comparing `wikidata-bot-framework-7.1.0/wikidata_bot_framework/utils.py` & `wikidata-bot-framework-7.2.0/wikidata_bot_framework/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,29 +267,39 @@
     return secrets.token_hex(num_chars // 2)
 
 
 def mark_claim_as_preferred(
     claim: Union[pywikibot.Claim, list[pywikibot.Claim]],
     claim_list: list[pywikibot.Claim],
     reason_for_preferred_rank_item: Union[pywikibot.ItemPage, None] = None,
-):
+) -> bool:
     """Mark a claim as preferred.
 
     :param claim: The claim or list of claims to mark as preferred.
     :param claim_list: The list of claims that have the same property as the target claim The target claim(s) will be marked preferred while all other claims will be unmarked.
     :param reason_for_preferred_rank_item: The item to use as the value for the qualifer "reason for preferred rank". Leave blank to not include the qualifier.
+    :return: True if the rank of any claims were changed.
     """
     if not isinstance(claim, list):
         claim = [claim]
+    changed = False
     for c in claim_list:
         if c in claim:
-            c.rank = "preferred"
+            if not c.rank == "preferred":
+                c.rank = "preferred"
+                changed = True
             if reason_for_preferred_rank_item:
                 qual = pywikibot.Claim(
                     site, preferred_rank_reason_prop, is_qualifier=True
                 )
                 qual.setTarget(reason_for_preferred_rank_item)
-                c.qualifiers[preferred_rank_reason_prop] = [qual]
+                if c.qualifiers.get(preferred_rank_reason_prop, None) != [qual]:
+                    c.qualifiers[preferred_rank_reason_prop] = [qual]
+                    changed = True
         else:
-            c.rank = "normal"
+            if c.rank == "preferred":
+                c.rank = "normal"
+                changed = True
             if preferred_rank_reason_prop in c.qualifiers:
                 del c.qualifiers[preferred_rank_reason_prop]
+                changed = True
+    return changed
```

### Comparing `wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/PKG-INFO` & `wikidata-bot-framework-7.2.0/wikidata_bot_framework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidata-bot-framework
-Version: 7.1.0
+Version: 7.2.0
 Summary: A framework for making Wikidata bots.
 License: MIT License
 Project-URL: repository, https://github.com/PythonCoderAS/wikidata-bot-framework
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `wikidata-bot-framework-7.1.0/wikidata_bot_framework.egg-info/SOURCES.txt` & `wikidata-bot-framework-7.2.0/wikidata_bot_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

