# Comparing `tmp/stlog-0.0.4.tar.gz` & `tmp/stlog-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlog-0.0.4.tar", max compression
+gzip compressed data, was "stlog-0.0.5.tar", max compression
```

## Comparing `stlog-0.0.4.tar` & `stlog-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-04-08 18:39:13.873915 stlog-0.0.4/LICENSE
--rw-r--r--   0        0        0     7675 2023-04-08 18:39:13.873915 stlog-0.0.4/README.md
--rw-r--r--   0        0        0     1240 2023-04-08 18:39:47.334145 stlog-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      318 2023-04-08 18:39:46.942142 stlog-0.0.4/stlog/__init__.py
--rw-r--r--   0        0        0      319 2023-04-08 18:39:46.942142 stlog-0.0.4/stlog/__init__.py.restore_version
--rw-r--r--   0        0        0     2508 2023-04-08 18:39:13.877915 stlog-0.0.4/stlog/adapter.py
--rw-r--r--   0        0        0     6957 2023-04-08 18:39:13.877915 stlog-0.0.4/stlog/base.py
--rw-r--r--   0        0        0     2647 2023-04-08 18:39:13.877915 stlog-0.0.4/stlog/context.py
--rw-r--r--   0        0        0    12835 2023-04-08 18:39:13.877915 stlog-0.0.4/stlog/formatter.py
--rw-r--r--   0        0        0     2526 2023-04-08 18:39:13.877915 stlog-0.0.4/stlog/handler.py
--rw-r--r--   0        0        0     4580 2023-04-08 18:39:13.877915 stlog-0.0.4/stlog/output.py
--rw-r--r--   0        0        0     4651 2023-04-08 18:39:13.877915 stlog-0.0.4/stlog/setup.py
--rw-r--r--   0        0        0     8227 1970-01-01 00:00:00.000000 stlog-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-09 08:00:18.688375 stlog-0.0.5/LICENSE
+-rw-r--r--   0        0        0     8010 2023-04-09 08:00:18.688375 stlog-0.0.5/README.md
+-rw-r--r--   0        0        0     1240 2023-04-09 08:00:58.407341 stlog-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-09 08:00:57.979309 stlog-0.0.5/stlog/__init__.py
+-rw-r--r--   0        0        0      301 2023-04-09 08:00:57.979309 stlog-0.0.5/stlog/__init__.py.restore_version
+-rw-r--r--   0        0        0     2463 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/adapter.py
+-rw-r--r--   0        0        0     7277 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/base.py
+-rw-r--r--   0        0        0     2638 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/context.py
+-rw-r--r--   0        0        0    12835 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/formatter.py
+-rw-r--r--   0        0        0     2499 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/handler.py
+-rw-r--r--   0        0        0     4580 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/output.py
+-rw-r--r--   0        0        0     4793 2023-04-09 08:00:18.692375 stlog-0.0.5/stlog/setup.py
+-rw-r--r--   0        0        0     8562 1970-01-01 00:00:00.000000 stlog-0.0.5/PKG-INFO
```

### Comparing `stlog-0.0.4/LICENSE` & `stlog-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stlog-0.0.4/README.md` & `stlog-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 
 <!-- WARNING: generated from README.md.j2, do not modify this file manually but modify README.md.j2 instead
      and execute 'poetry run poe readme' to regenerate this README.md file -->
 
 # stlog
 
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fabien-marty/stlog/lint.yaml)](https://github.com/fabien-marty/stlog/actions/workflows/lint.yaml)
+[![Codecov](https://img.shields.io/codecov/c/github/fabien-marty/stlog)](https://app.codecov.io/github/fabien-marty/stlog)
+[![pypi badge](https://img.shields.io/pypi/v/stlog?color=brightgreen)](https://pypi.org/project/stlog/)
+
 [Full documentation](https://fabien-marty.github.io/stlog/)
 
 <!--intro-start-->
 
 ## What is it?
 
 **ST**andard **ST**ructured **LOG** (`stlog`) is Python 3.7+ [structured logging](#structured) library:
@@ -94,28 +98,28 @@
 
 ![rich output](docs/python/qs1.svg)
  
 
 ### Usage with context
 
 ```python
-from stlog import ExecutionLogContext, getLogger, setup
+from stlog import LogContext, getLogger, setup
 
 # Set the logging default configuration (human output on stderr)
 setup()
 
 # ...
 
 # Set the (kind of) global execution context
 # (thread, worker, async friendly: one context by execution)
 # (for example in a wsgi/asgi middleware)
 # Note: ExecutionContext is a static class, so a kind of global singleton
-ExecutionLogContext.reset_context()
-ExecutionLogContext.add(request_id="4c2383f5")
-ExecutionLogContext.add(client_id=456, http_method="GET")
+LogContext.reset_context()
+LogContext.add(request_id="4c2383f5")
+LogContext.add(client_id=456, http_method="GET")
 
 # ... in another file/class/...
 
 # Get a logger
 logger = getLogger(__name__)
 logger.info("It works", foo="bar", x=123)
 logger.critical("Houston, we have a problem!")
@@ -135,32 +139,32 @@
 ![rich output](docs/python/qs2.svg)
  
 
 What about if you want to get a more parsing friendly output (for example in JSON on `stdout`) while keeping the human output on `stderr` (without any context)?
 
 ```python
 import sys
-from stlog import ExecutionLogContext, getLogger, setup
+from stlog import LogContext, getLogger, setup
 from stlog.output import StreamOutput
 from stlog.formatter import HumanFormatter, JsonFormatter
 
 setup(
     outputs=[
         StreamOutput(
             stream=sys.stderr,
             formatter=HumanFormatter(exclude_extras_keys_fnmatchs=["*"]),
         ),
         StreamOutput(stream=sys.stdout, formatter=JsonFormatter(indent=4)),
     ]
 )
 
 # See previous example for details
-ExecutionLogContext.reset_context()
-ExecutionLogContext.add(request_id="4c2383f5")
-ExecutionLogContext.add(client_id=456, http_method="GET")
+LogContext.reset_context()
+LogContext.add(request_id="4c2383f5")
+LogContext.add(client_id=456, http_method="GET")
 logger = getLogger(__name__)
 logger.info("It works", foo="bar", x=123)
 logger.critical("Houston, we have a problem!")
  
 ```
 
 Human output (on `stderr`):
```

### Comparing `stlog-0.0.4/pyproject.toml` & `stlog-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stlog"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Fabien MARTY <fabien.marty@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "stlog"}]
 
 [tool.poetry.dependencies]
```

### Comparing `stlog-0.0.4/stlog/adapter.py` & `stlog-0.0.5/stlog/adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import collections
 import logging
 import typing
 
 from stlog.base import RESERVED_ATTRS, STLOG_EXTRA_KEY, check_json_types_or_raise
-from stlog.context import ExecutionLogContext
+from stlog.context import LogContext
 
 
 # ligthly adapted from https://github.com/Mergifyio/daiquiri/blob/main/daiquiri/__init__.py
 class _KeywordArgumentAdapter(logging.LoggerAdapter):
     """Logger adapter to add keyword arguments to log record's extra data.
 
     Keywords passed to the log call are added to the "extra"
@@ -37,27 +37,27 @@
             extra[name] = kwargs.pop(name)
         extra[STLOG_EXTRA_KEY] = set(extra.keys())
         kwargs["extra"] = extra
         return msg, kwargs
 
 
 class StLogLoggerAdapter(_KeywordArgumentAdapter):
-    """stlog `LoggerAdapter` with `stlog.ExecutionLogContext` support."""
+    """stlog `LoggerAdapter` with `stlog.LogContext` support."""
 
     def process(
         self, msg: typing.Any, kwargs: collections.abc.MutableMapping[str, typing.Any]
     ) -> tuple[typing.Any, collections.abc.MutableMapping[str, typing.Any]]:
-        new_kwargs = {**ExecutionLogContext._get(), **kwargs}
+        new_kwargs = {**LogContext._get(), **kwargs}
         return super().process(msg, new_kwargs)
 
 
 def getLogger(name: str | None = None, **kwargs) -> StLogLoggerAdapter:  # noqa: N802
-    """Return a standard logger (adapted for `stlog` and `stlog.ExecutionLogContext` support).
+    """Return a standard logger (adapted for `stlog` and `stlog.LogContext` support).
 
     You can pass some context key/values in `**kwargs` which will be specific to this logger.
 
-    If you want to set more globally available context, use `stlog.ExecutionLogContext` class.
+    If you want to set more globally available context, use `stlog.LogContext` class.
 
     Args:
         name: logger name.
     """
     return StLogLoggerAdapter(logging.getLogger(name), kwargs)
```

### Comparing `stlog-0.0.4/stlog/base.py` & `stlog-0.0.5/stlog/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     RICH_AVAILABLE = True
 except ImportError:
     pass
 
 
 TRUE_VALUES = ("1", "true", "yes")
+FALSE_VALUES = ("0", "false", "no")
 
 
 class StLogError(Exception):
     pass
 
 
 @dataclass
@@ -180,16 +181,26 @@
 
 def check_true(value: str | None, default: bool = False) -> bool:
     if value is None:
         return default
     return value.lower() in TRUE_VALUES
 
 
+def check_false(value: str | None, default: bool = False) -> bool:
+    if value is None:
+        return default
+    return value.lower() in FALSE_VALUES
+
+
 def check_env_true(env_var: str, default: bool = False) -> bool:
-    return check_true(os.environ.get("env_var", None), default)
+    return check_true(os.environ.get(env_var, None), default)
+
+
+def check_env_false(env_var: str, default: bool = False) -> bool:
+    return check_false(os.environ.get(env_var, None), default)
 
 
 def rich_dump_exception_on_console(
     console: Any,
     exc_type: type[BaseException],
     value: BaseException,
     tb: types.TracebackType | None,
```

### Comparing `stlog-0.0.4/stlog/context.py` & `stlog-0.0.5/stlog/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ENV_CONTEXT = get_env_context()
 _LOGGING_CONTEXT_VAR: ContextVar = ContextVar(
     "stlog_logging_context", default=ENV_CONTEXT
 )
 
 
-class ExecutionLogContext:
+class LogContext:
     """This is a static class which hosts some utility (static) methods around a "log context"
     (global but by execution (worker/thread/async) thanks to contextvars).
 
     All values are (deeply) copied to avoid any changes after adding them to the context.
     """
 
     def __new__(cls):
```

### Comparing `stlog-0.0.4/stlog/formatter.py` & `stlog-0.0.5/stlog/formatter.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.4/stlog/handler.py` & `stlog-0.0.5/stlog/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from stlog.base import (
     RESERVED_ATTRS,
     STLOG_EXTRA_KEY,
     StLogError,
     rich_dump_exception_on_console,
 )
-from stlog.context import ExecutionLogContext
+from stlog.context import LogContext
 
 
 class ContextReinjectHandlerWrapper(logging.Handler):
-    """Logging Handler (built as a wrapper/adapter of another handler) to reinject `stlog.ExecutionLogContext`
+    """Logging Handler (built as a wrapper/adapter of another handler) to reinject `stlog.LogContext`
     content in log records (if they weren't sent by `stlog` special loggers)."""
 
     def __init__(
         self,
         *,
         wrapped: logging.Handler,
         read_extra_kwarg_from_standard_logging: bool = False,
@@ -27,15 +27,15 @@
         )
 
     def handle(self, record: logging.LogRecord):
         if not hasattr(record, STLOG_EXTRA_KEY):
             # the context is not already injected in record
             # (this log didn't pass by stlog ContextVarsAdapter)
             # => let's fix that
-            new_kwargs = ExecutionLogContext._get()
+            new_kwargs = LogContext._get()
             extra_keys: set[str] = getattr(record, STLOG_EXTRA_KEY, set())
             for k, v in new_kwargs.items():
                 setattr(record, k, v)
                 extra_keys.add(k)
             if self.read_extra_kwarg_from_standard_logging:
                 # try to find special keys set by extra kwargs in
                 # standard python logging
```

### Comparing `stlog-0.0.4/stlog/output.py` & `stlog-0.0.5/stlog/output.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.4/stlog/setup.py` & `stlog-0.0.5/stlog/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 import os
 import sys
 import traceback
 import types
 import typing
 
 from stlog.adapter import getLogger
-from stlog.base import GLOBAL_LOGGING_CONFIG, check_env_true
+from stlog.base import GLOBAL_LOGGING_CONFIG, check_env_false, check_env_true
 from stlog.handler import ContextReinjectHandlerWrapper
 from stlog.output import Output, make_stream_or_rich_stream_output
 
 DEFAULT_LEVEL: str = os.environ.get("STLOG_LEVEL", "INFO")
-DEFAULT_CAPTURE_WARNINGS: bool = check_env_true("STLOG_CAPTURE_WARNINGS", True)
-DEFAULT_REINJECT_CONTEXT_IN_STANDARD_LOGGING: bool = check_env_true(
+DEFAULT_CAPTURE_WARNINGS: bool = check_env_false("STLOG_CAPTURE_WARNINGS", True)
+DEFAULT_REINJECT_CONTEXT_IN_STANDARD_LOGGING: bool = check_env_false(
     "STLOG_REINJECT_CONTEXT_IN_STANDARD_LOGGING", True
 )
+DEFAULT_READ_EXTRA_KWARG_FROM_STANDARD_LOGGING: bool = check_env_true(
+    "STLOG_READ_EXTRA_KWARGS_FROM_STANDARD_LOGGING", False
+)
 DEFAULT_PROGRAM_NAME: str | None = os.environ.get("STLOG_PROGRAM_NAME", None)
 
 
 def _make_default_outputs() -> list[Output]:
     return [make_stream_or_rich_stream_output(stream=sys.stderr)]
 
 
@@ -72,15 +75,15 @@
         program_name: the name of the program, the default value is read in STLOG_PROGRAM_NAME
             env var or auto-detected if not set.
         capture_warnings: capture warnings from the `warnings` module.
         logging_excepthook: if not None, override sys.excepthook with the given callable
             See https://docs.python.org/3/library/sys.html#sys.excepthook for details.
         extra_levels: iterable of tuples (logger name, log level) for quick override of
             the root log level.
-        reinject_context_in_standard_logging: if True, reinject the ExecutionLogContext
+        reinject_context_in_standard_logging: if True, reinject the LogContext
             in log record emitted with python standard loggers.
         read_extra_kwarg_from_standard_logging: if try to reinject the extra kwargs from standard logging.
     """
     root_logger = logging.getLogger(None)
     if program_name is not None:
         GLOBAL_LOGGING_CONFIG.program_name = program_name
```

### Comparing `stlog-0.0.4/PKG-INFO` & `stlog-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlog
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 License: MIT
 Author: Fabien MARTY
 Author-email: fabien.marty@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,18 @@
 
 
 <!-- WARNING: generated from README.md.j2, do not modify this file manually but modify README.md.j2 instead
      and execute 'poetry run poe readme' to regenerate this README.md file -->
 
 # stlog
 
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fabien-marty/stlog/lint.yaml)](https://github.com/fabien-marty/stlog/actions/workflows/lint.yaml)
+[![Codecov](https://img.shields.io/codecov/c/github/fabien-marty/stlog)](https://app.codecov.io/github/fabien-marty/stlog)
+[![pypi badge](https://img.shields.io/pypi/v/stlog?color=brightgreen)](https://pypi.org/project/stlog/)
+
 [Full documentation](https://fabien-marty.github.io/stlog/)
 
 <!--intro-start-->
 
 ## What is it?
 
 **ST**andard **ST**ructured **LOG** (`stlog`) is Python 3.7+ [structured logging](#structured) library:
@@ -111,28 +115,28 @@
 
 ![rich output](docs/python/qs1.svg)
  
 
 ### Usage with context
 
 ```python
-from stlog import ExecutionLogContext, getLogger, setup
+from stlog import LogContext, getLogger, setup
 
 # Set the logging default configuration (human output on stderr)
 setup()
 
 # ...
 
 # Set the (kind of) global execution context
 # (thread, worker, async friendly: one context by execution)
 # (for example in a wsgi/asgi middleware)
 # Note: ExecutionContext is a static class, so a kind of global singleton
-ExecutionLogContext.reset_context()
-ExecutionLogContext.add(request_id="4c2383f5")
-ExecutionLogContext.add(client_id=456, http_method="GET")
+LogContext.reset_context()
+LogContext.add(request_id="4c2383f5")
+LogContext.add(client_id=456, http_method="GET")
 
 # ... in another file/class/...
 
 # Get a logger
 logger = getLogger(__name__)
 logger.info("It works", foo="bar", x=123)
 logger.critical("Houston, we have a problem!")
@@ -152,32 +156,32 @@
 ![rich output](docs/python/qs2.svg)
  
 
 What about if you want to get a more parsing friendly output (for example in JSON on `stdout`) while keeping the human output on `stderr` (without any context)?
 
 ```python
 import sys
-from stlog import ExecutionLogContext, getLogger, setup
+from stlog import LogContext, getLogger, setup
 from stlog.output import StreamOutput
 from stlog.formatter import HumanFormatter, JsonFormatter
 
 setup(
     outputs=[
         StreamOutput(
             stream=sys.stderr,
             formatter=HumanFormatter(exclude_extras_keys_fnmatchs=["*"]),
         ),
         StreamOutput(stream=sys.stdout, formatter=JsonFormatter(indent=4)),
     ]
 )
 
 # See previous example for details
-ExecutionLogContext.reset_context()
-ExecutionLogContext.add(request_id="4c2383f5")
-ExecutionLogContext.add(client_id=456, http_method="GET")
+LogContext.reset_context()
+LogContext.add(request_id="4c2383f5")
+LogContext.add(client_id=456, http_method="GET")
 logger = getLogger(__name__)
 logger.info("It works", foo="bar", x=123)
 logger.critical("Houston, we have a problem!")
  
 ```
 
 Human output (on `stderr`):
```

