# Comparing `tmp/incipyt-0.2.0.tar.gz` & `tmp/incipyt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incipyt-0.2.0.tar", last modified: Sat May 28 15:09:03 2022, max compression
+gzip compressed data, was "incipyt-0.3.0.tar", last modified: Sun Apr  9 13:14:49 2023, max compression
```

## Comparing `incipyt-0.2.0.tar` & `incipyt-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,57 @@
--rw-r--r--   0        0        0     1376 2022-05-26 11:37:40.198545 incipyt-0.2.0/.github/workflows/release-please.yml
--rw-r--r--   0        0        0     2411 2022-05-26 19:56:29.228113 incipyt-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1959 2022-05-26 11:37:40.209329 incipyt-0.2.0/.gitignore
--rw-r--r--   0        0        0     1222 2022-05-28 15:00:15.081016 incipyt-0.2.0/.gitmessage
--rw-r--r--   0        0        0      917 2022-05-26 11:37:40.210331 incipyt-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3577 2022-05-28 15:00:15.099524 incipyt-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1088 2022-05-26 11:37:40.211331 incipyt-0.2.0/LICENSE
--rw-r--r--   0        0        0     2132 2022-05-28 15:00:15.100528 incipyt-0.2.0/README.md
--rw-r--r--   0        0        0        0 2022-05-26 11:37:40.212332 incipyt-0.2.0/incipyt/__init__.py
--rw-r--r--   0        0        0     4311 2022-05-28 15:00:15.126575 incipyt-0.2.0/incipyt/__main__.py
--rw-r--r--   0        0        0        0 2022-05-26 11:37:40.212332 incipyt-0.2.0/incipyt/_internal/__init__.py
--rw-r--r--   0        0        0     2138 2022-05-26 11:37:40.213332 incipyt-0.2.0/incipyt/_internal/dumpers.py
--rw-r--r--   0        0        0      435 2022-05-26 11:37:40.213332 incipyt-0.2.0/incipyt/_internal/sanitizers.py
--rw-r--r--   0        0        0    15770 2022-05-26 11:37:40.213332 incipyt-0.2.0/incipyt/_internal/templates.py
--rw-r--r--   0        0        0     2997 2022-05-26 13:27:13.115378 incipyt-0.2.0/incipyt/_internal/utils.py
--rw-r--r--   0        0        0     3815 2022-05-26 11:37:40.214332 incipyt-0.2.0/incipyt/commands.py
--rw-r--r--   0        0        0     9398 2022-05-26 11:37:40.215332 incipyt-0.2.0/incipyt/project.py
--rw-r--r--   0        0        0      249 2022-05-26 11:37:40.215332 incipyt-0.2.0/incipyt/signals.py
--rw-r--r--   0        0        0      174 2022-05-26 11:37:40.216333 incipyt-0.2.0/incipyt/tools/__init__.py
--rw-r--r--   0        0        0      698 2022-05-26 11:37:40.216333 incipyt-0.2.0/incipyt/tools/base.py
--rw-r--r--   0        0        0     2221 2022-05-28 15:00:15.127592 incipyt-0.2.0/incipyt/tools/git.py
--rw-r--r--   0        0        0     6513 2022-05-28 15:00:15.128592 incipyt-0.2.0/incipyt/tools/setuptools.py
--rw-r--r--   0        0        0      709 2022-05-28 15:00:15.129593 incipyt-0.2.0/incipyt/tools/venv.py
--rw-r--r--   0        0        0     2278 2022-05-28 15:00:15.154878 incipyt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-26 11:37:40.218333 incipyt-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2995 2022-05-26 11:37:40.218333 incipyt-0.2.0/tests/test_dumpers.py
--rw-r--r--   0        0        0     5829 2022-05-26 11:37:40.219333 incipyt-0.2.0/tests/test_project.py
--rw-r--r--   0        0        0     3654 2022-05-26 11:37:40.219333 incipyt-0.2.0/tests/test_renderers.py
--rw-r--r--   0        0        0     9126 2022-05-26 11:37:40.220333 incipyt-0.2.0/tests/test_templates.py
--rw-r--r--   0        0        0      432 2022-05-26 11:37:40.220333 incipyt-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0      271 2022-05-26 11:37:40.220333 incipyt-0.2.0/tests/utils.py
--rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 incipyt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      335 2023-04-09 13:14:29.363232 incipyt-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1576 2023-04-09 13:14:29.363232 incipyt-0.3.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1552 2023-04-09 13:14:29.363232 incipyt-0.3.0/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0     2241 2023-04-09 13:14:29.363232 incipyt-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1826 2023-04-09 13:14:29.363232 incipyt-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1192 2023-04-09 13:14:29.363232 incipyt-0.3.0/.gitmessage
+-rw-r--r--   0        0        0      803 2023-04-09 13:14:29.363232 incipyt-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5709 2023-04-09 13:14:29.363232 incipyt-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2023-04-09 13:14:29.363232 incipyt-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2065 2023-04-09 13:14:29.363232 incipyt-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/__init__.py
+-rw-r--r--   0        0        0     5484 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/_internal/__init__.py
+-rw-r--r--   0        0        0     2056 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/_internal/dumpers.py
+-rw-r--r--   0        0        0      414 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/_internal/sanitizers.py
+-rw-r--r--   0        0        0    15570 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/_internal/templates.py
+-rw-r--r--   0        0        0     2900 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/_internal/utils.py
+-rw-r--r--   0        0        0     4746 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/commands.py
+-rw-r--r--   0        0        0    10044 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/project.py
+-rw-r--r--   0        0        0      240 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/signals.py
+-rw-r--r--   0        0        0       40 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/README.md
+-rw-r--r--   0        0        0     9132 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/Apache-2.0.txt
+-rw-r--r--   0        0        0     1268 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/BSD-2-Clause.txt
+-rw-r--r--   0        0        0     1460 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/BSD-3-Clause.txt
+-rw-r--r--   0        0        0    16375 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/CDDL-1.0.txt
+-rw-r--r--   0        0        0       45 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/Copyright.txt
+-rw-r--r--   0        0        0    14134 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/EPL-2.0.txt
+-rw-r--r--   0        0        0    17669 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/GPL-2.0.txt
+-rw-r--r--   0        0        0    34438 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/GPL-3.0.txt
+-rw-r--r--   0        0        0    24942 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/LGPL-2.0.txt
+-rw-r--r--   0        0        0    25972 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/licenses/LGPL-2.1.txt
+-rw-r--r--   0        0        0     7441 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/licenses/LGPL-3.0.txt
+-rw-r--r--   0        0        0     1055 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/licenses/MIT.txt
+-rw-r--r--   0        0        0    14944 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/licenses/MPL-2.0.txt
+-rw-r--r--   0        0        0     1826 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/python.gitignore
+-rw-r--r--   0        0        0        0 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/{PROJECT_NAME}/__init__.py
+-rw-r--r--   0        0        0      250 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/base.py
+-rw-r--r--   0        0        0     2646 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/git.py
+-rw-r--r--   0        0        0     1703 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/license.py
+-rw-r--r--   0        0        0      234 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/__init__.py
+-rw-r--r--   0        0        0     4541 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/base.py
+-rw-r--r--   0        0        0     1093 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/flit.py
+-rw-r--r--   0        0        0     1093 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/hatch.py
+-rw-r--r--   0        0        0     1083 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/pdm.py
+-rw-r--r--   0        0        0     1049 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/setuptools.py
+-rw-r--r--   0        0        0     5031 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/poetry.py
+-rw-r--r--   0        0        0      733 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/venv.py
+-rw-r--r--   0        0        0     2407 2023-04-09 13:14:29.367232 incipyt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2822 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/test_dumpers.py
+-rw-r--r--   0        0        0     5311 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/test_project.py
+-rw-r--r--   0        0        0     3437 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/test_renderers.py
+-rw-r--r--   0        0        0     8212 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/test_templates.py
+-rw-r--r--   0        0        0      411 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0      262 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/utils.py
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 incipyt-0.3.0/PKG-INFO
```

### Comparing `incipyt-0.2.0/.github/workflows/test.yml` & `incipyt-0.3.0/.github/workflows/test.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,80 @@
-name: CI - Test package
-
-on:
-  push:
-    branches: [main]
-    paths: [pyproject.toml, incipyt/**, tests/**, .github/workflows/test.yml]
-
-  pull_request:
-    branches: [main]
-    types: [opened, reopened, synchronize, ready_for_review]
-    paths: [pyproject.toml, incipyt/**, tests/**, .github/workflows/test.yml]
-
-
-jobs:
-  lint:
-    name: Lint
-    runs-on: ubuntu-latest
-    if: github.event.pull_request.draft == false
-
-    steps:
-    - name: Checkout
-      uses: actions/checkout@v2
-    - name: Set up Python
-      uses: actions/setup-python@v2
-      with:
-        python-version: '3.10'
-    - name: Cache python env
-      uses: actions/cache@v2
-      with:
-        path: ${{ env.pythonLocation }}
-        key: ${{ runner.os }}-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}
-    - name: Install deps
-      env:
-        PIP_UPGRADE: True
-        PIP_UPGRADE_STRATEGY: eager
-      run: |
-        python -m pip install pip flit
-        python -m flit install --pth-file --deps develop
-    - name: Check format with black
-      run: python -m black -v --check .
-    - name: Lint with flakeheaven
-      run: python -m flakeheaven lint -v incipyt
-
-  test:
-    name: Tests
-    needs: lint
-    strategy:
-      matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.7', '3.8', '3.9', '3.10']
-      fail-fast: false
-    runs-on: ${{ matrix.os }}
-    env:
-      _OS: ${{ matrix.os }}
-      _PY: ${{ matrix.python-version }}
-
-    steps:
-    - name: Checkout
-      uses: actions/checkout@v2
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-    - name: Cache python env
-      uses: actions/cache@v2
-      with:
-        path: ${{ env.pythonLocation }}
-        key: ${{ runner.os }}-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}
-    - name: Install deps
-      env:
-        PIP_UPGRADE: True
-        PIP_UPGRADE_STRATEGY: eager
-      run: |
-        python -m pip install pip flit
-        python -m flit install --pth-file --deps develop
-    - name: Run tests with pytest
-      run: pytest -v --cov=incipyt --cov-report=xml
-    - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v1
-      with:
-        fail_ci_if_error: true
-        env_vars: _OS,_PY
+name: CI - Test package
+
+concurrency:
+  cancel-in-progress: true
+  group: ${{ github.workflow }}-${{ github.head_ref || github.ref_name }}
+
+on:
+  push:
+    branches: [main]
+    paths: [pyproject.toml, incipyt/**, tests/**, .github/workflows/test.yml]
+
+  pull_request:
+    branches: [main]
+    types: [opened, reopened, synchronize, ready_for_review, unlocked]
+    paths: [pyproject.toml, incipyt/**, tests/**, .github/workflows/test.yml]
+
+jobs:
+  lint:
+    name: Pre-commit (include linter)
+    runs-on: ubuntu-latest
+    if: github.event.pull_request.draft == false
+
+    steps:
+    - name: Checkout
+      uses: actions/checkout@v3.5.0
+    - name: Set up Python
+      uses: actions/setup-python@v4.5.0
+      with:
+        cache: pip
+        cache-dependency-path: pyproject.toml
+        check-latest: true
+        python-version: 3.11
+    - name: Install deps
+      env:
+        PIP_UPGRADE: True
+        PIP_UPGRADE_STRATEGY: eager
+      run: python -m pip install -e ".[dev]"
+    - name: Pre-commit cache
+      uses: actions/cache@v3.3.1
+      with:
+        key: ${{ hashFiles('.pre-commit-config.yaml') }}
+        path: ~/.cache/pre-commit
+    - name: Run pre-commit on all files
+      run: pre-commit run --all-files
+
+  test:
+    name: Tests
+    needs: lint
+    strategy:
+      matrix:
+        os: [ubuntu-latest, macos-latest, windows-latest]
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+      fail-fast: false
+    runs-on: ${{ matrix.os }}
+    env:
+      _OS: ${{ matrix.os }}
+      _PY: ${{ matrix.python-version }}
+
+    steps:
+    - name: Checkout
+      uses: actions/checkout@v3.5.0
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v4.5.0
+      with:
+        cache: pip
+        cache-dependency-path: pyproject.toml
+        check-latest: true
+        python-version: ${{ matrix.python-version }}
+    - name: Install deps
+      env:
+        PIP_UPGRADE: True
+        PIP_UPGRADE_STRATEGY: eager
+      run: python -m pip install -e ".[test]"
+    - name: Run tests with pytest
+      run: pytest -v --cov=incipyt --cov-report=xml
+    - name: Upload coverage to Codecov
+      uses: codecov/codecov-action@v3.1.1
+      with:
+        fail_ci_if_error: true
+        env_vars: _OS,_PY
```

### Comparing `incipyt-0.2.0/.gitmessage` & `incipyt-0.3.0/.gitmessage`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-
-
-## type(scope): title under 50 chars
-##
-## Mandatory paragraph explaining WHY the changes are needed.
-##
-## Optional paragraphs detailing the changes.
-##
-## Closes #x
-## Co-authored-by: John <john.doe@example.com>
-#
-# The commit type should be one of: chore, feat, fix, perf, ref, rev.
-# The scope is optional, it should be set when the changes are related
-# to a plugin e.g. "fix(sphinx): broken home page url".
-#
-# Remember that this commit message will be read on two occasions:
-#
-# * during the code review, tonight, "what am I reviewing again?"
-# * during a git blame, in 5 years, "why is this line needed again?"
-#
-# During a code review, we expect to understand the overall system and
-# all the implications of your changes. The commit message should
-# contain an abstract of the system being modified and recall the
-# purpose of the changes.
-#
-# During a git-blame, we expect to remember the purpose of a specific
-# line of code. Reading the commit diff and the commit message should
-# give all the necessary information. If you don't feel like all your
-# changes are correctly explained, maybe you should add a comment in
-# the source code or isolate some changes in a new commit.
+
+
+## type(scope): title under 50 chars
+##
+## Mandatory paragraph explaining WHY the changes are needed.
+##
+## Optional paragraphs detailing the changes.
+##
+## Closes #x
+## Co-authored-by: John <john.doe@example.com>
+#
+# The commit type should be one of: chore, feat, fix, perf, ref, rev.
+# The scope is optional, it should be set when the changes are related
+# to a plugin e.g. "fix(sphinx): broken home page url".
+#
+# Remember that this commit message will be read on two occasions:
+#
+# * during the code review, tonight, "what am I reviewing again?"
+# * during a git blame, in 5 years, "why is this line needed again?"
+#
+# During a code review, we expect to understand the overall system and
+# all the implications of your changes. The commit message should
+# contain an abstract of the system being modified and recall the
+# purpose of the changes.
+#
+# During a git-blame, we expect to remember the purpose of a specific
+# line of code. Reading the commit diff and the commit message should
+# give all the necessary information. If you don't feel like all your
+# changes are correctly explained, maybe you should add a comment in
+# the source code or isolate some changes in a new commit.
```

### Comparing `incipyt-0.2.0/LICENSE` & `incipyt-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Not a Name
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Not a Name
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `incipyt-0.2.0/README.md` & `incipyt-0.3.0/README.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# incipyt
-
-*It begins...*
-
-incipyt \[ˈɪŋkɪpɪt̪\] is a command-line tool that bootstraps a Python project.
-
-	$ pip install incipyt
-
-## Usage
-
-incipyt is *not* opinated, by default it setups the tools recommanded in the
-[PyPA/packaging-projects] tutorial: [pyproject.toml] and [setuptools] in
-addition to [git] and [sphinx] which are de-facto standard.
-
-	$ python -m incipyt mynewproject
-	Project Name [mynewproject]:
-	Author [John Doe]:
-	Author email [john.doe@users.noreply.github.com]: john.doe@example.com
-	$ tree mynewproject
-	mynewproject/
-	├── .git/
-	├── docs/
-	│   ├── _build/
-	│   ├── _static/
-	│   ├── _templates/
-	│   ├── conf.py
-	│   ├── index.rst
-	│   ├── make.bat
-	│   └── Makefile
-	├── mynewproject/
-	│   └── __init__.py
-	├── tests/
-	├── .gitignore
-	├── LICENSE
-	├── pyproject.toml
-	├── README.md
-	├── setup.cfg
-	└── setup.py
-
-incipyt provides a rich command line interface so you can choose various build
-systems, version control system, virtual environments, documentation software,
-linters, formatters, etc.
-
-	$ python -m incipyt --help
-
-## Contribute
-
-incipyt is released under the MIT license and is open to contributions
-
-The complete setup instruction are found on the [dev-instructions]. Below is
-the minimum to get started:
-
-    $ git clone https://github.com/NotANameServer/incipyt
-    $ cd incipyt
-    $ git config commit.template .gitmessage
-    $ python -m venv --upgrade-deps .env
-    $ source .env/bin/activate
-    $ python -m pip install --upgrade flit
-    $ python -m flit install --pth-file --deps develop
-    $ python -m pytest -vv tests
-
-[PyPA/packaging-projects]: https://packaging.python.org/tutorials/packaging-projects/
-[pyproject.toml]: https://www.python.org/dev/peps/pep-0518/
-[setuptools]: https://pypi.org/project/setuptools/
-[git]: https://git-scm.com/
-[sphinx]: https://www.sphinx-doc.org/en/master/
-[dev-instructions]: https://github.com/NotANameServer/incipyt/wiki/Developper-instructions
+# incipyt
+
+*It begins...*
+
+incipyt \[ˈɪŋkɪpɪt̪\] is a command-line tool that bootstraps a Python project.
+
+	$ pip install incipyt
+
+## Usage
+
+incipyt is *not* opinated, by default it setups the tools recommanded in the
+[PyPA/packaging-projects] tutorial: [pyproject.toml] and [setuptools] in
+addition to [git] and [sphinx] which are de-facto standard.
+
+	$ python -m incipyt mynewproject
+	Project Name [mynewproject]:
+	Author [John Doe]:
+	Author email [john.doe@users.noreply.github.com]: john.doe@example.com
+	$ tree mynewproject
+	mynewproject/
+	├── .git/
+	├── docs/
+	│   ├── _build/
+	│   ├── _static/
+	│   ├── _templates/
+	│   ├── conf.py
+	│   ├── index.rst
+	│   ├── make.bat
+	│   └── Makefile
+	├── mynewproject/
+	│   └── __init__.py
+	├── tests/
+	├── .gitignore
+	├── LICENSE
+	├── pyproject.toml
+	├── README.md
+	├── setup.cfg
+	└── setup.py
+
+incipyt provides a rich command line interface so you can choose various build
+systems, version control system, virtual environments, documentation software,
+linters, formatters, etc.
+
+	$ python -m incipyt --help
+
+## Contribute
+
+incipyt is released under the MIT license and is open to contributions
+
+The complete setup instruction are found on the [dev-instructions]. Below is
+the minimum to get started:
+
+    $ git clone https://github.com/NotANameServer/incipyt
+    $ cd incipyt
+    $ git config commit.template .gitmessage
+    $ python -m venv --upgrade-deps .env
+    $ source .env/bin/activate
+    $ python -m pip install --upgrade flit
+    $ python -m flit install --pth-file --deps develop
+    $ python -m pytest -vv tests
+
+[PyPA/packaging-projects]: https://packaging.python.org/tutorials/packaging-projects/
+[pyproject.toml]: https://www.python.org/dev/peps/pep-0518/
+[setuptools]: https://pypi.org/project/setuptools/
+[git]: https://git-scm.com/
+[sphinx]: https://www.sphinx-doc.org/en/master/
+[dev-instructions]: https://github.com/NotANameServer/incipyt/wiki/Developper-instructions
```

### Comparing `incipyt-0.2.0/incipyt/_internal/templates.py` & `incipyt-0.3.0/incipyt/_internal/templates.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,473 +1,468 @@
-"""This module contains classes related to template definition and rendering.
-
-Incipyt mainly uses two kinds of templates: bare template strings that behave
-like builtin Python string formatting. It also provides special wrappers to
-allow easier templating of collections data structures, such as dict-like
-template objects.
-"""
-
-import contextlib
-import logging
-from abc import ABCMeta, abstractmethod
-from collections import abc
-from string import Formatter
-
-import click
-
-from incipyt import project
-from incipyt._internal import utils
-
-logger = logging.getLogger(__name__)
-
-
-class Formattable(metaclass=ABCMeta):
-    @abstractmethod
-    def format(self):  # noqa: A003
-        raise NotImplementedError
-
-
-class StringTemplate(Formattable):
-    """This class acts like a wrapper around a format string.
-
-    When an instance is called, it renders the underlying format string using
-    environ values and overrides.
-    """
-
-    def __init__(
-        self, format_string, confirmed=False, sanitizer=None, value_error=True, **kwargs
-    ):
-        r"""This class acts like a wrapper around a format string.
-
-        When an instance is called, it renders the underlying format string
-        using environ values and overrides.
-
-        :param format_string: A format string whose keyword argument will be substituted.
-        :type format_string: :class:`str`
-        :param confirmed: Confirmed status for new variables from keyword args.
-        :type confirmed: :class:`bool`, optionnal
-        :param sanitizer: An optionnal callable to sanitize the values given (key, value) pairs.
-        :type sanitizer: :class:`function` or `None`, optionnal
-        :param value_error: Empty values generate errors.
-        :type value_error: :class:`bool`
-        :param \**kwargs: Variables overrides that will be used for rendering and pushed to the environ.
-            Automatically wrapped in :class:`incipyt._internal.utils.EnvValue` if needed.
-        :type \**kwargs: :class:`str`, optionnal
-        """
-        self._confirmed = confirmed
-        self._sanitizer = sanitizer
-        self._value_error = value_error
-        self._format_string = format_string
-        self._kwargs = kwargs
-
-    def __eq__(self, other):
-        return utils.attrs_eq(
-            self,
-            other,
-            "_format_string",
-            "_confirmed",
-            "_sanitizer",
-            "_value_error",
-            "_kwargs",
-        )
-
-    def __hash__(self):
-        return utils.attrs_hash(
-            self,
-            "_format_string",
-            "_confirmed",
-            "_sanitizer",
-            "_value_error",
-            **self._kwargs,
-        )
-
-    def format(self):  # noqa: A003
-        """Format the underlying format string using variables from the environ.
-
-        :return: The formatted string.
-        :rtype: :class:`str`
-        """
-        return FormatterEnviron(
-            sanitizer=self._sanitizer, value_error=self._value_error
-        ).format(
-            self._format_string,
-            **{
-                key: (
-                    value
-                    if isinstance(value, utils.EnvValue)
-                    else utils.EnvValue(value, confirmed=self._confirmed)
-                )
-                for key, value in self._kwargs.items()
-            },
-        )
-
-    def __repr__(self):
-        return utils.make_repr(
-            self,
-            format_string=self._format_string,
-            confirmed=self._confirmed,
-            sanitizer=self._sanitizer,
-            value_error=self._value_error,
-            kwargs=self._kwargs,
-        )
-
-    @classmethod
-    def wrap(cls, value):
-        return value if isinstance(value, Formattable) else cls(value)
-
-
-class ChoiceTemplate(Formattable):
-    """Class to hold multiple values for a single key.
-
-    When an instance is called, the user will be asked to pick a value using
-    the command line interface.
-    """
-
-    def __init__(self, head, tail):
-        """Class to hold multiple string for a single key.
-
-        When an instance is called, the user will be asked to pick a string
-        using the command line interface.
-
-        :param head: Entry to put a the head of the stack.
-        :type tail: :class:str
-        :param tail: Tail of the stack.
-        :type tail: :class:`incipyt._intternal.templates.ChoiceTemplate` or any bare value
-        """
-        self._values = (
-            {StringTemplate.wrap(head)} | tail._values
-            if isinstance(tail, ChoiceTemplate)
-            else {
-                StringTemplate.wrap(head),
-                StringTemplate.wrap(tail),
-            }
-        )
-
-    def format(self):  # noqa: A003
-        """Ask the user to pick a value using the command line interface.
-
-        If it is :class:`incipyt._internal.templates.Formattable`, it will be formatted.
-
-        :return: The user-choosen value.
-        """
-        return click.prompt(
-            "Conflicting configuration, choose between",
-            type=click.Choice(
-                [
-                    value.format() if isinstance(value, Formattable) else value
-                    for value in self._values
-                ]
-            ),
-        )
-
-    def __eq__(self, other):
-        return utils.attrs_eq(self, other, "_values")
-
-    def __hash__(self):
-        return hash(tuple(self._values))
-
-    def __repr__(self):
-        return f"{type(self).__name__}({self._values})"
-
-    @classmethod
-    def from_items(cls, *args):
-        r"""Build a class instance from any number of bare values.
-
-        :param \*args: Entries to wrap.
-        :return: New class instance
-        :rtype: :class:`incipyt._intternal.templates.ChoiceTemplate`
-        """
-        instance = cls.__new__(cls)
-        instance._values = {StringTemplate.wrap(arg) for arg in args}
-        return instance
-
-
-class TemplateDict(abc.MutableMapping):
-    """Proxy class around a provided mapping.
-
-    This is itended to ease configuration templating.
-
-    :Class instanciation:
-
-    >>> cfg = TemplateDict({})
-
-    :Setting values:
-
-    Following exemples assume `cfg` is a :class:`incipyt._internal.templates.StringTemplate` around an empty `dict`.
-
-    Bare values will be wrapped into :class:`incipyt._internal.templates.StringTemplate`
-    automatically :
-
-    >>> cfg["key"] = "{VARIABLE_NAME}"
-    >>> print(cfg)
-        TemplateDict(data={'key': StringTemplate(format_string={VARIABLE_NAME})})
-
-    :class:`incipyt._internal.templates.Formattable` will be kept as-is:
-
-    >>> cfg["key"] = a_formattable
-    >>> print(cfg)
-        TemplateDict(data={'key': a_formattable})
-
-    Collections are supported as well:
-
-    >>> cfg["key"] = ["{VARIABLE_NAME}"]
-    >>> print(cfg)
-        TemplateDict(data={'key': [StringTemplate("{VARIABLE_NAME}")]})
-
-    >>> cfg["key"] = {"keyB": "{VARIABLE_NAME}"}
-    >>> print(cfg)
-        TemplateDict(data={'key': {'keyB': StringTemplate(format_string={VARIABLE_NAME})}})
-
-    :Nested keys:
-
-    To ease nested structure definition, the following syntax is supported:
-
-    >>> cfg["keyA", "keyB"] = "{VARIABLE_NAME}"
-    >>> print(cfg)
-        TemplateDict(data={'keyA': {'keyB': StringTemplate(format_string={VARIABLE_NAME})}})
-
-    :Multiple values:
-
-    Instances of :class:`incipyt._internal.templates.ChoiceTemplate` will be
-    created in case of value overrides. For instance, if `previous_value` is a
-    :class:`incipyt._internal.templates.Formattable`:
-
-    >>> cfg = TemplateDict({"key": previous_value})
-    >>> cfg["key"] = "{VARIABLE_NAME}"
-    >>> print(cfg)
-        TemplateDict(data={'key': ChoiceTemplate({StringTemplate(format_string={VARIABLE_NAME}), previous_value})})
-
-    If `previous_list` is a mutable sequence, any value not already present in
-    it will be appended:
-
-    >>> cfg = TemplateDict({"key": previous_list})
-    >>> cfg["key"] = ["{VARIABLE_NAME}"]
-    >>> cfg == {"key": previous_list + [StringTemplate("{VARIABLE_NAME}")]}
-        True
-
-    :Inplace union:
-
-    The inplace union operator `|=` can be used to set multiple keys at once:
-
-    >>> cfg = TemplateDict({})
-    >>> cgf |= {"keyA": "{VARIABLE_NAME}", "keyB": "{OTHER_NAME}"}
-    >>> print(cfg)
-        TemplateDict(data={'keyA': StringTemplate(format_string={VARIABLE_NAME}), 'keyB': StringTemplate(format_string={OTHER_NAME})})
-    """
-
-    def __init__(self, data):
-        """Proxy class around a provided mapping.
-
-        This is itended to ease configuration templating.
-
-        :param mapping: Existing mapping holding entries to wrap.
-        :type mapping: :class:`collections.abc.MutableMapping`
-        """
-        self.data = data
-
-    def __getitem__(self, keys):
-        if not utils.is_nonstring_sequence(keys):
-            keys = (keys,)
-
-        config = self.data
-
-        for key in keys:
-            if key not in config:
-                raise KeyError(f"Index [{', '.join(keys)}] does not exist.")
-            config = config[key]
-
-        if isinstance(config, abc.MutableMapping):
-            return TemplateDict(config)
-        elif utils.is_nonstring_sequence(config):
-            return TemplateList(config)
-        else:
-            return config
-
-    def __iter__(self):
-        return iter(self.data)
-
-    def __len__(self):
-        return len(self.data)
-
-    def __repr__(self):
-        return utils.make_repr(self, "data")
-
-    def __delitem__(self, key):
-        raise NotImplementedError(
-            f"{type(self)} do not support __delitem__, add-only dict-like."
-        )
-
-    def __setitem__(self, keys, value):
-        if utils.is_nonstring_sequence(keys):
-            config = self.data
-
-            for key in keys[:-1]:
-                if key not in config:
-                    config[key] = {}
-                config = config[key]
-
-            self[keys[:-1]][keys[-1]] = value
-            return
-
-        if isinstance(value, abc.Mapping):
-            if keys not in self.data:
-                self.data[keys] = {}
-
-            if utils.is_nonstring_sequence(self.data[keys]):
-                raise TypeError(
-                    f"{self.data[keys]}) is already a sequence, cannot set to a dict."
-                )
-            for k, v in value.items():
-                TemplateDict(self.data[keys])[k] = v
-
-        elif utils.is_nonstring_sequence(value):
-            if keys not in self.data:
-                self.data[keys] = []
-
-            if isinstance(self.data[keys], abc.Mapping):
-                raise TypeError(
-                    f"{self.data[keys]} is already a mapping, cannot set to a list."
-                )
-            TemplateList(self.data[keys]).extend(value)
-
-        else:
-            if keys in self.data:
-                self.data[keys] = ChoiceTemplate(value, self.data[keys])
-            else:
-                self.data[keys] = StringTemplate.wrap(value)
-
-    def __ior__(self, other):
-        self.update(other)
-        return self
-
-
-class TemplateList(abc.MutableSequence):
-    """Proxy class around a provided mapping.
-
-    This is itended to ease configuration templating.
-
-    See :class:`incipyt._internal.templates.StringTemplate` for usage details.
-    """
-
-    def __init__(self, data):
-        """Proxy class around a provided sequence.
-
-        This is itended to ease configuration templating.
-
-        :param mapping: Existing mapping holding entries to wrap.
-        :type mapping: :class:`collections.abc.MutableSequence`
-        """
-        self.data = data
-
-    def __getitem__(self, index):
-        if utils.is_nonstring_sequence(self.data[index]):
-            return TemplateList(self.data[index])
-        elif isinstance(self.data[index], abc.MutableMapping):
-            return TemplateDict(self.data[index])
-        else:
-            return self.data[index]
-
-    def __len__(self):
-        return len(self.data)
-
-    def __repr__(self):
-        return utils.make_repr(self, "data")
-
-    def __eq__(self, other):
-        return utils.attrs_eq(self, other, "data")
-
-    def __setitem__(self, index, value):
-        raise NotImplementedError(
-            f"{type(self)} do not support __setitem__, add-only list-like."
-        )
-
-    def __delitem__(self, value):
-        raise NotImplementedError(
-            f"{type(self)} do not support del, add-only list-like."
-        )
-
-    def insert(self, index, value):
-        if utils.is_nonstring_sequence(value):
-            self.data.insert(index, [])
-            TemplateList(self.data[index]).extend(value)
-        elif isinstance(value, abc.Mapping):
-            self.data.insert(index, {})
-            TemplateDict(self.data[index]).update(value)
-        else:
-            new_value = StringTemplate.wrap(value)
-            if new_value not in self.data:
-                self.data.insert(index, new_value)
-
-
-class FormatterEnviron(abc.Mapping):
-    """Class wrapping an environ and providing an interface to render templates.
-
-    It can be used to render template strings.
-    """
-
-    def __init__(self, sanitizer=None, value_error=True):
-        """Class wrapping an environ and providing an interface to render templates.
-
-        :param sanitizer: An optionnal callable to sanitize the values given (key, value) pairs.
-        :type sanitizer: :class:`function` or `None`, optionnal
-        :param environ: Consider empty string value as an error.
-        :type environ: :class:`bool`, optional
-        """
-        self.data = project.environ
-        self._keys = set()
-        self._sanitizer = sanitizer
-        self._value_error = value_error
-
-    def __contains__(self, key):
-        if key not in self.data:
-            self.data.__getitem__(key)
-
-        return True
-
-    def __getitem__(self, key):
-        # Call to inner dict __getitem__ will create missing keys
-        value = self.data[key]
-        if self._value_error and not value:
-            raise ValueError
-
-        return self._sanitizer(key, value) if self._sanitizer else value
-
-    def __iter__(self):
-        return iter(self._keys)
-
-    def __len__(self):
-        return len(self._keys)
-
-    def keys(self):
-        return iter(self)
-
-    def values(self):
-        return (self[key] for key in self)
-
-    def items(self):
-        return zip(self.keys(), self.values())
-
-    def format(self, format_string, **kwargs):  # noqa: A003
-        r"""Render a format string.
-
-        Variables will be request from the underlying environ, and undefined
-        variables will be created. If `self._value_error` is `True` and an
-        empty variable will cause the whole render result to be `None`.
-
-        Additional variables can be specified using keyword arguments. They
-        will be added to the environ, hence they will override environ values.
-
-        :param template: A format string whose keyword argument will be substituted.
-        :type template: :class:`str`
-        :param \**kwargs: Additional variables that will override environ variables.
-        :type \**kwargs: :class:`str`, optionnal
-        :return: The rendered template or `None` if a context variable is empty.
-        :rtype: :class:`str` or `None`
-        """
-
-        self._keys = {item[1] for item in Formatter().parse(format_string) if item[1]}
-        for key in self:
-            if key in kwargs:
-                self.data[key] = kwargs[key]
-
-        with contextlib.suppress(ValueError):
-            return format_string.format(**self)
+"""This module contains classes related to template definition and rendering.
+
+Incipyt mainly uses two kinds of templates: bare template strings that behave
+like builtin Python string formatting. It also provides special wrappers to
+allow easier templating of collections data structures, such as dict-like
+template objects.
+"""
+
+import contextlib
+import logging
+from abc import ABCMeta, abstractmethod
+from collections import abc
+from pathlib import Path
+from string import Formatter
+
+import click
+
+import incipyt
+from incipyt import project
+from incipyt._internal import utils
+
+logger = logging.getLogger(__name__)
+
+
+class Formattable(metaclass=ABCMeta):
+    @abstractmethod
+    def format(self):  # noqa: A003
+        raise NotImplementedError
+
+
+class StringTemplate(Formattable):
+    """This class acts like a wrapper around a format string.
+
+    When an instance is called, it renders the underlying format string using
+    environ values and overrides.
+    """
+
+    def __init__(
+        self, format_string, confirmed=False, sanitizer=None, value_error=True, **kwargs
+    ):
+        r"""This class acts like a wrapper around a format string.
+
+        When an instance is called, it renders the underlying format string
+        using environ values and overrides.
+
+        :param format_string: A format string whose keyword argument will be substituted.
+        :type format_string: :class:`str`
+        :param confirmed: Confirmed status for new variables from keyword args.
+        :type confirmed: :class:`bool`, optionnal
+        :param sanitizer: An optionnal callable to sanitize the values given (key, value) pairs.
+        :type sanitizer: :class:`function` or `None`, optionnal
+        :param value_error: Empty values generate errors.
+        :type value_error: :class:`bool`
+        :param \**kwargs: Variables overrides that will be used for rendering and pushed to the environ.
+            Automatically wrapped in :class:`incipyt._internal.utils.EnvValue` if needed.
+        :type \**kwargs: :class:`str`, optionnal
+        """
+        self._confirmed = confirmed
+        self._sanitizer = sanitizer
+        self._value_error = value_error
+        self._format_string = format_string
+        self._kwargs = kwargs
+
+    def __eq__(self, other):
+        if isinstance(other, str):
+            return self.format() == other
+        return utils.attrs_eq(
+            self, other, "_format_string", "_confirmed", "_sanitizer", "_value_error", "_kwargs"
+        )
+
+    def __lt__(self, other):
+        if isinstance(other, str):
+            return self.format() < other
+        return self.format() < other.format()
+
+    def __gt__(self, other):
+        if isinstance(other, str):
+            return self.format() > other
+        return self.format() > other.format()
+
+    def __hash__(self):
+        return utils.attrs_hash(
+            self, "_format_string", "_confirmed", "_sanitizer", "_value_error", **self._kwargs
+        )
+
+    def format(self):  # noqa: A003
+        """Format the underlying format string using variables from the environ.
+
+        :return: The formatted string.
+        :rtype: :class:`str`
+        """
+        return FormatterEnviron(sanitizer=self._sanitizer, value_error=self._value_error).format(
+            self._format_string,
+            **{
+                key: (
+                    value
+                    if isinstance(value, utils.EnvValue)
+                    else utils.EnvValue(value, confirmed=self._confirmed)
+                )
+                for key, value in self._kwargs.items()
+            },
+        )
+
+    def __repr__(self):
+        return utils.make_repr(
+            self,
+            format_string=self._format_string,
+            confirmed=self._confirmed,
+            sanitizer=self._sanitizer,
+            value_error=self._value_error,
+            kwargs=self._kwargs,
+        )
+
+    @classmethod
+    def wrap(cls, value):
+        return value if isinstance(value, Formattable) else cls(value)
+
+    @classmethod
+    def from_file(cls, filename):
+        path = Path(incipyt.__file__).parent / "templates" / filename
+        return cls(path.read_text())
+
+
+class ChoiceTemplate(Formattable):
+    """Class to hold multiple values for a single key.
+
+    When an instance is called, the user will be asked to pick a value using
+    the command line interface.
+    """
+
+    def __init__(self, head, tail):
+        """Class to hold multiple string for a single key.
+
+        When an instance is called, the user will be asked to pick a string
+        using the command line interface.
+
+        :param head: Entry to put a the head of the stack.
+        :type tail: :class:str
+        :param tail: Tail of the stack.
+        :type tail: :class:`incipyt._intternal.templates.ChoiceTemplate` or any bare value
+        """
+        self._values = (
+            {StringTemplate.wrap(head)} | tail._values
+            if isinstance(tail, ChoiceTemplate)
+            else {StringTemplate.wrap(head), StringTemplate.wrap(tail)}
+        )
+
+    def format(self):  # noqa: A003
+        """Ask the user to pick a value using the command line interface.
+
+        If it is :class:`incipyt._internal.templates.Formattable`, it will be formatted.
+
+        :return: The user-choosen value.
+        """
+        return click.prompt(
+            "Conflicting configuration, choose between",
+            type=click.Choice(
+                [
+                    value.format() if isinstance(value, Formattable) else value
+                    for value in self._values
+                ]
+            ),
+        )
+
+    def __eq__(self, other):
+        return utils.attrs_eq(self, other, "_values")
+
+    def __hash__(self):
+        return hash(tuple(self._values))
+
+    def __repr__(self):
+        return f"{type(self).__name__}({self._values})"
+
+    @classmethod
+    def from_items(cls, *args):
+        r"""Build a class instance from any number of bare values.
+
+        :param \*args: Entries to wrap.
+        :return: New class instance
+        :rtype: :class:`incipyt._intternal.templates.ChoiceTemplate`
+        """
+        instance = cls.__new__(cls)
+        instance._values = {StringTemplate.wrap(arg) for arg in args}
+        return instance
+
+
+class TemplateDict(abc.MutableMapping):
+    """Proxy class around a provided mapping.
+
+    This is itended to ease configuration templating.
+
+    :Class instanciation:
+
+    >>> cfg = TemplateDict({})
+
+    :Setting values:
+
+    Following exemples assume `cfg` is a :class:`incipyt._internal.templates.StringTemplate` around an empty `dict`.
+
+    Bare values will be wrapped into :class:`incipyt._internal.templates.StringTemplate`
+    automatically :
+
+    >>> cfg["key"] = "{VARIABLE_NAME}"
+    >>> print(cfg)
+        TemplateDict(data={'key': StringTemplate(format_string={VARIABLE_NAME})})
+
+    :class:`incipyt._internal.templates.Formattable` will be kept as-is:
+
+    >>> cfg["key"] = a_formattable
+    >>> print(cfg)
+        TemplateDict(data={'key': a_formattable})
+
+    Collections are supported as well:
+
+    >>> cfg["key"] = ["{VARIABLE_NAME}"]
+    >>> print(cfg)
+        TemplateDict(data={'key': [StringTemplate("{VARIABLE_NAME}")]})
+
+    >>> cfg["key"] = {"keyB": "{VARIABLE_NAME}"}
+    >>> print(cfg)
+        TemplateDict(data={'key': {'keyB': StringTemplate(format_string={VARIABLE_NAME})}})
+
+    :Nested keys:
+
+    To ease nested structure definition, the following syntax is supported:
+
+    >>> cfg["keyA", "keyB"] = "{VARIABLE_NAME}"
+    >>> print(cfg)
+        TemplateDict(data={'keyA': {'keyB': StringTemplate(format_string={VARIABLE_NAME})}})
+
+    :Multiple values:
+
+    Instances of :class:`incipyt._internal.templates.ChoiceTemplate` will be
+    created in case of value overrides. For instance, if `previous_value` is a
+    :class:`incipyt._internal.templates.Formattable`:
+
+    >>> cfg = TemplateDict({"key": previous_value})
+    >>> cfg["key"] = "{VARIABLE_NAME}"
+    >>> print(cfg)
+        TemplateDict(data={'key': ChoiceTemplate({StringTemplate(format_string={VARIABLE_NAME}), previous_value})})
+
+    If `previous_list` is a mutable sequence, any value not already present in
+    it will be appended:
+
+    >>> cfg = TemplateDict({"key": previous_list})
+    >>> cfg["key"] = ["{VARIABLE_NAME}"]
+    >>> cfg == {"key": previous_list + [StringTemplate("{VARIABLE_NAME}")]}
+        True
+
+    :Inplace union:
+
+    The inplace union operator `|=` can be used to set multiple keys at once:
+
+    >>> cfg = TemplateDict({})
+    >>> cgf |= {"keyA": "{VARIABLE_NAME}", "keyB": "{OTHER_NAME}"}
+    >>> print(cfg)
+        TemplateDict(data={'keyA': StringTemplate(format_string={VARIABLE_NAME}), 'keyB': StringTemplate(format_string={OTHER_NAME})})
+    """
+
+    def __init__(self, data):
+        """Proxy class around a provided mapping.
+
+        This is itended to ease configuration templating.
+
+        :param mapping: Existing mapping holding entries to wrap.
+        :type mapping: :class:`collections.abc.MutableMapping`
+        """
+        self.data = data
+
+    def __getitem__(self, keys):
+        if not utils.is_nonstring_sequence(keys):
+            keys = (keys,)
+
+        config = self.data
+
+        for key in keys:
+            if key not in config:
+                raise KeyError(f"Index [{', '.join(keys)}] does not exist.")
+            config = config[key]
+
+        if isinstance(config, abc.MutableMapping):
+            return TemplateDict(config)
+        elif utils.is_nonstring_sequence(config):
+            return TemplateList(config)
+        else:
+            return config
+
+    def __iter__(self):
+        return iter(self.data)
+
+    def __len__(self):
+        return len(self.data)
+
+    def __repr__(self):
+        return utils.make_repr(self, "data")
+
+    def __delitem__(self, key):
+        raise NotImplementedError(f"{type(self)} do not support __delitem__, add-only dict-like.")
+
+    def __setitem__(self, keys, value):
+        if utils.is_nonstring_sequence(keys):
+            config = self.data
+
+            for key in keys[:-1]:
+                if key not in config:
+                    config[key] = {}
+                config = config[key]
+
+            self[keys[:-1]][keys[-1]] = value
+            return
+
+        if isinstance(value, abc.Mapping):
+            if keys not in self.data:
+                self.data[keys] = {}
+
+            if utils.is_nonstring_sequence(self.data[keys]):
+                raise TypeError(
+                    f"{self.data[keys]}) is already a sequence, cannot set to a dict."
+                )
+            for k, v in value.items():
+                TemplateDict(self.data[keys])[k] = v
+
+        elif utils.is_nonstring_sequence(value):
+            if keys not in self.data:
+                self.data[keys] = []
+
+            if isinstance(self.data[keys], abc.Mapping):
+                raise TypeError(f"{self.data[keys]} is already a mapping, cannot set to a list.")
+            TemplateList(self.data[keys]).extend(value)
+
+        else:
+            if keys in self.data:
+                self.data[keys] = ChoiceTemplate(value, self.data[keys])
+            else:
+                self.data[keys] = StringTemplate.wrap(value)
+
+    def __ior__(self, other):
+        self.update(other)
+        return self
+
+
+class TemplateList(abc.MutableSequence):
+    """Proxy class around a provided mapping.
+
+    This is itended to ease configuration templating.
+
+    See :class:`incipyt._internal.templates.StringTemplate` for usage details.
+    """
+
+    def __init__(self, data):
+        """Proxy class around a provided sequence.
+
+        This is itended to ease configuration templating.
+
+        :param mapping: Existing mapping holding entries to wrap.
+        :type mapping: :class:`collections.abc.MutableSequence`
+        """
+        self.data = data
+
+    def __getitem__(self, index):
+        if utils.is_nonstring_sequence(self.data[index]):
+            return TemplateList(self.data[index])
+        elif isinstance(self.data[index], abc.MutableMapping):
+            return TemplateDict(self.data[index])
+        else:
+            return self.data[index]
+
+    def __len__(self):
+        return len(self.data)
+
+    def __repr__(self):
+        return utils.make_repr(self, "data")
+
+    def __eq__(self, other):
+        return utils.attrs_eq(self, other, "data")
+
+    def __setitem__(self, index, value):
+        raise NotImplementedError(f"{type(self)} do not support __setitem__, add-only list-like.")
+
+    def __delitem__(self, value):
+        raise NotImplementedError(f"{type(self)} do not support del, add-only list-like.")
+
+    def insert(self, index, value):
+        if utils.is_nonstring_sequence(value):
+            self.data.insert(index, [])
+            TemplateList(self.data[index]).extend(value)
+        elif isinstance(value, abc.Mapping):
+            self.data.insert(index, {})
+            TemplateDict(self.data[index]).update(value)
+        else:
+            new_value = StringTemplate.wrap(value)
+            if new_value not in self.data:
+                self.data.insert(index, new_value)
+
+
+class FormatterEnviron(abc.Mapping):
+    """Class wrapping an environ and providing an interface to render templates.
+
+    It can be used to render template strings.
+    """
+
+    def __init__(self, sanitizer=None, value_error=True):
+        """Class wrapping an environ and providing an interface to render templates.
+
+        :param sanitizer: An optionnal callable to sanitize the values given (key, value) pairs.
+        :type sanitizer: :class:`function` or `None`, optionnal
+        :param environ: Consider empty string value as an error.
+        :type environ: :class:`bool`, optional
+        """
+        self.data = project.environ
+        self._keys = set()
+        self._sanitizer = sanitizer
+        self._value_error = value_error
+
+    def __contains__(self, key):
+        if key not in self.data:
+            self.data.__getitem__(key)
+
+        return True
+
+    def __getitem__(self, key):
+        # Call to inner dict __getitem__ will create missing keys
+        value = self.data[key]
+        if self._value_error and not value:
+            raise ValueError
+
+        return self._sanitizer(key, value) if self._sanitizer else value
+
+    def __iter__(self):
+        return iter(self._keys)
+
+    def __len__(self):
+        return len(self._keys)
+
+    def keys(self):
+        return iter(self)
+
+    def values(self):
+        return (self[key] for key in self)
+
+    def items(self):
+        return zip(self.keys(), self.values())
+
+    def format(self, format_string, **kwargs):  # noqa: A003
+        r"""Render a format string.
+
+        Variables will be request from the underlying environ, and undefined
+        variables will be created. If `self._value_error` is `True` and an
+        empty variable will cause the whole render result to be `None`.
+
+        Additional variables can be specified using keyword arguments. They
+        will be added to the environ, hence they will override environ values.
+
+        :param template: A format string whose keyword argument will be substituted.
+        :type template: :class:`str`
+        :param \**kwargs: Additional variables that will override environ variables.
+        :type \**kwargs: :class:`str`, optionnal
+        :return: The rendered template or `None` if a context variable is empty.
+        :rtype: :class:`str` or `None`
+        """
+
+        self._keys = {item[1] for item in Formatter().parse(format_string) if item[1]}
+        for key in self:
+            if key in kwargs:
+                self.data[key] = kwargs[key]
+
+        with contextlib.suppress(ValueError):
+            return format_string.format(**self)
```

### Comparing `incipyt-0.2.0/incipyt/_internal/utils.py` & `incipyt-0.3.0/incipyt/_internal/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,95 @@
-import collections.abc
-import dataclasses
-
-from typing import Any
-
-
-@dataclasses.dataclass
-class EnvValue:
-    value: Any
-    update: bool = False
-    confirmed: bool = False
-
-
-def attrs_eq(a, b, *args):
-    r"""Compare two objects according to their attributes.
-
-    :param a: First object to compare.
-    :param b: Second object to compare.
-    :param \*args: Attributes names to check for.
-    :type \*args: :class:`str`
-    :return: `True` if all provided attributes of objects `a` and `b` are equals.
-    :rtype: :class:`bool`
-    """
-    try:
-        return all(getattr(a, attr) == getattr(b, attr) for attr in args)
-    except AttributeError:
-        return False
-
-
-def attrs_hash(a, *args, **kwargs):
-    return hash(tuple(getattr(a, attr) for attr in args) + tuple(kwargs.items()))
-
-
-def is_nonstring_sequence(obj):
-    """Check if a given object is a non-string sequence.
-
-    :param obj: Any object to check.
-    :return: `True` if `obj` is a non-string :class:`Sequence` instance.
-    :rtype: :class:`bool`
-    """
-    return (
-        isinstance(obj, collections.abc.Sequence)
-        and not isinstance(obj, collections.abc.ByteString)
-        and not isinstance(obj, str)
-    )
-
-
-def make_repr(obj, *args, **kwargs):
-    r"""Make a representation string with ease.
-
-    :param obj: Any object to make a representation for.
-    :param \*args: Attributes names to include.
-    :type \*args: :class:`str`
-    :param \**kwargs: Other `attribute_name=any_value` to include.
-    :return: String representation of `obj`.
-    :rtype: :class:`str`
-    """
-    from_attributes = [f"{a}={getattr(obj, a)}" for a in args]
-    from_kwargs = [f"{k}={v}" for k, v in kwargs.items()]
-    params = ", ".join(from_attributes + from_kwargs)
-
-    return f"""{type(obj).__name__}({params})"""
-
-
-def unfold_dict(config):
-    unfolded_config = {}
-
-    for key_section, value_section in config.items():
-        if isinstance(value_section, collections.abc.Mapping):
-            if key_section not in unfolded_config:
-                unfolded_config[key_section] = {}
-            for key, value in value_section.items():
-                if isinstance(value, collections.abc.Mapping):
-                    unfolded_config[key_section][key] = "\n" + "\n".join(
-                        f"{k} = {v}" for k, v in value.items()
-                    )
-                else:
-                    unfolded_config[key_section][key] = value
-        else:
-            unfolded_config[key_section] = value_section
-
-    return unfolded_config
-
-
-def unfold_list(config):
-    unfolded_config = {}
-
-    for key, value in config.items():
-        if isinstance(value, collections.abc.Mapping):
-            unfolded_config[key] = unfold_list(value)
-        elif is_nonstring_sequence(value):
-            unfolded_config[key] = "\n" + "\n".join(value)
-        else:
-            unfolded_config[key] = value
-
-    return unfolded_config
+import collections.abc
+import dataclasses
+from typing import Any
+
+
+@dataclasses.dataclass
+class EnvValue:
+    value: Any
+    update: bool = False
+    confirmed: bool = False
+
+
+def attrs_eq(a, b, *args):
+    r"""Compare two objects according to their attributes.
+
+    :param a: First object to compare.
+    :param b: Second object to compare.
+    :param \*args: Attributes names to check for.
+    :type \*args: :class:`str`
+    :return: `True` if all provided attributes of objects `a` and `b` are equals.
+    :rtype: :class:`bool`
+    """
+    try:
+        return all(getattr(a, attr) == getattr(b, attr) for attr in args)
+    except AttributeError:
+        return False
+
+
+def attrs_hash(a, *args, **kwargs):
+    return hash(tuple(getattr(a, attr) for attr in args) + tuple(kwargs.items()))
+
+
+def is_nonstring_sequence(obj):
+    """Check if a given object is a non-string sequence.
+
+    :param obj: Any object to check.
+    :return: `True` if `obj` is a non-string :class:`Sequence` instance.
+    :rtype: :class:`bool`
+    """
+    return (
+        isinstance(obj, collections.abc.Sequence)
+        and not isinstance(obj, collections.abc.ByteString)
+        and not isinstance(obj, str)
+    )
+
+
+def make_repr(obj, *args, **kwargs):
+    r"""Make a representation string with ease.
+
+    :param obj: Any object to make a representation for.
+    :param \*args: Attributes names to include.
+    :type \*args: :class:`str`
+    :param \**kwargs: Other `attribute_name=any_value` to include.
+    :return: String representation of `obj`.
+    :rtype: :class:`str`
+    """
+    from_attributes = [f"{a}={getattr(obj, a)}" for a in args]
+    from_kwargs = [f"{k}={v}" for k, v in kwargs.items()]
+    params = ", ".join(from_attributes + from_kwargs)
+
+    return f"""{type(obj).__name__}({params})"""
+
+
+def unfold_dict(config):
+    unfolded_config = {}
+
+    for key_section, value_section in config.items():
+        if isinstance(value_section, collections.abc.Mapping):
+            if key_section not in unfolded_config:
+                unfolded_config[key_section] = {}
+            for key, value in value_section.items():
+                if isinstance(value, collections.abc.Mapping):
+                    unfolded_config[key_section][key] = "\n" + "\n".join(
+                        f"{k} = {v}" for k, v in value.items()
+                    )
+                else:
+                    unfolded_config[key_section][key] = value
+        else:
+            unfolded_config[key_section] = value_section
+
+    return unfolded_config
+
+
+def unfold_list(config):
+    unfolded_config = {}
+
+    for key, value in config.items():
+        if isinstance(value, collections.abc.Mapping):
+            unfolded_config[key] = unfold_list(value)
+        elif is_nonstring_sequence(value):
+            unfolded_config[key] = "\n" + "\n".join(value)
+        else:
+            unfolded_config[key] = value
+
+    return unfolded_config
```

### Comparing `incipyt-0.2.0/incipyt/commands.py` & `incipyt-0.3.0/incipyt/commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,133 @@
-"""Functions to call system programs and python modulse."""
-
-import logging
-import os
-import subprocess
-
-from incipyt import project
-
-from incipyt._internal.templates import Formattable
-from incipyt._internal.utils import EnvValue
-
-logger = logging.getLogger(__name__)
-
-
-def run(args, check=True, **kwargs):
-    r"""Run a command after substitution using the environ.
-
-    :param args: List of the command elements.
-    :type args: :class:`list`
-    :param \**kwargs: Other options forwarded to `subprocess.run`
-    :return: Represents a process that has finished
-    :rtype: :class:`subprocess.CompletedProcess`
-    """
-    formatted = [arg.format() if isinstance(arg, Formattable) else arg for arg in args]
-    logger.info(" ".join(formatted))
-    result = subprocess.run(formatted, capture_output=True, check=False, **kwargs)
-    logger.info(result.stdout.decode())
-    if check and result.returncode:
-        logger.error(result.stderr.decode())
-        raise subprocess.CalledProcessError(
-            result.returncode, result.args, output=result.stdout, stderr=result.stderr
-        )
-    return result
-
-
-def setenv_python_cmd(python_path):
-    """Set PYTHON_CMD environment variable.
-
-    :param python_path: List of the command elements.
-    :type python_path: :class:`pathlib.Path`
-    """
-    assert python_path.is_absolute(), f"{python_path} is not absolute."
-    project.environ["PYTHON_CMD"] = EnvValue(os.fspath(python_path), update=True)
-
-
-def python_m(args, **kwargs):
-    r"""Run a python module after substitution using the environ.
-
-    :param args: List of the command elements, excluding `python -m`.
-    :type args: :class:`list`
-    :param \**kwargs: Other options forwarded to `subprocess.run`
-    :return: Represents a process that has finished
-    :rtype: :class:`subprocess.CompletedProcess`
-    """
-    # from incipyt._internal.templates import StringTemplate
-    return run([project.environ["PYTHON_CMD"], "-m"] + args, **kwargs)
-
-
-def build(args, **kwargs):
-    r"""Run a python build after substitution using the environ.
-
-    :param args: List of the command elements, excluding `python -m build`.
-    :type args: :class:`list`
-    :param \**kwargs: Other options forwarded to `subprocess.run`
-    :return: Represents a process that has finished
-    :rtype: :class:`subprocess.CompletedProcess`
-    """
-    return python_m(["build"] + args, **kwargs)
-
-
-def pip(args, **kwargs):
-    r"""Run a pip command after substitution using the environ.
-
-    :param args: List of the command elements, excluding `python -m pip`.
-    :type args: :class:`list`
-    :param \**kwargs: Other options forwarded to `subprocess.run`
-    :return: Represents a process that has finished
-    :rtype: :class:`subprocess.CompletedProcess`
-    """
-    return python_m(["pip", "--verbose"] + args, **kwargs)
-
-
-def pip_install(args, **kwargs):
-    r"""Run a pip install command after substitution using the environ.
-
-    :param args: List of the command elements, excluding `python -m pip`.
-    :type args: :class:`list`
-    :param \**kwargs: Other options forwarded to `subprocess.run`
-    :return: Represents a process that has finished
-    :rtype: :class:`subprocess.CompletedProcess`
-    """
-    return pip(["install", "--upgrade", "--upgrade-strategy", "eager"] + args, **kwargs)
-
-
-def venv(args, **kwargs):
-    r"""Run a venv command after substitution using the environ.
-
-    :param args: List of the command elements, excluding `python -m venv`.
-    :type args: :class:`list`
-    :param \**kwargs: Other options forwarded to `subprocess.run`
-    :return: Represents a process that has finished
-    :rtype: :class:`subprocess.CompletedProcess`
-    """
-    return python_m(["venv"] + args, **kwargs)
+"""Functions to call system programs and python modulse."""
+
+import logging
+import os
+import subprocess
+
+from incipyt import project
+from incipyt._internal.templates import Formattable
+from incipyt._internal.utils import EnvValue
+
+logger = logging.getLogger(__name__)
+
+
+def run(args, check=True, **kwargs):
+    r"""Run a command after substitution using the environ.
+
+    :param args: List of the command elements.
+    :type args: :class:`list`
+    :param \**kwargs: Other options forwarded to `subprocess.run`
+    :return: Represents a process that has finished
+    :rtype: :class:`subprocess.CompletedProcess`
+    """
+    formatted = [arg.format() if isinstance(arg, Formattable) else arg for arg in args]
+    logger.info(" ".join(formatted))
+    result = subprocess.run(formatted, capture_output=True, check=False, **kwargs)
+    logger.info(result.stdout.decode())
+    if check and result.returncode:
+        logger.error(result.stderr.decode())
+        raise subprocess.CalledProcessError(
+            result.returncode, result.args, output=result.stdout, stderr=result.stderr
+        )
+    return result
+
+
+def setenv_python_cmd(python_path):
+    """Set PYTHON_CMD environment variable.
+
+    :param python_path: List of the command elements.
+    :type python_path: :class:`pathlib.Path`
+    """
+    if not python_path.is_absolute():
+        raise AssertionError(f"{python_path} is not absolute.")
+    project.environ["PYTHON_CMD"] = EnvValue(os.fspath(python_path), update=True)
+
+
+def python_m(args, **kwargs):
+    r"""Run a python module after substitution using the environ.
+
+    :param args: List of the command elements, excluding `python -m`.
+    :type args: :class:`list`
+    :param \**kwargs: Other options forwarded to `subprocess.run`
+    :return: Represents a process that has finished
+    :rtype: :class:`subprocess.CompletedProcess`
+    """
+    return run([project.environ["PYTHON_CMD"], "-m", *args], **kwargs)
+
+
+def build(args, **kwargs):
+    r"""Run a python build after substitution using the environ.
+
+    :param args: List of the command elements, excluding `python -m build`.
+    :type args: :class:`list`
+    :param \**kwargs: Other options forwarded to `subprocess.run`
+    :return: Represents a process that has finished
+    :rtype: :class:`subprocess.CompletedProcess`
+    """
+    return python_m(["build", *args], **kwargs)
+
+
+def pip(args, **kwargs):
+    r"""Run a pip command after substitution using the environ.
+
+    :param args: List of the command elements, excluding `python -m pip`.
+    :type args: :class:`list`
+    :param \**kwargs: Other options forwarded to `subprocess.run`
+    :return: Represents a process that has finished
+    :rtype: :class:`subprocess.CompletedProcess`
+    """
+    return python_m(["pip", "--verbose", *args], **kwargs)
+
+
+def pip_install(args, **kwargs):
+    r"""Run a pip install command after substitution using the environ.
+
+    :param args: List of the command elements, excluding `python -m pip`.
+    :type args: :class:`list`
+    :param \**kwargs: Other options forwarded to `subprocess.run`
+    :return: Represents a process that has finished
+    :rtype: :class:`subprocess.CompletedProcess`
+    """
+    return pip(["install", "--upgrade", "--upgrade-strategy", "eager", *args], **kwargs)
+
+
+def venv(args, **kwargs):
+    r"""Run a venv command after substitution using the environ.
+
+    :param args: List of the command elements, excluding `python -m venv`.
+    :type args: :class:`list`
+    :param \**kwargs: Other options forwarded to `subprocess.run`
+    :return: Represents a process that has finished
+    :rtype: :class:`subprocess.CompletedProcess`
+    """
+    return python_m(["venv", *args], **kwargs)
+
+
+def git(args, workon=None, **kwargs):
+    r"""Run a git command inside of the ``workon`` dir.
+
+    :param args: List of the command elements, excluding `git`.
+    :type args: :class:`list`
+    :param workon: Directory where to run the command, instead of .
+    :type workon: :class:`pathlib.Path`
+    :param \**kwargs: Other options forwarded to `subprocess.run`
+    :return: Represents a process that has finished
+    :rtype: :class:`subprocess.CompletedProcess`
+    """
+    return run(["git", "-C", os.fspath(workon), *args] if workon else ["git", *args], **kwargs)
+
+
+def git_get_config(config, workon=None):
+    r"""Retrieve the value of ``git config <config>``.
+
+    :param config: The config name to retrieve
+    :type args: :class:`str`
+    :param workon: Directory where to run the command, instead of .
+    :type workon: :class:`pathlib.Path`
+    :return: The
+    :rtype: :class:`str` | None
+    """
+    cmd = git(["config", config], workon=workon, check=False)
+    if cmd.returncode == 0:
+        return cmd.stdout.decode().strip() or None
+    return None
```

### Comparing `incipyt-0.2.0/incipyt/project.py` & `incipyt-0.3.0/incipyt/project.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,260 +1,278 @@
-"""TO-DO."""
-
-import collections
-import logging
-import os
-import sys
-from collections import abc
-
-import click
-
-from incipyt._internal import templates
-
-from incipyt._internal.utils import EnvValue, is_nonstring_sequence
-
-logger = logging.getLogger(__name__)
-
-
-class _Environ(collections.UserDict):
-    """Manage environ variables using for substitutions in patterns.
-
-    A :class:`Environ` object `environ` is a dictionnary initialized with
-    system environ variables `os.environ`, a variable can be add like that:
-
-    .. code-block::
-
-        environ["VARIABLE_NAME"] = "something"
-
-    However such a variable will not be considered in `environ` before being
-    `confirmed`. Such confirmation will happen the first it is asked for:
-
-    .. code-block::
-
-        var_first = environ["VARIABLE_NAME"]
-        # Prompt a message for confirmation of the value for `VARIABLE_NAME`
-        var_second = environ["VARIABLE_NAME"]
-        # As `VARIABLE_NAME` as been confirmed, don't ask anything
-
-    Moreover, even if a specific variable hasn't been set, it can be asked for
-    it anyway and it will be confirmed immediately. A variable can also be set
-    and confirmed at the same time:
-
-    .. code-block::
-
-        environ["VARIABLE_NAME"] = EnvValue("something", confirmed=True)
-
-    Note that if a variable has been set, it cannot be set again, except if
-    explicitly specified:
-
-    .. code-block::
-
-        environ["VARIABLE_NAME"] = EnvValue("new_value", update=True)
-
-    All iterative methods and in operator consider only `confirmed` variables.
-    """
-
-    def clear(self):
-        self._confirmed = set()
-        self.data = os.environ.copy()
-
-        if "PYTHON_CMD" not in self.data:
-            self.data["PYTHON_CMD"] = sys.executable
-        self._confirmed.add("PYTHON_CMD")
-
-    def __init__(self):
-        self.clear()
-
-    def __getitem__(self, key):
-        if key not in self._confirmed:
-            logger.debug("Missing environ variable %s, request it.", key)
-            self.data[key] = self._prompt(key)
-            self._confirmed.add(key)
-
-        return self.data[key]
-
-    def __setitem__(self, key, env_value):
-        if not isinstance(env_value, EnvValue):
-            env_value = EnvValue(env_value)
-
-        if key in self.data and not env_value.update:
-            raise ValueError(f"Environ variable {key} already exists, use update.")
-
-        logger.debug("Set environ variable %s=%s.", key, env_value.value)
-        self.data[key] = env_value.value
-        if env_value.confirmed and key not in self._confirmed:
-            self._confirmed.add(key)
-
-    def __iter__(self):
-        return iter(self._confirmed)
-
-    def __contains__(self, key):
-        return key in self._confirmed
-
-    def keys(self):  # noqa: D102
-        return self._confirmed
-
-    def values(self):  # noqa: D102
-        return [self.data[key] for key in self._confirmed]
-
-    def items(self):  # noqa: D102
-        return [(key, self.data[key]) for key in self._confirmed]
-
-    def getitems_sanitized(self, keys, sanitizer=None):
-        """Get multiple items at once and sanitize them.
-
-        See also :func:`incipyt.system.Environment.__getitem__`, which will be
-        used to pull each key from the environment.
-
-        :param keys: Required environment keys. If a key is `None`, it will be ignored.
-        :type keys: :class:`collections.abc.Sequence`
-        :param sanitizer: Will be called on key-value pairs to sanitize values.
-        :type sanitizer: :class:`function`
-        :return: Sanitized environment key-value pairs.
-        :rtype: :class:`dict`
-        """
-        return {
-            key: sanitizer(key, self[key]) if sanitizer else self[key]
-            for key in keys
-            if key is not None
-        }
-
-    def _prompt(self, key):
-        return click.prompt(
-            key.replace("_", " ").lower().capitalize(),
-            default=self.data[key] if key in self.data else "",
-            type=str,
-        )
-
-    def __ior__(self, other):
-        self.update(other)
-        return self
-
-
-environ = _Environ()
-
-
-class _Structure:
-    """Represents all configuration and template files to commit for the new project.
-
-    An instance internally stores mappables between path objects and template
-    files or dictionaries modeling configuration files.
-
-    Functions :meth:`get_configuration` and :meth:`register_template` add
-    respectively configuration dictionary and template to the instance.
-
-    When the project structure is finally ready, functions :meth:`mkdir` :meth:`commit`
-    can be used to write folder and files in a new folder after substituting
-    variables in path and files using an :class:`incipyt.project.Environ`.
-    """
-
-    def clear(self):
-        self._configurations = {}
-
-    def __init__(self):
-        self.clear()
-
-    def get_config_dict(self, config_root):
-        """Get a configuration dictionary associated to the relative path `config_root`.
-
-        :param config_root: Relative path of the configuration file.
-        :type config_root: :class:`pathlib.Path`
-        :return: A reference to the configuration dictionary
-        :rtype: :class:`incipyt._internal.templates.TempateDict`
-        """
-        if config_root not in self._configurations:
-            logger.debug(
-                "Register configuration %s in project structure.", str(config_root)
-            )
-            self._configurations[config_root] = {}
-
-        if not isinstance(self._configurations[config_root], abc.MutableMapping):
-            raise TypeError(f"{config_root} is not a dict.")
-        return templates.TemplateDict(self._configurations[config_root])
-
-    def get_config_list(self, config_root):
-        """Get a configuration list associated to the relative path `config_root`.
-
-        :param config_root: Relative path of the configuration file.
-        :type config_root: :class:`pathlib.Path`
-        :return: A reference to the configuration list
-        :rtype: :class:`incipyt._internal.templates.TempateList`
-        """
-        if config_root not in self._configurations:
-            logger.debug(
-                "Register configuration %s in project structure.", str(config_root)
-            )
-            self._configurations[config_root] = []
-
-        if not is_nonstring_sequence(self._configurations[config_root]):
-            raise TypeError(f"{config_root} is not a list.")
-        return templates.TemplateList(self._configurations[config_root])
-
-    def commit(self):
-        """Commit current project structure on disk.
-
-        :raises RuntimeError: If one of the configuration file already exists.
-        """
-        for config_root, config in self._configurations.items():
-            logger.info("Process environ variables for %s.", str(config_root))
-            _Structure._visit(config)
-
-        for config_root, config in self._configurations.items():
-            logger.info("Write configuration file %s.", str(config_root))
-            config_root.dump_in(config)
-
-    def mkdir(self, workon):
-        """Make all directories of the project structure in workon.
-
-        :param workon: Work-on path.
-        :type workon: :class:`pathlib.Path`
-        """
-        for config_root in self._configurations:
-            logger.debug("Commit %s path.", str(config_root))
-            config_root.commit(workon)
-
-        for config_root in self._configurations:
-            logger.info("Mkdir folders for %s.", str(config_root))
-            config_root.mkdir()
-
-    @staticmethod
-    def _visit(template):
-        """Visit the `template` nested-dictionary structure.
-
-        All :class:`incipyt._internal.templates.Formattable` values of the template dictionary will be
-        evaluated and replaced by their results. All nested structures will be recursively
-        visited and processed too.
-
-        :param template: The template dictionary or list to visit.
-        :type template: :class:`collections.abc.MutableMapping` of :class:`collections.abc.MutableSequence`
-        """
-        if is_nonstring_sequence(template):
-            for index, value in enumerate(template):
-                if isinstance(value, templates.Formattable):
-                    template[index] = value.format()
-                else:
-                    _Structure._visit(value)
-                if not template[index]:
-                    template[index] = None
-
-            while None in template:
-                template.remove(None)
-
-        elif isinstance(template, abc.MutableMapping):  # noqa: SIM106
-            for key, value in template.items():
-                logger.debug("Visit %s to process environ variables.", key)
-
-                if isinstance(value, templates.Formattable):
-                    template[key] = value.format()
-                else:
-                    _Structure._visit(value)
-                if not template[key]:
-                    template[key] = None
-
-            for key in [key for key, value in template.items() if value is None]:
-                del template[key]
-
-        else:
-            raise AssertionError(f"{type(template)} do not support visitation.")
-
-
-structure = _Structure()
+import collections
+import logging
+import os
+import sys
+from collections import abc
+from datetime import date
+
+import click
+
+from incipyt._internal import dumpers, templates
+from incipyt._internal.utils import EnvValue, is_nonstring_sequence
+
+logger = logging.getLogger(__name__)
+
+
+class _Environ(collections.UserDict):
+    """Manage environ variables using for substitutions in patterns.
+
+    A :class:`Environ` object `environ` is a dictionnary initialized with
+    system environ variables `os.environ`, a variable can be add like that:
+
+    .. code-block::
+
+        environ["VARIABLE_NAME"] = "something"
+
+    However such a variable will not be considered in `environ` before being
+    `confirmed`. Such confirmation will happen the first it is asked for:
+
+    .. code-block::
+
+        var_first = environ["VARIABLE_NAME"]
+        # Prompt a message for confirmation of the value for `VARIABLE_NAME`
+        var_second = environ["VARIABLE_NAME"]
+        # As `VARIABLE_NAME` as been confirmed, don't ask anything
+
+    Moreover, even if a specific variable hasn't been set, it can be asked for
+    it anyway and it will be confirmed immediately. A variable can also be set
+    and confirmed at the same time:
+
+    .. code-block::
+
+        environ["VARIABLE_NAME"] = EnvValue("something", confirmed=True)
+
+    Note that if a variable has been set, it cannot be set again, except if
+    explicitly specified:
+
+    .. code-block::
+
+        environ["VARIABLE_NAME"] = EnvValue("new_value", update=True)
+
+    All iterative methods and in operator consider only `confirmed` variables.
+    """
+
+    def clear(self):
+        self._confirmed.clear()
+        self.data.clear()
+        self.data.update(os.environ.copy())
+
+        self.data.setdefault("PYTHON_CMD", sys.executable)
+        self._confirmed.add("PYTHON_CMD")
+        self.data.setdefault("YEAR", date.today().year)
+        self._confirmed.add("YEAR")
+
+    def __init__(self):
+        self._confirmed = set()
+        self.data = {}
+        self.clear()
+
+    def __getitem__(self, key):
+        if key not in self._confirmed:
+            logger.debug("Missing environ variable %s, request it.", key)
+            self.data[key] = self._prompt(key)
+            self._confirmed.add(key)
+
+        return self.data[key]
+
+    def __setitem__(self, key, env_value):
+        if not isinstance(env_value, EnvValue):
+            env_value = EnvValue(env_value)
+
+        if key in self.data and not env_value.update:
+            raise ValueError(f"Environ variable {key} already exists, use update.")
+
+        logger.debug("Set environ variable %s=%s.", key, env_value.value)
+        self.data[key] = env_value.value
+        if env_value.confirmed and key not in self._confirmed:
+            self._confirmed.add(key)
+
+    def setdefault(self, key, value):
+        if key in self:
+            return self.data[key]
+        self[key] = value
+        return self.data[key]
+
+    def __iter__(self):
+        return iter(self._confirmed)
+
+    def __contains__(self, key):
+        return key in self._confirmed
+
+    def keys(self):
+        return self._confirmed
+
+    def values(self):
+        return [self.data[key] for key in self._confirmed]
+
+    def items(self):
+        return [(key, self.data[key]) for key in self._confirmed]
+
+    def getitems_sanitized(self, keys, sanitizer=None):
+        """Get multiple items at once and sanitize them.
+
+        See also :func:`incipyt.system.Environment.__getitem__`, which will be
+        used to pull each key from the environment.
+
+        :param keys: Required environment keys. If a key is `None`, it will be ignored.
+        :type keys: :class:`collections.abc.Sequence`
+        :param sanitizer: Will be called on key-value pairs to sanitize values.
+        :type sanitizer: :class:`function`
+        :return: Sanitized environment key-value pairs.
+        :rtype: :class:`dict`
+        """
+        return {
+            key: sanitizer(key, self[key]) if sanitizer else self[key]
+            for key in keys
+            if key is not None
+        }
+
+    def _prompt(self, key):
+        return click.prompt(
+            key.replace("_", " ").lower().capitalize(),
+            default=self.data[key] if key in self.data else "",
+            type=str,
+        )
+
+    def __ior__(self, other):
+        self.update(other)
+        return self
+
+
+environ = _Environ()
+
+
+class _Structure:
+    """Represents all configuration and template files to commit for the new project.
+
+    An instance internally stores mappables between path objects and template
+    files or dictionaries modeling configuration files.
+
+    Functions :meth:`get_configuration` and :meth:`register_template` add
+    respectively configuration dictionary and template to the instance.
+
+    When the project structure is finally ready, functions :meth:`mkdir` :meth:`commit`
+    can be used to write folder and files in a new folder after substituting
+    variables in path and files using an :class:`incipyt.project.Environ`.
+    """
+
+    def clear(self):
+        self._configurations = {}
+
+    def __init__(self):
+        self.clear()
+
+    def get_config_dict(self, config_root):
+        """Get a configuration dictionary associated to the relative path `config_root`.
+
+        :param config_root: Relative path of the configuration file.
+        :type config_root: :class:`pathlib.Path`
+        :return: A reference to the configuration dictionary
+        :rtype: :class:`incipyt._internal.templates.TempateDict`
+        """
+        if config_root not in self._configurations:
+            logger.debug("Register configuration %s in project structure.", str(config_root))
+            self._configurations[config_root] = {}
+
+        if not isinstance(self._configurations[config_root], abc.MutableMapping):
+            raise TypeError(f"{config_root} is not a dict.")
+        return templates.TemplateDict(self._configurations[config_root])
+
+    def get_config_list(self, config_root):
+        """Get a configuration list associated to the relative path `config_root`.
+
+        :param config_root: Relative path of the configuration file.
+        :type config_root: :class:`pathlib.Path`
+        :return: A reference to the configuration list
+        :rtype: :class:`incipyt._internal.templates.TempateList`
+        """
+        if config_root not in self._configurations:
+            logger.debug("Register configuration %s in project structure.", str(config_root))
+            self._configurations[config_root] = []
+
+        if not is_nonstring_sequence(self._configurations[config_root]):
+            raise TypeError(f"{config_root} is not a list.")
+        return templates.TemplateList(self._configurations[config_root])
+
+    def use_template(self, template_name, dest=None, sanitizer=None):
+        """Use a file as template to populate a configuration file.
+
+        :param template_name: Relative path of the template file.
+        :type template_name: :class:`str`
+        :param dest: Relative path of the configuration file.
+        :type dest: :class:`str` or `None`, optionnal
+        :param sanitizer: An optionnal callable to sanitize the values given (key, value) pairs.
+        :type sanitizer: :class:`function` or `None`, optionnal
+        """
+        self.get_config_list(dumpers.TextFile(dest or template_name, sanitizer=sanitizer)).append(
+            templates.StringTemplate.from_file(template_name)
+        )
+
+    def commit(self):
+        """Commit current project structure on disk.
+
+        :raises RuntimeError: If one of the configuration file already exists.
+        """
+        for config_root, config in self._configurations.items():
+            logger.info("Process environ variables for %s.", str(config_root))
+            _Structure._visit(config)
+
+        for config_root, config in self._configurations.items():
+            logger.info("Write configuration file %s.", str(config_root))
+            config_root.dump_in(config)
+
+    def mkdir(self, workon):
+        """Make all directories of the project structure in workon.
+
+        :param workon: Work-on path.
+        :type workon: :class:`pathlib.Path`
+        """
+        for config_root in self._configurations:
+            logger.debug("Commit %s path.", str(config_root))
+            config_root.commit(workon)
+
+        for config_root in self._configurations:
+            logger.info("Mkdir folders for %s.", str(config_root))
+            config_root.mkdir()
+
+    @staticmethod
+    def _visit(template):
+        """Visit the `template` nested-dictionary structure.
+
+        All :class:`incipyt._internal.templates.Formattable` values of the template dictionary will be
+        evaluated and replaced by their results. All nested structures will be recursively
+        visited and processed too.
+
+        :param template: The template dictionary or list to visit.
+        :type template: :class:`collections.abc.MutableMapping` of :class:`collections.abc.MutableSequence`
+        """
+        if is_nonstring_sequence(template):
+            for index, value in enumerate(template):
+                if isinstance(value, templates.Formattable):
+                    template[index] = value.format()
+                else:
+                    _Structure._visit(value)
+                if not template[index]:
+                    template[index] = None
+
+            while None in template:
+                template.remove(None)
+
+        elif isinstance(template, abc.MutableMapping):
+            for key, value in template.items():
+                logger.debug("Visit %s to process environ variables.", key)
+
+                if isinstance(value, templates.Formattable):
+                    template[key] = value.format()
+                else:
+                    _Structure._visit(value)
+                if not template[key]:
+                    template[key] = None
+
+            for key in [key for key, value in template.items() if value is None]:
+                del template[key]
+
+        else:
+            raise AssertionError(f"{type(template)} do not support visitation.")
+
+
+structure = _Structure()
```

### Comparing `incipyt-0.2.0/incipyt/tools/git.py` & `incipyt-0.3.0/incipyt/tools/git.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,73 @@
-import logging
-import os
-import shutil
-import sys
-
-from incipyt import commands, project, signals, tools
-from incipyt._internal.dumpers import TextFile
-
-
-logger = logging.getLogger(__name__)
-
-
-class Git(tools.Tool):
-    """Scripts to add Git to :class:`incipyt.project._Structure`."""
-
-    def __init__(self):
-        if not shutil.which("git"):
-            logger.error("%r is missing from the PATH. Abort.", "git")
-            sys.exit(1)
-
-        signals.vcs_ignore.connect(self._slot)
-
-    def add_to_structure(self):
-        """Add git configuration to `project.structure`.
-
-        Register git related project URLs.
-
-        URLs:
-            - Repository: {REPOSITORY}
-            - Issue: {REPOSITORY}/issues
-            - Documentation: {REPOSITORY}/wiki
-        """
-        signals.project_url.emit(
-            url_kind="Documentation", url_value="{REPOSITORY}/wiki"
-        )
-        signals.project_url.emit(url_kind="Issue", url_value="{REPOSITORY}/issues")
-        signals.project_url.emit(url_kind="Repository", url_value="{REPOSITORY}")
-
-    def _slot(self, pattern, **kwargs):
-        project.structure.get_config_list(TextFile(".gitignore")).append(pattern)
-
-    def pre(self, workon):
-        """Run `git init`.
-
-        Also push {AUTHOR_NAME} and {AUTHOR_EMAIL} using `git config user.*`.
-
-        :param workon: Work-on folder.
-        :type workon: :class:`pathlib.Path`
-        """
-        commands.run(["git", "init", os.fspath(workon)])
-
-        project.environ["AUTHOR_EMAIL"] = project.EnvValue(
-            commands.run(["git", "-C", os.fspath(workon), "config", "user.email"])
-            .stdout.decode()
-            .strip(),
-            update=True,
-        )
-        project.environ["AUTHOR_NAME"] = project.EnvValue(
-            commands.run(["git", "-C", os.fspath(workon), "config", "user.name"])
-            .stdout.decode()
-            .strip(),
-            update=True,
-        )
-
-    def post(self, workon):
-        """Run `git add --all`.
-
-        :param workon: Work-on folder.
-        :type workon: :class:`pathlib.Path`
-        """
-        commands.run(["git", "-C", os.fspath(workon), "add", "--all"])
+import logging
+import os
+import shutil
+import sys
+
+import click
+
+from incipyt import project, signals, tools
+from incipyt._internal.dumpers import TextFile
+from incipyt.commands import git, git_get_config
+
+logger = logging.getLogger(__name__)
+
+
+class Git(tools.Tool):
+    """Scripts to add Git to :class:`incipyt.project._Structure`."""
+
+    def __init__(self):
+        if not shutil.which("git"):
+            logger.error("%r is missing from the PATH. Abort.", "git")
+            sys.exit(1)
+
+        signals.vcs_ignore.connect(self._slot)
+
+    def add_to_structure(self):
+        """Add git configuration to `project.structure`.
+
+        Register git related project URLs.
+
+        URLs:
+            - Repository: {REPOSITORY}
+            - Issue: {REPOSITORY}/issues
+            - Documentation: {REPOSITORY}/wiki
+        """
+        project.structure.use_template("python.gitignore", ".gitignore")
+        signals.project_url.emit(url_kind="Documentation", url_value="{REPOSITORY}/wiki")
+        signals.project_url.emit(url_kind="Issue", url_value="{REPOSITORY}/issues")
+        signals.project_url.emit(url_kind="Repository", url_value="{REPOSITORY}")
+
+    def _slot(self, pattern, **kwargs):
+        project.structure.get_config_list(TextFile(".gitignore")).append(pattern)
+
+    def pre(self, workon):
+        """Run `git init`.
+
+        Also push {AUTHOR_NAME} and {AUTHOR_EMAIL} using `git config user.*`.
+
+        :param workon: Work-on folder.
+        :type workon: :class:`pathlib.Path`
+        """
+        git(["init", os.fspath(workon)])
+        project.environ.setdefault("AUTHOR_EMAIL", git_get_config("user.email", workon=workon))
+        project.environ.setdefault("AUTHOR_NAME", git_get_config("user.name", workon=workon))
+
+    def post(self, workon):
+        """Check config name+email and then run `git add --all`.
+
+        :param workon: Work-on folder.
+        :type workon: :class:`pathlib.Path`
+        """
+        env_name = project.environ["AUTHOR_NAME"]
+        git_name = git_get_config("user.name", workon=workon)
+        prompt = f"Git user name is {git_name!r}, use {env_name!r} instead?"
+        if env_name != git_name and click.confirm(prompt, default=None):
+            git(["config", "user.name", env_name], workon=workon)
+
+        env_email = project.environ["AUTHOR_EMAIL"]
+        git_email = git_get_config("user.email", workon=workon)
+        prompt = f"Git user email is {git_email!r}, use {env_email!r} instead?"
+        if env_email != git_email and click.confirm(prompt, default=None):
+            git(["config", "user.email", env_email], workon=workon)
+
+        git(["add", "--all"], workon=workon)
```

### Comparing `incipyt-0.2.0/tests/test_project.py` & `incipyt-0.3.0/tests/test_project.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,171 +1,133 @@
-import os
-import sys
-
-from pytest import fixture, mark, raises
-
-from incipyt import project, commands
-from incipyt._internal.dumpers import TextFile, Toml
-from incipyt._internal.templates import StringTemplate
-
-from tests.utils import mock_stdin
-
-
-class TestEnviron:
-    @fixture
-    def empty_environ(self, fake_process):
-        fake_process.register_subprocess(["cmd", "arg"], stdout=["lineA", "lineB"])
-        project.environ.clear()
-
-    @fixture
-    def simple_environ(self, fake_process):
-        fake_process.register_subprocess(["cmd", "arg"], stdout=["lineA", "lineB"])
-        project.environ.clear()
-        project.environ["ONE"] = project.EnvValue("1", confirmed=True)
-
-    @fixture
-    def empty_auto_env(self, fake_process):
-        fake_process.register_subprocess(["cmd", "arg"], stdout=["lineA", "lineB"])
-        project.environ.clear()
-
-    @fixture
-    def simple_auto_env(self, fake_process):
-        fake_process.register_subprocess(["cmd", "arg"], stdout=["lineA", "lineB"])
-        project.environ.clear()
-        project.environ["ONE"] = project.EnvValue("1", confirmed=True)
-
-    @mark.parametrize(
-        "env, input_values",
-        (
-            ("empty_environ", ["1"]),
-            ("simple_environ", [""]),
-            ("empty_auto_env", ["1"]),
-            ("simple_auto_env", []),
-        ),
-    )
-    def test_pull(self, env, input_values, monkeypatch, request):
-        request.getfixturevalue(env)
-        mock_stdin(monkeypatch, input_values)
-        assert project.environ["ONE"] == "1"
-
-    @mark.parametrize(
-        "env",
-        (
-            "simple_environ",
-            "simple_auto_env",
-        ),
-    )
-    def test_push(self, env, request):
-        request.getfixturevalue(env)
-        with raises(ValueError):
-            project.environ["ONE"] = "11"
-
-    @mark.parametrize(
-        "env, input_values",
-        (
-            ("simple_environ", [""]),
-            ("simple_auto_env", []),
-        ),
-    )
-    def test_update(self, env, input_values, monkeypatch, request):
-        request.getfixturevalue(env)
-        project.environ["ONE"] = project.EnvValue("11", update=True)
-        mock_stdin(monkeypatch, input_values)
-        assert project.environ["ONE"] == "11"
-
-    @mark.parametrize(
-        "env",
-        (
-            "empty_environ",
-            "empty_auto_env",
-        ),
-    )
-    def test_confirmed(self, env, request):
-        request.getfixturevalue(env)
-        project.environ["ONE"] = project.EnvValue("1", confirmed=True)
-        assert project.environ["ONE"] == "1"
-
-    @mark.parametrize(
-        "env",
-        (
-            "empty_environ",
-            "simple_environ",
-            "empty_auto_env",
-            "simple_auto_env",
-        ),
-    )
-    def test_python_cmd(self, env, request):
-        request.getfixturevalue(env)
-        assert project.environ["PYTHON_CMD"] == sys.executable
-
-    @mark.parametrize(
-        "env",
-        (
-            "empty_environ",
-            "empty_auto_env",
-        ),
-    )
-    def test_iter(self, env, request):
-        request.getfixturevalue(env)
-        project.environ["TWO"] = project.EnvValue("2", confirmed=True)
-        result = {key: project.environ[key] for key in project.environ}
-        assert result == {"PYTHON_CMD": sys.executable, "TWO": "2"}
-
-    @mark.parametrize(
-        "env",
-        (
-            "empty_environ",
-            "simple_environ",
-            "empty_auto_env",
-            "simple_auto_env",
-        ),
-    )
-    def test_run(self, env, request):
-        request.getfixturevalue(env)
-        result = commands.run(["cmd", "arg"])
-        assert result.stdout.decode() == f"lineA{os.linesep}lineB{os.linesep}"
-
-
-class TestStructure:
-    @fixture
-    def reset_environ(self, fake_process):
-        fake_process.register_subprocess(["cmd", "arg"], stdout=["lineA", "lineB"])
-        project.environ.clear()
-        project.environ["FOLDER_A"] = project.EnvValue("folderA", confirmed=True)
-        project.environ["FOLDER_B"] = project.EnvValue("folderB", confirmed=True)
-        project.environ["NAME_A"] = project.EnvValue("testA", confirmed=True)
-        project.environ["NAME_B"] = project.EnvValue("testB", confirmed=True)
-        project.environ["VALUE"] = project.EnvValue("1", confirmed=True)
-        project.environ["CONTENT"] = project.EnvValue("text", confirmed=True)
-
-    @fixture
-    def reset_structure(self):
-        project.structure.clear()
-        project.structure.get_config_dict(Toml("{FOLDER_A}/{NAME_A}.toml"))[
-            "section"
-        ] = {"first": "{VALUE}"}
-        project.structure.get_config_list(
-            TextFile("{FOLDER_B}/{NAME_B}", sep="\n\n")
-        ).append("{CONTENT}")
-
-    def test_get_new_configuration(self, reset_structure):
-        configuration = project.structure.get_config_dict(Toml("testC.toml"))
-        assert configuration == {}
-
-    def test_get_old_configuration(self, reset_structure):
-        configuration = project.structure.get_config_dict(
-            Toml("{FOLDER_A}/{NAME_A}.toml")
-        )
-        assert configuration == {"section": {"first": StringTemplate("{VALUE}")}}
-
-    def test_mkdir(self, reset_structure, reset_environ, tmp_path):
-        project.structure.mkdir(tmp_path)
-        assert (tmp_path / "folderA").is_dir()
-        assert (tmp_path / "folderB").is_dir()
-
-    def test_commit(self, reset_structure, reset_environ, tmp_path):
-        project.structure.mkdir(tmp_path)
-        project.structure.commit()
-        assert (
-            tmp_path / "folderA" / "testA.toml"
-        ).read_text() == '[section]\nfirst = "1"\n'
-        assert (tmp_path / "folderB" / "testB").read_text() == "text\n\n"
+import os
+import sys
+from datetime import date
+
+from pytest import fixture, mark, raises
+
+from incipyt import commands, project
+from incipyt._internal.dumpers import TextFile, Toml
+from incipyt._internal.templates import StringTemplate
+from tests.utils import mock_stdin
+
+YEAR = date.today().year
+
+
+class TestEnviron:
+    @fixture
+    def empty_environ(self, fake_process):
+        fake_process.register_subprocess(["cmd", "arg"], stdout=["lineA", "lineB"])
+        project.environ.clear()
+
+    @fixture
+    def simple_environ(self, fake_process):
+        fake_process.register_subprocess(["cmd", "arg"], stdout=["lineA", "lineB"])
+        project.environ.clear()
+        project.environ["ONE"] = project.EnvValue("1", confirmed=True)
+
+    @fixture
+    def empty_auto_env(self, fake_process):
+        fake_process.register_subprocess(["cmd", "arg"], stdout=["lineA", "lineB"])
+        project.environ.clear()
+
+    @fixture
+    def simple_auto_env(self, fake_process):
+        fake_process.register_subprocess(["cmd", "arg"], stdout=["lineA", "lineB"])
+        project.environ.clear()
+        project.environ["ONE"] = project.EnvValue("1", confirmed=True)
+
+    @mark.parametrize(
+        "env, input_values",
+        (
+            ("empty_environ", ["1"]),
+            ("simple_environ", [""]),
+            ("empty_auto_env", ["1"]),
+            ("simple_auto_env", []),
+        ),
+    )
+    def test_pull(self, env, input_values, monkeypatch, request):
+        request.getfixturevalue(env)
+        mock_stdin(monkeypatch, input_values)
+        assert project.environ["ONE"] == "1"
+
+    @mark.parametrize("env", ("simple_environ", "simple_auto_env"))
+    def test_push(self, env, request):
+        request.getfixturevalue(env)
+        with raises(ValueError):
+            project.environ["ONE"] = "11"
+
+    @mark.parametrize("env, input_values", (("simple_environ", [""]), ("simple_auto_env", [])))
+    def test_update(self, env, input_values, monkeypatch, request):
+        request.getfixturevalue(env)
+        project.environ["ONE"] = project.EnvValue("11", update=True)
+        mock_stdin(monkeypatch, input_values)
+        assert project.environ["ONE"] == "11"
+
+    @mark.parametrize("env", ("empty_environ", "empty_auto_env"))
+    def test_confirmed(self, env, request):
+        request.getfixturevalue(env)
+        project.environ["ONE"] = project.EnvValue("1", confirmed=True)
+        assert project.environ["ONE"] == "1"
+
+    @mark.parametrize(
+        "env", ("empty_environ", "simple_environ", "empty_auto_env", "simple_auto_env")
+    )
+    def test_python_cmd(self, env, request):
+        request.getfixturevalue(env)
+        assert project.environ["PYTHON_CMD"] == sys.executable
+
+    @mark.parametrize("env", ("empty_environ", "empty_auto_env"))
+    def test_iter(self, env, request):
+        request.getfixturevalue(env)
+        project.environ["TWO"] = project.EnvValue("2", confirmed=True)
+        result = {key: project.environ[key] for key in project.environ}
+        assert result == {"PYTHON_CMD": sys.executable, "TWO": "2", "YEAR": YEAR}
+
+    @mark.parametrize(
+        "env", ("empty_environ", "simple_environ", "empty_auto_env", "simple_auto_env")
+    )
+    def test_run(self, env, request):
+        request.getfixturevalue(env)
+        result = commands.run(["cmd", "arg"])
+        assert result.stdout.decode() == f"lineA{os.linesep}lineB{os.linesep}"
+
+
+class TestStructure:
+    @fixture
+    def reset_environ(self, fake_process):
+        fake_process.register_subprocess(["cmd", "arg"], stdout=["lineA", "lineB"])
+        project.environ.clear()
+        project.environ["FOLDER_A"] = project.EnvValue("folderA", confirmed=True)
+        project.environ["FOLDER_B"] = project.EnvValue("folderB", confirmed=True)
+        project.environ["NAME_A"] = project.EnvValue("testA", confirmed=True)
+        project.environ["NAME_B"] = project.EnvValue("testB", confirmed=True)
+        project.environ["VALUE"] = project.EnvValue("1", confirmed=True)
+        project.environ["CONTENT"] = project.EnvValue("text", confirmed=True)
+
+    @fixture
+    def reset_structure(self):
+        project.structure.clear()
+        project.structure.get_config_dict(Toml("{FOLDER_A}/{NAME_A}.toml"))["section"] = {
+            "first": "{VALUE}"
+        }
+        project.structure.get_config_list(TextFile("{FOLDER_B}/{NAME_B}", sep="\n\n")).append(
+            "{CONTENT}"
+        )
+
+    def test_get_new_configuration(self, reset_structure):
+        configuration = project.structure.get_config_dict(Toml("testC.toml"))
+        assert configuration == {}
+
+    def test_get_old_configuration(self, reset_structure):
+        configuration = project.structure.get_config_dict(Toml("{FOLDER_A}/{NAME_A}.toml"))
+        assert configuration == {"section": {"first": StringTemplate("{VALUE}")}}
+
+    def test_mkdir(self, reset_structure, reset_environ, tmp_path):
+        project.structure.mkdir(tmp_path)
+        assert (tmp_path / "folderA").is_dir()
+        assert (tmp_path / "folderB").is_dir()
+
+    def test_commit(self, reset_structure, reset_environ, tmp_path):
+        project.structure.mkdir(tmp_path)
+        project.structure.commit()
+        assert (tmp_path / "folderA" / "testA.toml").read_text() == '[section]\nfirst = "1"\n'
+        assert (tmp_path / "folderB" / "testB").read_text() == "text\n\n"
```

### Comparing `incipyt-0.2.0/PKG-INFO` & `incipyt-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incipyt
-Version: 0.2.0
+Version: 0.3.0
 Summary: incipyt is a command-line tool that bootstraps a python project.
 Author-email: Not at Name <julien@drlazor.be>
 Maintainer-email: Not at Name <julien@drlazor.be>
 Requires-Python: >=3.7, <4.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -12,32 +12,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Requires-Dist: click
 Requires-Dist: signalslot
 Requires-Dist: toml
-Requires-Dist: black ; extra == "dev"
-Requires-Dist: build ; extra == "dev"
-Requires-Dist: flake8 ; extra == "dev"
-Requires-Dist: flakeheaven ; extra == "dev"
-Requires-Dist: flake8-bandit ; extra == "dev"
-Requires-Dist: flake8-bugbear ; extra == "dev"
-Requires-Dist: flake8-builtins ; extra == "dev"
-Requires-Dist: flake8-comprehensions ; extra == "dev"
-Requires-Dist: flake8-docstrings ; extra == "dev"
-Requires-Dist: flake8-simplify ; extra == "dev"
-Requires-Dist: flake8-use-fstring ; extra == "dev"
-Requires-Dist: pep8-naming ; extra == "dev"
-Requires-Dist: pre-commit ; extra == "dev"
-Requires-Dist: m2r2 ; extra == "doc"
-Requires-Dist: sphinxcontrib-apidoc ; extra == "doc"
-Requires-Dist: sphinx_rtd_theme ; extra == "doc"
-Requires-Dist: pytest-cov ; extra == "test"
-Requires-Dist: pytest-subprocess ; extra == "test"
+Requires-Dist: flit==3.8.0 ; extra == "dev"
+Requires-Dist: pre-commit==3.2.2 ; extra == "dev"
+Requires-Dist: m2r2==0.3.2 ; extra == "doc"
+Requires-Dist: sphinxcontrib-apidoc==0.3.0 ; extra == "doc"
+Requires-Dist: sphinx_rtd_theme==1.2.0 ; extra == "doc"
+Requires-Dist: pytest-cov==4.0.0 ; extra == "test"
+Requires-Dist: pytest-subprocess==1.5.0 ; extra == "test"
 Project-URL: documentation, https://github.com/NotANameServer/incipyt/wiki
 Project-URL: homepage, https://pypi.org/incipyt
 Project-URL: repository, https://github.com/NotANameServer/incipyt
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
```

