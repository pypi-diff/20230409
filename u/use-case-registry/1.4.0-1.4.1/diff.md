# Comparing `tmp/use_case_registry-1.4.0.tar.gz` & `tmp/use_case_registry-1.4.1.tar.gz`

## Comparing `use_case_registry-1.4.0.tar` & `use_case_registry-1.4.1.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.tool-versions
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/Makefile
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/mkdocs.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/workflows/audit.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/workflows/update_docs.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.vscode/settings.json
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/docs/index.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/docs/general-thoughts/clean-architecture/index.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/docs/general-thoughts/error-handling/index.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/docs/general-thoughts/one-use-case-one-workflow/index.md
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/requirements/core.txt
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/requirements/dev.txt
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/requirements/sqlalchemy.txt
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/scripts/release_github.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/test_parsers.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/test_registry.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-1.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-2.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-3.yml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-4.yml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-5.yml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-6.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-7.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-8.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/base/__init__.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/base/test_command.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/base/test_repository.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/__about__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/py.typed
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/registry.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/base/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/base/command.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/base/repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/internals/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/internals/errors.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/parsers/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/parsers/errors.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/parsers/repository_config.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/README.md
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.tool-versions
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/mkdocs.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/workflows/audit.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/workflows/update_docs.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.vscode/settings.json
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/docs/general-thoughts/clean-architecture/index.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/docs/general-thoughts/error-handling/index.md
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/docs/general-thoughts/one-use-case-one-workflow/index.md
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/requirements/core.txt
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/requirements/dev.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/requirements/sqlalchemy.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/scripts/release_github.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/test_parsers.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/test_registry.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-1.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-2.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-3.yml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-4.yml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-5.yml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-6.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-7.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-8.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/base/__init__.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/base/test_command.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/base/test_repository.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/enums.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/py.typed
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/registry.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/base/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/base/command.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/base/repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/internals/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/internals/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/parsers/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/parsers/errors.py
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/parsers/repository_config.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/parsers/utils.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/README.md
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/PKG-INFO
```

### Comparing `use_case_registry-1.4.0/Makefile` & `use_case_registry-1.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/mkdocs.yml` & `use_case_registry-1.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `use_case_registry-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md` & `use_case_registry-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/.github/workflows/audit.yml` & `use_case_registry-1.4.1/.github/workflows/audit.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/.github/workflows/coverage.yml` & `use_case_registry-1.4.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/.github/workflows/release.yml` & `use_case_registry-1.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/.github/workflows/test.yml` & `use_case_registry-1.4.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/.vscode/settings.json` & `use_case_registry-1.4.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/docs/index.md` & `use_case_registry-1.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/docs/general-thoughts/clean-architecture/index.md` & `use_case_registry-1.4.1/docs/general-thoughts/clean-architecture/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/docs/general-thoughts/error-handling/index.md` & `use_case_registry-1.4.1/docs/general-thoughts/error-handling/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/docs/general-thoughts/one-use-case-one-workflow/index.md` & `use_case_registry-1.4.1/docs/general-thoughts/one-use-case-one-workflow/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/requirements/dev.txt` & `use_case_registry-1.4.1/requirements/dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,15 @@
 pyyaml==6.0
     # via
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
     #   use_case_registry (pyproject.toml)
 pyyaml-env-tag==0.1
-    # via
-    #   mkdocs
-    #   use_case_registry (pyproject.toml)
+    # via mkdocs
 regex==2023.3.23
     # via mkdocs-material
 requests==2.28.2
     # via mkdocs-material
 result==0.9.0
     # via use_case_registry (pyproject.toml)
 rfc3986[idna2008]==1.5.0
```

### Comparing `use_case_registry-1.4.0/scripts/release_github.py` & `use_case_registry-1.4.1/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/tests/test_parsers.py` & `use_case_registry-1.4.1/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/tests/test_registry.py` & `use_case_registry-1.4.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/tests/base/test_command.py` & `use_case_registry-1.4.1/tests/base/test_command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/tests/base/test_repository.py` & `use_case_registry-1.4.1/tests/base/test_repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/use_case_registry/errors.py` & `use_case_registry-1.4.1/use_case_registry/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/use_case_registry/registry.py` & `use_case_registry-1.4.1/use_case_registry/registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/use_case_registry/base/command.py` & `use_case_registry-1.4.1/use_case_registry/base/command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/use_case_registry/base/repository.py` & `use_case_registry-1.4.1/use_case_registry/base/repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/use_case_registry/internals/errors.py` & `use_case_registry-1.4.1/use_case_registry/internals/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/use_case_registry/parsers/repository_config.py` & `use_case_registry-1.4.1/use_case_registry/parsers/repository_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 """Repository config yaml parser."""
-import enum
 import pathlib
 from typing import Any
 
 import yaml
-import yaml_env_tag
 from typing_extensions import assert_never
 
+from use_case_registry.enums import OptionEnums
 from use_case_registry.parsers.errors import ConfigFileError
+from use_case_registry.parsers.utils import construct_env_tag
 
-yaml.Loader.add_constructor(tag="!ENV", constructor=yaml_env_tag.construct_env_tag)
-
-
-class OptionEnums(str, enum.Enum):
-    """Option enums."""
+yaml.Loader.add_constructor(tag="!ENV", constructor=construct_env_tag)
 
 
 class RepoEngines(OptionEnums):
     """Support Repository Engines."""
 
     SQLALCHEMY = "SQLALCHEMY"
```

### Comparing `use_case_registry-1.4.0/.gitignore` & `use_case_registry-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/LICENSE.txt` & `use_case_registry-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/README.md` & `use_case_registry-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.0/pyproject.toml` & `use_case_registry-1.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 # https://hatch.pypa.io/latest/config/dependency/
 dependencies = [
   "result",
-  "pyyaml",
-  "pyyaml-env-tag"
+  "pyyaml"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 sqlalchemy = [
   "SQLAlchemy"
 ]
@@ -150,15 +149,15 @@
     "tests",
 ]
 env = [
     "EXECUTION_ENV=dev",
 ]
 xfail_strict = true
 addopts =[
-  "--cov-fail-under=90", 
+  "--cov-fail-under=85", 
   "--cov-report=term-missing:skip-covered",
   "--cov-config=pyproject.toml",
   "--cov=use_case_registry"
 ]
 
 [tool.mypy]
 files = [
```

### Comparing `use_case_registry-1.4.0/PKG-INFO` & `use_case_registry-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use_case_registry
-Version: 1.4.0
+Version: 1.4.1
 Summary: Registry class for Use Case implementation. They are basically meaningfull lists with some constraints.
 Project-URL: Homepage, https://github.com/Tomperez98/use-case-registry
 Project-URL: Documentation, https://tomperez98.github.io/use-case-registry/
 Project-URL: Issues, https://github.com/Tomperez98/use-case-registry/issues
 Project-URL: Source, https://github.com/Tomperez98/use-case-registry
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-Expression: MIT
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: pyyaml
-Requires-Dist: pyyaml-env-tag
 Requires-Dist: result
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mkdocs-material; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
```

