# Comparing `tmp/griptape_core-0.2.1.tar.gz` & `tmp/griptape_core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_core-0.2.1.tar", max compression
+gzip compressed data, was "griptape_core-0.3.0.tar", max compression
```

## Comparing `griptape_core-0.2.1.tar` & `griptape_core-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.2.1/LICENSE
--rw-r--r--   0        0        0     2812 2023-04-07 15:41:17.241816 griptape_core-0.2.1/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.2.1/griptape/__init__.py
--rw-r--r--   0        0        0      349 2023-04-07 15:43:24.029341 griptape_core-0.2.1/griptape/core/__init__.py
--rw-r--r--   0        0        0      184 2023-04-07 15:22:12.494258 griptape_core-0.2.1/griptape/core/adapters/__init__.py
--rw-r--r--   0        0        0     2389 2023-04-07 15:41:17.249886 griptape_core-0.2.1/griptape/core/adapters/chatgpt_plugin_adapter.py
--rw-r--r--   0        0        0     1137 2023-04-07 15:41:45.232080 griptape_core-0.2.1/griptape/core/adapters/langchain_tool_adapter.py
--rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.2.1/griptape/core/base_adapter.py
--rw-r--r--   0        0        0      467 2023-04-07 15:43:24.032498 griptape_core-0.2.1/griptape/core/base_executor.py
--rw-r--r--   0        0        0     3283 2023-04-07 15:41:17.246638 griptape_core-0.2.1/griptape/core/base_tool.py
--rw-r--r--   0        0        0      358 2023-04-06 20:17:23.179136 griptape_core-0.2.1/griptape/core/decorators.py
--rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.2.1/griptape/core/executors/__init__.py
--rw-r--r--   0        0        0     3048 2023-04-07 15:57:20.791900 griptape_core-0.2.1/griptape/core/executors/docker_executor.py
--rw-r--r--   0        0        0     1887 2023-04-07 15:42:00.394059 griptape_core-0.2.1/griptape/core/executors/local_executor.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.2.1/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.2.1/griptape/core/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      233 2023-04-06 20:17:23.179816 griptape_core-0.2.1/griptape/core/utils/__init__.py
--rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.2.1/griptape/core/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.2.1/griptape/core/utils/manifest_validator.py
--rw-r--r--   0        0        0      708 2023-04-07 15:58:04.457023 griptape_core-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 griptape_core-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2812 2023-04-07 15:41:17.241816 griptape_core-0.3.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.3.0/griptape/__init__.py
+-rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.3.0/griptape/core/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.3.0/griptape/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2399 2023-04-08 22:46:20.173376 griptape_core-0.3.0/griptape/core/adapters/chatgpt_plugin_adapter.py
+-rw-r--r--   0        0        0     1010 2023-04-08 22:52:20.104416 griptape_core-0.3.0/griptape/core/adapters/langchain_tool_adapter.py
+-rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.3.0/griptape/core/base_adapter.py
+-rw-r--r--   0        0        0      467 2023-04-07 15:43:24.032498 griptape_core-0.3.0/griptape/core/base_executor.py
+-rw-r--r--   0        0        0     3287 2023-04-08 22:48:21.389760 griptape_core-0.3.0/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      533 2023-04-08 22:54:40.019493 griptape_core-0.3.0/griptape/core/decorators.py
+-rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.3.0/griptape/core/executors/__init__.py
+-rw-r--r--   0        0        0     3048 2023-04-07 15:57:20.791900 griptape_core-0.3.0/griptape/core/executors/docker_executor.py
+-rw-r--r--   0        0        0     1887 2023-04-07 15:42:00.394059 griptape_core-0.3.0/griptape/core/executors/local_executor.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.3.0/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.3.0/griptape/core/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      233 2023-04-06 20:17:23.179816 griptape_core-0.3.0/griptape/core/utils/__init__.py
+-rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.3.0/griptape/core/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.3.0/griptape/core/utils/manifest_validator.py
+-rw-r--r--   0        0        0      708 2023-04-09 16:41:52.228246 griptape_core-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 griptape_core-0.3.0/PKG-INFO
```

### Comparing `griptape_core-0.2.1/LICENSE` & `griptape_core-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.1/README.md` & `griptape_core-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.1/griptape/core/adapters/chatgpt_plugin_adapter.py` & `griptape_core-0.3.0/griptape/core/adapters/chatgpt_plugin_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             functools.partial(self.generate_api_spec, app),
             methods=["GET"],
             description="OpenAPI plugin spec"
         )
 
         for action in tool.actions():
             app.add_api_route(
-                f"{self.path_prefix}{action.name}",
+                f"{self.path_prefix}{action.config['name']}",
                 functools.partial(self.__execute_action, action),
                 methods=["GET"],
                 description=tool.get_action_description(action)
             )
 
         return app
```

### Comparing `griptape_core-0.2.1/griptape/core/base_tool.py` & `griptape_core-0.3.0/griptape/core/base_tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import inspect
 import json
 import os
 from abc import ABC
 from typing import Optional
 import yaml
 from attr import define, fields, Attribute
-from schema import Literal
 
 
 @define
 class BaseTool(ABC):
     MANIFEST_FILE = "manifest.yml"
     DOCKERFILE_FILE = "Dockerfile"
     REQUIREMENTS_FILE = "requirements.txt"
 
-
     @property
     def env_fields(self) -> list[Attribute]:
         return [f for f in fields(self.__class__) if f.metadata.get("env")]
 
     @property
     def env(self) -> dict[str, str]:
         return {f.metadata["env"]: str(getattr(self, f.name)) for f in self.env_fields}
@@ -66,25 +64,26 @@
                 None
             )
 
     def get_action_description(self, action: callable) -> str:
         if action is None or not getattr(action, "is_action", False):
             raise Exception("This method is not a tool action.")
         else:
-            return [
-                f"{key.description}"
-                for key in action.schema.schema.keys()
-                if isinstance(key, Literal) and str(key) == "action_input" and key.description
-            ][0]
+            schema = action.config['input_schema'].json_schema('ToolActionSchema')
+
+            return str.join("\n", [
+                action.config["description"],
+                f"Input schema: {json.dumps(schema)}"
+            ])
 
-    def get_action_schema(self, action: callable) -> str:
+    def get_action_input_schema(self, action: callable) -> str:
         if action is None or not getattr(action, "is_action", False):
             raise Exception("This method is not a tool action.")
         else:
-            return json.dumps(action.schema.json_schema("ToolInputSchema"))
+            return json.dumps(action.config["input_schema"].json_schema("ToolInputSchema"))
 
     def actions(self) -> list[callable]:
         methods = []
 
         for name, method in inspect.getmembers(self, predicate=inspect.ismethod):
             if getattr(method, "is_action", False):
                 methods.append(method)
```

### Comparing `griptape_core-0.2.1/griptape/core/executors/docker_executor.py` & `griptape_core-0.3.0/griptape/core/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.1/griptape/core/executors/local_executor.py` & `griptape_core-0.3.0/griptape/core/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.1/griptape/core/utils/j2.py` & `griptape_core-0.3.0/griptape/core/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.1/pyproject.toml` & `griptape_core-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-core"
-version = "0.2.1"
+version = "0.3.0"
 description = "Python framework for LLM middleware tools. Build once, run anywhere."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-core"
 
 packages = [
@@ -17,15 +17,15 @@
 jinja2 = ">=3.1"
 docker = ">=6"
 stringcase = ">=1"
 schema = ">=0.7"
 pyyaml = ">=6"
 openai = ">=0.27"
 langchain = ">=0.0.120"
-fastapi = ">=0.90"
+fastapi = ">=0.80"
 uvicorn = ">= 0.20"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-mock = "*"
 
 [build-system]
```

### Comparing `griptape_core-0.2.1/PKG-INFO` & `griptape_core-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: griptape-core
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python framework for LLM middleware tools. Build once, run anywhere.
 Home-page: https://github.com/griptape-ai/griptape-core
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=22)
 Requires-Dist: docker (>=6)
-Requires-Dist: fastapi (>=0.90)
+Requires-Dist: fastapi (>=0.80)
 Requires-Dist: jinja2 (>=3.1)
 Requires-Dist: langchain (>=0.0.120)
 Requires-Dist: openai (>=0.27)
 Requires-Dist: pyyaml (>=6)
 Requires-Dist: schema (>=0.7)
 Requires-Dist: stringcase (>=1)
 Requires-Dist: uvicorn (>=0.20)
```

