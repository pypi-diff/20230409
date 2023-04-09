# Comparing `tmp/types-croniter-1.3.2.7.tar.gz` & `tmp/types-croniter-1.3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-croniter-1.3.2.7.tar", last modified: Mon Mar 27 18:22:34 2023, max compression
+gzip compressed data, was "types-croniter-1.3.2.8.tar", last modified: Sun Apr  9 15:13:39 2023, max compression
```

## Comparing `types-croniter-1.3.2.7.tar` & `types-croniter-1.3.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:34.654028 types-croniter-1.3.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-03-27 18:22:33.000000 types-croniter-1.3.2.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:33.000000 types-croniter-1.3.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 18:22:34.654028 types-croniter-1.3.2.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:34.654028 types-croniter-1.3.2.7/croniter-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:22:33.000000 types-croniter-1.3.2.7/croniter-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-27 18:21:24.000000 types-croniter-1.3.2.7/croniter-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-03-27 18:21:24.000000 types-croniter-1.3.2.7/croniter-stubs/croniter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:34.654028 types-croniter-1.3.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-27 18:22:33.000000 types-croniter-1.3.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:34.654028 types-croniter-1.3.2.7/types_croniter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 18:22:34.000000 types-croniter-1.3.2.7/types_croniter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-27 18:22:34.000000 types-croniter-1.3.2.7/types_croniter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:34.000000 types-croniter-1.3.2.7/types_croniter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 18:22:34.000000 types-croniter-1.3.2.7/types_croniter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:13:39.447228 types-croniter-1.3.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-09 15:13:38.000000 types-croniter-1.3.2.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 15:13:38.000000 types-croniter-1.3.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-09 15:13:39.447228 types-croniter-1.3.2.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:13:39.447228 types-croniter-1.3.2.8/croniter-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-09 15:13:38.000000 types-croniter-1.3.2.8/croniter-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-09 15:13:26.000000 types-croniter-1.3.2.8/croniter-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-09 15:13:26.000000 types-croniter-1.3.2.8/croniter-stubs/croniter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 15:13:39.447228 types-croniter-1.3.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-09 15:13:38.000000 types-croniter-1.3.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:13:39.447228 types-croniter-1.3.2.8/types_croniter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-09 15:13:39.000000 types-croniter-1.3.2.8/types_croniter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-09 15:13:39.000000 types-croniter-1.3.2.8/types_croniter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:13:39.000000 types-croniter-1.3.2.8/types_croniter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 15:13:39.000000 types-croniter-1.3.2.8/types_croniter.egg-info/top_level.txt
```

### Comparing `types-croniter-1.3.2.7/CHANGELOG.md` & `types-croniter-1.3.2.8/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.3.2.8 (2023-04-09)
+
+Update `croniter` to 1.3.10 (#10027)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 1.3.2.7 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
 
 ## 1.3.2.6 (2023-02-22)
 
 Update `Unused` parameters in `stubs/` (#9704)
```

### Comparing `types-croniter-1.3.2.7/PKG-INFO` & `types-croniter-1.3.2.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-croniter
-Version: 1.3.2.7
+Version: 1.3.2.8
 Summary: Typing stubs for croniter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `02b8f77630c8dbb60a4d00c362d01519e9639591`.
```

### Comparing `types-croniter-1.3.2.7/croniter-stubs/croniter.pyi` & `types-croniter-1.3.2.8/croniter-stubs/croniter.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import datetime
 from _typeshed import ReadableBuffer, Unused
 from collections import OrderedDict
 from collections.abc import Iterator
 from re import Match, Pattern
 from typing import Any, overload
-from typing_extensions import Literal, Self, TypeAlias
+from typing_extensions import Final, Literal, Self, TypeAlias
 
 _RetType: TypeAlias = type[float | datetime.datetime]
 
 step_search_re: Pattern[str]
 only_int_re: Pattern[str]
 star_or_int_re: Pattern[str]
-special_weekday_re: Pattern[str]
+special_dow_re: Pattern[str]
 hash_expression_re: Pattern[str]
-VALID_LEN_EXPRESSION: list[int]
+VALID_LEN_EXPRESSION: Final[list[int]]
+ALPHAS: Final[dict[str, int]]
+DOW_ALPHAS: Final[dict[str, int]]
+MONTHS: Final[str]
+M_ALPHAS: Final[dict[str, int]]
+WEEKDAYS: Final[str]
 
 def timedelta_to_seconds(td: datetime.timedelta) -> float: ...
 
 class CroniterError(ValueError): ...
 class CroniterBadTypeRangeError(TypeError): ...
 class CroniterBadCronError(CroniterError): ...
 class CroniterUnsupportedSyntaxError(CroniterBadCronError): ...
```

### Comparing `types-croniter-1.3.2.7/setup.py` & `types-croniter-1.3.2.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `02b8f77630c8dbb60a4d00c362d01519e9639591`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.3.2.7",
+      version="1.3.2.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md",
```

### Comparing `types-croniter-1.3.2.7/types_croniter.egg-info/PKG-INFO` & `types-croniter-1.3.2.8/types_croniter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-croniter
-Version: 1.3.2.7
+Version: 1.3.2.8
 Summary: Typing stubs for croniter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `02b8f77630c8dbb60a4d00c362d01519e9639591`.
```

