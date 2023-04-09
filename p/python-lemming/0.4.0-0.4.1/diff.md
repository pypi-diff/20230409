# Comparing `tmp/python-lemming-0.4.0.tar.gz` & `tmp/python-lemming-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lemming-0.4.0.tar", last modified: Tue Mar 28 17:40:11 2023, max compression
+gzip compressed data, was "python-lemming-0.4.1.tar", last modified: Sun Apr  9 18:26:14 2023, max compression
```

## Comparing `python-lemming-0.4.0.tar` & `python-lemming-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 17:40:11.939268 python-lemming-0.4.0/
--rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     6320 2023-03-28 17:40:11.939268 python-lemming-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     5356 2023-03-08 18:21:42.000000 python-lemming-0.4.0/README.md
--rw-rw-rw-   0        0        0     1126 2023-03-08 18:13:58.000000 python-lemming-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     1420 2023-03-28 17:40:11.944269 python-lemming-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-28 17:40:11.512768 python-lemming-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-28 17:40:11.909269 python-lemming-0.4.0/src/lemming/
--rw-rw-rw-   0        0        0      922 2023-03-28 17:37:03.000000 python-lemming-0.4.0/src/lemming/__init__.py
--rw-rw-rw-   0        0        0    11301 2023-03-08 18:14:19.000000 python-lemming-0.4.0/src/lemming/__main__.py
--rw-rw-rw-   0        0        0    11385 2023-03-08 18:00:48.000000 python-lemming-0.4.0/src/lemming/config.py
--rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.4.0/src/lemming/py.typed
-drwxrwxrwx   0        0        0        0 2023-03-28 17:40:11.938268 python-lemming-0.4.0/src/python_lemming.egg-info/
--rw-rw-rw-   0        0        0     6320 2023-03-28 17:40:11.000000 python-lemming-0.4.0/src/python_lemming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-03-28 17:40:11.000000 python-lemming-0.4.0/src/python_lemming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 17:40:11.000000 python-lemming-0.4.0/src/python_lemming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-03-28 17:40:11.000000 python-lemming-0.4.0/src/python_lemming.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.4.0/src/python_lemming.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2023-03-28 17:40:11.000000 python-lemming-0.4.0/src/python_lemming.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-28 17:40:11.000000 python-lemming-0.4.0/src/python_lemming.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 18:26:14.116500 python-lemming-0.4.1/
+-rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     6320 2023-04-09 18:26:14.117501 python-lemming-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5356 2023-03-08 18:21:42.000000 python-lemming-0.4.1/README.md
+-rw-rw-rw-   0        0        0     1126 2023-03-08 18:13:58.000000 python-lemming-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1447 2023-04-09 18:26:14.130500 python-lemming-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 18:26:14.042501 python-lemming-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-09 18:26:14.074504 python-lemming-0.4.1/src/lemming/
+-rw-rw-rw-   0        0        0      922 2023-04-09 18:25:14.000000 python-lemming-0.4.1/src/lemming/__init__.py
+-rw-rw-rw-   0        0        0    11301 2023-03-08 18:14:19.000000 python-lemming-0.4.1/src/lemming/__main__.py
+-rw-rw-rw-   0        0        0    11451 2023-04-09 18:17:18.000000 python-lemming-0.4.1/src/lemming/config.py
+-rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.4.1/src/lemming/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-09 18:26:14.115501 python-lemming-0.4.1/src/python_lemming.egg-info/
+-rw-rw-rw-   0        0        0     6320 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.4.1/src/python_lemming.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       85 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/top_level.txt
```

### Comparing `python-lemming-0.4.0/LICENSE` & `python-lemming-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lemming-0.4.0/PKG-INFO` & `python-lemming-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lemming
-Version: 0.4.0
+Version: 0.4.1
 Summary: Lemming is a tool for formatting and linting code.
 Home-page: https://github.com/koviubi56/lemming
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: GPL
 Keywords: lemming,format,formatter,lint,linting,linter
 Platform: unix
```

### Comparing `python-lemming-0.4.0/README.md` & `python-lemming-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `python-lemming-0.4.0/pyproject.toml` & `python-lemming-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-lemming-0.4.0/setup.cfg` & `python-lemming-0.4.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -56,34 +56,36 @@
 00000370: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
 00000380: 6167 6573 203d 200d 0a09 6c65 6d6d 696e  ages = ...lemmin
 00000390: 670d 0a69 6e73 7461 6c6c 5f72 6571 7569  g..install_requi
 000003a0: 7265 7320 3d20 0d0a 0974 6f6d 6c69 3b20  res = ...tomli; 
 000003b0: 7079 7468 6f6e 5f76 6572 7369 6f6e 3c27  python_version<'
 000003c0: 332e 3131 270d 0a09 7079 7468 6f6e 2d6d  3.11'...python-m
 000003d0: 796c 6f67 3e3d 302e 372e 300d 0a09 636f  ylog>=0.7.0...co
-000003e0: 6e66 7a0d 0a70 7974 686f 6e5f 7265 7175  nfz..python_requ
-000003f0: 6972 6573 203d 203e 3d33 2e31 310d 0a70  ires = >=3.11..p
-00000400: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
-00000410: 3d73 7263 0d0a 7a69 705f 7361 6665 203d  =src..zip_safe =
-00000420: 206e 6f0d 0a0d 0a5b 6f70 7469 6f6e 732e   no....[options.
-00000430: 7061 636b 6167 655f 6461 7461 5d0d 0a6c  package_data]..l
-00000440: 656d 6d69 6e67 203d 2070 792e 7479 7065  emming = py.type
-00000450: 640d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  d....[options.en
-00000460: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
-00000470: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
-00000480: 0a09 6c65 6d6d 696e 6720 3d20 6c65 6d6d  ..lemming = lemm
-00000490: 696e 672e 5f5f 6d61 696e 5f5f 3a6d 6169  ing.__main__:mai
-000004a0: 6e0d 0a0d 0a5b 7079 636f 6465 7374 796c  n....[pycodestyl
-000004b0: 655d 0d0a 6967 6e6f 7265 203d 2045 3230  e]..ignore = E20
-000004c0: 330d 0a0d 0a5b 7079 6c61 6d61 5d0d 0a69  3....[pylama]..i
-000004d0: 676e 6f72 6520 3d20 5735 3033 0d0a 0d0a  gnore = W503....
-000004e0: 5b66 6c61 6b65 385d 0d0a 6578 7465 6e64  [flake8]..extend
-000004f0: 2d69 676e 6f72 6520 3d20 5735 3033 0d0a  -ignore = W503..
-00000500: 6578 7465 6e64 2d65 7863 6c75 6465 203d  extend-exclude =
-00000510: 2076 656e 762c 2a63 6163 6865 2a0d 0a70   venv,*cache*..p
-00000520: 6572 2d66 696c 652d 6967 6e6f 7265 7320  er-file-ignores 
-00000530: 3d20 0d0a 0974 6573 7473 2f2a 3a20 5331  = ...tests/*: S1
-00000540: 3031 0d0a 0d0a 5b69 736f 7274 5d0d 0a70  01....[isort]..p
-00000550: 726f 6669 6c65 203d 2062 6c61 636b 0d0a  rofile = black..
-00000560: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000570: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000580: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+000003e0: 6e66 7a0d 0a09 7479 7069 6e67 2d65 7874  nfz...typing-ext
+000003f0: 656e 7369 6f6e 733e 3d34 2e34 2e30 0d0a  ensions>=4.4.0..
+00000400: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000410: 3d20 3e3d 332e 3131 0d0a 7061 636b 6167  = >=3.11..packag
+00000420: 655f 6469 7220 3d20 0d0a 093d 7372 630d  e_dir = ...=src.
+00000430: 0a7a 6970 5f73 6166 6520 3d20 6e6f 0d0a  .zip_safe = no..
+00000440: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000450: 6765 5f64 6174 615d 0d0a 6c65 6d6d 696e  ge_data]..lemmin
+00000460: 6720 3d20 7079 2e74 7970 6564 0d0a 0d0a  g = py.typed....
+00000470: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
+00000480: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
+00000490: 7363 7269 7074 7320 3d20 0d0a 096c 656d  scripts = ...lem
+000004a0: 6d69 6e67 203d 206c 656d 6d69 6e67 2e5f  ming = lemming._
+000004b0: 5f6d 6169 6e5f 5f3a 6d61 696e 0d0a 0d0a  _main__:main....
+000004c0: 5b70 7963 6f64 6573 7479 6c65 5d0d 0a69  [pycodestyle]..i
+000004d0: 676e 6f72 6520 3d20 4532 3033 0d0a 0d0a  gnore = E203....
+000004e0: 5b70 796c 616d 615d 0d0a 6967 6e6f 7265  [pylama]..ignore
+000004f0: 203d 2057 3530 330d 0a0d 0a5b 666c 616b   = W503....[flak
+00000500: 6538 5d0d 0a65 7874 656e 642d 6967 6e6f  e8]..extend-igno
+00000510: 7265 203d 2057 3530 330d 0a65 7874 656e  re = W503..exten
+00000520: 642d 6578 636c 7564 6520 3d20 7665 6e76  d-exclude = venv
+00000530: 2c2a 6361 6368 652a 0d0a 7065 722d 6669  ,*cache*..per-fi
+00000540: 6c65 2d69 676e 6f72 6573 203d 200d 0a09  le-ignores = ...
+00000550: 7465 7374 732f 2a3a 2053 3130 310d 0a0d  tests/*: S101...
+00000560: 0a5b 6973 6f72 745d 0d0a 7072 6f66 696c  .[isort]..profil
+00000570: 6520 3d20 626c 6163 6b0d 0a0d 0a5b 6567  e = black....[eg
+00000580: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000590: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+000005a0: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `python-lemming-0.4.0/src/lemming/__init__.py` & `python-lemming-0.4.1/src/lemming/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # SPDX-License-Identifier: GPL-3.0-or-later
 __all__ = ["__version__", "logger"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 import mylog
 
 logger = mylog.root.get_child("lemming")
 logger.threshold = mylog.Level.info
```

### Comparing `python-lemming-0.4.0/src/lemming/__main__.py` & `python-lemming-0.4.1/src/lemming/__main__.py`

 * *Files identical despite different names*

### Comparing `python-lemming-0.4.0/src/lemming/config.py` & `python-lemming-0.4.1/src/lemming/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,16 +315,17 @@
             dict_,
             ["packages", "command", "run_first"],
         )
         return cls(**dict_)
 
 
 class Config(ConfZ):
-    formatters: List[Formatter]
-    linters: List[Linter]
+    # we should be safe with mutable default arguments
+    formatters: List[Formatter] = []
+    linters: List[Linter] = []
     # ^ also modify within read_config_file()
     fail_fast: bool = True
 
     def get_first_linters(self) -> List[Linter]:
         return [linter for linter in self.linters if linter.run_first]
 
     def get_other_linters(self) -> List[Linter]:
```

### Comparing `python-lemming-0.4.0/src/python_lemming.egg-info/PKG-INFO` & `python-lemming-0.4.1/src/python_lemming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lemming
-Version: 0.4.0
+Version: 0.4.1
 Summary: Lemming is a tool for formatting and linting code.
 Home-page: https://github.com/koviubi56/lemming
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: GPL
 Keywords: lemming,format,formatter,lint,linting,linter
 Platform: unix
```

