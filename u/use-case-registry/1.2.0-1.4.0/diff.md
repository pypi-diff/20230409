# Comparing `tmp/use_case_registry-1.2.0.tar.gz` & `tmp/use_case_registry-1.4.0.tar.gz`

## Comparing `use_case_registry-1.2.0.tar` & `use_case_registry-1.4.0.tar`

### file list

```diff
@@ -1,39 +1,52 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.tool-versions
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/Makefile
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/mkdocs.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.github/workflows/audit.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.github/workflows/update_docs.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.vscode/settings.json
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/docs/index.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/docs/general-thoughts/clean-architecture/index.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/docs/general-thoughts/error-handling/index.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/docs/general-thoughts/one-use-case-one-workflow/index.md
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/requirements/core.txt
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/requirements/dev.txt
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/scripts/release_github.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/tests/test_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/tests/base/__init__.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/tests/base/test_command.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/tests/base/test_repository.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/use_case_registry/__about__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/use_case_registry/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/use_case_registry/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/use_case_registry/py.typed
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/use_case_registry/registry.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/use_case_registry/base/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/use_case_registry/base/command.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/use_case_registry/base/repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/use_case_registry/internals/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/use_case_registry/internals/errors.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/README.md
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 use_case_registry-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.tool-versions
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/workflows/audit.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.github/workflows/update_docs.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/docs/general-thoughts/clean-architecture/index.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/docs/general-thoughts/error-handling/index.md
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/docs/general-thoughts/one-use-case-one-workflow/index.md
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/requirements/core.txt
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/requirements/dev.txt
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/requirements/sqlalchemy.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/scripts/release_github.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/test_parsers.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/test_registry.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-1.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-2.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-3.yml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-4.yml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-5.yml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-6.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-7.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/assets/repo_configs/conf-8.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/base/__init__.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/base/test_command.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/tests/base/test_repository.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/py.typed
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/registry.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/base/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/base/command.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/base/repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/internals/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/internals/errors.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/parsers/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/parsers/errors.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/use_case_registry/parsers/repository_config.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/README.md
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 use_case_registry-1.4.0/PKG-INFO
```

### Comparing `use_case_registry-1.2.0/Makefile` & `use_case_registry-1.4.0/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 .PHONY: new-release
 new-release: ## Prepare new release for github.
 	python scripts/release_github.py
 
 .PHONY: refresh-lockfiles
 refresh-lockfiles: ## Rewrite requirements lockfiles
 	@echo "Updating requirements/*.txt files using `pip-compile`"
+	find requirements/ -name '*.txt' ! -name 'all.txt' -type f -delete
 	mkdir -p requirements
 	# https://github.com/dependabot/dependabot-core/issues/3940
 	pip-compile -q --upgrade --resolver=backtracking --no-emit-trusted-host -o requirements/core.txt pyproject.toml
-	pip-compile -q --upgrade --extra dev --resolver=backtracking --no-emit-trusted-host -o requirements/dev.txt pyproject.toml
+	pip-compile -q --upgrade --extra sqlalchemy --resolver=backtracking --no-emit-trusted-host -o requirements/sqlalchemy.txt pyproject.toml
+	pip-compile -q --upgrade --extra dev --extra sqlalchemy --resolver=backtracking --no-emit-trusted-host -o requirements/dev.txt pyproject.toml
 	rm -f requirements.txt
 
 .PHONY: sync-to-env
 sync-to-env: ## sync dev virtualenv
 	@pip-sync requirements/$(env).txt
 	@pip install -e .
```

### Comparing `use_case_registry-1.2.0/mkdocs.yml` & `use_case_registry-1.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `use_case_registry-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `use_case_registry-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/.github/workflows/audit.yml` & `use_case_registry-1.4.0/.github/workflows/audit.yml`

 * *Files 14% similar despite different names*

```diff
@@ -29,8 +29,10 @@
         with:
           python-version: ${{ steps.versions.outputs.python }}
 
       - name: Install pip audit
         run: pip install pip-audit
 
       - name: Audit dependencies
-        run: pip-audit -r requirements/core.txt -l --desc
+        run: |
+          pip-audit -r requirements/core.txt -l --desc
+          pip-audit -r requirements/sqlalchemy.txt -l --desc
```

### Comparing `use_case_registry-1.2.0/.github/workflows/coverage.yml` & `use_case_registry-1.4.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/.github/workflows/release.yml` & `use_case_registry-1.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/.github/workflows/test.yml` & `use_case_registry-1.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/.vscode/settings.json` & `use_case_registry-1.4.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/docs/index.md` & `use_case_registry-1.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/docs/general-thoughts/clean-architecture/index.md` & `use_case_registry-1.4.0/docs/general-thoughts/clean-architecture/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/docs/general-thoughts/error-handling/index.md` & `use_case_registry-1.4.0/docs/general-thoughts/error-handling/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/docs/general-thoughts/one-use-case-one-workflow/index.md` & `use_case_registry-1.4.0/docs/general-thoughts/one-use-case-one-workflow/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/requirements/dev.txt` & `use_case_registry-1.4.0/requirements/dev.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=dev --no-emit-trusted-host --output-file=requirements/dev.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=dev --extra=sqlalchemy --no-emit-trusted-host --output-file=requirements/dev.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-attrs==22.2.0
-    # via pytest
-black==23.1.0
+black==23.3.0
     # via use_case_registry (pyproject.toml)
 build==0.10.0
     # via pip-tools
 certifi==2022.12.7
     # via
     #   httpcore
     #   httpx
@@ -24,46 +22,49 @@
     #   black
     #   hatch
     #   mkdocs
     #   pip-tools
     #   userpath
 colorama==0.4.6
     # via mkdocs-material
-coverage[toml]==7.2.1
+coverage[toml]==7.2.3
     # via pytest-cov
 distlib==0.3.6
     # via virtualenv
 editables==0.3
     # via hatchling
 exceptiongroup==1.1.1
     # via pytest
-filelock==3.9.0
+filelock==3.11.0
     # via virtualenv
 ghp-import==2.1.0
     # via mkdocs
 h11==0.14.0
     # via httpcore
-hatch==1.6.3
+hatch==1.7.0
     # via use_case_registry (pyproject.toml)
-hatchling==1.13.0
+hatchling==1.14.0
     # via hatch
 httpcore==0.16.3
     # via httpx
 httpx==0.23.3
     # via hatch
 hyperlink==21.0.0
     # via hatch
 idna==3.4
     # via
     #   anyio
     #   hyperlink
     #   requests
     #   rfc3986
-importlib-metadata==6.0.0
-    # via keyring
+importlib-metadata==6.2.0
+    # via
+    #   keyring
+    #   markdown
+    #   mkdocs
 iniconfig==2.0.0
     # via pytest
 jaraco-classes==3.2.3
     # via keyring
 jinja2==3.1.2
     # via
     #   mkdocs
@@ -81,125 +82,141 @@
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.4.2
     # via mkdocs-material
-mkdocs-material==9.1.2
+mkdocs-material==9.1.6
     # via use_case_registry (pyproject.toml)
 mkdocs-material-extensions==1.1.1
     # via mkdocs-material
 more-itertools==9.1.0
     # via jaraco-classes
-mypy==1.1.1
+mypy==1.2.0
     # via use_case_registry (pyproject.toml)
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 packaging==23.0
     # via
     #   black
     #   build
     #   hatch
     #   hatchling
     #   mkdocs
     #   pytest
-pathspec==0.11.0
+pathspec==0.11.1
     # via
     #   black
     #   hatchling
 pexpect==4.8.0
     # via hatch
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via use_case_registry (pyproject.toml)
-platformdirs==3.1.1
+platformdirs==3.2.0
     # via
     #   black
     #   hatch
     #   virtualenv
 pluggy==1.0.0
     # via
     #   hatchling
     #   pytest
 ptyprocess==0.7.0
     # via pexpect
 pygments==2.14.0
     # via
     #   mkdocs-material
     #   rich
-pymdown-extensions==9.10
+pymdown-extensions==9.11
     # via mkdocs-material
 pyperclip==1.8.2
     # via hatch
 pyproject-hooks==1.0.0
     # via build
-pytest==7.2.2
+pytest==7.3.0
     # via
     #   pytest-cov
+    #   pytest-env
     #   use_case_registry (pyproject.toml)
 pytest-cov==4.0.0
     # via use_case_registry (pyproject.toml)
+pytest-env==0.8.1
+    # via use_case_registry (pyproject.toml)
 python-dateutil==2.8.2
     # via ghp-import
 pyyaml==6.0
     # via
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
+    #   use_case_registry (pyproject.toml)
 pyyaml-env-tag==0.1
-    # via mkdocs
-regex==2022.10.31
+    # via
+    #   mkdocs
+    #   use_case_registry (pyproject.toml)
+regex==2023.3.23
     # via mkdocs-material
 requests==2.28.2
     # via mkdocs-material
 result==0.9.0
     # via use_case_registry (pyproject.toml)
 rfc3986[idna2008]==1.5.0
     # via httpx
-rich==13.3.2
+rich==13.3.3
     # via hatch
-ruff==0.0.255
+ruff==0.0.261
     # via use_case_registry (pyproject.toml)
 shellingham==1.5.0.post1
     # via hatch
 six==1.16.0
     # via python-dateutil
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
     #   httpx
+sqlalchemy==2.0.9
+    # via use_case_registry (pyproject.toml)
 toml==0.10.2
     # via use_case_registry (pyproject.toml)
 tomli==2.0.1
     # via
     #   black
     #   build
     #   coverage
     #   hatchling
     #   mypy
     #   pyproject-hooks
     #   pytest
 tomli-w==1.0.0
     # via hatch
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via hatch
+trove-classifiers==2023.3.9
+    # via hatchling
+types-pyyaml==6.0.12.9
+    # via use_case_registry (pyproject.toml)
 typing-extensions==4.5.0
-    # via mypy
+    # via
+    #   black
+    #   mypy
+    #   result
+    #   sqlalchemy
 urllib3==1.26.15
     # via requests
 userpath==1.8.0
     # via hatch
 virtualenv==20.21.0
     # via hatch
-watchdog==2.3.1
+watchdog==3.0.0
     # via mkdocs
-wheel==0.38.4
+wheel==0.40.0
     # via pip-tools
 zipp==3.15.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `use_case_registry-1.2.0/scripts/release_github.py` & `use_case_registry-1.4.0/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/tests/test_registry.py` & `use_case_registry-1.4.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/tests/base/test_command.py` & `use_case_registry-1.4.0/tests/base/test_command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/tests/base/test_repository.py` & `use_case_registry-1.4.0/tests/base/test_repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/use_case_registry/errors.py` & `use_case_registry-1.4.0/use_case_registry/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/use_case_registry/registry.py` & `use_case_registry-1.4.0/use_case_registry/registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/use_case_registry/base/command.py` & `use_case_registry-1.4.0/use_case_registry/base/command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/use_case_registry/base/repository.py` & `use_case_registry-1.4.0/use_case_registry/base/repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/use_case_registry/internals/errors.py` & `use_case_registry-1.4.0/use_case_registry/internals/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/.gitignore` & `use_case_registry-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/LICENSE.txt` & `use_case_registry-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/README.md` & `use_case_registry-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.2.0/pyproject.toml` & `use_case_registry-1.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,36 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 # https://hatch.pypa.io/latest/config/dependency/
 dependencies = [
-  "result"
+  "result",
+  "pyyaml",
+  "pyyaml-env-tag"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
+sqlalchemy = [
+  "SQLAlchemy"
+]
 dev = [
   "pytest",
   "pytest-cov",
   "mypy",
   "ruff",
   "pip-tools",
   "hatch",
   "mkdocs-material",
   "toml",
-  "black"
+  "black",
+  "types-PyYAML",
+  "pytest-env"
 ]
 
 [project.urls]
 Homepage = "https://github.com/Tomperez98/use-case-registry"
 Documentation = "https://tomperez98.github.io/use-case-registry/"
 Issues = "https://github.com/Tomperez98/use-case-registry/issues"
 Source = "https://github.com/Tomperez98/use-case-registry"
@@ -138,14 +145,17 @@
 docstring-quotes = "double"
 inline-quotes = "double"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
+env = [
+    "EXECUTION_ENV=dev",
+]
 xfail_strict = true
 addopts =[
   "--cov-fail-under=90", 
   "--cov-report=term-missing:skip-covered",
   "--cov-config=pyproject.toml",
   "--cov=use_case_registry"
 ]
@@ -167,7 +177,13 @@
 no_implicit_reexport = true
 warn_unused_configs = true
 disallow_subclassing_any = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
+
+[[tool.mypy.overrides]]
+module = [
+  "yaml_env_tag"
+]
+ignore_missing_imports = true
```

### Comparing `use_case_registry-1.2.0/PKG-INFO` & `use_case_registry-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use_case_registry
-Version: 1.2.0
+Version: 1.4.0
 Summary: Registry class for Use Case implementation. They are basically meaningfull lists with some constraints.
 Project-URL: Homepage, https://github.com/Tomperez98/use-case-registry
 Project-URL: Documentation, https://tomperez98.github.io/use-case-registry/
 Project-URL: Issues, https://github.com/Tomperez98/use-case-registry/issues
 Project-URL: Source, https://github.com/Tomperez98/use-case-registry
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-Expression: MIT
@@ -13,25 +13,31 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
+Requires-Dist: pyyaml
+Requires-Dist: pyyaml-env-tag
 Requires-Dist: result
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mkdocs-material; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-env; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: toml; extra == 'dev'
+Requires-Dist: types-pyyaml; extra == 'dev'
+Provides-Extra: sqlalchemy
+Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Description-Content-Type: text/markdown
 
 # use-case-registry
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Build Status](https://github.com/Tomperez98/use-case-registry/workflows/test/badge.svg?branch=main&event=push)](https://github.com/Tomperez98/use-case-registry/actions?query=workflow%3Atest)
 [![Coverage badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Tomperez98/use-case-registry/python-coverage-comment-action-data/endpoint.json)](https://htmlpreview.github.io/?https://github.com/Tomperez98/use-case-registry/blob/python-coverage-comment-action-data/htmlcov/index.html)
```

