# Comparing `tmp/httpdate-1.1.0.tar.gz` & `tmp/httpdate-1.2.0.tar.gz`

## Comparing `httpdate-1.1.0.tar` & `httpdate-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,15 @@
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 httpdate-1.1.0/.justfile
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 httpdate-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 httpdate-1.1.0/.pylintrc
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 httpdate-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpdate-1.1.0/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpdate-1.1.0/.changelog.d/.keep
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 httpdate-1.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 httpdate-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 httpdate-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 httpdate-1.1.0/src/httpdate/__about__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 httpdate-1.1.0/src/httpdate/__init__.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 httpdate-1.1.0/src/httpdate/httpdate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpdate-1.1.0/src/httpdate/py.typed
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 httpdate-1.1.0/tests/test_httpdate_to_unixtime.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 httpdate-1.1.0/tests/test_is_valid_httpdate.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 httpdate-1.1.0/tests/test_unixtime_to_httpdate.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 httpdate-1.1.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 httpdate-1.1.0/LICENSE
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 httpdate-1.1.0/README.md
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 httpdate-1.1.0/hatch.toml
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 httpdate-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 httpdate-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 httpdate-1.2.0/.justfile
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 httpdate-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 httpdate-1.2.0/.pylintrc
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 httpdate-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpdate-1.2.0/setup.cfg
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 httpdate-1.2.0/src/httpdate/__about__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 httpdate-1.2.0/src/httpdate/__init__.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 httpdate-1.2.0/src/httpdate/httpdate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpdate-1.2.0/src/httpdate/py.typed
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 httpdate-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 httpdate-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 httpdate-1.2.0/README.md
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 httpdate-1.2.0/hatch.toml
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 httpdate-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 httpdate-1.2.0/PKG-INFO
```

### Comparing `httpdate-1.1.0/.justfile` & `httpdate-1.2.0/.justfile`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 help:
   @just --list
 
 current_version := `hatch version`
 
 # Create changelog entry
 changelog:
+  mkdir -p .changelog.d
   scriv create --edit
 
 # Tag and changelog
 tag:
   #!/usr/bin/env bash
   set -euo pipefail
   if [[ "$(git rev-parse --abbrev-ref HEAD)" != "main" ]]; then
```

### Comparing `httpdate-1.1.0/.pre-commit-config.yaml` & `httpdate-1.2.0/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: f71fa2c1f9cf5cb705f73dffe4b21f7c61470ba9 # v4.4.0
+    rev: f71fa2c1f9cf5cb705f73dffe4b21f7c61470ba9  # frozen: v4.4.0
     hooks:
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-shebang-scripts-are-executable
       - id: check-symlinks
       - id: check-json
       - id: check-toml
@@ -19,18 +19,19 @@
     hooks:
       - id: pylint
         name: pylint
         entry: pylint
         language: system
         types: [python]
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: 3c6d40da8d90069e86c0ba3942239d773aadad1a # v0.0.260
+    rev: f6346ef27faac608d493bf3926528b308d175d9e  # frozen: v0.0.261
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
-    rev: bf7a16254ec96b084a6caf3d435ec18f0f245cc7 # 23.3.0
+    rev: bf7a16254ec96b084a6caf3d435ec18f0f245cc7  # frozen: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/bwhmather/ssort
-    rev: 85ce691bd9dd6528a267aaf3e1ac7d455ecd773c # v0.11.6
+    rev: 85ce691bd9dd6528a267aaf3e1ac7d455ecd773c  # frozen: v0.11.6
     hooks:
       - id: ssort
+        args: ["src"]
```

### Comparing `httpdate-1.1.0/src/httpdate/__init__.py` & `httpdate-1.2.0/src/httpdate/__init__.py`

 * *Files identical despite different names*

### Comparing `httpdate-1.1.0/src/httpdate/httpdate.py` & `httpdate-1.2.0/src/httpdate/httpdate.py`

 * *Files identical despite different names*

### Comparing `httpdate-1.1.0/.gitignore` & `httpdate-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `httpdate-1.1.0/LICENSE` & `httpdate-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpdate-1.1.0/README.md` & `httpdate-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,30 +98,30 @@
 
 - **`is_valid_httpdate(httpdate)`**:
   - *Args*
     - `httpdate (str)`: An HTTP date string.
   - *Returns*
     - `bool`: True if `httpdate` is a valid HTTP date string, otherwise False.
   - *Raises*
-    - `TypeError` if input is not of type `str`.
+    - `TypeError` if `httpdate` is not of type `str`.
 - **`httpdate_to_unixtime(httpdate)`**:
   - *Args*
     - `httpdate (str)`: An HTTP date string.
   - *Returns*
-    - `int`: A Unix timestamp (`int`) if input is valid.
+    - `int`: A Unix timestamp (`int`).
   - *Raises*
-    - `TypeError` if input is not of type `str`.
+    - `TypeError` if `httpdate` is not of type `str`.
     - `ValueError` if `httpdate` is not a valid HTTP date string.
 - **`unixtime_to_httpdate(unixtime)`**:
   - *Args*
     - `unixtime (int)`: A Unix timestamp.
   - *Returns*
     - `str`: An HTTP date string.
   - *Raises*
-    - `TypeError` if input is not of type `int`.
+    - `TypeError` if `unixtime` is not of type `int`.
     - `ValueError` if `unixtime` represents a year before 1900, or if it is outside
       the range supported by the operating system.
 
 ## Why Unix timestamps?
 
 Unix timestamps are unambiguous, efficient, and can easily be converted to other
 date-time formats using only the standard library.
```

### Comparing `httpdate-1.1.0/hatch.toml` & `httpdate-1.2.0/hatch.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 7061 7468 203d  [version].path =
 00000010: 2022 7372 632f 6874 7470 6461 7465 2f5f   "src/httpdate/_
-00000020: 5f61 626f 7574 5f5f 2e70 7922 0a0a 2320  _about__.py"..# 
-00000030: 4c6f 6361 6c20 7465 7374 730a 5b65 6e76  Local tests.[env
-00000040: 732e 6465 6661 756c 745d 0a64 6570 656e  s.default].depen
-00000050: 6465 6e63 6965 7320 3d20 5b0a 2020 2262  dencies = [.  "b
-00000060: 6c61 636b 203e 3d20 3233 2e31 2e30 222c  lack >= 23.1.0",
-00000070: 0a20 2022 636f 7665 7261 6765 207e 3d20  .  "coverage ~= 
-00000080: 372e 3222 2c0a 2020 2268 6174 6368 2d63  7.2",.  "hatch-c
-00000090: 6f6e 7461 696e 6572 7320 7e3d 2030 2e37  ontainers ~= 0.7
-000000a0: 222c 0a20 2022 7072 652d 636f 6d6d 6974  ",.  "pre-commit
-000000b0: 207e 3d20 332e 3222 2c0a 2020 2270 796c   ~= 3.2",.  "pyl
-000000c0: 696e 7420 7e3d 2032 2e31 3722 2c0a 2020  int ~= 2.17",.  
-000000d0: 2270 7974 6573 7420 7e3d 2037 2e32 222c  "pytest ~= 7.2",
-000000e0: 0a20 2022 7275 6666 203e 3d20 302e 302e  .  "ruff >= 0.0.
-000000f0: 3235 3722 2c0a 2020 2273 6372 6976 203e  257",.  "scriv >
-00000100: 3d20 312e 322e 3122 2c0a 2020 2273 736f  = 1.2.1",.  "sso
-00000110: 7274 203e 3d20 302e 3131 2e36 222c 0a5d  rt >= 0.11.6",.]
-00000120: 0a5b 656e 7673 2e64 6566 6175 6c74 2e73  .[envs.default.s
-00000130: 6372 6970 7473 5d0a 636f 7620 3d20 5b22  cripts].cov = ["
-00000140: 636f 7665 7261 6765 2072 756e 207b 6172  coverage run {ar
-00000150: 6773 7d22 2c20 2263 6f76 6572 6167 6520  gs}", "coverage 
-00000160: 7265 706f 7274 202d 6d22 5d0a 6c69 6e74  report -m"].lint
-00000170: 203d 205b 0a20 2022 2d20 7275 6666 2063   = [.  "- ruff c
-00000180: 6865 636b 202e 222c 0a20 2022 2d20 7079  heck .",.  "- py
-00000190: 6c69 6e74 2073 7263 222c 0a20 2022 2d20  lint src",.  "- 
-000001a0: 626c 6163 6b20 2d2d 7175 6965 7420 2d2d  black --quiet --
-000001b0: 6368 6563 6b20 2d2d 6469 6666 202e 222c  check --diff .",
-000001c0: 0a20 2022 2d20 7079 7269 6768 7422 2c0a  .  "- pyright",.
-000001d0: 2020 222d 2073 736f 7274 202d 2d63 6865    "- ssort --che
-000001e0: 636b 202d 2d64 6966 6620 2e22 2c0a 5d0a  ck --diff .",.].
-000001f0: 0a23 2054 656d 706c 6174 6573 0a5b 656e  .# Templates.[en
-00000200: 7673 2e62 6173 655d 0a64 6570 656e 6465  vs.base].depende
-00000210: 6e63 6965 7320 3d20 5b0a 2020 2263 6f76  ncies = [.  "cov
-00000220: 6572 6167 6520 7e3d 2037 2e32 222c 0a20  erage ~= 7.2",. 
-00000230: 2022 7079 7465 7374 207e 3d20 372e 3222   "pytest ~= 7.2"
-00000240: 2c0a 5d0a 0a23 2047 6974 4875 6220 576f  ,.]..# GitHub Wo
-00000250: 726b 666c 6f77 3a20 4349 0a5b 656e 7673  rkflow: CI.[envs
-00000260: 2e63 695d 0a74 656d 706c 6174 6520 3d20  .ci].template = 
-00000270: 2262 6173 6522 0a70 6c61 7466 6f72 6d73  "base".platforms
-00000280: 203d 205b 226c 696e 7578 222c 2022 6d61   = ["linux", "ma
-00000290: 636f 7322 2c20 2277 696e 646f 7773 225d  cos", "windows"]
-000002a0: 0a5b 656e 7673 2e63 692e 7363 7269 7074  .[envs.ci.script
-000002b0: 735d 0a63 6f76 203d 205b 2263 6f76 6572  s].cov = ["cover
-000002c0: 6167 6520 7275 6e20 7b61 7267 737d 222c  age run {args}",
-000002d0: 2022 636f 7665 7261 6765 2063 6f6d 6269   "coverage combi
-000002e0: 6e65 202d 7120 2d2d 6b65 6570 222c 2022  ne -q --keep", "
-000002f0: 636f 7665 7261 6765 2072 6570 6f72 7420  coverage report 
-00000300: 2d6d 225d 0a63 6f76 2d63 6f6d 6269 6e65  -m"].cov-combine
-00000310: 203d 205b 2263 6f76 6572 6167 6520 636f   = ["coverage co
-00000320: 6d62 696e 6520 2d71 222c 2022 636f 7665  mbine -q", "cove
-00000330: 7261 6765 206a 736f 6e20 2d71 202d 6f20  rage json -q -o 
-00000340: 636f 7665 7261 6765 2e6a 736f 6e22 5d0a  coverage.json"].
-00000350: 5b5b 656e 7673 2e63 692e 6d61 7472 6978  [[envs.ci.matrix
-00000360: 5d5d 0a70 7974 686f 6e20 3d20 5b22 332e  ]].python = ["3.
-00000370: 3722 2c20 2233 2e38 222c 2022 332e 3922  7", "3.8", "3.9"
-00000380: 2c20 2233 2e31 3022 2c20 2233 2e31 3122  , "3.10", "3.11"
-00000390: 2c20 2270 7970 7933 2e37 222c 2022 7079  , "pypy3.7", "py
-000003a0: 7079 332e 3822 2c20 2270 7970 7933 2e39  py3.8", "pypy3.9
-000003b0: 225d 0a                                  "].
+00000020: 5f61 626f 7574 5f5f 2e70 7922 0a0a 5b62  _about__.py"..[b
+00000030: 7569 6c64 2e74 6172 6765 7473 2e73 6469  uild.targets.sdi
+00000040: 7374 5d0a 6578 636c 7564 6520 3d20 5b0a  st].exclude = [.
+00000050: 2020 222f 2e63 6861 6e67 656c 6f67 2e64    "/.changelog.d
+00000060: 222c 0a20 2022 2f2e 6769 7468 7562 222c  ",.  "/.github",
+00000070: 0a20 2022 2f74 6573 7473 222c 0a5d 0a0a  .  "/tests",.]..
+00000080: 2320 4c6f 6361 6c20 7465 7374 730a 5b65  # Local tests.[e
+00000090: 6e76 732e 6465 6661 756c 745d 0a64 6570  nvs.default].dep
+000000a0: 656e 6465 6e63 6965 7320 3d20 5b0a 2020  endencies = [.  
+000000b0: 2262 6c61 636b 203e 3d20 3233 2e31 2e30  "black >= 23.1.0
+000000c0: 222c 0a20 2022 636f 7665 7261 6765 207e  ",.  "coverage ~
+000000d0: 3d20 372e 3222 2c0a 2020 2270 7265 2d63  = 7.2",.  "pre-c
+000000e0: 6f6d 6d69 7420 7e3d 2033 2e32 222c 0a20  ommit ~= 3.2",. 
+000000f0: 2022 7079 6c69 6e74 207e 3d20 322e 3137   "pylint ~= 2.17
+00000100: 222c 0a20 2022 7079 7269 6768 742d 706f  ",.  "pyright-po
+00000110: 6c69 7465 207e 3d20 312e 3022 2c0a 2020  lite ~= 1.0",.  
+00000120: 2270 7974 6573 7420 7e3d 2037 2e32 222c  "pytest ~= 7.2",
+00000130: 0a20 2022 7275 6666 203e 3d20 302e 302e  .  "ruff >= 0.0.
+00000140: 3235 3722 2c0a 2020 2273 6372 6976 203e  257",.  "scriv >
+00000150: 3d20 312e 322e 3122 2c0a 2020 2273 736f  = 1.2.1",.  "sso
+00000160: 7274 203e 3d20 302e 3131 2e36 222c 0a5d  rt >= 0.11.6",.]
+00000170: 0a5b 656e 7673 2e64 6566 6175 6c74 2e73  .[envs.default.s
+00000180: 6372 6970 7473 5d0a 636f 7620 3d20 5b22  cripts].cov = ["
+00000190: 636f 7665 7261 6765 2072 756e 207b 6172  coverage run {ar
+000001a0: 6773 7d22 2c20 2263 6f76 6572 6167 6520  gs}", "coverage 
+000001b0: 7265 706f 7274 202d 6d22 5d0a 6c69 6e74  report -m"].lint
+000001c0: 203d 205b 0a20 2022 2d20 7275 6666 2063   = [.  "- ruff c
+000001d0: 6865 636b 202e 222c 0a20 2022 2d20 7079  heck .",.  "- py
+000001e0: 6c69 6e74 2073 7263 222c 0a20 2022 2d20  lint src",.  "- 
+000001f0: 626c 6163 6b20 2d2d 7175 6965 7420 2d2d  black --quiet --
+00000200: 6368 6563 6b20 2d2d 6469 6666 202e 222c  check --diff .",
+00000210: 0a20 2022 2d20 7079 7269 6768 742d 706f  .  "- pyright-po
+00000220: 6c69 7465 222c 0a20 2022 2d20 7373 6f72  lite",.  "- ssor
+00000230: 7420 2d2d 6368 6563 6b20 2d2d 6469 6666  t --check --diff
+00000240: 2073 7263 222c 0a5d 0a0a 2320 5465 6d70   src",.]..# Temp
+00000250: 6c61 7465 730a 5b65 6e76 732e 6261 7365  lates.[envs.base
+00000260: 5d0a 6465 7065 6e64 656e 6369 6573 203d  ].dependencies =
+00000270: 205b 0a20 2022 636f 7665 7261 6765 207e   [.  "coverage ~
+00000280: 3d20 372e 3222 2c0a 2020 2270 7974 6573  = 7.2",.  "pytes
+00000290: 7420 7e3d 2037 2e32 222c 0a5d 0a0a 2320  t ~= 7.2",.]..# 
+000002a0: 4769 7448 7562 2057 6f72 6b66 6c6f 773a  GitHub Workflow:
+000002b0: 2043 490a 5b65 6e76 732e 6369 5d0a 7465   CI.[envs.ci].te
+000002c0: 6d70 6c61 7465 203d 2022 6261 7365 220a  mplate = "base".
+000002d0: 706c 6174 666f 726d 7320 3d20 5b22 6c69  platforms = ["li
+000002e0: 6e75 7822 2c20 226d 6163 6f73 222c 2022  nux", "macos", "
+000002f0: 7769 6e64 6f77 7322 5d0a 5b65 6e76 732e  windows"].[envs.
+00000300: 6369 2e73 6372 6970 7473 5d0a 636f 7620  ci.scripts].cov 
+00000310: 3d20 5b22 636f 7665 7261 6765 2072 756e  = ["coverage run
+00000320: 207b 6172 6773 7d22 2c20 2263 6f76 6572   {args}", "cover
+00000330: 6167 6520 636f 6d62 696e 6520 2d71 202d  age combine -q -
+00000340: 2d6b 6565 7022 2c20 2263 6f76 6572 6167  -keep", "coverag
+00000350: 6520 7265 706f 7274 202d 6d22 5d0a 636f  e report -m"].co
+00000360: 762d 636f 6d62 696e 6520 3d20 5b22 636f  v-combine = ["co
+00000370: 7665 7261 6765 2063 6f6d 6269 6e65 202d  verage combine -
+00000380: 7122 2c20 2263 6f76 6572 6167 6520 6a73  q", "coverage js
+00000390: 6f6e 202d 7120 2d6f 2063 6f76 6572 6167  on -q -o coverag
+000003a0: 652e 6a73 6f6e 225d 0a5b 5b65 6e76 732e  e.json"].[[envs.
+000003b0: 6369 2e6d 6174 7269 785d 5d0a 7079 7468  ci.matrix]].pyth
+000003c0: 6f6e 203d 205b 2233 2e37 222c 2022 332e  on = ["3.7", "3.
+000003d0: 3822 2c20 2233 2e39 222c 2022 332e 3130  8", "3.9", "3.10
+000003e0: 222c 2022 332e 3131 222c 2022 7079 7079  ", "3.11", "pypy
+000003f0: 332e 3722 2c20 2270 7970 7933 2e38 222c  3.7", "pypy3.8",
+00000400: 2022 7079 7079 332e 3922 5d0a             "pypy3.9"].
```

### Comparing `httpdate-1.1.0/pyproject.toml` & `httpdate-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -26,27 +26,30 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
-  "leapseconds >= 2023.3.3",
+  "leapseconds >= 2023.4.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/jamielinux/httpdate"
 Issues = "https://github.com/jamielinux/httpdate/issues"
 Source = "https://github.com/jamielinux/httpdate"
 
 # pytest & coverage
 [tool.pytest.ini_options]
 addopts = [
   "--import-mode=importlib",
+  "--strict-markers",
+  "--strict-config",
+  "-ra",
 ]
 [tool.coverage.run]
 branch = true
 command_line = "-m pytest"
 omit = [
   "tests/*"
 ]
```

### Comparing `httpdate-1.1.0/PKG-INFO` & `httpdate-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpdate
-Version: 1.1.0
+Version: 1.2.0
 Summary: Parse and format HTTP dates, such as Last-Modified and If-Modified-Since headers.
 Project-URL: Homepage, https://github.com/jamielinux/httpdate
 Project-URL: Issues, https://github.com/jamielinux/httpdate/issues
 Project-URL: Source, https://github.com/jamielinux/httpdate
 Author-email: Jamie Nguyen <j@jamielinux.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
-Requires-Dist: leapseconds>=2023.3.3
+Requires-Dist: leapseconds>=2023.4.0
 Description-Content-Type: text/markdown
 
 # httpdate
 
 [![PyPi Version][pypi-img]][pypi-url]
 [![License][license-img]][license-url]
 [![Continuous Integration][ci-img]][ci-url]
@@ -125,30 +125,30 @@
 
 - **`is_valid_httpdate(httpdate)`**:
   - *Args*
     - `httpdate (str)`: An HTTP date string.
   - *Returns*
     - `bool`: True if `httpdate` is a valid HTTP date string, otherwise False.
   - *Raises*
-    - `TypeError` if input is not of type `str`.
+    - `TypeError` if `httpdate` is not of type `str`.
 - **`httpdate_to_unixtime(httpdate)`**:
   - *Args*
     - `httpdate (str)`: An HTTP date string.
   - *Returns*
-    - `int`: A Unix timestamp (`int`) if input is valid.
+    - `int`: A Unix timestamp (`int`).
   - *Raises*
-    - `TypeError` if input is not of type `str`.
+    - `TypeError` if `httpdate` is not of type `str`.
     - `ValueError` if `httpdate` is not a valid HTTP date string.
 - **`unixtime_to_httpdate(unixtime)`**:
   - *Args*
     - `unixtime (int)`: A Unix timestamp.
   - *Returns*
     - `str`: An HTTP date string.
   - *Raises*
-    - `TypeError` if input is not of type `int`.
+    - `TypeError` if `unixtime` is not of type `int`.
     - `ValueError` if `unixtime` represents a year before 1900, or if it is outside
       the range supported by the operating system.
 
 ## Why Unix timestamps?
 
 Unix timestamps are unambiguous, efficient, and can easily be converted to other
 date-time formats using only the standard library.
```

