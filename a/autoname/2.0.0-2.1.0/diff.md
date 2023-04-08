# Comparing `tmp/autoname-2.0.0.tar.gz` & `tmp/autoname-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoname-2.0.0.tar", max compression
+gzip compressed data, was "autoname-2.1.0.tar", max compression
```

## Comparing `autoname-2.0.0.tar` & `autoname-2.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3192 2021-06-14 10:20:40.624251 autoname-2.0.0/autoname/__init__.py
--rw-r--r--   0        0        0      757 2021-06-12 15:00:35.753842 autoname-2.0.0/LICENSE.md
--rw-r--r--   0        0        0      495 2021-06-14 10:32:36.925515 autoname-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1502 2021-06-14 10:31:58.436113 autoname-2.0.0/README.md
--rw-r--r--   0        0        0     2189 2021-06-14 10:32:45.697984 autoname-2.0.0/setup.py
--rw-r--r--   0        0        0     2181 2021-06-14 10:32:45.697984 autoname-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3458 2023-04-08 03:57:47.553537 autoname-2.1.0/autoname/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-08 03:23:34.490334 autoname-2.1.0/autoname/py.typed
+-rw-r--r--   0        0        0      771 2023-04-08 02:50:41.636905 autoname-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0      713 2023-04-08 05:00:12.963491 autoname-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1583 2023-04-08 02:50:41.637907 autoname-2.1.0/README.md
+-rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 autoname-2.1.0/PKG-INFO
```

### Comparing `autoname-2.0.0/autoname/__init__.py` & `autoname-2.1.0/autoname/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,112 @@
-__all__ = ['AutoName', 'StrEnum', "AutoNameLower", "AutoNameUpper", "LowerStrEnum", "UpperStrEnum", "AutoNameSnake2Camel", 'snake2camel', 'transform', 'make_strEnum', ]
-
-import inspect
-import re
-import uuid
-from enum import Enum, auto
-from typing import Type, Callable
-
-
-class AutoName(str, Enum):
-    """
-    an enum `AutoName` from [python docs](https://docs.python.org/3/library/enum.html#using-automatic-values) with multiple stringcase options.
-    """
-    def _generate_next_value_(name, start, count, last_values):
-        return name
-
-StrEnum = AutoName
-
-class AutoNameLower(AutoName):
-    def _generate_next_value_(name, start, count, last_values):
-        return str.lower(name)
-
-LowerStrEnum = AutoNameLower
-
-class AutoNameUpper(AutoName):
-    def _generate_next_value_(name, start, count, last_values):
-        return str.upper(name)
-
-UpperStrEnum = AutoNameUpper
-
-# From https://github.com/dmontagu/fastapi-utils/blob/af95ff4a8195caaa9edaa3dbd5b6eeb09691d9c7/fastapi_utils/camelcase.py#L4
-def snake2camel(snake: str, start_lower: bool = False) -> str:
-    """
-    Converts a snake_case string to camelCase.
-    The `start_lower` argument determines whether the first letter in the generated camelcase should
-    be lowercase (if `start_lower` is True), or capitalized (if `start_lower` is False).
-    """
-    camel = snake.title()
-    camel = re.sub("([0-9A-Za-z])_(?=[0-9A-Z])", lambda m: m.group(1), camel)
-    if start_lower:
-        camel = re.sub("(^_*[A-Z])", lambda m: m.group(1).lower(), camel)
-    return camel
-
-class AutoNameSnake2Camel(AutoName):
-    """
-    CamelStrEnum subclasses that create variants using `auto()` will have values equal to their camelCase names
-    """
-    def _generate_next_value_(name, start, count, last_values):
-        return snake2camel(name, start_lower=True)
-
-
-
-def transform(_class: Type[AutoName]=None, *, function: Callable[[str], str]=None):
-    if function is None:
-        raise ValueError(f"transform require `transform` function, pass it as a keyword argument.")
-
-    def autoname_customized(class_: Type[AutoName]):
-        function # this line makes the variable available at locals()
-        class_name = class_.__name__
-        unique_suffix = uuid.uuid4().hex
-        root_class = f"AutoName_Customized_{unique_suffix}"
-        transform_function_variableName = f"transform_{unique_suffix}"
-
-        part1 = f"""global {class_name}, {root_class}, {transform_function_variableName}
-                    {transform_function_variableName} = function
-
-                    class {root_class}(AutoName):
-                        def _generate_next_value_(name, start, count, last_values):
-                            return {transform_function_variableName}(name)
-
-                    class {class_name}({root_class}):
-
-                    """
-        part1 = inspect.cleandoc(part1)
-        part2_classMembers = "".join([f"\t{v} = auto()\n" for v, obj in class_._member_map_.items()])
-        exec(
-            part1 + '\n' + part2_classMembers
-        )
-        return eval(class_name)
-
-    if _class is None:
-        return autoname_customized
-    else:
-        raise NotImplementedError("`_class` arg should not be specified.")
+__all__ = [
+    "AutoName",
+    "StrEnum",
+    "AutoNameLower",
+    "AutoNameUpper",
+    "LowerStrEnum",
+    "UpperStrEnum",
+    "AutoNameSnake2Camel",
+    "snake2camel",
+    "transform",
+    "make_strEnum",
+]
+
+import inspect
+import re
+import uuid
+
+# auto is required for the `exec` call
+from enum import Enum, auto  # noqa
+from typing import Optional, Type, Callable
+
+
+class AutoName(str, Enum):
+    """
+    an enum `AutoName` from [python docs](https://docs.python.org/3/library/enum.html#using-automatic-values)
+    with multiple stringcase options.
+    """
+
+    def _generate_next_value_(name, start, count, last_values):
+        return name
+
+
+StrEnum = AutoName
+
+
+class AutoNameLower(AutoName):
+    def _generate_next_value_(name, start, count, last_values):
+        return str.lower(name)
+
+
+LowerStrEnum = AutoNameLower
+
+
+class AutoNameUpper(AutoName):
+    def _generate_next_value_(name, start, count, last_values):
+        return str.upper(name)
+
+
+UpperStrEnum = AutoNameUpper
+
+
+# From https://github.com/dmontagu/fastapi-utils/blob/af95ff4a8195caaa9edaa3dbd5b6eeb09691d9c7/fastapi_utils/camelcase.py#L4
+def snake2camel(snake: str, start_lower: bool = False) -> str:
+    """
+    Converts a snake_case string to camelCase.
+    The `start_lower` argument determines whether the first letter in
+    the generated camelcase should be lowercase (if `start_lower` is True),
+    or capitalized (if `start_lower` is False).
+    """
+    camel = snake.title()
+    camel = re.sub("([0-9A-Za-z])_(?=[0-9A-Z])", lambda m: m.group(1), camel)
+    if start_lower:
+        camel = re.sub("(^_*[A-Z])", lambda m: m.group(1).lower(), camel)
+    return camel
+
+
+class AutoNameSnake2Camel(AutoName):
+    """
+    CamelStrEnum subclasses that create variants using `auto()`
+    will have values equal to their camelCase names
+    """
+
+    def _generate_next_value_(name, start, count, last_values):
+        return snake2camel(name, start_lower=True)
+
+
+def transform(
+    _class: Optional[Type[AutoName]] = None, *, function: Callable[[str], str]
+):
+    if function is None:
+        raise ValueError(
+            "transform require `transform` function, pass it as a keyword argument."
+        )
+
+    def autoname_customized(class_: Type[AutoName]):
+        function  # this line makes the variable available at locals()
+        class_name = class_.__name__
+        unique_suffix = uuid.uuid4().hex
+        root_class = f"AutoName_Customized_{unique_suffix}"
+        transform_function_variableName = f"transform_{unique_suffix}"
+
+        part1 = f"""global {class_name}, {root_class}, {transform_function_variableName}
+                    {transform_function_variableName} = function
+
+                    class {root_class}(AutoName):
+                        def _generate_next_value_(name, start, count, last_values):
+                            return {transform_function_variableName}(name)
+
+                    class {class_name}({root_class}):
+
+                    """
+        part1 = inspect.cleandoc(part1)
+        part2_classMembers = "".join(
+            [f"\t{v} = auto()\n" for v, obj in class_._member_map_.items()]
+        )
+        exec(part1 + "\n" + part2_classMembers)
+        return eval(class_name)
+
+    if _class is None:
+        return autoname_customized
+    else:
+        raise NotImplementedError("`_class` arg should not be specified.")
```

### Comparing `autoname-2.0.0/LICENSE.md` & `autoname-2.1.0/LICENSE.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-
-Copyright (c) 2020, Nutchanon Ninyawee <me@nutchanon.org>
-
-Permission to use, copy, modify, and/or distribute this software for any
-purpose with or without fee is hereby granted, provided that the above
-copyright notice and this permission notice appear in all copies.
-
-THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
-WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
-MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
-ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
-WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
-ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
-OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+
+Copyright (c) 2020, Nutchanon Ninyawee <me@nutchanon.org>
+
+Permission to use, copy, modify, and/or distribute this software for any
+purpose with or without fee is hereby granted, provided that the above
+copyright notice and this permission notice appear in all copies.
+
+THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
+WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
+MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
+ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
+WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
+ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
+OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
```

### Comparing `autoname-2.0.0/PKG-INFO` & `autoname-2.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: autoname
-Version: 2.0.0
+Version: 2.1.0
 Summary: an enum `AutoName` from python docs with multiple stringcase options
-Home-page: https://github.com/CircleOnCircles/autoname
+Home-page: https://github.com/wasdee/autoname
 License: ISC
 Author: Nutchanon Ninyawee
 Author-email: me@nutchanon.org
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Project-URL: Repository, https://github.com/CircleOnCircles/autoname
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/wasdee/autoname
 Description-Content-Type: text/markdown
 
 
 # autoname
 
 an enum `AutoName` from [python docs](https://docs.python.org/3/library/enum.html#using-automatic-values) with multiple stringcase options.
```

