# Comparing `tmp/jupyter_server_fileid-0.8.0.tar.gz` & `tmp/jupyter_server_fileid-0.9.0.tar.gz`

## Comparing `jupyter_server_fileid-0.8.0.tar` & `jupyter_server_fileid-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/.flake8
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    12346 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/RELEASE.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/conftest.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/.github/workflows/test-python.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/docs/Makefile
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/docs/conf.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/docs/make.bat
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/docs/requirements.txt
--rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/docs/_static/jupyter_logo.png
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/docs/user_guide/index.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/jupyter-config/jupyter_server_config.d/jupyter_server_fileid.json
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/jupyter_server_fileid/__init__.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/jupyter_server_fileid/cli.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/jupyter_server_fileid/extension.py
--rw-r--r--   0        0        0    35052 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/jupyter_server_fileid/manager.py
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/jupyter_server_fileid/pytest_plugin.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/tests/test_manager.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/LICENSE
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/.flake8
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/RELEASE.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/conftest.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/.github/workflows/test-python.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/docs/requirements.txt
+-rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/docs/_static/jupyter_logo.png
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/docs/user_guide/index.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/jupyter-config/jupyter_server_config.d/jupyter_server_fileid.json
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/jupyter_server_fileid/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/jupyter_server_fileid/cli.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/jupyter_server_fileid/extension.py
+-rw-r--r--   0        0        0    34827 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/jupyter_server_fileid/manager.py
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/jupyter_server_fileid/pytest_plugin.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/tests/test_manager.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.0/PKG-INFO
```

### Comparing `jupyter_server_fileid-0.8.0/.pre-commit-config.yaml` & `jupyter_server_fileid-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/CHANGELOG.md` & `jupyter_server_fileid-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.9.0
+
+([Full Changelog](https://github.com/jupyter-server/jupyter_server_fileid/compare/v0.8.0...505806162b4df60b4cbb461cfec1266b81df32ce))
+
+### Enhancements made
+
+- add Jupyter Releaser workflows [#65](https://github.com/jupyter-server/jupyter_server_fileid/pull/65) ([@dlqqq](https://github.com/dlqqq))
+- Fix behavior for OOB move followed by IB move [#63](https://github.com/jupyter-server/jupyter_server_fileid/pull/63) ([@dlqqq](https://github.com/dlqqq))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_server_fileid/graphs/contributors?from=2023-02-23&to=2023-04-09&type=c))
+
+[@dleen](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Adleen+updated%3A2023-02-23..2023-04-09&type=Issues) | [@dlqqq](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Adlqqq+updated%3A2023-02-23..2023-04-09&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.8.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_server_fileid/compare/v0.7.0...542ccebfcf7713a81a4f2fbd07e8227573c3a282))
 
 ### Enhancements made
 
 - Add db_journal_mode trait to FileIdManager classes [#61](https://github.com/jupyter-server/jupyter_server_fileid/pull/61) ([@kevin-bates](https://github.com/kevin-bates))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_server_fileid/graphs/contributors?from=2023-02-16&to=2023-02-23&type=c))
 
 [@codecov](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Acodecov+updated%3A2023-02-16..2023-02-23&type=Issues) | [@kevin-bates](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Akevin-bates+updated%3A2023-02-16..2023-02-23&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.7.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_server_fileid/compare/v0.6.0...f42d481b072f8c1a961ad8dc6c2b3ab35a6d0777))
 
 ### Enhancements made
 
 - remove mtime fallback [#47](https://github.com/jupyter-server/jupyter_server_fileid/pull/47) ([@dlqqq](https://github.com/dlqqq))
```

### Comparing `jupyter_server_fileid-0.8.0/RELEASE.md` & `jupyter_server_fileid-0.9.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/.github/workflows/build.yml` & `jupyter_server_fileid-0.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/.github/workflows/check-release.yml` & `jupyter_server_fileid-0.9.0/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/.github/workflows/test-python.yml` & `jupyter_server_fileid-0.9.0/.github/workflows/test-python.yml`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/docs/Makefile` & `jupyter_server_fileid-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/docs/conf.py` & `jupyter_server_fileid-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/docs/make.bat` & `jupyter_server_fileid-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/docs/_static/jupyter_logo.png` & `jupyter_server_fileid-0.9.0/docs/_static/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/docs/user_guide/index.md` & `jupyter_server_fileid-0.9.0/docs/user_guide/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/jupyter_server_fileid/extension.py` & `jupyter_server_fileid-0.9.0/jupyter_server_fileid/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/jupyter_server_fileid/manager.py` & `jupyter_server_fileid-0.9.0/jupyter_server_fileid/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -798,31 +798,26 @@
         new_path = self._normalize_path(new_path)
 
         # verify file exists at new_path
         stat_info = self._stat(new_path)
         if stat_info is None:
             return None
 
-        if stat_info.is_dir:
-            self._move_recursive(old_path, new_path)
-
-        # attempt to fetch ID associated with old path
-        # we avoid using get_id() here since that will always return None as file no longer exists at old path
-        row = self.con.execute("SELECT id FROM Files WHERE path = ?", (old_path,)).fetchone()
-        if row is None:
+        # sync the file and see if it was already indexed
+        #
+        # originally this method did not call _sync_file() for performance
+        # reasons, but this is needed to handle an edge case:
+        # https://github.com/jupyter-server/jupyter_server_fileid/issues/62
+        id = self._sync_file(new_path, stat_info)
+        if id is None:
             # if no existing record, create a new one
             id = self._create(new_path, stat_info)
-            self.con.commit()
-            return id
-        else:
-            # update existing record with new path and stat info
-            id = row[0]
-            self._update(id, stat_info, new_path)
-            self.con.commit()
-            return id
+
+        self.con.commit()
+        return id
 
     def _copy_recursive(self, from_path: str, to_path: str, _: str = "") -> None:
         """Copy all children of a given directory at `from_path` to a new
         directory at `to_path`. Inserts stat_info with record."""
         from_path_glob = os.path.join(from_path, "*")
         records = self.con.execute(
             "SELECT path FROM Files WHERE path GLOB ?", (from_path_glob,)
```

### Comparing `jupyter_server_fileid-0.8.0/jupyter_server_fileid/pytest_plugin.py` & `jupyter_server_fileid-0.9.0/jupyter_server_fileid/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/tests/test_manager.py` & `jupyter_server_fileid-0.9.0/tests/test_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -466,24 +466,46 @@
 
     assert old_id == new_id
     assert any_fid_manager.get_id(old_path) is None
     assert any_fid_manager.get_id(new_path) == new_id
     assert any_fid_manager.get_path(old_id) == new_path
 
 
-# test for disjoint move handling
-# disjoint move: any out-of-band move that does not preserve stat info
-def test_disjoint_move_indexed(any_fid_manager, old_path, new_path, fs_helpers):
-    old_id = any_fid_manager.index(old_path)
-
-    fs_helpers.delete(old_path)
-    fs_helpers.touch(new_path, dir=True)
-    new_id = any_fid_manager.move(old_path, new_path)
+def test_oob_ib_move(fid_manager, test_path, fs_helpers):
+    """
+    Test an out-of-band move followed by an in-band move.
+    """
+    new_path_1 = "path1"
+    new_path_2 = "path2"
+    id = fid_manager.index(test_path)
+
+    # out-of-band
+    fs_helpers.move(test_path, new_path_1)
+    # in-band
+    fs_helpers.move(new_path_1, new_path_2)
+    fid_manager.move(new_path_1, new_path_2)
+
+    assert id == fid_manager.get_id(new_path_2)
+
+
+def test_ib_oob_move(fid_manager, test_path, fs_helpers):
+    """
+    Test an in-band move followed by an out-of-band move.
+    """
+    new_path_1 = "path1"
+    new_path_2 = "path2"
+    id = fid_manager.index(test_path)
+
+    # in-band
+    fs_helpers.move(test_path, new_path_1)
+    fid_manager.move(test_path, new_path_1)
+    # out-of-band
+    fs_helpers.move(new_path_1, new_path_2)
 
-    assert old_id == new_id
+    assert id == fid_manager.get_id(new_path_2)
 
 
 def test_move_recursive(
     any_fid_manager,
     old_path,
     old_path_child,
     old_path_grandchild,
```

### Comparing `jupyter_server_fileid-0.8.0/.gitignore` & `jupyter_server_fileid-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/LICENSE` & `jupyter_server_fileid-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/README.md` & `jupyter_server_fileid-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/pyproject.toml` & `jupyter_server_fileid-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.8.0/PKG-INFO` & `jupyter_server_fileid-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_server_fileid
-Version: 0.8.0
+Version: 0.9.0
 Project-URL: Home, https://github.com/jupyter-server/jupyter_server_fileid
 Author-email: "David L. Qiu" <david@qiu.dev>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, David L. Qiu
         All rights reserved.
```

