# Comparing `tmp/sqliteio-0.1.0.tar.gz` & `tmp/sqliteio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqliteio-0.1.0.tar", last modified: Sat Apr  1 02:52:52 2023, max compression
+gzip compressed data, was "sqliteio-0.2.0.tar", last modified: Sun Apr  9 01:46:51 2023, max compression
```

## Comparing `sqliteio-0.1.0.tar` & `sqliteio-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2023-04-01 02:52:52.976883 sqliteio-0.1.0/
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     1072 2023-04-01 02:01:04.000000 sqliteio-0.1.0/LICENSE
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      984 2023-04-01 02:52:52.976883 sqliteio-0.1.0/PKG-INFO
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      460 2023-04-01 02:51:47.000000 sqliteio-0.1.0/README.rst
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)       38 2023-04-01 02:52:52.976883 sqliteio-0.1.0/setup.cfg
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      641 2023-04-01 02:19:02.000000 sqliteio-0.1.0/setup.py
-drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2023-04-01 02:52:52.976883 sqliteio-0.1.0/sqliteio/
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    10053 2023-04-01 02:08:37.000000 sqliteio-0.1.0/sqliteio/__init__.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    36466 2023-04-01 02:08:37.000000 sqliteio-0.1.0/sqliteio/btree.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     9019 2023-04-01 02:08:37.000000 sqliteio-0.1.0/sqliteio/pager.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     3285 2023-04-01 02:08:37.000000 sqliteio-0.1.0/sqliteio/record.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    12039 2023-04-01 02:08:37.000000 sqliteio-0.1.0/sqliteio/schema.py
-drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2023-04-01 02:52:52.976883 sqliteio-0.1.0/sqliteio.egg-info/
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      984 2023-04-01 02:52:52.000000 sqliteio-0.1.0/sqliteio.egg-info/PKG-INFO
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      250 2023-04-01 02:52:52.000000 sqliteio-0.1.0/sqliteio.egg-info/SOURCES.txt
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)        1 2023-04-01 02:52:52.000000 sqliteio-0.1.0/sqliteio.egg-info/dependency_links.txt
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)        9 2023-04-01 02:52:52.000000 sqliteio-0.1.0/sqliteio.egg-info/top_level.txt
+drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2023-04-09 01:46:51.160973 sqliteio-0.2.0/
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     1072 2023-04-01 02:01:04.000000 sqliteio-0.2.0/LICENSE
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     4272 2023-04-09 01:46:51.156976 sqliteio-0.2.0/PKG-INFO
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     3748 2023-04-09 01:41:03.000000 sqliteio-0.2.0/README.rst
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)       38 2023-04-09 01:46:51.160973 sqliteio-0.2.0/setup.cfg
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      641 2023-04-09 01:45:37.000000 sqliteio-0.2.0/setup.py
+drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2023-04-09 01:46:51.156976 sqliteio-0.2.0/sqliteio/
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    12147 2023-04-09 00:42:05.000000 sqliteio-0.2.0/sqliteio/__init__.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    37810 2023-04-09 01:32:41.000000 sqliteio-0.2.0/sqliteio/btree.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    10311 2023-04-03 23:18:45.000000 sqliteio-0.2.0/sqliteio/pager.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     4577 2023-04-03 23:24:02.000000 sqliteio-0.2.0/sqliteio/record.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    13331 2023-04-08 09:30:11.000000 sqliteio-0.2.0/sqliteio/schema.py
+drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2023-04-09 01:46:51.156976 sqliteio-0.2.0/sqliteio.egg-info/
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     4272 2023-04-09 01:46:51.000000 sqliteio-0.2.0/sqliteio.egg-info/PKG-INFO
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      250 2023-04-09 01:46:51.000000 sqliteio-0.2.0/sqliteio.egg-info/SOURCES.txt
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)        1 2023-04-09 01:46:51.000000 sqliteio-0.2.0/sqliteio.egg-info/dependency_links.txt
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)        9 2023-04-09 01:46:51.000000 sqliteio-0.2.0/sqliteio.egg-info/top_level.txt
```

### Comparing `sqliteio-0.1.0/LICENSE` & `sqliteio-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqliteio-0.1.0/setup.py` & `sqliteio-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'Programming Language :: Python :: 3',
     'Topic :: Database',
 ]
 
 
 setup(
     name="sqliteio",
-    version="0.1.0",
+    version="0.2.0",
     url='https://github.com/nakagami/sqliteio/',
     classifiers=classifiers,
     keywords=['SQLite3'],
     author='Hajime Nakagami',
     author_email='nakagami@gmail.com',
     description='SQLite3 I/O library',
     long_description=open('README.rst').read(),
```

### Comparing `sqliteio-0.1.0/sqliteio/__init__.py` & `sqliteio-0.2.0/sqliteio/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+################################################################################
+# MIT License
+#
+# Copyright (c) 2023 Hajime Nakagami<nakagami@gmail.com>
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+################################################################################
 import builtins
 from .pager import Pager
 from .schema import TableSchema, IndexSchema, ViewSchema
 from .btree import TableLeafNode, TableInteriorNode, IndexInteriorNode, swap_node
 
 
 __all__ = ("Database", "open")
@@ -71,22 +94,25 @@
             index_schema.pgno,
             key_values, key_values,
             index_schema.orders,
             list(range(len(index_schema.columns)))
         ):
             yield self.get_by_rowid(index_schema.table_name, r[-1])
 
-    def get_by_rowid(self, table_name, rowid):
-        "Get table record by rowid"
-        table_schema = self.table_schema(table_name)
+    def _get_by_rowid(self, table_schema, rowid):
         try:
             return next(self.pager.rowid_range_records(table_schema.pgno, rowid, rowid, table_schema.row_converter))
         except StopIteration:
             return None
 
+    def get_by_rowid(self, table_name, rowid):
+        "Get table record by rowid"
+        table_schema = self.table_schema(table_name)
+        return self._get_by_rowid(table_schema, rowid)
+
     def get_by_pk(self, table_name, value):
         "Get table record by primary key"
         table_schema = self.table_schema(table_name)
         index_schema = self._get_primary_key_index(table_name)
         if any([c.is_rowid for c in table_schema.columns]):
             try:
                 return next(self.pager.rowid_range_records(table_schema.pgno, value, value, table_schema.row_converter))
@@ -137,14 +163,15 @@
         rowid, value_list = table_schema.dict_to_value_list(r)
         if rowid is None:
             rowid = self._get_next_rowid(table_schema)
 
         table_ancestors, table_leaf, table_leaf_cell_index, found = self.pager.find_rowid_table_path(table_schema.pgno, rowid)
 
         if found:
+            self.rollback()
             raise ValueError("rowid:{} is exists".format(rowid))
 
         # Insert record to TableLeafNode
         cell_block = table_leaf.to_cell_block(rowid, value_list)
         cell_index = table_leaf.find_cell_index(rowid)
         if table_leaf.free_cell_size() >= len(cell_block):
             table_leaf.insert(rowid, cell_index, cell_block)
@@ -199,37 +226,55 @@
         """insert data
         dict_list is iterator of value dict
         """
         table_schema = self.table_schema(table_name)
         index_schemas = self.index_schemas(table_name)
 
         for r in dict_list:
+            # TODO: check constraint
             self._insert1(r, table_schema, index_schemas)
 
-    def delete_by_rowid(self, table_name, rowid):
-        "delete table record by rowid"
-        table_schema = self.table_schema(table_name)
+    def _delete_by_rowid(self, table_schema, rowid):
         table_ancestors, table_leaf, table_leaf_cell_index, found = self.pager.find_rowid_table_path(table_schema.pgno, rowid)
 
         if not found:
             raise ValueError("rowid can't found:{}".format(rowid))
         _, row = table_leaf.record(table_leaf_cell_index, table_schema.row_converter)
         # find related index and remove index
-        for index_schema in self.index_schemas(table_name):
+        for index_schema in self.index_schemas(table_schema.table_name):
             key = [row[c.name] for c in index_schema.columns]
             index_ancestors, index_leaf, index_leaf_cell_index, found = self.pager.find_rowid_index_path(
                 index_schema.pgno, key, rowid, index_schema.orders, False
             )
             if found:
                 index_leaf.delete(index_leaf_cell_index)
         # remove record
         table_leaf.delete(table_leaf_cell_index)
         if table_ancestors:
             table_ancestors[-1].merge_children()
 
+    def delete_by_rowid(self, table_name, rowid):
+        "delete table record by rowid"
+        table_schema = self.table_schema(table_name)
+        # TODO: check constraint
+        return self._delete_by_rowid(table_schema, rowid)
+
+    def update_by_rowid(self, table_name, rowid, update_dict):
+        """update table record
+        """
+        table_schema = self.table_schema(table_name)
+        index_schemas = self.index_schemas(table_name)
+
+        # TODO: check constraint
+        rowid_r = self._get_by_rowid(table_schema, rowid)
+        new_rowid, r = rowid_r
+        r.update(update_dict)
+        self._delete_by_rowid(table_schema, rowid)
+        self._insert1(r, table_schema, index_schemas)
+
     def commit(self):
         "Save cache page data to storage"
         self.pager.flush()
 
     def rollback(self):
         "Rollback dirty pages"
         self.pager.rollback()
```

### Comparing `sqliteio-0.1.0/sqliteio/btree.py` & `sqliteio-0.2.0/sqliteio/btree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+################################################################################
+# MIT License
+#
+# Copyright (c) 2023 Hajime Nakagami<nakagami@gmail.com>
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+################################################################################
 import binascii
 from .record import varint_and_next_index, to_varint, decode_payload, pack_value_list
 
 BTREE_PAGE_TYPE_RAW_PAGE = -1       # pseudo number
 BTREE_PAGE_TYPE_FREE_PAGE = 0       # pseudo number
 BTREE_PAGE_TYPE_INTERIOR_INDEX = 2
 BTREE_PAGE_TYPE_INTERIOR_TABLE = 5
@@ -59,14 +82,15 @@
             page = self.node.pager.get_page(overflow)
             overflow = int.from_bytes(page.data[:4], 'big')
             buf += page.data[4:]
 
         return buf[:self.payload_len]
 
     def free_overflow_pages(self):
+        "overflow page to free list"
         overflow_pgno = self.overflow_pgno
         while overflow_pgno:
             page = self.node.pager.get_page(overflow_pgno)
             overflow_pgno = int.from_bytes(page.data[:4], 'big')
             self.node.pager.add_to_freelist(page)
 
     def __repr__(self):
@@ -252,15 +276,15 @@
     def _first_payload_and_trailing(self, r):
         if self.max_in_page_payload() >= len(r):
             return r
         i = self.calculate_cell_in_page_bytes(len(r))
         first_payload = r[:i]
         trailing_pages = []
         while r[i:]:
-            j = i + self.pager.page_size -4
+            j = i + self.pager.page_size - 4
             trailing_pages.append(r[i:j])
             i = j
 
         assert len(first_payload) > 0
         assert len(trailing_pages) > 0
 
         next_page = self.pager.new_page(BTREE_PAGE_TYPE_RAW_PAGE)
@@ -307,14 +331,16 @@
                     if self.free_block_offset == free_block_offset:
                         self.free_block_offset = next_offset
                         return free_block_offset
                 free_block_offset = next_offset
         return None
 
     def merge_free_block(self):
+        """if free cell blocks are contiguous, merge them.
+        """
         free_block_offset = self.free_block_offset
         while free_block_offset:
             if self._merge_free_block(free_block_offset):
                 free_block_offset = self.free_block_offset
             else:
                 next_offset, size = self._next_free_block_offset_and_current_free_block_size(free_block_offset)
                 free_block_offset = next_offset
@@ -593,19 +619,17 @@
                 self.append_cell_block(cell_block)
         else:
             self.insert_cell_block(cell_index, cell_block)
 
     def insert_node_after(self, leaf_node, ancestors, prev_leaf_node):
         """insert TaleLeafNode page leaf_node befre prev_leaf_node
         """
-        if self.right_most == prev_leaf_node.page.pgno:
-            self.right_most = leaf_node.page.pgno
-            self.insert_node_index(prev_leaf_node, len(self.cells))
-        else:
-            raise ValueError("TODO:")
+        assert self.right_most == prev_leaf_node.page.pgno
+        self.right_most = leaf_node.page.pgno
+        self.insert_node_index(prev_leaf_node, len(self.cells))
 
     def find_rowid_table_path(self, rowid, ancestors):
         for cell in self.cells:
             if rowid > cell.key:
                 continue
             if rowid > cell.key:
                 break
```

### Comparing `sqliteio-0.1.0/sqliteio/pager.py` & `sqliteio-0.2.0/sqliteio/pager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+################################################################################
+# MIT License
+#
+# Copyright (c) 2023 Hajime Nakagami<nakagami@gmail.com>
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+################################################################################
 import binascii
 from .btree import (
     BTREE_PAGE_TYPE_LEAF_TABLE,
     BTREE_PAGE_TYPE_INTERIOR_TABLE,
     BTREE_PAGE_TYPE_LEAF_INDEX,
     BTREE_PAGE_TYPE_INTERIOR_INDEX,
     BTREE_PAGE_TYPE_FREE_PAGE,
```

### Comparing `sqliteio-0.1.0/sqliteio/schema.py` & `sqliteio-0.2.0/sqliteio/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+################################################################################
+# MIT License
+#
+# Copyright (c) 2023 Hajime Nakagami<nakagami@gmail.com>
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+################################################################################
 import re
 
 
 # https://www.sqlite.org/lang_createtable.html
 # https://www.sqlite.org/datatype3.html
 
 TOK_NAME = 1
```

