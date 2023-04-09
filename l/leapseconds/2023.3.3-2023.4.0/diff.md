# Comparing `tmp/leapseconds-2023.3.3.tar.gz` & `tmp/leapseconds-2023.4.0.tar.gz`

## Comparing `leapseconds-2023.3.3.tar` & `leapseconds-2023.4.0.tar`

### file list

```diff
@@ -1,20 +1,15 @@
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/.justfile
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/.pylintrc
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/.changelog.d/.keep
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/.github/dependabot.yml
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/src/leapseconds/__about__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/src/leapseconds/__init__.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/src/leapseconds/leapseconds.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/src/leapseconds/py.typed
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/tests/test_leapseconds.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/LICENSE
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/README.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/hatch.toml
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/pyproject.toml
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 leapseconds-2023.3.3/PKG-INFO
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/.justfile
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/.pylintrc
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/setup.cfg
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/src/leapseconds/__about__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/src/leapseconds/__init__.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/src/leapseconds/leapseconds.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/src/leapseconds/py.typed
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/LICENSE
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/README.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/hatch.toml
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 leapseconds-2023.4.0/PKG-INFO
```

### Comparing `leapseconds-2023.3.3/.justfile` & `leapseconds-2023.4.0/.justfile`

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

### Comparing `leapseconds-2023.3.3/.pre-commit-config.yaml` & `leapseconds-2023.4.0/.pre-commit-config.yaml`

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

### Comparing `leapseconds-2023.3.3/src/leapseconds/leapseconds.py` & `leapseconds-2023.4.0/src/leapseconds/leapseconds.py`

 * *Files identical despite different names*

### Comparing `leapseconds-2023.3.3/.gitignore` & `leapseconds-2023.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `leapseconds-2023.3.3/LICENSE` & `leapseconds-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leapseconds-2023.3.3/README.md` & `leapseconds-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `leapseconds-2023.3.3/hatch.toml` & `leapseconds-2023.4.0/hatch.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 7061 7468 203d  [version].path =
 00000010: 2022 7372 632f 6c65 6170 7365 636f 6e64   "src/leapsecond
 00000020: 732f 5f5f 6162 6f75 745f 5f2e 7079 220a  s/__about__.py".
-00000030: 0a23 204c 6f63 616c 2074 6573 7473 0a5b  .# Local tests.[
-00000040: 656e 7673 2e64 6566 6175 6c74 5d0a 6465  envs.default].de
-00000050: 7065 6e64 656e 6369 6573 203d 205b 0a20  pendencies = [. 
-00000060: 2022 626c 6163 6b20 3e3d 2032 332e 312e   "black >= 23.1.
-00000070: 3022 2c0a 2020 2263 6f76 6572 6167 6520  0",.  "coverage 
-00000080: 7e3d 2037 2e32 222c 0a20 2022 6861 7463  ~= 7.2",.  "hatc
-00000090: 682d 636f 6e74 6169 6e65 7273 207e 3d20  h-containers ~= 
-000000a0: 302e 3722 2c0a 2020 2270 7265 2d63 6f6d  0.7",.  "pre-com
-000000b0: 6d69 7420 7e3d 2033 2e32 222c 0a20 2022  mit ~= 3.2",.  "
-000000c0: 7079 6c69 6e74 207e 3d20 322e 3137 222c  pylint ~= 2.17",
-000000d0: 0a20 2022 7079 7465 7374 207e 3d20 372e  .  "pytest ~= 7.
-000000e0: 3222 2c0a 2020 2272 7566 6620 3e3d 2030  2",.  "ruff >= 0
-000000f0: 2e30 2e32 3537 222c 0a20 2022 7363 7269  .0.257",.  "scri
-00000100: 7620 3e3d 2031 2e32 2e31 222c 0a20 2022  v >= 1.2.1",.  "
-00000110: 7373 6f72 7420 3e3d 2030 2e31 312e 3622  ssort >= 0.11.6"
-00000120: 2c0a 5d0a 5b65 6e76 732e 6465 6661 756c  ,.].[envs.defaul
-00000130: 742e 7363 7269 7074 735d 0a63 6f76 203d  t.scripts].cov =
-00000140: 205b 2263 6f76 6572 6167 6520 7275 6e20   ["coverage run 
-00000150: 7b61 7267 737d 222c 2022 636f 7665 7261  {args}", "covera
-00000160: 6765 2072 6570 6f72 7420 2d6d 225d 0a6c  ge report -m"].l
-00000170: 696e 7420 3d20 5b0a 2020 222d 2072 7566  int = [.  "- ruf
-00000180: 6620 6368 6563 6b20 2e22 2c0a 2020 222d  f check .",.  "-
-00000190: 2070 796c 696e 7420 7372 6322 2c0a 2020   pylint src",.  
-000001a0: 222d 2062 6c61 636b 202d 2d71 7569 6574  "- black --quiet
-000001b0: 202d 2d63 6865 636b 202d 2d64 6966 6620   --check --diff 
-000001c0: 2e22 2c0a 2020 222d 2070 7972 6967 6874  .",.  "- pyright
-000001d0: 222c 0a20 2022 2d20 7373 6f72 7420 2d2d  ",.  "- ssort --
-000001e0: 6368 6563 6b20 2d2d 6469 6666 202e 222c  check --diff .",
-000001f0: 0a5d 0a0a 2320 5465 6d70 6c61 7465 730a  .]..# Templates.
-00000200: 5b65 6e76 732e 6261 7365 5d0a 6465 7065  [envs.base].depe
-00000210: 6e64 656e 6369 6573 203d 205b 0a20 2022  ndencies = [.  "
-00000220: 636f 7665 7261 6765 207e 3d20 372e 3222  coverage ~= 7.2"
-00000230: 2c0a 2020 2270 7974 6573 7420 7e3d 2037  ,.  "pytest ~= 7
-00000240: 2e32 222c 0a5d 0a0a 2320 4769 7448 7562  .2",.]..# GitHub
-00000250: 2057 6f72 6b66 6c6f 773a 2043 490a 5b65   Workflow: CI.[e
-00000260: 6e76 732e 6369 5d0a 7465 6d70 6c61 7465  nvs.ci].template
-00000270: 203d 2022 6261 7365 220a 706c 6174 666f   = "base".platfo
-00000280: 726d 7320 3d20 5b22 6c69 6e75 7822 2c20  rms = ["linux", 
-00000290: 226d 6163 6f73 222c 2022 7769 6e64 6f77  "macos", "window
-000002a0: 7322 5d0a 5b65 6e76 732e 6369 2e73 6372  s"].[envs.ci.scr
-000002b0: 6970 7473 5d0a 636f 7620 3d20 5b22 636f  ipts].cov = ["co
-000002c0: 7665 7261 6765 2072 756e 207b 6172 6773  verage run {args
-000002d0: 7d22 2c20 2263 6f76 6572 6167 6520 636f  }", "coverage co
-000002e0: 6d62 696e 6520 2d71 202d 2d6b 6565 7022  mbine -q --keep"
-000002f0: 2c20 2263 6f76 6572 6167 6520 7265 706f  , "coverage repo
-00000300: 7274 202d 6d22 5d0a 636f 762d 636f 6d62  rt -m"].cov-comb
-00000310: 696e 6520 3d20 5b22 636f 7665 7261 6765  ine = ["coverage
-00000320: 2063 6f6d 6269 6e65 202d 7122 2c20 2263   combine -q", "c
-00000330: 6f76 6572 6167 6520 6a73 6f6e 202d 7120  overage json -q 
-00000340: 2d6f 2063 6f76 6572 6167 652e 6a73 6f6e  -o coverage.json
-00000350: 225d 0a5b 5b65 6e76 732e 6369 2e6d 6174  "].[[envs.ci.mat
-00000360: 7269 785d 5d0a 7079 7468 6f6e 203d 205b  rix]].python = [
-00000370: 2233 2e37 222c 2022 332e 3822 2c20 2233  "3.7", "3.8", "3
-00000380: 2e39 222c 2022 332e 3130 222c 2022 332e  .9", "3.10", "3.
-00000390: 3131 222c 2022 7079 7079 332e 3722 2c20  11", "pypy3.7", 
-000003a0: 2270 7970 7933 2e38 222c 2022 7079 7079  "pypy3.8", "pypy
-000003b0: 332e 3922 5d0a                           3.9"].
+00000030: 0a5b 6275 696c 642e 7461 7267 6574 732e  .[build.targets.
+00000040: 7364 6973 745d 0a65 7863 6c75 6465 203d  sdist].exclude =
+00000050: 205b 0a20 2022 2f2e 6368 616e 6765 6c6f   [.  "/.changelo
+00000060: 672e 6422 2c0a 2020 222f 2e67 6974 6875  g.d",.  "/.githu
+00000070: 6222 2c0a 2020 222f 7465 7374 7322 2c0a  b",.  "/tests",.
+00000080: 5d0a 0a23 204c 6f63 616c 2074 6573 7473  ]..# Local tests
+00000090: 0a5b 656e 7673 2e64 6566 6175 6c74 5d0a  .[envs.default].
+000000a0: 6465 7065 6e64 656e 6369 6573 203d 205b  dependencies = [
+000000b0: 0a20 2022 626c 6163 6b20 3e3d 2032 332e  .  "black >= 23.
+000000c0: 312e 3022 2c0a 2020 2263 6f76 6572 6167  1.0",.  "coverag
+000000d0: 6520 7e3d 2037 2e32 222c 0a20 2022 7072  e ~= 7.2",.  "pr
+000000e0: 652d 636f 6d6d 6974 207e 3d20 332e 3222  e-commit ~= 3.2"
+000000f0: 2c0a 2020 2270 796c 696e 7420 7e3d 2032  ,.  "pylint ~= 2
+00000100: 2e31 3722 2c0a 2020 2270 7972 6967 6874  .17",.  "pyright
+00000110: 2d70 6f6c 6974 6520 7e3d 2031 2e30 222c  -polite ~= 1.0",
+00000120: 0a20 2022 7079 7465 7374 207e 3d20 372e  .  "pytest ~= 7.
+00000130: 3222 2c0a 2020 2272 7566 6620 3e3d 2030  2",.  "ruff >= 0
+00000140: 2e30 2e32 3537 222c 0a20 2022 7363 7269  .0.257",.  "scri
+00000150: 7620 3e3d 2031 2e32 2e31 222c 0a20 2022  v >= 1.2.1",.  "
+00000160: 7373 6f72 7420 3e3d 2030 2e31 312e 3622  ssort >= 0.11.6"
+00000170: 2c0a 5d0a 5b65 6e76 732e 6465 6661 756c  ,.].[envs.defaul
+00000180: 742e 7363 7269 7074 735d 0a63 6f76 203d  t.scripts].cov =
+00000190: 205b 2263 6f76 6572 6167 6520 7275 6e20   ["coverage run 
+000001a0: 7b61 7267 737d 222c 2022 636f 7665 7261  {args}", "covera
+000001b0: 6765 2072 6570 6f72 7420 2d6d 225d 0a6c  ge report -m"].l
+000001c0: 696e 7420 3d20 5b0a 2020 222d 2072 7566  int = [.  "- ruf
+000001d0: 6620 6368 6563 6b20 2e22 2c0a 2020 222d  f check .",.  "-
+000001e0: 2070 796c 696e 7420 7372 6322 2c0a 2020   pylint src",.  
+000001f0: 222d 2062 6c61 636b 202d 2d71 7569 6574  "- black --quiet
+00000200: 202d 2d63 6865 636b 202d 2d64 6966 6620   --check --diff 
+00000210: 2e22 2c0a 2020 222d 2070 7972 6967 6874  .",.  "- pyright
+00000220: 2d70 6f6c 6974 6522 2c0a 2020 222d 2073  -polite",.  "- s
+00000230: 736f 7274 202d 2d63 6865 636b 202d 2d64  sort --check --d
+00000240: 6966 6620 7372 6322 2c0a 5d0a 0a23 2054  iff src",.]..# T
+00000250: 656d 706c 6174 6573 0a5b 656e 7673 2e62  emplates.[envs.b
+00000260: 6173 655d 0a64 6570 656e 6465 6e63 6965  ase].dependencie
+00000270: 7320 3d20 5b0a 2020 2263 6f76 6572 6167  s = [.  "coverag
+00000280: 6520 7e3d 2037 2e32 222c 0a20 2022 7079  e ~= 7.2",.  "py
+00000290: 7465 7374 207e 3d20 372e 3222 2c0a 5d0a  test ~= 7.2",.].
+000002a0: 0a23 2047 6974 4875 6220 576f 726b 666c  .# GitHub Workfl
+000002b0: 6f77 3a20 4349 0a5b 656e 7673 2e63 695d  ow: CI.[envs.ci]
+000002c0: 0a74 656d 706c 6174 6520 3d20 2262 6173  .template = "bas
+000002d0: 6522 0a70 6c61 7466 6f72 6d73 203d 205b  e".platforms = [
+000002e0: 226c 696e 7578 222c 2022 6d61 636f 7322  "linux", "macos"
+000002f0: 2c20 2277 696e 646f 7773 225d 0a5b 656e  , "windows"].[en
+00000300: 7673 2e63 692e 7363 7269 7074 735d 0a63  vs.ci.scripts].c
+00000310: 6f76 203d 205b 2263 6f76 6572 6167 6520  ov = ["coverage 
+00000320: 7275 6e20 7b61 7267 737d 222c 2022 636f  run {args}", "co
+00000330: 7665 7261 6765 2063 6f6d 6269 6e65 202d  verage combine -
+00000340: 7120 2d2d 6b65 6570 222c 2022 636f 7665  q --keep", "cove
+00000350: 7261 6765 2072 6570 6f72 7420 2d6d 225d  rage report -m"]
+00000360: 0a63 6f76 2d63 6f6d 6269 6e65 203d 205b  .cov-combine = [
+00000370: 2263 6f76 6572 6167 6520 636f 6d62 696e  "coverage combin
+00000380: 6520 2d71 222c 2022 636f 7665 7261 6765  e -q", "coverage
+00000390: 206a 736f 6e20 2d71 202d 6f20 636f 7665   json -q -o cove
+000003a0: 7261 6765 2e6a 736f 6e22 5d0a 5b5b 656e  rage.json"].[[en
+000003b0: 7673 2e63 692e 6d61 7472 6978 5d5d 0a70  vs.ci.matrix]].p
+000003c0: 7974 686f 6e20 3d20 5b22 332e 3722 2c20  ython = ["3.7", 
+000003d0: 2233 2e38 222c 2022 332e 3922 2c20 2233  "3.8", "3.9", "3
+000003e0: 2e31 3022 2c20 2233 2e31 3122 2c20 2270  .10", "3.11", "p
+000003f0: 7970 7933 2e37 222c 2022 7079 7079 332e  ypy3.7", "pypy3.
+00000400: 3822 2c20 2270 7970 7933 2e39 225d 0a    8", "pypy3.9"].
```

### Comparing `leapseconds-2023.3.3/pyproject.toml` & `leapseconds-2023.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,18 @@
 Homepage = "https://github.com/jamielinux/leapseconds"
 Issues = "https://github.com/jamielinux/leapseconds/issues"
 Source = "https://github.com/jamielinux/leapseconds"
 
 # pytest & coverage
 [tool.pytest.ini_options]
 addopts = [
-    "--import-mode=importlib",
+  "--import-mode=importlib",
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

### Comparing `leapseconds-2023.3.3/PKG-INFO` & `leapseconds-2023.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leapseconds
-Version: 2023.3.3
+Version: 2023.4.0
 Summary: Data for official leap seconds, provided as a tuple of Unix timestamps
 Project-URL: Homepage, https://github.com/jamielinux/leapseconds
 Project-URL: Issues, https://github.com/jamielinux/leapseconds/issues
 Project-URL: Source, https://github.com/jamielinux/leapseconds
 Author-email: Jamie Nguyen <j@jamielinux.com>
 License-Expression: MIT
 License-File: LICENSE
```

