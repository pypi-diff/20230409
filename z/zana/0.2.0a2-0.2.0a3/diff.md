# Comparing `tmp/zana-0.2.0a2.tar.gz` & `tmp/zana-0.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zana-0.2.0a2.tar", max compression
+gzip compressed data, was "zana-0.2.0a3.tar", max compression
```

## Comparing `zana-0.2.0a2.tar` & `zana-0.2.0a3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1067 2023-03-29 23:12:55.268359 zana-0.2.0a2/LICENSE.txt
--rw-r--r--   0        0        0     1261 2023-03-29 23:13:12.913374 zana-0.2.0a2/README.md
--rw-r--r--   0        0        0     2533 2023-03-29 23:12:55.272359 zana-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/__init__.pyi
--rw-r--r--   0        0        0      949 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/canvas/__init__.py
--rw-r--r--   0        0        0     1126 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/canvas/__init__.pyi
--rw-r--r--   0        0        0    20988 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/canvas/core.py
--rw-r--r--   0        0        0    12892 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/canvas/operator.py
--rw-r--r--   0        0        0    12100 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/canvas/proxy.py
--rw-r--r--   0        0        0        0 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/canvas/py.typed
--rw-r--r--   0        0        0    13646 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/proxy/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/testing/__init__.py
--rw-r--r--   0        0        0      344 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/testing/mock.py
--rw-r--r--   0        0        0     7728 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/types/__init__.py
--rw-r--r--   0        0        0    11980 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/types/collections.py
--rw-r--r--   0        0        0     4123 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/types/enums.py
--rw-r--r--   0        0        0     9045 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/types/mypy_plugin.py
--rw-r--r--   0        0        0        0 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/types/py.typed
--rw-r--r--   0        0        0     7984 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/util/__init__.py
--rw-r--r--   0        0        0    12131 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/util/operator.py
--rw-r--r--   0        0        0      235 2023-03-29 23:12:55.272359 zana-0.2.0a2/zana/zana/__init__.py
--rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 zana-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-09 18:44:38.853773 zana-0.2.0a3/LICENSE.txt
+-rw-r--r--   0        0        0     1261 2023-04-09 18:44:58.737624 zana-0.2.0a3/README.md
+-rw-r--r--   0        0        0     2533 2023-04-09 18:44:38.853773 zana-0.2.0a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/__init__.pyi
+-rw-r--r--   0        0        0      949 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/__init__.py
+-rw-r--r--   0        0        0     1126 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/__init__.pyi
+-rw-r--r--   0        0        0    20972 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/core.py
+-rw-r--r--   0        0        0    12892 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/operator.py
+-rw-r--r--   0        0        0    12100 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/proxy.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/canvas/py.typed
+-rw-r--r--   0        0        0    13646 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/proxy/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/testing/__init__.py
+-rw-r--r--   0        0        0      344 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/testing/mock.py
+-rw-r--r--   0        0        0     7892 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/types/__init__.py
+-rw-r--r--   0        0        0    11980 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/types/collections.py
+-rw-r--r--   0        0        0     4123 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/types/enums.py
+-rw-r--r--   0        0        0     9045 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/types/mypy_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/types/py.typed
+-rw-r--r--   0        0        0     7984 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/util/__init__.py
+-rw-r--r--   0        0        0    12131 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/util/operator.py
+-rw-r--r--   0        0        0      235 2023-04-09 18:44:38.857773 zana-0.2.0a3/zana/zana/__init__.py
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 zana-0.2.0a3/PKG-INFO
```

### Comparing `zana-0.2.0a2/LICENSE.txt` & `zana-0.2.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/README.md` & `zana-0.2.0a3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 [pyversions-link]: https://pypi.python.org/pypi/zana
 [ci-image]: https://github.com/python-zana/zana/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main
 [ci-link]: https://github.com/python-zana/zana/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amain
 [codecov-image]: https://codecov.io/gh/python-zana/zana/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/python-zana/zana
 
 
-See this release on GitHub: [v0.2.0a2](https://github.com/python-zana/zana/releases/tag/0.2.0a2)
+See this release on GitHub: [v0.2.0a3](https://github.com/python-zana/zana/releases/tag/0.2.0a3)
```

### Comparing `zana-0.2.0a2/pyproject.toml` & `zana-0.2.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zana"
-version = "0.2.0a2"
+version = "0.2.0a3"
 description = "general utility functions and types"
 authors = ["David Kyalo <davidmkyalo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/python-zana/zana"
 documentation = "https://python-zana.github.io/zana"
 classifiers = [
```

### Comparing `zana-0.2.0a2/zana/canvas/__init__.py` & `zana-0.2.0a3/zana/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/zana/canvas/__init__.pyi` & `zana-0.2.0a3/zana/canvas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/zana/canvas/core.py` & `zana-0.2.0a3/zana/canvas/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,23 +674,21 @@
                     name = "__zana_composer_call__"
                 setattr(cls, name, method)
 
 
 class magic(Composer[_T_Co]):
     __slots__ = ()
 
-    def forbid(nm):
+    def forbid(nm):  # type: ignore
         def meth(self, *a, **kw) -> None:  # pragma: no cover
             raise TypeError(f"none trappable operation {nm!r}")
 
         meth.__name__ = meth.__qualname__ = nm
         return meth
 
     for nm in ("__setattr__", "__delattr__", "__setitem__", "__delitem__"):
         vars()[nm] = forbid(nm)
 
     del forbid, nm
 
 
 this = _THIS = magic[_T_Co]()
-
-from .operator import registry
```

### Comparing `zana-0.2.0a2/zana/canvas/operator.py` & `zana-0.2.0a3/zana/canvas/operator.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/zana/canvas/proxy.py` & `zana-0.2.0a3/zana/canvas/proxy.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/zana/proxy/__init__.py` & `zana-0.2.0a3/zana/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/zana/types/__init__.py` & `zana-0.2.0a3/zana/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,34 +132,38 @@
                     parents, forbidden, check, members = (
                         f_parents(),
                         f_forbidden(),
                         f_check(),
                         f_members(),
                     )
                     names = self.__abstractmethods__ if members is None else members
-                    msg = (
-                        f"issubclass({sub.__name__},  {cls.__name__}) {parents = }, {forbidden = }\n -->"
-                        f""
-                        f"{predicate.__name__}({sub.__name__}, {[*names]}, {check}) is "
-                        f"{expected} = {predicate(sub, names, check) is expected}\n"
-                    )
-                    logger.error(msg)
+
+                    # msg = (
+                    #     f"issubclass({sub.__name__},  {cls.__name__}) {parents = }, {forbidden = }\n -->"
+                    #     f""
+                    #     f"{predicate.__name__}({sub.__name__}, {[*names]}, {check}) is "
+                    #     f"{expected} = {predicate(sub, names, check) is expected}\n"
+                    # )
+                    # logger.error(msg)
 
                     if all(issubclass(sub, p) for p in parents):
                         if not (forbidden and issubclass(sub, forbidden)):
                             if predicate(sub, names, check) is expected:
                                 return True
                 return NotImplemented
 
             cls.__subclasshook__ = __subclasshook__
 
             def __new__(cls: type[Self], *args, **kwargs) -> Self:
                 raise TypeError(f"interfaces cannot be instantiated. {cls} called.")
 
             cls.__init__ = cls.__new__ = __new__
+            logger.error(
+                f"{cls.__name__!r} subclasses '{__name__}.Interface' which is not tested. USE AT YOUR RISK!"
+            )
 
 
 class Descriptor(Interface, t.Generic[_T, _RT], total=False):
     __slots__ = ()
 
     @classmethod
     def __subclasshook__(self, sub: type[Self]):
```

### Comparing `zana-0.2.0a2/zana/types/collections.py` & `zana-0.2.0a3/zana/types/collections.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/zana/types/enums.py` & `zana-0.2.0a3/zana/types/enums.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/zana/types/mypy_plugin.py` & `zana-0.2.0a3/zana/types/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/zana/util/__init__.py` & `zana-0.2.0a3/zana/util/__init__.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/zana/util/operator.py` & `zana-0.2.0a3/zana/util/operator.py`

 * *Files identical despite different names*

### Comparing `zana-0.2.0a2/PKG-INFO` & `zana-0.2.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zana
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: general utility functions and types
 Home-page: https://github.com/python-zana/zana
 License: MIT
 Keywords: zana,toolkit
 Author: David Kyalo
 Author-email: davidmkyalo@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -61,9 +61,9 @@
 [pyversions-link]: https://pypi.python.org/pypi/zana
 [ci-image]: https://github.com/python-zana/zana/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main
 [ci-link]: https://github.com/python-zana/zana/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amain
 [codecov-image]: https://codecov.io/gh/python-zana/zana/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/python-zana/zana
 
 
-See this release on GitHub: [v0.2.0a2](https://github.com/python-zana/zana/releases/tag/0.2.0a2)
+See this release on GitHub: [v0.2.0a3](https://github.com/python-zana/zana/releases/tag/0.2.0a3)
```

