# Comparing `tmp/lintrunner_adapters-0.7.0.tar.gz` & `tmp/lintrunner_adapters-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lintrunner_adapters-0.7.0.tar", max compression
+gzip compressed data, was "lintrunner_adapters-0.7.1.tar", max compression
```

## Comparing `lintrunner_adapters-0.7.0.tar` & `lintrunner_adapters-0.7.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     4389 2023-04-07 00:20:34.688240 lintrunner_adapters-0.7.0/LICENSE
--rw-r--r--   0        0        0     1984 2023-04-07 00:20:34.688240 lintrunner_adapters-0.7.0/README.md
--rw-r--r--   0        0        0      711 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/__init__.py
--rw-r--r--   0        0        0     1491 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/__main__.py
--rw-r--r--   0        0        0     3546 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/_common/lintrunner_common.py
--rw-r--r--   0        0        0     4097 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/add_trailing_comma_linter.py
--rw-r--r--   0        0        0     5321 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/black_isort_linter.py
--rw-r--r--   0        0        0     4790 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/black_linter.py
--rw-r--r--   0        0        0     6348 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/clangformat_linter.py
--rw-r--r--   0        0        0     7640 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/clippy_linter.py
--rw-r--r--   0        0        0     3453 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/cmake_linter.py
--rw-r--r--   0        0        0     4374 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/django_upgrade_linter.py
--rw-r--r--   0        0        0     3140 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/editorconfig_checker_linter.py
--rw-r--r--   0        0        0     1776 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/exec_linter.py
--rw-r--r--   0        0        0    10327 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/flake8_linter.py
--rw-r--r--   0        0        0     7062 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/grep_linter.py
--rw-r--r--   0        0        0     4269 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/isort_linter.py
--rw-r--r--   0        0        0     5933 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/mypy_linter.py
--rw-r--r--   0        0        0     4593 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/newlines_linter.py
--rw-r--r--   0        0        0     3371 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/pip_init.py
--rw-r--r--   0        0        0     6048 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/pylint_linter.py
--rw-r--r--   0        0        0     4532 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/pyupgrade_linter.py
--rw-r--r--   0        0        0     4722 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/refurb_linter.py
--rw-r--r--   0        0        0     4135 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/ruff_fix_linter.py
--rw-r--r--   0        0        0     6413 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/ruff_linter.py
--rw-r--r--   0        0        0     7223 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/rustfmt_linter.py
--rw-r--r--   0        0        0     2305 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/shellcheck_linter.py
--rw-r--r--   0        0        0     3122 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/ufmt_linter.py
--rw-r--r--   0        0        0     4060 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/tools/convert_to_sarif.py
--rw-r--r--   0        0        0     6820 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/lintrunner_adapters/tools/convert_to_sarif_test.py
--rw-r--r--   0        0        0     2335 2023-04-07 00:20:34.692240 lintrunner_adapters-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 lintrunner_adapters-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     4389 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1984 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/README.md
+-rw-r--r--   0        0        0      711 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/lintrunner_adapters/__init__.py
+-rw-r--r--   0        0        0     1752 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/lintrunner_adapters/__main__.py
+-rw-r--r--   0        0        0     3546 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/lintrunner_adapters/_common/lintrunner_common.py
+-rw-r--r--   0        0        0     4097 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/add_trailing_comma_linter.py
+-rw-r--r--   0        0        0     5321 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/black_isort_linter.py
+-rw-r--r--   0        0        0     4790 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/black_linter.py
+-rw-r--r--   0        0        0     6348 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/clangformat_linter.py
+-rw-r--r--   0        0        0     7640 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/clippy_linter.py
+-rw-r--r--   0        0        0     3453 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/cmake_linter.py
+-rw-r--r--   0        0        0     4374 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/django_upgrade_linter.py
+-rw-r--r--   0        0        0     3140 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/editorconfig_checker_linter.py
+-rw-r--r--   0        0        0     1776 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/exec_linter.py
+-rw-r--r--   0        0        0    10327 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/flake8_linter.py
+-rw-r--r--   0        0        0     7062 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/grep_linter.py
+-rw-r--r--   0        0        0     4269 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/isort_linter.py
+-rw-r--r--   0        0        0     5933 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/mypy_linter.py
+-rw-r--r--   0        0        0     4593 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/newlines_linter.py
+-rw-r--r--   0        0        0     3371 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pip_init.py
+-rw-r--r--   0        0        0     6048 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pylint_linter.py
+-rw-r--r--   0        0        0     4532 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pyupgrade_linter.py
+-rw-r--r--   0        0        0     4722 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/refurb_linter.py
+-rw-r--r--   0        0        0     4135 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ruff_fix_linter.py
+-rw-r--r--   0        0        0     6413 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ruff_linter.py
+-rw-r--r--   0        0        0     7223 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/rustfmt_linter.py
+-rw-r--r--   0        0        0     2305 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/shellcheck_linter.py
+-rw-r--r--   0        0        0     3122 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ufmt_linter.py
+-rw-r--r--   0        0        0     4060 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/tools/convert_to_sarif.py
+-rw-r--r--   0        0        0     6820 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/tools/convert_to_sarif_test.py
+-rw-r--r--   0        0        0     2335 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 lintrunner_adapters-0.7.1/PKG-INFO
```

### Comparing `lintrunner_adapters-0.7.0/LICENSE` & `lintrunner_adapters-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/README.md` & `lintrunner_adapters-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/__init__.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/__main__.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,20 @@
         allow_extra_args=True,
     ),
 )
 @click.argument(
     "adapter", type=click.Choice(list(lintrunner_adapters.available_adapters().keys()))
 )
 def run(adapter: str) -> None:
-    """Run an adapter."""
+    """Run an adapter.
+
+    \u001b[35mIf you get an error like \u001b[1m"Error: Invalid value"\u001b[0m\u001b[35m,
+    a new adapter may have been added to a newer version of lintrunner_adapters.
+    Try upgrading by running "pip install --upgrade lintrunner_adapters".\u001b[0m
+    """
     adapters = lintrunner_adapters.available_adapters()
     try:
         subprocess.run(
             [
                 sys.executable,
                 adapters[adapter],
                 *sys.argv[3:],
```

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/_common/lintrunner_common.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/_common/lintrunner_common.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/add_trailing_comma_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/add_trailing_comma_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/black_isort_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/black_isort_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/black_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/black_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/clangformat_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/clangformat_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/clippy_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/clippy_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/cmake_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/cmake_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/django_upgrade_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/django_upgrade_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/editorconfig_checker_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/editorconfig_checker_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/exec_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/exec_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/flake8_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/flake8_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/grep_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/grep_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/isort_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/isort_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/mypy_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/mypy_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/newlines_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/newlines_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/pip_init.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pip_init.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/pylint_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pylint_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/pyupgrade_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pyupgrade_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/refurb_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/refurb_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/ruff_fix_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ruff_fix_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/ruff_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ruff_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/rustfmt_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/rustfmt_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/shellcheck_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/shellcheck_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/adapters/ufmt_linter.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ufmt_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/tools/convert_to_sarif.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/tools/convert_to_sarif.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/lintrunner_adapters/tools/convert_to_sarif_test.py` & `lintrunner_adapters-0.7.1/lintrunner_adapters/tools/convert_to_sarif_test.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.0/pyproject.toml` & `lintrunner_adapters-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lintrunner-adapters"
-version = "0.7.0"
+version = "0.7.1"
 description = "Adapters and tools for lintrunner"
 authors = ["Justin Chu <justinchu@microsoft.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/justinchuby/lintrunner-adapters"
 keywords = ["lintrunner", "lint", "cli", "sarif", "linting", "ci", "linter", "flake8", "clippy", "ruff", "rustfmt", "github-code-scanning"]
 classifiers = [
```

### Comparing `lintrunner_adapters-0.7.0/PKG-INFO` & `lintrunner_adapters-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lintrunner-adapters
-Version: 0.7.0
+Version: 0.7.1
 Summary: Adapters and tools for lintrunner
 Home-page: https://github.com/justinchuby/lintrunner-adapters
 License: MIT
 Keywords: lintrunner,lint,cli,sarif,linting,ci,linter,flake8,clippy,ruff,rustfmt,github-code-scanning
 Author: Justin Chu
 Author-email: justinchu@microsoft.com
 Requires-Python: >=3.7,<4.0
```

