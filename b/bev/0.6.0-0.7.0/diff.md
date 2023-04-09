# Comparing `tmp/bev-0.6.0.tar.gz` & `tmp/bev-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bev-0.6.0.tar", last modified: Mon Jan 30 19:16:37 2023, max compression
+gzip compressed data, was "bev-0.7.0.tar", last modified: Sun Apr  9 19:35:45 2023, max compression
```

## Comparing `bev-0.6.0.tar` & `bev-0.7.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 19:16:37.687378 bev-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-01-30 19:16:35.000000 bev-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-30 19:16:35.000000 bev-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-01-30 19:16:37.687378 bev-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-01-30 19:16:35.000000 bev-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 19:16:37.683378 bev-0.6.0/bev/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-30 19:16:35.000000 bev-0.6.0/bev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-30 19:16:35.000000 bev-0.6.0/bev/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 19:16:37.687378 bev-0.6.0/bev/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/blame.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-01-30 19:16:35.000000 bev-0.6.0/bev/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 19:16:37.687378 bev-0.6.0/bev/config/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-30 19:16:35.000000 bev-0.6.0/bev/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-01-30 19:16:35.000000 bev-0.6.0/bev/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-01-30 19:16:35.000000 bev-0.6.0/bev/config/hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-01-30 19:16:35.000000 bev-0.6.0/bev/config/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-01-30 19:16:35.000000 bev-0.6.0/bev/config/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-01-30 19:16:35.000000 bev-0.6.0/bev/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-01-30 19:16:35.000000 bev-0.6.0/bev/config/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-01-30 19:16:35.000000 bev-0.6.0/bev/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-30 19:16:35.000000 bev-0.6.0/bev/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-01-30 19:16:35.000000 bev-0.6.0/bev/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-30 19:16:35.000000 bev-0.6.0/bev/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-01-30 19:16:35.000000 bev-0.6.0/bev/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-01-30 19:16:35.000000 bev-0.6.0/bev/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-30 19:16:35.000000 bev-0.6.0/bev/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-01-30 19:16:35.000000 bev-0.6.0/bev/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 19:16:35.000000 bev-0.6.0/bev/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-30 19:16:35.000000 bev-0.6.0/bev/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-01-30 19:16:35.000000 bev-0.6.0/bev/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-30 19:16:35.000000 bev-0.6.0/bev/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-01-30 19:16:35.000000 bev-0.6.0/bev/vc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-01-30 19:16:35.000000 bev-0.6.0/bev/wc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 19:16:37.683378 bev-0.6.0/bev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-01-30 19:16:37.000000 bev-0.6.0/bev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-30 19:16:37.000000 bev-0.6.0/bev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 19:16:37.000000 bev-0.6.0/bev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-30 19:16:37.000000 bev-0.6.0/bev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-30 19:16:37.000000 bev-0.6.0/bev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-30 19:16:37.000000 bev-0.6.0/bev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-01-30 19:16:35.000000 bev-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-30 19:16:35.000000 bev-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 19:16:37.687378 bev-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-01-30 19:16:35.000000 bev-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:45.350534 bev-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-04-09 19:35:41.000000 bev-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-09 19:35:41.000000 bev-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-09 19:35:45.350534 bev-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-09 19:35:41.000000 bev-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:45.346534 bev-0.7.0/bev/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-09 19:35:41.000000 bev-0.7.0/bev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 19:35:41.000000 bev-0.7.0/bev/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:45.350534 bev-0.7.0/bev/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/blame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:45.350534 bev-0.7.0/bev/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-09 19:35:41.000000 bev-0.7.0/bev/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-09 19:35:41.000000 bev-0.7.0/bev/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-09 19:35:41.000000 bev-0.7.0/bev/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-09 19:35:41.000000 bev-0.7.0/bev/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-04-09 19:35:41.000000 bev-0.7.0/bev/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:41.000000 bev-0.7.0/bev/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-09 19:35:41.000000 bev-0.7.0/bev/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:41.000000 bev-0.7.0/bev/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-09 19:35:41.000000 bev-0.7.0/bev/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-09 19:35:41.000000 bev-0.7.0/bev/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-09 19:35:41.000000 bev-0.7.0/bev/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-09 19:35:41.000000 bev-0.7.0/bev/vc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-04-09 19:35:41.000000 bev-0.7.0/bev/wc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:45.350534 bev-0.7.0/bev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-09 19:35:41.000000 bev-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 19:35:41.000000 bev-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:35:45.350534 bev-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-09 19:35:41.000000 bev-0.7.0/setup.py
```

### Comparing `bev-0.6.0/LICENSE` & `bev-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bev-0.6.0/PKG-INFO` & `bev-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bev
-Version: 0.6.0
+Version: 0.7.0
 Summary: A small manager for versioned data
 Home-page: https://github.com/neuro-ml/bev
 License: MIT
-Download-URL: https://github.com/neuro-ml/bev/archive/v0.6.0.tar.gz
+Download-URL: https://github.com/neuro-ml/bev/archive/v0.7.0.tar.gz
 Keywords: data,version control
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bev-0.6.0/README.md` & `bev-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bev-0.6.0/bev/cli/add.py` & `bev-0.7.0/bev/cli/add.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
 import os
 import shutil
 from collections import OrderedDict
 from pathlib import Path
-from typing import Optional, List
+from typing import List, Optional
 
 import typer
-from tqdm.auto import tqdm
 from rich.progress import track
+from tqdm.auto import tqdm
 
-from .app import app_command
-from .utils import normalize_sources_and_destination
 from ..exceptions import HashError
 from ..hash import is_hash, to_hash
 from ..interface import Repository
-from ..ops import gather, Conflict, save_hash, load_hash
-from ..utils import deprecate, PathOrStr
+from ..ops import Conflict, gather, load_hash, save_hash
+from ..utils import PathOrStr, deprecate
+from .app import app_command
+from .utils import normalize_sources_and_destination
 
 
 @app_command
 def add(
         sources: List[Path] = typer.Argument(..., help='The source paths to add', show_default=False),
         destination: Optional[Path] = typer.Option(
             None, '--destination', '--dst',
@@ -117,27 +117,27 @@
     tree = OrderedDict((k, tree[k]) for k in sorted(tree))
     # FIXME
     tree_path = destination.parent / f'{destination.name}.hash.temp'
 
     # TODO: storage should allow writing directly from memory
     with open(tree_path, 'w') as file:
         json.dump(tree, file)
-    key = repo.storage.write(tree_path)
+    key = repo.storage.write(tree_path).hex()
     os.remove(tree_path)
 
     with open(destination, 'w') as file:
         file.write(f'T:{key}')
 
     return key
 
 
 @deprecate
 def add_file(repo: Repository, source: Path, destination: Optional[Path], keep: bool):  # pragma: no cover
     validate_file(source)
-    key = repo.storage.write(source)
+    key = repo.storage.write(source).hex()
 
     if destination is not None:
         assert is_hash(destination)
         with open(destination, 'w') as file:
             file.write(key)
 
     if not keep:
```

### Comparing `bev-0.6.0/bev/cli/app.py` & `bev-0.7.0/bev/cli/app.py`

 * *Files identical despite different names*

### Comparing `bev-0.6.0/bev/cli/blame.py` & `bev-0.7.0/bev/cli/blame.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from pathlib import Path
 from datetime import datetime
+from pathlib import Path
 
 import typer
 from tqdm.auto import tqdm
 
-from .app import app_command
 from ..hash import from_hash, is_hash
 from ..shortcuts import get_current_repo
 from ..utils import call_git
+from .app import app_command
 
 
 @app_command
 def blame(
         path: Path = typer.Argument(..., help='Path to the hash'),
         relative: str = typer.Argument(..., help='The relative path inside the hashed folder')
 ):
```

### Comparing `bev-0.6.0/bev/cli/fetch.py` & `bev-0.7.0/bev/cli/fetch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-from typing import List
 from pathlib import Path
+from typing import List
 
 import typer
 from rich.progress import track
 
 from ..exceptions import HashError
+from ..hash import from_hash, is_hash, is_tree, load_key, load_tree, strip_tree, to_hash
 from ..interface import Repository
 from ..shortcuts import get_consistent_repo
-from ..hash import is_hash, to_hash, load_tree, load_key, strip_tree, is_tree, from_hash
 from ..utils import HashNotFound
 from .app import app_command
 
 
 def _fetch(repo: Repository, path: Path):
     key = load_key(path)
     if is_tree(key):
         key = strip_tree(key)
-        keys = list(set(repo.storage.read(load_tree, key, fetch=True).values()))
+        keys = sorted(set(map(bytes.fromhex, repo.storage.read(load_tree, key, fetch=True).values())))
     else:
-        keys = [key]
+        keys = [bytes.fromhex(key)]
 
     desc = str(from_hash(path))
     if len(desc) > 30:
         desc = desc[:27] + '...'
 
-    missing = set(keys) - set(track(
-        repo.storage.fetch(keys, verbose=False, legacy=False),
-        description=desc, total=len(keys),
-    ))
+    missing = {k for k, success in track(repo.storage.fetch(keys), description=desc, total=len(keys)) if not success}
     if missing:
         raise HashNotFound(f'Could not fetch {len(missing)} key(s) from remote')
 
 
 @app_command
 def fetch(
         paths: List[Path] = typer.Argument(None, help='The paths to fetch', show_default='The current directory'),
```

### Comparing `bev-0.6.0/bev/cli/init.py` & `bev-0.7.0/bev/cli/init.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 
 import typer
 import yaml
 from tarn.config import CONFIG_NAME as STORAGE_CONFIG_NAME, StorageConfig
 from tarn.utils import mkdir
 
-from .app import app_command
 from ..config import CONFIG, load_config
 from ..shortcuts import get_consistent_repo_root
+from .app import app_command
 
 
 @app_command
 def init(
         repository: Path = typer.Option(
             None, '--repository', '--repo', help='The bev repository. It is usually detected automatically',
             show_default=False,
```

### Comparing `bev-0.6.0/bev/cli/pull.py` & `bev-0.7.0/bev/cli/pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import shutil
 import warnings
 from enum import Enum
 from pathlib import Path
-from typing import Optional, List
+from typing import List, Optional
 
 import typer
 from rich.progress import track
 
+from ..exceptions import HashError
+from ..hash import from_hash, is_hash, to_hash
+from ..ops import Conflict, load_hash
 from .add import add
-from .app import cli_error, _app, app_command
+from .app import _app, app_command, cli_error
 from .utils import normalize_sources, normalize_sources_and_destination
-from ..exceptions import HashError
-from ..hash import is_hash, to_hash, from_hash
-from ..ops import load_hash, Conflict
 
 
 class PullMode(Enum):
     """
     How to restore the files:
 
     hash - restore the file hash. Useful for basic files/folders manipulation, e.g. removing parts of a tree
```

### Comparing `bev-0.6.0/bev/cli/storage.py` & `bev-0.7.0/bev/cli/storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import hashlib
 from enum import Enum
 from pathlib import Path
 from typing import List
 
 import typer
-from tarn.config import init_storage, StorageConfig
+from tarn.config import StorageConfig, init_storage
 
 from .app import app_command, cli_error
 
 
 # because typer can't just accept a list of choices
 def upd(d):
     for algo in sorted(hashlib.algorithms_guaranteed):
```

### Comparing `bev-0.6.0/bev/cli/update.py` & `bev-0.7.0/bev/cli/update.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import warnings
 from pathlib import Path
 from typing import Optional
 
 import typer
 
+from ..ops import Conflict
 from .add import add
 from .app import _app
-from ..ops import Conflict
 
 
 @_app.command(deprecated=True)
 def update(
         source: Path = typer.Argument(..., help='The source path to gather', show_default=False),
         destination: Optional[Path] = typer.Option(
             None, '--destination', '--dst',
```

### Comparing `bev-0.6.0/bev/cli/utils.py` & `bev-0.7.0/bev/cli/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from pathlib import Path
 
-from .app import cli_error
 from ..exceptions import HashError
 from ..shortcuts import get_consistent_repo
+from .app import cli_error
 
 
 def normalize_sources(sources):
     if isinstance(sources, (str, os.PathLike)):
         sources = [Path(sources)]
     else:
         sources = list(map(Path, sources))
```

### Comparing `bev-0.6.0/bev/config/base.py` & `bev-0.7.0/bev/config/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
-from typing import Dict, Sequence, Any, Union, Optional
+from typing import Any, Dict, Optional, Sequence, Union
 
-from pydantic import validator, root_validator, ValidationError
+from pydantic import ValidationError, root_validator, validator
 from tarn.config import HashConfig
 
 from .hostname import HostName
 from .include import Include
-from .remote import RemoteConfig, NoExtra
 from .registry import find
+from .remote import NoExtra, RemoteConfig
 
 
 class LocationConfig(NoExtra):
     root: Path = None
     remote: Sequence[RemoteConfig] = ()
     optional: bool = False
```

### Comparing `bev-0.6.0/bev/config/hostname.py` & `bev-0.7.0/bev/config/hostname.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from .registry import register, find, add_type
+from .registry import add_type, find, register
 
 
 @add_type
 class HostName:
     def __init__(self, value):
         self.value = value
```

### Comparing `bev-0.6.0/bev/config/include.py` & `bev-0.7.0/bev/config/include.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib
 from pathlib import Path
-from typing import Union, Tuple
+from typing import Tuple, Union
 
 from yaml import safe_load
 
-from .registry import register, find, add_type
+from .registry import add_type, find, register
 
 
 @add_type
 class Include:
     def __init__(self, value, optional: bool):
         self.value = value
         self.optional = optional
```

### Comparing `bev-0.6.0/bev/config/parse.py` & `bev-0.7.0/bev/config/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from pathlib import Path
-from typing import Sequence, Tuple, Callable, NamedTuple
 import importlib
+from pathlib import Path
+from typing import Callable, NamedTuple, Sequence, Tuple
 
+from tarn import DiskDict, HashKeyStorage, Location
 from yaml import safe_load
-from tarn import Storage, Disk, RemoteStorage
 
-from .base import StorageLevelConfig, RepositoryConfig, ConfigMeta, StorageCluster
-from .utils import CONFIG, identity, _filter_levels, choose_local, default_choose, wrap_levels
 from ..exceptions import ConfigError
+from .base import ConfigMeta, RepositoryConfig, StorageCluster, StorageLevelConfig
+from .utils import CONFIG, _filter_levels, choose_local, default_choose, identity, wrap_levels
 
 
 class CacheStorageIndex(NamedTuple):
     local: Sequence[StorageLevelConfig]
-    remote: Sequence[RemoteStorage]
-    storage: Storage
+    remote: Sequence[Location]
+    storage: HashKeyStorage
 
 
 def load_config(config: Path) -> RepositoryConfig:
     with open(config, 'r') as file:
         return parse(Path(config), safe_load(file))
 
 
-def build_storage(root: Path) -> Tuple[Storage, CacheStorageIndex]:
+def build_storage(root: Path) -> Tuple[HashKeyStorage, CacheStorageIndex]:
     config = load_config(root / CONFIG)
     meta = config.meta
 
-    order_func: Callable[[Sequence[Disk]], Sequence[Disk]] = identity
+    order_func: Callable[[Sequence[Location]], Sequence[Location]] = identity
     if meta.order is not None:
         path, attr = meta.order.rsplit('.', 1)
         order_func = getattr(importlib.import_module(path), attr)
 
-    storage = Storage(
-        *wrap_levels(config.local.storage, Disk, order_func),
+    storage = HashKeyStorage(
+        wrap_levels(config.local.storage, DiskDict, order_func),
         remote=filter_remotes([remote.storage for remote in config.remotes])
     )
     index = None
     if config.local.cache is not None:
-        cache_storage = Storage(
-            *wrap_levels(config.local.cache.storage, Disk, order_func),
+        cache_storage = HashKeyStorage(
+            wrap_levels(config.local.cache.storage, DiskDict, order_func),
             remote=filter_remotes([remote.cache.storage for remote in config.remotes if remote.cache is not None])
         )
         index = CacheStorageIndex(
             tuple(_filter_levels(config.local.cache.index)),
             filter_remotes([remote.cache.index for remote in config.remotes if remote.cache is not None]),
             cache_storage,
         )
```

### Comparing `bev-0.6.0/bev/config/registry.py` & `bev-0.7.0/bev/config/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Type
+from typing import Optional, Type
 
 _REGISTRY = {}
 
 
-def register(name, cls: Type = None):
+def register(name, cls: Optional[Type] = None):
     def decorator(kls: Type):
         if not isinstance(kls, type):
             raise TypeError(f'{kls} is not a type')
 
         match = {kind for kind in _REGISTRY if issubclass(kls, kind)}
         if len(match) != 1:
             raise TypeError(f"Couldn't match the type {kls}")
```

### Comparing `bev-0.6.0/bev/config/utils.py` & `bev-0.7.0/bev/config/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import os
 import socket
 from itertools import chain
 from pathlib import Path
 
-from tarn import StorageLevel
+from tarn import Fanout, Level, Levels
 
-from .base import StorageCluster
-from .hostname import StrHostName
 from ..exceptions import ConfigError
 from ..utils import PathOrStr
+from .base import StorageCluster
+from .hostname import StrHostName
 
 CONFIG = '.bev.yml'
 
 
 def identity(x):
     return x
 
 
 def wrap_levels(levels, cls, order=identity, **kwargs):
-    return tuple(
-        StorageLevel(
-            order([cls(location.root, **kwargs) for location in level.locations]),
+    return Levels(*(
+        Level(
+            Fanout(*order([cls(location.root, **kwargs) for location in level.locations])),
             write=level.write, replicate=level.replicate, name=level.name,
         )
         for level in _filter_levels(levels)
-    )
+    ))
 
 
 def _filter_levels(levels):
     for level in levels:
         locations = [
             x for x in level.locations
             if not x.optional or x.root.exists()
```

### Comparing `bev-0.6.0/bev/hash.py` & `bev-0.7.0/bev/hash.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import os
 import tempfile
 from collections import OrderedDict
 from pathlib import Path
-from typing import NamedTuple, Dict, Union
+from typing import Dict, NamedTuple, Union
 
-from tarn import Storage
+from tarn import HashKeyStorage
 
-from .utils import PathOrStr, deprecate
 from .exceptions import HashError
+from .utils import PathOrStr, deprecate
 
 Key = str
 Tree = Dict[PathOrStr, Union[Key, Dict]]
 HashType = Union[Key, Tree]
 
 
 def is_hash(path: PathOrStr):
@@ -49,25 +49,25 @@
 
 def strip_tree(key):
     if key.startswith('T:'):
         key = key[2:]
     return key
 
 
-def tree_to_hash(tree: Tree, storage: Storage):
+def tree_to_hash(tree: Tree, storage: HashKeyStorage):
     tree = normalize_tree(tree, storage.digest_size)
     # making sure that each time the same string will be saved
     tree = OrderedDict((k, tree[k]) for k in sorted(map(os.fspath, tree)))
     with tempfile.TemporaryDirectory() as tmp:
         tree_path = Path(tmp, 'hash')
         # TODO: storage should allow writing directly from memory
         with open(tree_path, 'w') as file:
             json.dump(tree, file)
 
-        return 'T:' + storage.write(tree_path)
+        return 'T:' + storage.write(tree_path).hex()
 
 
 def normalize_tree(tree: Tree, digest_size: int):
     def flatten(x):
         for key, value in x.items():
             key = Path(os.fspath(key))
 
@@ -80,15 +80,15 @@
 
             elif isinstance(value, dict):
                 for k, v in flatten(value):
                     yield key / k, v
 
             else:
                 # TODO
-                raise ValueError(value)
+                raise TypeError(value)
 
     # TODO: detect absolute paths
     result = {}
     for path, hash_ in flatten(tree):
         path = os.fspath(path)
         if path in result and result[path] != hash_:
             # TODO
```

### Comparing `bev-0.6.0/bev/interface.py` & `bev-0.7.0/bev/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import inspect
 import os
 from functools import lru_cache
 from pathlib import Path
-from typing import Sequence, Union, Optional
+from typing import Optional, Sequence, Union
 
-from tarn.digest import digest_file
+from tarn.digest import digest_value
 from wcmatch.glob import GLOBSTAR
 
 from .config import CONFIG, build_storage, find_vcs_root
-from .exceptions import RepositoryNotFound, HashNotFound, InconsistentHash, NameConflict, InconsistentRepositories
-from .hash import is_hash, to_hash, load_tree, strip_tree, Key, load_key, is_tree
+from .exceptions import HashNotFound, InconsistentHash, InconsistentRepositories, NameConflict, RepositoryNotFound
+from .hash import Key, is_hash, is_tree, load_key, load_tree, strip_tree, to_hash
 from .local import Local
 from .utils import PathOrStr
-from .vc import Version, CommittedVersion, VC, SubprocessGit
+from .vc import VC, CommittedVersion, SubprocessGit, Version
 from .wc import BevLocalGlob, BevVCGlob
 
 
 class Repository:
     """
     Interface that represents a `bev` repository.
 
@@ -104,15 +104,15 @@
             means that the local (possibly uncommitted) version of the files will be used
         check: bool
             if True - the file's hash will be additionally checked for consistency
         """
 
         def _resolve(path):
             if check:
-                digest = digest_file(path, self.storage.algorithm)
+                digest = digest_value(path, self.storage.algorithm).hex()
                 if digest != key:
                     raise InconsistentHash(
                         f'The path "{Path(*parts)}" has a wrong hash: expected "{key}", actual "{digest}"'
                     )
 
             return path
```

### Comparing `bev-0.6.0/bev/ops.py` & `bev-0.7.0/bev/ops.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from pathlib import Path
-from typing import Union, Callable, Optional
+from typing import Callable, Optional, Union
 
-from tarn import Storage
+from tarn import HashKeyStorage
 
 from .config import identity
-from .hash import is_hash, load_key, is_tree, load_tree, from_hash, strip_tree, normalize_tree, HashType, tree_to_hash
+from .hash import HashType, from_hash, is_hash, is_tree, load_key, load_tree, normalize_tree, strip_tree, tree_to_hash
 from .interface import Repository
 from .utils import PathOrStr
 
 
 class Conflict(Enum):
     """
     Conflict resolution policy, in case the destination already exists:
@@ -21,15 +21,15 @@
     """
     update = 'update'
     override = 'override'
     replace = 'replace'
     error = 'error'
 
 
-def gather(source: PathOrStr, storage: Union[Storage, Repository], progressbar: Callable = identity,
+def gather(source: PathOrStr, storage: Union[HashKeyStorage, Repository], progressbar: Callable = identity,
            fetch: Optional[bool] = None) -> HashType:
     source = Path(source)
     if not source.exists():
         # TODO
         raise FileNotFoundError(source)
 
     if isinstance(storage, Repository):
@@ -54,33 +54,33 @@
                         key = load_key(child)
                         if is_tree(key):
                             key = storage.read(load_tree, strip_tree(key), fetch=fetch)
 
                         gathered[from_hash(relative)] = key
 
                     else:
-                        gathered[relative] = storage.write(child)
+                        gathered[relative] = storage.write(child).hex()
 
             gathered = normalize_tree(gathered, storage.digest_size)
 
         else:
             assert source.is_file()
-            gathered = storage.write(source)
+            gathered = storage.write(source).hex()
 
     return gathered
 
 
 def load_hash(path: PathOrStr, storage, fetch: bool = False) -> HashType:
     key = load_key(path)
     if is_tree(key):
         return normalize_tree(storage.read(load_tree, strip_tree(key), fetch=fetch), storage.digest_size)
     return key
 
 
-def save_hash(tree: HashType, path: PathOrStr, storage: Union[Storage, Repository]):
+def save_hash(tree: HashType, path: PathOrStr, storage: Union[HashKeyStorage, Repository]):
     if isinstance(storage, Repository):
         storage = storage.storage
     if isinstance(tree, dict):
         tree = tree_to_hash(tree, storage)
 
     with open(path, 'w') as file:
         file.write(tree)
```

### Comparing `bev-0.6.0/bev/shortcuts.py` & `bev-0.7.0/bev/shortcuts.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Sequence
 
 from .config import CONFIG, find_repo_root
-from .interface import Repository
 from .exceptions import InconsistentRepositories, RepositoryNotFound
+from .interface import Repository
 from .utils import PathOrStr
 
 
 def get_current_repo(path: PathOrStr = '.') -> Repository:
     root = find_repo_root(path)
     if root is None:
         raise RepositoryNotFound(f"{CONFIG} files not found in current folder's parents")
```

### Comparing `bev-0.6.0/bev/testing.py` & `bev-0.7.0/bev/testing.py`

 * *Files identical despite different names*

### Comparing `bev-0.6.0/bev/utils.py` & `bev-0.7.0/bev/utils.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import shlex
+import subprocess
 import warnings
 from functools import wraps
 from os import PathLike
-import subprocess
-import shlex
 from typing import Union
 
 from .exceptions import *
 
 PathOrStr = Union[str, PathLike]
```

### Comparing `bev-0.6.0/bev/vc.py` & `bev-0.7.0/bev/vc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import os
 import shlex
 import subprocess
 from abc import abstractmethod
 from contextlib import suppress
 from functools import lru_cache
 from pathlib import Path
-from typing import Union, Sequence, NamedTuple
+from typing import NamedTuple, Sequence, Union
 
 from .config import find_vcs_root
 from .local import LocalVersion
 
-# from dulwich.object_store import tree_lookup_path
-# from dulwich.objects import Commit
-# from dulwich.repo import Repo
-
-
 CommittedVersion = str
 Version = Union[CommittedVersion, LocalVersion]
 
 
 class TreeEntry(NamedTuple):
     name: str
     is_dir: bool
@@ -98,35 +93,7 @@
             result.append(TreeEntry(name, kind == 'tree', kind == 'link'))
 
         return result
 
     @staticmethod
     def _call_git(command: str, cwd) -> str:
         return subprocess.check_output(shlex.split(command), cwd=cwd, stderr=subprocess.DEVNULL).decode('utf-8').strip()
-
-# TODO: this interface is not ready yet
-# class Dulwich(VC):
-#     def __init__(self, root: Path):
-#         super().__init__(root)
-#         self._real_repo = None
-#
-#     def read(self, relative: str, version: CommittedVersion):
-#         with suppress(KeyError):
-#             commit: Commit = self._repo.get_object(version.encode())
-#             _, h = tree_lookup_path(self._repo.get_object, commit.tree, self._relative(relative))
-#             return self._repo[h].data.decode().strip()
-#
-#     def get_version(self, relative: str, n: int = 0):
-#         entries = list(self._repo.get_walker(max_entries=n + 1, paths=[self._relative(relative)]))
-#         if len(entries) <= n:
-#             raise FileNotFoundError(relative)
-#         commit: Commit = entries[n].commit
-#         return commit.sha().hexdigest()
-#
-#     def _relative(self, path):
-#         return str((self.root / path).relative_to(self._repo.path)).encode()
-#
-#     @property
-#     def _repo(self):
-#         if self._real_repo is None:
-#             self._real_repo = Repo.discover(self.root)
-#         return self._real_repo
```

### Comparing `bev-0.6.0/bev/wc.py` & `bev-0.7.0/bev/wc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
-from typing import Optional, AnyStr, Iterator, Tuple, NamedTuple
+from typing import AnyStr, Iterator, NamedTuple, Optional, Sequence, Tuple
 
 from wcmatch.glob import Glob
 
 from .exceptions import NameConflict
-from .hash import is_hash, from_hash, to_hash, is_tree, load_key, strip_tree, load_tree
+from .hash import from_hash, is_hash, is_tree, load_key, load_tree, strip_tree, to_hash
 from .vc import VC, TreeEntry
 
 
 class DirEntry(NamedTuple):
     name: AnyStr
     is_dir: bool
     is_hidden: bool
@@ -40,21 +40,24 @@
         super().__init__(pattern, flags, Path(repo_root, relative))
         self._cache = cache
         self._version = version
         self._repo_root = Path(repo_root)
         self._storage = storage
         self._fetch = fetch
 
-    def _list_dir(self, relative: Path):
+    def _list_dir(self, relative: Path) -> Sequence[Path]:
+        """ Return the contents of a directory `relative` to `self._repo_root` """
         raise NotImplementedError
 
-    def _exists(self, relative: Path):
+    def _exists(self, relative: Path) -> bool:
+        """ Whether the path `relative` to `self._repo_root` exists """
         raise NotImplementedError
 
     def _read_tree_key(self, relative: Path):
+        """ Read a tree key located `relative` to `self._repo_root` """
         raise NotImplementedError
 
     def _get_cached(self, relative: Path):
         for parent in relative.parents:
             if (self._version, parent) in self._cache:
                 cache = self._cache[self._version, parent]
                 for part in relative.relative_to(parent).parts:
@@ -88,15 +91,15 @@
                 self._get_cached(relative) is not None
                 or self._exists(relative)
                 or self._exists(to_hash(relative))
         )
 
     def _scandir(self, curdir: Optional[AnyStr]) -> Iterator[DirEntry]:
         current = Path(self.root_dir)
-        if curdir is not None:
+        if curdir:
             current /= curdir
         relative = current.relative_to(self._repo_root)
 
         # is it already cached?
         cached = self._get_cached(relative)
         if cached is None and relative.parts:
             key = self._read_tree_key(to_hash(relative))
@@ -142,22 +145,22 @@
 class BevLocalGlob(BevGlob):
     def __init__(self, pattern, repo_root, relative, storage, fetch, flags: int):
         super().__init__(pattern, repo_root, relative, None, {}, storage, fetch, flags)
 
     def _list_dir(self, relative: Path):
         return [
             TreeEntry(entry.name, entry.is_dir(), entry.is_symlink())
-            for entry in (self.root_dir / relative).iterdir()
+            for entry in (self._repo_root / relative).iterdir()
         ]
 
     def _exists(self, relative: Path):
-        return (self.root_dir / relative).exists()
+        return (self._repo_root / relative).exists()
 
     def _read_tree_key(self, relative: Path):
-        path = self.root_dir / relative
+        path = self._repo_root / relative
         if path.exists():
             return load_key(path)
 
 
 class BevVCGlob(BevGlob):
     def __init__(self, pattern, repo_root, relative, version, cache, vc: VC, storage, fetch, flags: int):
         super().__init__(pattern, repo_root, relative, version, cache, storage, fetch, flags)
```

### Comparing `bev-0.6.0/bev.egg-info/PKG-INFO` & `bev-0.7.0/bev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bev
-Version: 0.6.0
+Version: 0.7.0
 Summary: A small manager for versioned data
 Home-page: https://github.com/neuro-ml/bev
 License: MIT
-Download-URL: https://github.com/neuro-ml/bev/archive/v0.6.0.tar.gz
+Download-URL: https://github.com/neuro-ml/bev/archive/v0.7.0.tar.gz
 Keywords: data,version control
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bev-0.6.0/bev.egg-info/SOURCES.txt` & `bev-0.7.0/bev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bev-0.6.0/setup.py` & `bev-0.7.0/setup.py`

 * *Files identical despite different names*

