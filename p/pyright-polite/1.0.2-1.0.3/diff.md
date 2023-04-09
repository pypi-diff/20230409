# Comparing `tmp/pyright_polite-1.0.2.tar.gz` & `tmp/pyright_polite-1.0.3.tar.gz`

## Comparing `pyright_polite-1.0.2.tar` & `pyright_polite-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/.justfile
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/.pylintrc
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/setup.cfg
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/src/pyright_polite/__about__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/src/pyright_polite/__init__.py
--rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/src/pyright_polite/cli.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/src/pyright_polite/main.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/src/pyright_polite/platform.py
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/src/pyright_polite/polite.py
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/src/pyright_polite/pyright.py
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/LICENSE
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/README.md
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/hatch.toml
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 pyright_polite-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/.justfile
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/.pylintrc
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/setup.cfg
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/__about__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/__init__.py
+-rw-r--r--   0        0        0     8846 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/cli.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/main.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/platform.py
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/polite.py
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/src/pyright_polite/pyright.py
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/LICENSE
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/README.md
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/hatch.toml
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 pyright_polite-1.0.3/PKG-INFO
```

### Comparing `pyright_polite-1.0.2/.justfile` & `pyright_polite-1.0.3/.justfile`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.2/.pre-commit-config.yaml` & `pyright_polite-1.0.3/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -30,7 +30,8 @@
     rev: bf7a16254ec96b084a6caf3d435ec18f0f245cc7  # frozen: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/bwhmather/ssort
     rev: 85ce691bd9dd6528a267aaf3e1ac7d455ecd773c  # frozen: v0.11.6
     hooks:
       - id: ssort
+        args: ["src"]
```

### Comparing `pyright_polite-1.0.2/src/pyright_polite/cli.py` & `pyright_polite-1.0.3/src/pyright_polite/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             argv.append(flag)
             if isinstance(arg_value, list):
                 argv.append(arg_value[0])
 
     # If the user passes `--outputjson` manually, always pass this to pyright even if
     # it will clash with one of the other command-line arguments that don't support
     # this mode. We'll just let pyright complain to the user about the clash.
-    if parsed_args.outputjson or set(argv[1:]).isdisjoint(NON_JSON_ARGS):
+    if parsed_args.outputjson or not any(arg in NON_JSON_ARGS for arg in argv[1:]):
         argv.append("--outputjson")
 
     for file in parsed_args.files:
         argv.append(file)
 
     return argv
 
@@ -201,18 +201,18 @@
         Mode: The deduced mode of operation.
     """
     mode: Mode = Mode.JSON
 
     if "--outputjson" in args:
         return mode
 
-    if not set(args).isdisjoint(PLAINTEXT_ARGS):
+    if any(arg in PLAINTEXT_ARGS for arg in args):
         mode = Mode.PLAINTEXT
 
-    if not set(args).isdisjoint(UNFILTERED_ARGS):
+    if any(arg in UNFILTERED_ARGS for arg in args):
         mode = Mode.UNFILTERED
 
     return mode
 
 
 def parse_cli() -> CommandLine:
     """Handle command line arguments.
```

### Comparing `pyright_polite-1.0.2/src/pyright_polite/main.py` & `pyright_polite-1.0.3/src/pyright_polite/main.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.2/src/pyright_polite/platform.py` & `pyright_polite-1.0.3/src/pyright_polite/platform.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.2/src/pyright_polite/polite.py` & `pyright_polite-1.0.3/src/pyright_polite/polite.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.2/src/pyright_polite/pyright.py` & `pyright_polite-1.0.3/src/pyright_polite/pyright.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.2/.gitignore` & `pyright_polite-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.2/LICENSE` & `pyright_polite-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.2/README.md` & `pyright_polite-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 cmd [3] | - pyright-polite
 Found 8 source files
 0 errors, 0 warnings, 0 informations
 cmd [4] | - ssort --check --diff .
 8 files would be left unchanged
 ```
 
-Error messages are still shown (eg, if your config file is invalid).
+Error messages are still shown (eg, if your pyright config file is invalid).
 
 ## Installation
 
 You need `pyright` installed (ie, available somewhere in your `PATH`).
 
 See pyright's installation instructions [here][installation]. Usually people install
 either the [pyright npm][pkg_npm] or the [pyright PyPI][pkg_pypi] package.
@@ -133,15 +133,15 @@
 (minus the useless messages), and takes advantage of pyright's `--outputjson` option
 when possible. It launches `pyright` as a subprocess and reads from both stderr and
 stdout using `asyncio` tasks, which means that `--watch` is also supported.
 
 For insight into what messages get hidden, see the [`print_filtered`][print_filtered]
 method.
 
-[print_filtered]: https://github.com/jamielinux/pyright-polite/blob/379f5ed852388000f0c874bff089d72777c90db8/src/pyright_polite/pyright.py#L183-L233
+[print_filtered]: https://github.com/jamielinux/pyright-polite/blob/main/src/pyright_polite/pyright.py#L183-L233
 
 ## Isn't this a bit overkill?
 
 Yes :rofl:
 
 It was primarily a fun weekend project to learn `asyncio`.
```

### Comparing `pyright_polite-1.0.2/hatch.toml` & `pyright_polite-1.0.3/hatch.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,78 +10,77 @@
 00000090: 2022 2f70 6163 6b61 6765 2e6a 736f 6e22   "/package.json"
 000000a0: 2c0a 2020 222f 7465 7374 7322 2c0a 5d0a  ,.  "/tests",.].
 000000b0: 0a23 204c 6f63 616c 2074 6573 7473 0a5b  .# Local tests.[
 000000c0: 656e 7673 2e64 6566 6175 6c74 5d0a 6465  envs.default].de
 000000d0: 7065 6e64 656e 6369 6573 203d 205b 0a20  pendencies = [. 
 000000e0: 2022 626c 6163 6b20 3e3d 2032 332e 312e   "black >= 23.1.
 000000f0: 3022 2c0a 2020 2263 6f76 6572 6167 6520  0",.  "coverage 
-00000100: 7e3d 2037 2e32 222c 0a20 2022 6861 7463  ~= 7.2",.  "hatc
-00000110: 682d 636f 6e74 6169 6e65 7273 207e 3d20  h-containers ~= 
-00000120: 302e 3722 2c0a 2020 2270 7265 2d63 6f6d  0.7",.  "pre-com
-00000130: 6d69 7420 7e3d 2033 2e32 222c 0a20 2022  mit ~= 3.2",.  "
-00000140: 7079 6c69 6e74 207e 3d20 322e 3137 222c  pylint ~= 2.17",
-00000150: 0a20 2022 7079 7465 7374 207e 3d20 372e  .  "pytest ~= 7.
-00000160: 3222 2c0a 2020 2270 7974 6573 742d 6173  2",.  "pytest-as
-00000170: 796e 6369 6f20 7e3d 2030 2e32 3122 2c0a  yncio ~= 0.21",.
-00000180: 2020 2272 7566 6620 3e3d 2030 2e30 2e32    "ruff >= 0.0.2
-00000190: 3537 222c 0a20 2022 7363 7269 7620 3e3d  57",.  "scriv >=
-000001a0: 2031 2e32 2e31 222c 0a20 2022 7373 6f72   1.2.1",.  "ssor
-000001b0: 7420 3e3d 2030 2e31 312e 3622 2c0a 5d0a  t >= 0.11.6",.].
-000001c0: 5b65 6e76 732e 6465 6661 756c 742e 7363  [envs.default.sc
-000001d0: 7269 7074 735d 0a63 6f76 203d 205b 2263  ripts].cov = ["c
-000001e0: 6f76 6572 6167 6520 7275 6e20 7b61 7267  overage run {arg
-000001f0: 737d 222c 2022 636f 7665 7261 6765 2072  s}", "coverage r
-00000200: 6570 6f72 7420 2d6d 225d 0a6c 696e 7420  eport -m"].lint 
-00000210: 3d20 5b0a 2020 222d 2072 7566 6620 6368  = [.  "- ruff ch
-00000220: 6563 6b20 2e22 2c0a 2020 222d 2070 796c  eck .",.  "- pyl
-00000230: 696e 7420 7372 6322 2c0a 2020 222d 2062  int src",.  "- b
-00000240: 6c61 636b 202d 2d71 7569 6574 202d 2d63  lack --quiet --c
-00000250: 6865 636b 202d 2d64 6966 6620 2e22 2c0a  heck --diff .",.
-00000260: 2020 222d 2070 7972 6967 6874 2d70 6f6c    "- pyright-pol
-00000270: 6974 6520 7372 6320 7465 7374 732f 7465  ite src tests/te
-00000280: 7374 5f2a 2e70 7922 2c0a 2020 222d 2073  st_*.py",.  "- s
-00000290: 736f 7274 202d 2d63 6865 636b 202d 2d64  sort --check --d
-000002a0: 6966 6620 7372 6322 2c0a 5d0a 0a23 2054  iff src",.]..# T
-000002b0: 656d 706c 6174 6573 0a5b 656e 7673 2e62  emplates.[envs.b
-000002c0: 6173 655d 0a64 6570 656e 6465 6e63 6965  ase].dependencie
-000002d0: 7320 3d20 5b0a 2020 2263 6f76 6572 6167  s = [.  "coverag
-000002e0: 6520 7e3d 2037 2e32 222c 0a20 2022 7079  e ~= 7.2",.  "py
-000002f0: 7465 7374 207e 3d20 372e 3222 2c0a 2020  test ~= 7.2",.  
-00000300: 2270 7974 6573 742d 6173 796e 6369 6f20  "pytest-asyncio 
-00000310: 7e3d 2030 2e32 3122 2c0a 5d0a 0a23 2070  ~= 0.21",.]..# p
-00000320: 7965 6e76 0a5b 656e 7673 2e70 7965 6e76  yenv.[envs.pyenv
-00000330: 5d0a 7465 6d70 6c61 7465 203d 2022 6261  ].template = "ba
-00000340: 7365 220a 706c 6174 666f 726d 7320 3d20  se".platforms = 
-00000350: 5b22 6c69 6e75 7822 5d0a 5b65 6e76 732e  ["linux"].[envs.
-00000360: 7079 656e 762e 7363 7269 7074 735d 0a63  pyenv.scripts].c
-00000370: 6f76 203d 205b 2263 6f76 6572 6167 6520  ov = ["coverage 
-00000380: 7275 6e20 7b61 7267 737d 222c 2022 636f  run {args}", "co
-00000390: 7665 7261 6765 2072 6570 6f72 7420 2d6d  verage report -m
-000003a0: 225d 0a74 6573 7420 3d20 5b22 7079 7465  "].test = ["pyte
-000003b0: 7374 207b 6172 6773 7d22 5d0a 5b5b 656e  st {args}"].[[en
-000003c0: 7673 2e70 7965 6e76 2e6d 6174 7269 785d  vs.pyenv.matrix]
-000003d0: 5d0a 7079 7468 6f6e 203d 205b 2233 2e37  ].python = ["3.7
-000003e0: 222c 2022 332e 3822 2c20 2233 2e39 222c  ", "3.8", "3.9",
-000003f0: 2022 332e 3130 222c 2022 332e 3131 225d   "3.10", "3.11"]
-00000400: 0a0a 2320 4769 7448 7562 2057 6f72 6b66  ..# GitHub Workf
-00000410: 6c6f 773a 2043 490a 5b65 6e76 732e 6369  low: CI.[envs.ci
-00000420: 5d0a 7465 6d70 6c61 7465 203d 2022 6261  ].template = "ba
-00000430: 7365 220a 706c 6174 666f 726d 7320 3d20  se".platforms = 
-00000440: 5b22 6c69 6e75 7822 2c20 226d 6163 6f73  ["linux", "macos
-00000450: 222c 2022 7769 6e64 6f77 7322 5d0a 5b65  ", "windows"].[e
-00000460: 6e76 732e 6369 2e73 6372 6970 7473 5d0a  nvs.ci.scripts].
-00000470: 636f 7620 3d20 5b22 636f 7665 7261 6765  cov = ["coverage
-00000480: 2072 756e 207b 6172 6773 7d22 2c20 2263   run {args}", "c
-00000490: 6f76 6572 6167 6520 636f 6d62 696e 6520  overage combine 
-000004a0: 2d71 202d 2d6b 6565 7022 2c20 2263 6f76  -q --keep", "cov
-000004b0: 6572 6167 6520 7265 706f 7274 202d 6d22  erage report -m"
-000004c0: 5d0a 636f 762d 636f 6d62 696e 6520 3d20  ].cov-combine = 
-000004d0: 5b22 636f 7665 7261 6765 2063 6f6d 6269  ["coverage combi
-000004e0: 6e65 202d 7122 2c20 2263 6f76 6572 6167  ne -q", "coverag
-000004f0: 6520 6a73 6f6e 202d 7120 2d6f 2063 6f76  e json -q -o cov
-00000500: 6572 6167 652e 6a73 6f6e 225d 0a5b 5b65  erage.json"].[[e
-00000510: 6e76 732e 6369 2e6d 6174 7269 785d 5d0a  nvs.ci.matrix]].
-00000520: 7079 7468 6f6e 203d 205b 2233 2e37 222c  python = ["3.7",
-00000530: 2022 332e 3822 2c20 2233 2e39 222c 2022   "3.8", "3.9", "
-00000540: 332e 3130 222c 2022 332e 3131 222c 2022  3.10", "3.11", "
-00000550: 7079 7079 332e 3722 2c20 2270 7970 7933  pypy3.7", "pypy3
-00000560: 2e38 222c 2022 7079 7079 332e 3922 5d0a  .8", "pypy3.9"].
+00000100: 7e3d 2037 2e32 222c 0a20 2022 7072 652d  ~= 7.2",.  "pre-
+00000110: 636f 6d6d 6974 207e 3d20 332e 3222 2c0a  commit ~= 3.2",.
+00000120: 2020 2270 796c 696e 7420 7e3d 2032 2e31    "pylint ~= 2.1
+00000130: 3722 2c0a 2020 2270 7974 6573 7420 7e3d  7",.  "pytest ~=
+00000140: 2037 2e32 222c 0a20 2022 7079 7465 7374   7.2",.  "pytest
+00000150: 2d61 7379 6e63 696f 207e 3d20 302e 3231  -asyncio ~= 0.21
+00000160: 222c 0a20 2022 7275 6666 203e 3d20 302e  ",.  "ruff >= 0.
+00000170: 302e 3235 3722 2c0a 2020 2273 6372 6976  0.257",.  "scriv
+00000180: 203e 3d20 312e 322e 3122 2c0a 2020 2273   >= 1.2.1",.  "s
+00000190: 736f 7274 203e 3d20 302e 3131 2e36 222c  sort >= 0.11.6",
+000001a0: 0a5d 0a5b 656e 7673 2e64 6566 6175 6c74  .].[envs.default
+000001b0: 2e73 6372 6970 7473 5d0a 636f 7620 3d20  .scripts].cov = 
+000001c0: 5b22 636f 7665 7261 6765 2072 756e 207b  ["coverage run {
+000001d0: 6172 6773 7d22 2c20 2263 6f76 6572 6167  args}", "coverag
+000001e0: 6520 7265 706f 7274 202d 6d22 5d0a 6c69  e report -m"].li
+000001f0: 6e74 203d 205b 0a20 2022 2d20 7275 6666  nt = [.  "- ruff
+00000200: 2063 6865 636b 202e 222c 0a20 2022 2d20   check .",.  "- 
+00000210: 7079 6c69 6e74 2073 7263 222c 0a20 2022  pylint src",.  "
+00000220: 2d20 626c 6163 6b20 2d2d 7175 6965 7420  - black --quiet 
+00000230: 2d2d 6368 6563 6b20 2d2d 6469 6666 202e  --check --diff .
+00000240: 222c 0a20 2022 2d20 7079 7269 6768 742d  ",.  "- pyright-
+00000250: 706f 6c69 7465 2073 7263 2074 6573 7473  polite src tests
+00000260: 2f74 6573 745f 2a2e 7079 222c 0a20 2022  /test_*.py",.  "
+00000270: 2d20 7373 6f72 7420 2d2d 6368 6563 6b20  - ssort --check 
+00000280: 2d2d 6469 6666 2073 7263 222c 0a5d 0a0a  --diff src",.]..
+00000290: 2320 5465 6d70 6c61 7465 730a 5b65 6e76  # Templates.[env
+000002a0: 732e 6261 7365 5d0a 6465 7065 6e64 656e  s.base].dependen
+000002b0: 6369 6573 203d 205b 0a20 2022 636f 7665  cies = [.  "cove
+000002c0: 7261 6765 207e 3d20 372e 3222 2c0a 2020  rage ~= 7.2",.  
+000002d0: 2270 7974 6573 7420 7e3d 2037 2e32 222c  "pytest ~= 7.2",
+000002e0: 0a20 2022 7079 7465 7374 2d61 7379 6e63  .  "pytest-async
+000002f0: 696f 207e 3d20 302e 3231 222c 0a5d 0a0a  io ~= 0.21",.]..
+00000300: 2320 7079 656e 760a 5b65 6e76 732e 7079  # pyenv.[envs.py
+00000310: 656e 765d 0a74 656d 706c 6174 6520 3d20  env].template = 
+00000320: 2262 6173 6522 0a70 6c61 7466 6f72 6d73  "base".platforms
+00000330: 203d 205b 226c 696e 7578 225d 0a5b 656e   = ["linux"].[en
+00000340: 7673 2e70 7965 6e76 2e73 6372 6970 7473  vs.pyenv.scripts
+00000350: 5d0a 636f 7620 3d20 5b22 636f 7665 7261  ].cov = ["covera
+00000360: 6765 2072 756e 207b 6172 6773 7d22 2c20  ge run {args}", 
+00000370: 2263 6f76 6572 6167 6520 7265 706f 7274  "coverage report
+00000380: 202d 6d22 5d0a 7465 7374 203d 205b 2270   -m"].test = ["p
+00000390: 7974 6573 7420 7b61 7267 737d 225d 0a5b  ytest {args}"].[
+000003a0: 5b65 6e76 732e 7079 656e 762e 6d61 7472  [envs.pyenv.matr
+000003b0: 6978 5d5d 0a70 7974 686f 6e20 3d20 5b22  ix]].python = ["
+000003c0: 332e 3722 2c20 2233 2e38 222c 2022 332e  3.7", "3.8", "3.
+000003d0: 3922 2c20 2233 2e31 3022 2c20 2233 2e31  9", "3.10", "3.1
+000003e0: 3122 5d0a 0a23 2047 6974 4875 6220 576f  1"]..# GitHub Wo
+000003f0: 726b 666c 6f77 3a20 4349 0a5b 656e 7673  rkflow: CI.[envs
+00000400: 2e63 695d 0a74 656d 706c 6174 6520 3d20  .ci].template = 
+00000410: 2262 6173 6522 0a70 6c61 7466 6f72 6d73  "base".platforms
+00000420: 203d 205b 226c 696e 7578 222c 2022 6d61   = ["linux", "ma
+00000430: 636f 7322 2c20 2277 696e 646f 7773 225d  cos", "windows"]
+00000440: 0a5b 656e 7673 2e63 692e 7363 7269 7074  .[envs.ci.script
+00000450: 735d 0a63 6f76 203d 205b 2263 6f76 6572  s].cov = ["cover
+00000460: 6167 6520 7275 6e20 7b61 7267 737d 222c  age run {args}",
+00000470: 2022 636f 7665 7261 6765 2063 6f6d 6269   "coverage combi
+00000480: 6e65 202d 7120 2d2d 6b65 6570 222c 2022  ne -q --keep", "
+00000490: 636f 7665 7261 6765 2072 6570 6f72 7420  coverage report 
+000004a0: 2d6d 225d 0a63 6f76 2d63 6f6d 6269 6e65  -m"].cov-combine
+000004b0: 203d 205b 2263 6f76 6572 6167 6520 636f   = ["coverage co
+000004c0: 6d62 696e 6520 2d71 222c 2022 636f 7665  mbine -q", "cove
+000004d0: 7261 6765 206a 736f 6e20 2d71 202d 6f20  rage json -q -o 
+000004e0: 636f 7665 7261 6765 2e6a 736f 6e22 5d0a  coverage.json"].
+000004f0: 5b5b 656e 7673 2e63 692e 6d61 7472 6978  [[envs.ci.matrix
+00000500: 5d5d 0a70 7974 686f 6e20 3d20 5b22 332e  ]].python = ["3.
+00000510: 3722 2c20 2233 2e38 222c 2022 332e 3922  7", "3.8", "3.9"
+00000520: 2c20 2233 2e31 3022 2c20 2233 2e31 3122  , "3.10", "3.11"
+00000530: 2c20 2270 7970 7933 2e37 222c 2022 7079  , "pypy3.7", "py
+00000540: 7079 332e 3822 2c20 2270 7970 7933 2e39  py3.8", "pypy3.9
+00000550: 225d 0a                                  "].
```

### Comparing `pyright_polite-1.0.2/pyproject.toml` & `pyright_polite-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 pyright-polite = "pyright_polite.main:main"
 
 # pytest & coverage
 [tool.pytest.ini_options]
 addopts = [
   "--import-mode=importlib",
   "--strict-markers",
+  "--strict-config",
+  "-ra",
 ]
 markers = [
   "asyncio",
   "disable_autouse",
 ]
 asyncio_mode = "auto"
 [tool.coverage.run]
```

### Comparing `pyright_polite-1.0.2/PKG-INFO` & `pyright_polite-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright-polite
-Version: 1.0.2
+Version: 1.0.3
 Summary: An intelligent cross-platform wrapper for pyright that makes it less noisy.
 Project-URL: Homepage, https://github.com/jamielinux/pyright-polite
 Project-URL: Issues, https://github.com/jamielinux/pyright-polite/issues
 Project-URL: Source, https://github.com/jamielinux/pyright-polite
 Author-email: Jamie Nguyen <j@jamielinux.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -95,15 +95,15 @@
 cmd [3] | - pyright-polite
 Found 8 source files
 0 errors, 0 warnings, 0 informations
 cmd [4] | - ssort --check --diff .
 8 files would be left unchanged
 ```
 
-Error messages are still shown (eg, if your config file is invalid).
+Error messages are still shown (eg, if your pyright config file is invalid).
 
 ## Installation
 
 You need `pyright` installed (ie, available somewhere in your `PATH`).
 
 See pyright's installation instructions [here][installation]. Usually people install
 either the [pyright npm][pkg_npm] or the [pyright PyPI][pkg_pypi] package.
@@ -160,15 +160,15 @@
 (minus the useless messages), and takes advantage of pyright's `--outputjson` option
 when possible. It launches `pyright` as a subprocess and reads from both stderr and
 stdout using `asyncio` tasks, which means that `--watch` is also supported.
 
 For insight into what messages get hidden, see the [`print_filtered`][print_filtered]
 method.
 
-[print_filtered]: https://github.com/jamielinux/pyright-polite/blob/379f5ed852388000f0c874bff089d72777c90db8/src/pyright_polite/pyright.py#L183-L233
+[print_filtered]: https://github.com/jamielinux/pyright-polite/blob/main/src/pyright_polite/pyright.py#L183-L233
 
 ## Isn't this a bit overkill?
 
 Yes :rofl:
 
 It was primarily a fun weekend project to learn `asyncio`.
```

