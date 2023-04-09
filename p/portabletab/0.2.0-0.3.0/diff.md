# Comparing `tmp/portabletab-0.2.0.tar.gz` & `tmp/portabletab-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portabletab-0.2.0.tar", max compression
+gzip compressed data, was "portabletab-0.3.0.tar", max compression
```

## Comparing `portabletab-0.2.0.tar` & `portabletab-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-03-23 04:47:41.138638 portabletab-0.2.0/LICENSE
--rw-r--r--   0        0        0      203 2023-04-04 07:41:11.567861 portabletab-0.2.0/PortableTab/__init__.py
--rw-r--r--   0        0        0     1917 2023-04-04 07:41:11.567861 portabletab-0.2.0/PortableTab/base_table.py
--rw-r--r--   0        0        0     4673 2023-04-04 07:41:11.567861 portabletab-0.2.0/PortableTab/capnp_manager.py
--rw-r--r--   0        0        0    13474 2023-04-04 07:41:11.567861 portabletab-0.2.0/PortableTab/capnp_table.py
--rw-r--r--   0        0        0      843 2023-04-03 01:10:02.651537 portabletab-0.2.0/README.md
--rw-r--r--   0        0        0      546 2023-04-05 09:01:05.876267 portabletab-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 portabletab-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-01 08:14:02.855946 portabletab-0.3.0/LICENSE
+-rw-r--r--   0        0        0      203 2023-04-09 02:51:51.561890 portabletab-0.3.0/PortableTab/__init__.py
+-rw-r--r--   0        0        0     2744 2023-04-09 02:51:51.561890 portabletab-0.3.0/PortableTab/__main__.py
+-rw-r--r--   0        0        0     1917 2023-04-05 12:03:54.103133 portabletab-0.3.0/PortableTab/base_table.py
+-rw-r--r--   0        0        0     4673 2023-04-05 12:03:54.103133 portabletab-0.3.0/PortableTab/capnp_manager.py
+-rw-r--r--   0        0        0    18222 2023-04-09 02:51:51.561890 portabletab-0.3.0/PortableTab/capnp_table.py
+-rw-r--r--   0        0        0     1837 2023-04-09 02:51:51.561890 portabletab-0.3.0/README.md
+-rw-r--r--   0        0        0      634 2023-04-09 02:51:51.561890 portabletab-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 portabletab-0.3.0/setup.py
+-rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 portabletab-0.3.0/PKG-INFO
```

### Comparing `portabletab-0.2.0/LICENSE` & `portabletab-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `portabletab-0.2.0/PortableTab/base_table.py` & `portabletab-0.3.0/PortableTab/base_table.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.2.0/PortableTab/capnp_manager.py` & `portabletab-0.3.0/PortableTab/capnp_manager.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.2.0/PortableTab/capnp_table.py` & `portabletab-0.3.0/PortableTab/capnp_table.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from functools import lru_cache
 import json
 from logging import getLogger
 import math
 import mmap
 from pathlib import Path
-from typing import Any, Iterator, Iterable, List, Optional
+from typing import Any, Callable, Iterator, Iterable, Optional
+
+import marisa_trie
 
 from .capnp_manager import CapnpManager
 
 logger = getLogger(__name__)
 
 
 class CapnpTable(CapnpManager):
@@ -31,40 +33,41 @@
     def __init__(
             self,
             tablename: str,
             db_dir=None):
         super().__init__(db_dir)
         self.tablename = tablename
         self.readers = {}
+        self.trie_indexes = {}
 
     def __del__(self):
         self.unload()
 
     def unload(self) -> None:
         """
         Release loaded resources manually,
         including the capnp module corresponding to this table.
         """
         super().unload()
         self.__class__.unload_schema(self.tablename)
 
-    @lru_cache
+    @lru_cache(maxsize=128)
     def get_dir(self) -> Path:
         """
         Get the directory where the table are placed.
         """
         return self.db_dir / self.tablename
 
     def _get_config_path(self) -> Path:
         """
         Get path to the config file of the table.
         """
         return self.get_dir() / "config.json"
 
-    @lru_cache
+    @lru_cache(maxsize=128)
     def get_config(self) -> Path:
         """
         Get the contents of the config file of the table.
         """
         with open(self._get_config_path(), "r") as f:
             config = json.load(f)
 
@@ -93,15 +96,15 @@
         config = self.get_config()
         module_name = config["module_name"]
         if module_name not in CapnpManager.modules:
             CapnpManager.load_schema(
                 self.get_dir() / config["capnp_file"],
                 module_name)
 
-    @lru_cache
+    @lru_cache(maxsize=128)
     def get_record_type(self) -> Any:
         """
         Get the record type.
 
         Returns
         -------
         Any
@@ -114,15 +117,15 @@
         config = self.get_config()
         self._load_capnp_file()
         record_type = getattr(
             CapnpManager.modules[config["module_name"]],
             config["record_type"])
         return record_type
 
-    @lru_cache
+    @lru_cache(maxsize=128)
     def get_list_type(self) -> Any:
         """
         Get the list type.
 
         Returns
         -------
         Any
@@ -457,7 +460,160 @@
 
         if current_page is not None:
             # Write the page to file
             self._write_page(
                 page=current_page,
                 records=records
             )
+
+    def create_trie_on(
+        self,
+        attr: str,
+        func: Optional[Callable] = None
+    ) -> None:
+        """
+        Create TRIE index on the specified attribute.
+
+        Paramters
+        ---------
+        attr: str
+            The name of target attribute.
+        func: Callable
+            Function to generate a set of strings to be indexed.
+            If not specified, 'str' will be used.
+
+        Notes
+        -----
+        - The created index is saved in the same directory as
+          the page files with the file name "<attr>.trie".
+        """
+
+        def kvgen():
+            # Generator function to enumerate sets of
+            # attribute value and position.
+            for pos in range(self.count_records()):
+                record = CapnpTable.get_record(
+                    self, pos=pos)  # Call base class method
+                if pos == 0 and not hasattr(record, attr):
+                    raise ValueError(f"Attribute '{attr}' doesn't exist.")
+
+                if func is None:
+                    strings = str(getattr(record, attr))
+                else:
+                    strings = func(getattr(record, attr))
+
+                if isinstance(strings, str) and strings != "":
+                    yield (strings, (pos,))
+                else:
+                    for string in strings:
+                        if string != "":
+                            yield (string, (pos,))
+
+        # Create RecordTrie
+        # https://marisa-trie.readthedocs.io/en/latest/tutorial.html#marisa-trie-recordtrie  # noqa: E501
+        trie = marisa_trie.RecordTrie("<L", kvgen())
+        path = self.get_dir() / f"{attr}.trie"
+        trie.save(str(path))
+
+        # Open the trie using mmap.
+        self.open_trie_on(attr)
+
+    def open_trie_on(self, attr: str) -> marisa_trie.RecordTrie:
+        """
+        Open TRIE index on the specified attribute.
+
+        Paramters
+        ---------
+        attr: str
+            The name of target attribute.
+
+        Returns
+        -------
+        RecordTrie
+            The TRIE index.
+
+        Notes
+        -----
+        - The index is mmapped from the file name "<attr>.trie",
+          in the same directory as the page files.
+        """
+        if attr in self.trie_indexes:
+            return self.trie_indexes[attr]
+
+        path = self.get_dir() / f"{attr}.trie"
+        trie = marisa_trie.RecordTrie("<L").mmap(str(path))
+        self.trie_indexes[attr] = trie
+        return trie
+
+    def delete_trie_on(self, attr: str):
+        """
+        Delete TRIE index on the specified attribute.
+
+        Paramters
+        ---------
+        attr: str
+            The name of target attribute.
+
+        Notes
+        -----
+        - Delete any file named "<attr>.trie" in the same directory
+          as the page files.
+        - If the index is already loaded, unload it.
+        """
+        path = self.get_dir() / f"{attr}.trie"
+        if path.exists():
+            path.unlink()
+
+        if attr in self.trie_indexes:
+            del self.trie_indexes[attr]
+
+    def search_records_on(
+            self,
+            attr: str,
+            value: str,
+            funcname: str = "get") -> list:
+        """
+        Search value from the table on the specified attribute.
+
+        Paramters
+        ---------
+        attr: str
+            The name of target attribute.
+        value: str
+            The target value.
+        funcname: str
+            The name of search method.
+            - "get" searches for records that exactly match the value.
+            - "prefixes" searches for records that contained in the value.
+            - "keys" searches for records that containing the value.
+
+        Returns
+        -------
+        List[Record]
+            List of records.
+
+        Notes
+        -----
+        - TRIE index must be created on the column before searching.
+        - The TRIE index file will be automatically opened if it exists.
+        """
+        if funcname not in ("get", "prefixes", "keys"):
+            raise ValueError("'func' must be 'get', 'prefixes' or 'keys'.")
+
+        trie = self.open_trie_on(attr)
+        positions = []
+        if funcname == "get":
+            positions = trie.get(value, [])
+        elif funcname == "prefixes":
+            for v in trie.prefixes(value):
+                positions += trie.get(v, [])
+
+        elif funcname == "keys":
+            for v in trie.keys(value):
+                positions += trie.get(v, [])
+
+        records = []
+        pos_tuples = set([p[0] for p in positions])
+        for pos in pos_tuples:
+            records.append(self.get_record(pos=pos))
+
+        return records
```

### Comparing `portabletab-0.2.0/pyproject.toml` & `portabletab-0.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [tool.poetry]
 name = "PortableTab"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python package for serializing tables in portable format with Capnp."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "PortableTab"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 docopt = "^0.6.2"
 pycapnp = "^1.3.0"
+marisa-trie = "^0.7.8"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 flake8 = "*"
 sphinx = "<6"
 sphinx-rtd-theme = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+portabletab = "PortableTab.__main__:main"
```

