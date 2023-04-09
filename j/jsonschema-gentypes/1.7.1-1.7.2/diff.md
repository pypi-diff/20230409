# Comparing `tmp/jsonschema_gentypes-1.7.1.tar.gz` & `tmp/jsonschema_gentypes-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_gentypes-1.7.1.tar", max compression
+gzip compressed data, was "jsonschema_gentypes-1.7.2.tar", max compression
```

## Comparing `jsonschema_gentypes-1.7.1.tar` & `jsonschema_gentypes-1.7.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1304 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/LICENSE
--rw-r--r--   0        0        0     3554 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/README.md
--rw-r--r--   0        0        0    39080 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/jsonschema_gentypes/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/jsonschema_gentypes/cli.py
--rw-r--r--   0        0        0     2429 2023-04-07 20:27:45.723875 jsonschema_gentypes-1.7.1/jsonschema_gentypes/configuration.py
--rw-r--r--   0        0        0     5956 2023-04-07 20:27:45.971897 jsonschema_gentypes-1.7.1/jsonschema_gentypes/jsonschema.py
--rw-r--r--   0        0        0        0 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/jsonschema_gentypes/py.typed
--rw-r--r--   0        0        0     2842 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/jsonschema_gentypes/schema.json
--rw-r--r--   0        0        0     5413 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/jsonschema_gentypes/validate.py
--rw-r--r--   0        0        0     2500 2023-04-07 20:27:51.956477 jsonschema_gentypes-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     5051 1970-01-01 00:00:00.000000 jsonschema_gentypes-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1304 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/LICENSE
+-rw-r--r--   0        0        0     3554 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/README.md
+-rw-r--r--   0        0        0    41603 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/jsonschema_gentypes/__init__.py
+-rw-r--r--   0        0        0     7376 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/jsonschema_gentypes/cli.py
+-rw-r--r--   0        0        0     2429 2023-04-09 06:57:21.171635 jsonschema_gentypes-1.7.2/jsonschema_gentypes/configuration.py
+-rw-r--r--   0        0        0     5125 2023-04-09 06:57:21.575640 jsonschema_gentypes-1.7.2/jsonschema_gentypes/jsonschema.py
+-rw-r--r--   0        0        0        0 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/jsonschema_gentypes/py.typed
+-rw-r--r--   0        0        0     2842 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/jsonschema_gentypes/schema.json
+-rw-r--r--   0        0        0     5413 2023-04-09 06:54:25.625692 jsonschema_gentypes-1.7.2/jsonschema_gentypes/validate.py
+-rw-r--r--   0        0        0     2500 2023-04-09 06:57:27.759710 jsonschema_gentypes-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     5051 1970-01-01 00:00:00.000000 jsonschema_gentypes-1.7.2/PKG-INFO
```

### Comparing `jsonschema_gentypes-1.7.1/LICENSE` & `jsonschema_gentypes-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.1/README.md` & `jsonschema_gentypes-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.1/jsonschema_gentypes/__init__.py` & `jsonschema_gentypes-1.7.2/jsonschema_gentypes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,14 +182,77 @@
     def set_comments(self, comments: List[str]) -> None:
         """
         Set comment on the type.
         """
         self._comments = comments
 
 
+class TypeProxy(Type):
+    """
+    A proxy on a type that can be set later.
+    """
+
+    _type: Optional[Type] = None
+
+    def name(self) -> str:
+        """
+        Return what we need to use the type.
+        """
+        assert self._type is not None
+        return self._type.name()
+
+    def imports(self, python_version: Tuple[int, ...]) -> List[Tuple[str, str]]:
+        """
+        Return the needed imports.
+        """
+        assert self._type is not None
+        return self._type.imports(python_version)
+
+    def definition(self, line_length: Optional[int] = None) -> List[str]:
+        """
+        Return the type declaration.
+
+        Arguments:
+            line_length: the maximum line length
+        """
+        assert self._type is not None
+        return self._type.definition()
+
+    def depends_on(self) -> List["Type"]:
+        """
+        Return the needed sub types.
+        """
+        assert self._type is not None
+        return self._type.depends_on()
+
+    def add_depends_on(self, depends_on: "Type") -> None:
+        """
+        Add a sub type.
+        """
+        raise NotImplementedError
+
+    def comments(self) -> List[str]:
+        """
+        Additional comments shared by the type.
+        """
+        return self._type.comments() if self._type is not None else []
+
+    def set_comments(self, comments: List[str]) -> None:
+        """
+        Set comment on the type.
+        """
+        print(f"Warning: set_comments on a TypeProxy, lost comments: {comments}")
+
+    def set_type(self, type_: Type) -> None:
+        """
+        Set the type.
+        """
+        self._type = type_
+
+
 class NamedType(Type):
     """
     The based type of named type.
     """
 
     def __init__(self, name: str) -> None:
         """
@@ -337,15 +400,14 @@
         Arguments:
             base: the base type (e.-g. for `Union[str, int]` the base type is `Union`)
             sub_types: the sub types (e.-g. for `Union[str]` the sub types are `str` and `int`)
         """
         super().__init__()
         self.base = base
         self.sub_types = sub_types
-        self.name()
 
     def name(self) -> str:
         """
         Return what we need to use the type.
         """
         assert isinstance(self.base, Type)
         return f"{self.base.name()}[{', '.join([sub_type.name() for sub_type in self.sub_types])}]"
@@ -717,22 +779,16 @@
         """
         Initialize with a resolver.
         """
         self.resolver = resolver
         self.additional_properties = additional_properties
         # types by reference
         self.ref_type: Dict[str, Type] = {}
-        self.base_name = "Base"
-        self.recursive_anchor_path: List[str] = []
-
-    def set_base_name(self, name: str) -> None:
-        """
-        Set the name of the base element.
-        """
-        self.base_name = name
+        self.recursive_anchor_path: List[Type] = []
+        self.root: Optional[TypeProxy] = None
 
     def get_type_handler(self, schema_type: str) -> Callable[[jsonschema.JSONSchemaItem, str], Type]:
         """
         Get a handler from this schema draft version.
         """
         if schema_type.startswith("_"):
             raise AttributeError("No way friend")
@@ -740,31 +796,38 @@
         if handler is None:
             raise NotImplementedError(
                 f"Type `{schema_type}` is not supported. If you think that this is an error, "
                 f"say something at {ISSUE_URL}"
             )
         return handler
 
-    def get_type(
-        self, schema: jsonschema.JSONSchema, proposed_name: Optional[str] = None, auto_alias: bool = True
-    ) -> Type:
+    def get_type(self, schema: jsonschema.JSONSchema, proposed_name: str, auto_alias: bool = True) -> Type:
         """
         Get a :class:`.Type` for a JSON schema.
         """
+        root = self.root is None
+        if root:
+            self.root = TypeProxy()
         if schema is True:
-            return NativeType("Any")
+            type_ = NativeType("Any")
+            if root:
+                assert self.root is not None
+                self.root.set_type(type_)
+            return type_
         if schema is False:
-            return BuiltinType("None")
+            type_ = NativeType("None")
+            if root:
+                assert self.root is not None
+                self.root.set_type(type_)
+            return type_
         assert not isinstance(schema, bool)
 
-        if proposed_name is None:
-            proposed_name = self.base_name
-
+        proxy = TypeProxy()
         if schema.get("$recursiveAnchor", False):
-            self.recursive_anchor_path.append(get_name(schema, proposed_name))
+            self.recursive_anchor_path.append(proxy)
 
         the_type = self._get_type_internal(schema, proposed_name)
         assert the_type is not None
         additional_description = the_type.comments()
         description = get_description(schema)
         if description and additional_description:
             description.append("")
@@ -780,14 +843,19 @@
                 Constant(
                     f"{get_name(schema, proposed_name, True)}_DEFAULT",
                     schema["default"],
                     [f"Default value of the field path '{proposed_name}'"],
                 )
             )
 
+        proxy.set_type(the_type)
+        if root:
+            assert self.root is not None
+            self.root.set_type(the_type)
+
         if schema.get("$recursiveAnchor", False):
             self.recursive_anchor_path.pop()
 
         return the_type
 
     def _resolve_ref(self, schema: jsonschema.JSONSchemaItem) -> jsonschema.JSONSchemaItem:
         if "$ref" in schema:
@@ -1062,15 +1130,18 @@
         """
         items = schema.get("items")
         if items is True:
             return CombinedType(NativeType("List"), [NativeType("Any")])
         elif items is False:
             raise NotImplementedError('"items": false is not supported')
         elif isinstance(items, list):
-            inner_types = [self.get_type(cast(jsonschema.JSONSchemaItem, item)) for item in items]
+            inner_types = [
+                self.get_type(cast(jsonschema.JSONSchemaItem, item), f"{proposed_name} {nb}")
+                for nb, item in enumerate(items)
+            ]
             type_: Type = CombinedType(NativeType("Tuple"), inner_types)
             if {schema.get("minItems"), schema.get("maxItems")} - {None, len(items)}:
                 type_.set_comments(
                     [
                         "WARNING: 'items': If list, must have minItems == maxItems.",
                         "See: https://json-schema.org/understanding-json-schema/"
                         "reference/array.html#tuple-validation",
@@ -1111,15 +1182,16 @@
 
     def ref(self, schema: jsonschema.JSONSchemaItem, proposed_name: str) -> Type:
         """
         Handle a `$ref`.
         """
 
         if schema.get("$recursiveRef") == "#":
-            return NamedType(self.recursive_anchor_path[-1])
+            del schema["$recursiveRef"]  # type: ignore
+            return self.recursive_anchor_path[-1]
 
         ref = schema["$ref"]
         del schema["$ref"]
 
         if ref == "#":  # Self ref.
             # Per @ilevkivskyi:
             #
@@ -1128,30 +1200,42 @@
             # > Support for recursive types is limited to proper classes
             # > currently
             #
             # forward_ref = ForwardRef(UnboundType(self.outer_name))
             # self.forward_refs.append(forward_ref)
             # return forward_ref
 
-            return NamedType(self.base_name)
+            assert self.root is not None
+            return self.root
 
         if ref in self.ref_type:
             return self.ref_type[ref]
 
+        ref_proposed_name = ref
+        if ref.startswith("#/definitions/"):
+            ref_proposed_name = ref[len("#/definitions/") :]
+        elif ref.startswith("#/"):
+            ref_proposed_name = ref[len("#/") :]
+        if "/" in ref_proposed_name:
+            ref_proposed_name = ref_proposed_name.replace("/", " ")
+        else:
+            if re.search("[a-z]", ref_proposed_name):
+                ref_proposed_name = re.sub("([a-z0-9])([A-Z])", r"\1 \2", ref_proposed_name).lower()
+
         resolve = getattr(self.resolver, "resolve", None)
         if resolve is None:
             with self.resolver.resolving(ref) as resolved:
                 schema.update(resolved)
-                type_ = self.get_type(schema)
+                type_ = self.get_type(schema, ref_proposed_name)
         else:
             scope, resolved = self.resolver.resolve(ref)
             self.resolver.push_scope(scope)
             try:
                 schema.update(resolved)
-                type_ = self.get_type(schema, proposed_name)
+                type_ = self.get_type(schema, ref_proposed_name)
             finally:
                 self.resolver.pop_scope()
 
         if ref:
             self.ref_type[ref] = type_
         return type_
```

### Comparing `jsonschema_gentypes-1.7.1/jsonschema_gentypes/cli.py` & `jsonschema_gentypes-1.7.2/jsonschema_gentypes/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,58 +7,64 @@
 import logging
 import os
 import pkgutil
 import random
 import re
 import subprocess  # nosec
 import sys
-from typing import Dict, Set, Tuple, cast
+from typing import Dict, Optional, Set, Tuple, cast
 
 import requests
 import ruamel.yaml
 from jsonschema import RefResolver
 
 import jsonschema_gentypes
-from jsonschema_gentypes import configuration, get_name, validate
+from jsonschema_gentypes import configuration, validate
 
 LOG = logging.getLogger(__name__)
 
 
 def _add_type(
     type_: jsonschema_gentypes.Type,
     imports: Dict[str, Set[str]],
     types: Dict[str, jsonschema_gentypes.Type],
     gen: configuration.GenerateItem,
     config: configuration.Configuration,
     minimal_python_version: Tuple[int, ...],
+    added_types: Optional[Set[jsonschema_gentypes.Type]] = None,
 ) -> None:
+    if added_types is None:
+        added_types = set()
+    if type_ in added_types:
+        return
+    added_types.add(type_)
     if (
         isinstance(type_, jsonschema_gentypes.NamedType)
         and type_.unescape_name() in types
         and type_.definition(config.get("lineLength"))
         == types[type_.unescape_name()].definition(config.get("lineLength"))
     ):
         return
     name_mapping = gen.get("name_mapping", {})
     assert name_mapping is not None
     if isinstance(type_, jsonschema_gentypes.NamedType) and type_.unescape_name() in name_mapping:
         type_.set_name(name_mapping[type_.unescape_name()])
     if isinstance(type_, jsonschema_gentypes.NamedType) and type_.unescape_name() in types:
         print(f"WARNING: the type {type_.unescape_name()} is already defined, it will be renamed")
         type_.postfix_name(f"Gen{random.randrange(999999)}")  # nosec
-        _add_type(type_, imports, types, gen, config, minimal_python_version)
+        _add_type(type_, imports, types, gen, config, minimal_python_version, added_types)
     else:
         if isinstance(type_, jsonschema_gentypes.NamedType):
             types[type_.unescape_name()] = type_
         for package, imp in type_.imports(minimal_python_version):
             if package not in imports:
                 imports[package] = set()
             imports[package].add(imp)
         for sub_type in type_.depends_on():
-            _add_type(sub_type, imports, types, gen, config, minimal_python_version)
+            _add_type(sub_type, imports, types, gen, config, minimal_python_version, added_types)
 
 
 def main() -> None:
     """
     Generate the Python type files from the JSON schema files.
     """
     parser = argparse.ArgumentParser(usage="Generate the Python type files from the JSON schema files")
@@ -110,14 +116,15 @@
     if str_python_version is not None:
         python_version = tuple(int(x) for x in str_python_version.split("."))
     else:
         python_version = sys.version_info[:3]
 
     for gen in config["generate"]:
         source = gen["source"]
+        print(f"Processing {source}")
         if source.startswith("http://") or source.startswith("https://"):
             response = requests.get(source, timeout=60)
             response.raise_for_status()
             schema = response.json()
         else:
             with open(os.path.abspath(source), encoding="utf-8") as source_file:
                 schema = json.load(source_file)
@@ -136,15 +143,14 @@
         api_args = gen.get("api_arguments", {})
         api = api_version(resolver, **api_args)
 
         types: Dict[str, jsonschema_gentypes.Type] = {}
         imports: Dict[str, Set[str]] = {}
 
         root_name = gen.get("root_name", "Root")
-        api.set_base_name(get_name(schema, root_name))
         base_type = api.get_type(schema, root_name)
         if "root_name" in gen and isinstance(base_type, jsonschema_gentypes.NamedType):
             assert gen["root_name"] is not None
             base_type.set_name(gen["root_name"])
 
         _add_type(base_type, imports, types, gen, config, python_version)
```

### Comparing `jsonschema_gentypes-1.7.1/jsonschema_gentypes/configuration.py` & `jsonschema_gentypes-1.7.2/jsonschema_gentypes/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Automatically generated file from a JSON schema.
 """
 
 
-from typing import List, Any, TypedDict, Union, Dict, Literal
+from typing import Union, Any, TypedDict, Dict, List, Literal
 from typing_extensions import Required
 
 
 AdditionalProperties = Union[Literal["Always"], Literal["Only explicit"]]
 """
 Additional properties.
```

### Comparing `jsonschema_gentypes-1.7.1/jsonschema_gentypes/schema.json` & `jsonschema_gentypes-1.7.2/jsonschema_gentypes/schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.1/jsonschema_gentypes/validate.py` & `jsonschema_gentypes-1.7.2/jsonschema_gentypes/validate.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.1/pyproject.toml` & `jsonschema_gentypes-1.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 ignore_missing_imports = true
 strict = true
 
 [tool.poetry]
 name = "jsonschema-gentypes"
-version = "1.7.1"
+version = "1.7.2"
 description = "Tool to generate Python types based on TypedDict from a JSON Schema"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 repository = "https://github.com/camptocamp/jsonschema-gentypes"
 license = "BSD-2-Clause"
 keywords = ["jsonschema", "types"]
 packages = [{ include = "jsonschema_gentypes" }]
```

### Comparing `jsonschema_gentypes-1.7.1/PKG-INFO` & `jsonschema_gentypes-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-gentypes
-Version: 1.7.1
+Version: 1.7.2
 Summary: Tool to generate Python types based on TypedDict from a JSON Schema
 Home-page: https://github.com/camptocamp/jsonschema-gentypes
 License: BSD-2-Clause
 Keywords: jsonschema,types
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4
```

