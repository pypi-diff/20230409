# Comparing `tmp/better-translation-0.3.0.tar.gz` & `tmp/better-translation-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better-translation-0.3.0.tar", last modified: Fri Mar 31 19:33:15 2023, max compression
+gzip compressed data, was "better-translation-0.3.1.tar", last modified: Sun Apr  9 21:32:18 2023, max compression
```

## Comparing `better-translation-0.3.0.tar` & `better-translation-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:15.163493 better-translation-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-31 19:33:15.163493 better-translation-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-31 19:33:09.000000 better-translation-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:15.159492 better-translation-0.3.0/better_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:15.163493 better-translation-0.3.0/better_translation/_babel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/_babel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/_babel/lazy_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:15.163493 better-translation-0.3.0/better_translation/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:15.163493 better-translation-0.3.0/better_translation/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/integrations/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/integrations/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/integrations/django/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-31 19:33:09.000000 better-translation-0.3.0/better_translation/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:33:15.159492 better-translation-0.3.0/better_translation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-31 19:33:15.000000 better-translation-0.3.0/better_translation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-31 19:33:15.000000 better-translation-0.3.0/better_translation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:33:15.000000 better-translation-0.3.0/better_translation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-31 19:33:15.000000 better-translation-0.3.0/better_translation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-31 19:33:09.000000 better-translation-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 19:33:15.163493 better-translation-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-31 19:33:13.000000 better-translation-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.286028 better-translation-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-09 21:32:18.286028 better-translation-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-09 21:32:15.000000 better-translation-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.282028 better-translation-0.3.1/better_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.282028 better-translation-0.3.1/better_translation/_babel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/_babel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/_babel/lazy_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.282028 better-translation-0.3.1/better_translation/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.286028 better-translation-0.3.1/better_translation/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/integrations/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/integrations/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/integrations/django/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.282028 better-translation-0.3.1/better_translation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-09 21:32:18.000000 better-translation-0.3.1/better_translation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-09 21:32:18.000000 better-translation-0.3.1/better_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:32:18.000000 better-translation-0.3.1/better_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 21:32:18.000000 better-translation-0.3.1/better_translation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-09 21:32:15.000000 better-translation-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 21:32:18.286028 better-translation-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-09 21:32:17.000000 better-translation-0.3.1/setup.py
```

### Comparing `better-translation-0.3.0/better_translation/_babel/lazy_proxy.py` & `better-translation-0.3.1/better_translation/_babel/lazy_proxy.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.0/better_translation/extractor.py` & `better-translation-0.3.1/better_translation/extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,21 +75,24 @@
             self.generic_visit(node)
 
     visitor = FunctionCallVisitor()
     tree = ast.parse(code)
     visitor.visit(tree)
 
     for function_call_params in function_calls_params:
+        args = function_call_params["args"]
+        kwargs = function_call_params["kwargs"]
+
+        if None in args:
+            continue
+
         call_params = ", ".join(
             (
-                *(f"{value!r}" for value in function_call_params["args"]),
-                *(
-                    f"{key}={value!r}"
-                    for key, value in function_call_params["kwargs"].items()
-                ),
+                *(f"{value!r}" for value in args),
+                *(f"{key}={value!r}" for key, value in kwargs.items()),
             ),
         )
         yield eval(f"ExtractedMessage({call_params})")  # noqa: PGH001
 
 
 def extract_from_file(
     file_path: Path,
```

### Comparing `better-translation-0.3.0/better_translation/integrations/django/admin.py` & `better-translation-0.3.1/better_translation/integrations/django/admin.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.0/better_translation/integrations/django/models.py` & `better-translation-0.3.1/better_translation/integrations/django/models.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.0/better_translation/integrations/django/storage.py` & `better-translation-0.3.1/better_translation/integrations/django/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             context=message.context,
             has_plural=message.has_plural,
             translations={
                 translation.locale: StorageTranslation(
                     singular=translation.singular,
                     plural=translation.singular,
                 )
-                for translation in message.translations
+                for translation in message.translations.all()
             },
         )
 
     def _get_message_model(
         self,
         storage_message: StorageMessage,
     ) -> BaseMessage:
```

### Comparing `better-translation-0.3.0/better_translation/provider.py` & `better-translation-0.3.1/better_translation/provider.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.0/better_translation/storage.py` & `better-translation-0.3.1/better_translation/storage.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.0/better_translation/translator.py` & `better-translation-0.3.1/better_translation/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import asyncio
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 from better_translation.storage import StorageMessage
 
@@ -114,23 +115,31 @@
         logger.warning(
             "No message found for '%s'. Using the default values: '%s', '%s'",
             message_id,
             default,
             default_plural,
         )
 
-        return StorageMessage(
+        message = StorageMessage(
             id=message_id,
             default=default,
             default_plural=default_plural,
             translations={},
-            context="<no context>",
+            context="",
             has_plural=False,
         )
 
+        _ = asyncio.create_task(
+            self.storage.add_messages(
+                messages=(message,),
+            ),
+        )
+
+        return message
+
     def _get_singular_or_plural(
         self,
         n: int,
         singular: TranslatedText,
         plural: TranslatedText,
     ) -> TranslatedText:
         if n == 1:
```

### Comparing `better-translation-0.3.0/better_translation.egg-info/SOURCES.txt` & `better-translation-0.3.1/better_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.0/pyproject.toml` & `better-translation-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.0/setup.py` & `better-translation-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 _version = (
-    "0.3.0"  # Version will be replaced by the CD pipeline
+    "0.3.1"  # Version will be replaced by the CD pipeline
 )
 VERSION = "0.0.0" if _version.startswith("{{") else _version
 
 
 def get_readme() -> str:
     readme = Path("README.md")
     return readme.read_text(encoding="utf-8")
```

