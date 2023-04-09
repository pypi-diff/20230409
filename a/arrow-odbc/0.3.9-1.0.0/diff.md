# Comparing `tmp/arrow_odbc-0.3.9.tar.gz` & `tmp/arrow_odbc-1.0.0.tar.gz`

## Comparing `arrow_odbc-0.3.9.tar` & `arrow_odbc-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 arrow_odbc-0.3.9/Cargo.toml
--rw-r--r--   0        0        0      136 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/.gitattributes
--rw-r--r--   0        0        0      131 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/.github/dependabot.yml
--rw-r--r--   0        0        0     1522 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/.github/workflows/test.yml
--rw-r--r--   0        0        0     1807 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/.github/workflows/wheel.yml
--rw-r--r--   0        0        0      275 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/.gitignore
--rw-r--r--   0        0        0      841 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/.readthedocs.yaml
--rw-r--r--   0        0        0     3637 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/Changelog.md
--rw-r--r--   0        0        0     1834 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/Contributing.md
--rw-r--r--   0        0        0     1069 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/LICENSE
--rw-r--r--   0        0        0     6967 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/README.md
--rw-r--r--   0        0        0       14 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/cbindgen.toml
--rw-r--r--   0        0        0      639 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/conftest.py
--rw-r--r--   0        0        0      638 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/doc/Makefile
--rw-r--r--   0        0        0      804 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/doc/make.bat
--rw-r--r--   0        0        0       16 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/doc/requirements.txt
--rw-r--r--   0        0        0      155 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/doc/source/arrow_odbc.rst
--rw-r--r--   0        0        0     1965 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/doc/source/conf.py
--rw-r--r--   0        0        0      458 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/doc/source/index.rst
--rw-r--r--   0        0        0       67 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/doc/source/modules.rst
--rw-r--r--   0        0        0      348 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/docker-compose.yml
--rw-r--r--   0        0        0      563 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/manylinux/Dockerfile
--rw-r--r--   0        0        0      121 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/manylinux/Readme.md
--rw-r--r--   0        0        0      148 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/manylinux/WHEEL
--rw-r--r--   0        0        0     1256 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/manylinux/build_wheel.sh
--rw-r--r--   0        0        0      617 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/pyproject.toml
--rw-r--r--   0        0        0      265 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/python/arrow_odbc/__init__.py
--rw-r--r--   0        0        0     1321 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/python/arrow_odbc/connect.py
--rw-r--r--   0        0        0      672 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/python/arrow_odbc/error.py
--rw-r--r--   0        0        0     8737 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/python/arrow_odbc/reader.py
--rw-r--r--   0        0        0     4612 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/python/arrow_odbc/writer.py
--rw-r--r--   0        0        0     2133 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/src/error.rs
--rw-r--r--   0        0        0     2591 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/src/lib.rs
--rw-r--r--   0        0        0     1283 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/src/parameter.rs
--rw-r--r--   0        0        0     6320 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/src/reader.rs
--rw-r--r--   0        0        0     3650 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/src/writer.rs
--rw-r--r--   0        0        0        0 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/tests/__init__.py
--rw-r--r--   0        0        0     4115 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/tests/iris.csv
--rw-r--r--   0        0        0    14814 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/tests/test_arrow_odbc.py
--rw-r--r--   0        0        0    47685 2023-01-13 18:28:04.000000 arrow_odbc-0.3.9/Cargo.lock
--rw-r--r--   0        0        0     7491 1970-01-01 00:00:00.000000 arrow_odbc-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 arrow_odbc-1.0.0/Cargo.toml
+-rw-r--r--   0      501       20      136 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.gitattributes
+-rw-r--r--   0      501       20      131 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.github/dependabot.yml
+-rw-r--r--   0      501       20     1522 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0      501       20     1807 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.github/workflows/wheel.yml
+-rw-r--r--   0      501       20      286 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.gitignore
+-rw-r--r--   0      501       20      841 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.readthedocs.yaml
+-rw-r--r--   0      501       20     4815 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/Changelog.md
+-rw-r--r--   0      501       20     1834 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/Contributing.md
+-rw-r--r--   0      501       20     1069 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/LICENSE
+-rw-r--r--   0      501       20     7305 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/README.md
+-rw-r--r--   0      501       20       14 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/cbindgen.toml
+-rw-r--r--   0      501       20      639 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/conftest.py
+-rw-r--r--   0      501       20      638 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/Makefile
+-rw-r--r--   0      501       20      804 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/make.bat
+-rw-r--r--   0      501       20       16 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/requirements.txt
+-rw-r--r--   0      501       20      155 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/source/arrow_odbc.rst
+-rw-r--r--   0      501       20     1965 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/source/conf.py
+-rw-r--r--   0      501       20      458 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/source/index.rst
+-rw-r--r--   0      501       20       67 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/source/modules.rst
+-rw-r--r--   0      501       20      348 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/docker-compose.yml
+-rw-r--r--   0      501       20      564 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/manylinux/Dockerfile
+-rw-r--r--   0      501       20      121 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/manylinux/Readme.md
+-rw-r--r--   0      501       20      148 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/manylinux/WHEEL
+-rw-r--r--   0      501       20     1256 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/manylinux/build_wheel.sh
+-rw-r--r--   0      501       20      617 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/pyproject.toml
+-rw-r--r--   0      501       20      307 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/python/arrow_odbc/__init__.py
+-rw-r--r--   0      501       20     1645 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/python/arrow_odbc/connect.py
+-rw-r--r--   0      501       20      672 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/python/arrow_odbc/error.py
+-rw-r--r--   0      501       20    13961 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/python/arrow_odbc/reader.py
+-rw-r--r--   0      501       20     7915 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/python/arrow_odbc/writer.py
+-rw-r--r--   0      501       20     2131 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/src/error.rs
+-rw-r--r--   0      501       20     2842 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/src/lib.rs
+-rw-r--r--   0      501       20     1239 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/src/parameter.rs
+-rw-r--r--   0      501       20     8314 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/src/reader.rs
+-rw-r--r--   0      501       20     3613 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/src/writer.rs
+-rw-r--r--   0      501       20        0 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/tests/__init__.py
+-rw-r--r--   0      501       20     4115 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/tests/iris.csv
+-rw-r--r--   0      501       20     2413 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/tests/iris.parquet
+-rw-r--r--   0      501       20    19182 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/tests/test_arrow_odbc.py
+-rw-r--r--   0      501       20    35304 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/Cargo.lock
+-rw-r--r--   0        0        0     7829 1970-01-01 00:00:00.000000 arrow_odbc-1.0.0/PKG-INFO
```

### Comparing `arrow_odbc-0.3.9/Cargo.toml` & `arrow_odbc-1.0.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 [lib]
 # Name needs to be identical to python package name
 name = "arrow_odbc"
 crate-type = ["cdylib"]
 
 [dependencies]
-arrow-odbc = "0.26.0"
+arrow-odbc = "0.27.0"
 # arrow would be included indirectly using arrow-odbc, but we need to explicitly specify the ffi
 # feature.
-arrow = { version = "30.0.1", default-features = false, features = ["ffi"] }
+arrow = { version = "36.0.0", default-features = false, features = ["ffi"] }
 lazy_static = "1.4.0"
 # We only depend indirectly on log, but we include it directly here to disable logging at compile
 # time.
 log = { version = "0.4.17", features = ["release_max_level_off"] }
 
 [profile.release]
 # Panics should only be caused by logic errors and are considered bugs
```

### Comparing `arrow_odbc-0.3.9/.github/workflows/test.yml` & `arrow_odbc-1.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/.github/workflows/wheel.yml` & `arrow_odbc-1.0.0/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/.readthedocs.yaml` & `arrow_odbc-1.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/Changelog.md` & `arrow_odbc-1.0.0/Changelog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,36 @@
 # Changelog
 
+## 1.0.0
+
+- Breaking change: `read_arrow_batches_from_odbc` now also returns a batch reader instead of `None`, even if the SQL statement did not produce a result set. The resulting reader will be empty, i.e. iterating over batches stops immediatly. The assaciated schema attribute will contain no columns.
+- Support for querying stored procedures returning multiple result sets is added. Call `more_results` on the reader to advance to the next result set.
+
+## 0.3.14
+
+- Update Rust dependencies
+- Add `from_table_to_db` to better support insertion directly from an arrow header rather than a record batch reader.
+
+## 0.3.13
+
+- Support for inserting large binary strings
+
+## 0.3.12
+
+- Fix: If an error occurrs during inintalizing the writer it is now correctly translated into a python exception interrupting the control flow befor accessing an invalid writer object. Before this fix an error would have caused an invalid memory access violation.
+
+## 0.3.11
+
+- Fix manylinux wheel build
+
+## 0.3.10
+
+- Support for explicit login timeout in seconds via the `login_timeout_sec` parameter in both `read_arrow_batches_from_odbc` and `insert_into_table`.
+- Updated Rust dependencies
+
 ## 0.3.9
 
 - Updated Rust dependencies
   - This includes an update to `odbc-api 0.54.0`. This avoids escalating into an error if a query emits at least 32767 warnings.
 
 ## 0.3.8
```

### Comparing `arrow_odbc-0.3.9/Contributing.md` & `arrow_odbc-1.0.0/Contributing.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/LICENSE` & `arrow_odbc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/README.md` & `arrow_odbc-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Fill Apache Arrow arrays from ODBC data sources. This package is build on top of the [`pyarrow`](https://pypi.org/project/arrow/) Python package and [`arrow-odbc`](https://crates.io/crates/arrow-odbc) Rust crate and enables you to read the data of an ODBC data source as sequence of Apache Arrow record batches.
 
 This package can also be used to insert data in Arrow record batches to database tables.
 
 This package has been designed to be easily deployable, so it provides a prebuild many linux wheel which is independent of the specific version of your Python interpreter and the specific Arrow Version you want to use. It will dynamically link against the ODBC driver manager provided by your system.
 
-Users looking for more features than just bulk fetching/inserting data from/into ODBC data sources in Python should also take a look at [`turbodbc`](https://github.com/blue-yonder/turbodbc) which has a helpful community and seen a lot of battle testing. This Python package is more narrow in Scope (which is a fancy way of saying it has less features), as it is only concerned with bulk fetching Arrow Arrays. `turbodbc` may be harder to install using `pip` though, due to it's reliance on C++ API and external dependencies like `boost`.
+Users looking for more features than just bulk fetching/inserting data from/into ODBC data sources in Python should also take a look at [`turbodbc`](https://github.com/blue-yonder/turbodbc) which has a helpful community and seen a lot of battle testing. This Python package is more narrow in Scope (which is a fancy way of saying it has less features), as it is only concerned with bulk fetching Arrow Arrays. `arrow-odbc` may have less features than `turbodbc`, but it is easier to install and more resilient to version changes in `pyarrow`, since it is independent of C++ ABI, system dependencies (with the exeception of your ODBC driver manager of course) and your specific Python ABI. It also offers pre build wheels windows, linux and OS-X on [`pypi`](https://pypi.org/project/arrow-odbc/). In addition to that there is also a conda-forge recipie (thanks to @timkpaine).
 
 ## About Arrow
 
 > [Apache Arrow](https://arrow.apache.org/) defines a language-independent columnar memory format for flat and hierarchical data, organized for efficient analytic operations on modern hardware like CPUs and GPUs. The Arrow memory format also supports zero-copy reads for lightning-fast data access without serialization overhead.
 
 ## About ODBC
```

### Comparing `arrow_odbc-0.3.9/conftest.py` & `arrow_odbc-1.0.0/conftest.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/doc/Makefile` & `arrow_odbc-1.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/doc/make.bat` & `arrow_odbc-1.0.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/doc/source/conf.py` & `arrow_odbc-1.0.0/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "arrow-odbc"
 copyright = "2021, Markus Klein"
 author = "Markus Klein"
 
 # The full version, including alpha/beta/rc tags
-release = "0.3.9"
+release = "1.0.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `arrow_odbc-0.3.9/manylinux/Dockerfile` & `arrow_odbc-1.0.0/manylinux/Dockerfile`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 FROM quay.io/pypa/manylinux2014_x86_64
 
 # Install unix-odbc from source. Version installed via YUM is too old
-RUN curl http://www.unixodbc.org/unixODBC-2.3.9.tar.gz > unixODBC-2.3.9.tar.gz
+RUN curl https://www.unixodbc.org/unixODBC-2.3.9.tar.gz > unixODBC-2.3.9.tar.gz
 RUN tar -xzf unixODBC-2.3.9.tar.gz
 RUN cd unixODBC-2.3.9 && ./configure && make && make install
 
 # RUN yum search unixodbc
 # RUN yum install unixODBC.x86_64 -y
 
 RUN curl https://sh.rustup.rs -sSf | sh -s -- -y --default-toolchain stable
```

### Comparing `arrow_odbc-0.3.9/manylinux/build_wheel.sh` & `arrow_odbc-1.0.0/manylinux/build_wheel.sh`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/pyproject.toml` & `arrow_odbc-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "maturin"
 
 [project]
 name = "arrow-odbc"
 authors = [{name = "Markus Klein"}]
 description="Read the data of an ODBC data source as sequence of Apache Arrow record batches."
 readme = "README.md"
-version = "0.3.9"
+version = "1.0.0"
 dependencies = ["cffi", "pyarrow"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = ["pytest < 8.0.0"]
```

### Comparing `arrow_odbc-0.3.9/python/arrow_odbc/error.py` & `arrow_odbc-1.0.0/python/arrow_odbc/error.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/python/arrow_odbc/reader.py` & `arrow_odbc-1.0.0/python/arrow_odbc/reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,81 @@
+import pyarrow as pa
+
 from typing import List, Optional, Tuple
 from cffi.api import FFI  # type: ignore
 
 from pyarrow.cffi import ffi as arrow_ffi  # type: ignore
 from pyarrow import RecordBatch, Schema, Array
 
 from arrow_odbc.connect import to_bytes_and_len, connect_to_database  # type: ignore
 
 from .arrow_odbc import ffi, lib  # type: ignore
 from .error import raise_on_error
 
 
+def _schema_from_handle(handle) -> Schema:
+    """
+    Take a handle to an ArrowOdbcReader and return the associated pyarrow schema
+    """
+    if handle == ffi.NULL:
+        # The query ran successfully, but did not produce a result
+        return pa.schema([])
+    else:
+        # Expose schema as attribute
+        # https://github.com/apache/arrow/blob/5ead37593472c42f61c76396dde7dcb8954bde70/python/pyarrow/tests/test_cffi.py
+        with arrow_ffi.new("struct ArrowSchema *") as schema_out:
+            error = lib.arrow_odbc_reader_schema(handle, schema_out)
+
+            raise_on_error(error)
+            ptr_schema = int(ffi.cast("uintptr_t", schema_out))
+            return Schema._import_from_c(ptr_schema)
+
+
 class BatchReader:
     """
     Iterates over Arrow batches from an ODBC data source
     """
 
     def __init__(self, handle):
         """
         Low level constructor, users should rather invoke
         `read_arrow_batches_from_odbc` in order to create instances of
         `BatchReader`.
         """
 
         # We take owners of the corresponding reader written in Rust and keep it alive until `self`
-        # is deleted
+        # is deleted.
+        #
+        # The introduction of `more_results` made it necessary to also be able to represent already
+        # consumed or empty cursors. In Python the user can always keep a reference to a
+        # BatchReader alive and we have no way to force him/her to release it in case we move past
+        # the last result set. Therfore we mutate this instance and represent these states with
+        # handle == NULL and an empty schema.
         self.handle = handle
-        # Expose schema as attribute
-        # https://github.com/apache/arrow/blob/5ead37593472c42f61c76396dde7dcb8954bde70/python/pyarrow/tests/test_cffi.py
-        schema_out = arrow_ffi.new("struct ArrowSchema *")
-        error = lib.arrow_odbc_reader_schema(self.handle, schema_out)
-        raise_on_error(error)
-        ptr_schema = int(ffi.cast("uintptr_t", schema_out))
-        self.schema = Schema._import_from_c(ptr_schema)
+
+        # If this raises `__del__` will be invoked and free the handle, so we do not leak
+        # resources here.
+        self.schema = _schema_from_handle(self.handle)
 
     def __del__(self):
-        # Free the resources associated with this handle.
-        lib.arrow_odbc_reader_free(self.handle)
+        if self.handle != ffi.NULL:
+            # Free the resources associated with this handle.
+            lib.arrow_odbc_reader_free(self.handle)
 
     def __iter__(self):
         # Implement iterable protocol so reader can be used in for loops.
         return self
 
     def __next__(self) -> RecordBatch:
         # Implment iterator protocol
 
+        # In case this represents a non-cursor behave as iterating over an empty set of batches
+        if self.handle == ffi.NULL:
+            raise StopIteration()
+
         # In case of an error this is going to be a non null handle to the error
         array = arrow_ffi.new("struct ArrowArray *")
         schema = arrow_ffi.new("struct ArrowSchema *")
 
         has_next_out = ffi.new("int*")
 
         error = lib.arrow_odbc_reader_next(self.handle, array, schema, has_next_out)
@@ -57,32 +85,104 @@
             raise StopIteration()
         else:
             array_ptr = int(ffi.cast("uintptr_t", array))
             schema_ptr = int(ffi.cast("uintptr_t", schema))
             struct_array = Array._import_from_c(array_ptr, schema_ptr)
             return RecordBatch.from_struct_array(struct_array)
 
+    def more_results(
+        self,
+        batch_size: int,
+        max_text_size: Optional[int] = None,
+        max_binary_size: Optional[int] = None,
+        falliable_allocations: bool = True,
+    ) -> bool:
+        """
+        Move the reader to the next result set returned by the data source.
+
+        A datasource may return multiple results if multiple SQL statements are executed in a single
+        query or a stored procedure is called. This method closes the current cursor and moves it to
+        the next result set. You may move to the next result set without extracting the current one.
+
+        :param batch_size: The maximum number rows within each batch. Batch size can be individually
+            choosen for each result set.
+        :param max_text_size: An upper limit for the size of buffers bound to variadic text columns
+            of the data source. This limit does not (directly) apply to the size of the created
+            arrow buffers, but rather applies to the buffers used for the data in transit. Use this
+            option if you have e.g. VARCHAR(MAX) fields the next batch.
+        :param max_binary_size: An upper limit for the size of buffers bound to variadic binary
+            columns of the data source. This limit does not (directly) apply to the size of the
+            created arrow buffers, but rather applies to the buffers used for the data in transit.
+            Use this option if you have e.g. VARBINARY(MAX) fields in your next batch.
+        :param falliable_allocations: If ``True`` an recoverable error is raised in case there is
+            not enough memory to allocate the buffers. This option may incurr a performance penalty
+            which scales with the batch size parameter (but not with the amount of actual data in
+            the source). In case you can test your query against the schema you can safely set this
+            to ``False``. The required memory will not depend on the amount of data in the data
+            source. Default is ``True`` though, safety first.
+        :return: ``True`` in case there is another result set. ``False`` in case that the last
+            result set has been processed.
+        """
+        if self.handle == ffi.NULL:
+            # Last result set has already been processed
+            return False
+
+        if max_text_size is None:
+            max_text_size = 0
+        if max_binary_size is None:
+            max_binary_size = 0
+
+        reader_out = ffi.new("ArrowOdbcReader **")
+
+        error = lib.arrow_odbc_reader_more_results(
+            self.handle,
+            reader_out,
+            batch_size,
+            max_text_size,
+            max_binary_size,
+            falliable_allocations,
+        )
+
+        # We passed ownership of handle to more_results. We must do this before raising, since
+        # self.handle is otherwise invalid.
+        self.handle = reader_out[0]
+
+        # See if we managed to execute the query successfully and return an
+        # error if not
+        raise_on_error(error)
+
+        # Every result set can have its own schema, so we must update our member
+        self.schema = _schema_from_handle(self.handle)
+
+        return self.handle != FFI.NULL
+
 
 def read_arrow_batches_from_odbc(
     query: str,
     batch_size: int,
     connection_string: str,
     user: Optional[str] = None,
     password: Optional[str] = None,
     parameters: Optional[List[Optional[str]]] = None,
     max_text_size: Optional[int] = None,
     max_binary_size: Optional[int] = None,
     falliable_allocations: bool = True,
+    login_timeout_sec: Optional[int] = None,
 ) -> Optional[BatchReader]:
     """
     Execute the query and read the result as an iterator over Arrow batches.
 
     :param query: The SQL statement yielding the result set which is converted into arrow record
         batches.
-    :param batch_size: The maxmium number rows within each batch.
+    :param batch_size: The maximum number rows within each batch. Please note that the actual batch
+        size is up to the ODBC driver of your database. This parameter influences primarily the size
+        of the buffers the ODBC driver is supposed to fill with data, yet it is up to the driver how
+        many values it fills in one go. Also note that the primary use-case of batching is to reduce
+        IO overhead. So even if you fetch millions of rows a batch size of 100 or 1000 may be
+        entirely reasonable. This is trading memory for speed, but with diminishing returns.
     :param connection_string: ODBC Connection string used to connect to the data source. To find a
         connection string for your data source try https://www.connectionstrings.com/.
     :param user: Allows for specifying the user seperatly from the connection string if it is not
         already part of it. The value will eventually be escaped and attached to the connection
         string as `UID`.
     :param password: Allows for specifying the password seperatly from the connection string if it
         is not already part of it. The value will eventually be escaped and attached to the
@@ -114,21 +214,28 @@
         looking for. This is the maximum size in bytes of the binary column.
     :param falliable_allocations: If ``True`` an recoverable error is raised in case there is not
         enough memory to allocate the buffers. This option may incurr a performance penalty which
         scales with the batch size parameter (but not with the amount of actual data in the source).
         In case you can test your query against the schema you can safely set this to ``False``. The
         required memory will not depend on the amount of data in the data source. Default is
         ``True`` though, safety first.
+    :param login_timeout_sec: Number of seconds to wait for a login request to complete before
+        returning to the application. The default is driver-dependent. If ``0``, the timeout is
+        disabled and a connection attempt will wait indefinitely. If the specified timeout exceeds
+        the maximum login timeout in the data source, the driver substitutes that value and uses
+        that instead.
     :return: In case the query does not produce a result set (e.g. in case of an INSERT statement),
         ``None`` is returned. Should the statement return a result set a ``BatchReader`` is
         returned, which implements the iterator protocol and iterates over individual arrow batches.
     """
     query_bytes = query.encode("utf-8")
 
-    connection = connect_to_database(connection_string, user, password)
+    connection = connect_to_database(
+        connection_string, user, password, login_timeout_sec
+    )
 
     # Connecting to the database has been successful. Note that connection does not truly take
     # ownership of the connection. If it runs out of scope (e.g. due to a raised exception) the
     # connection would not be closed and its associated resources would not be freed.
     # However, this is fine since everything from here on out until we call arrow_odbc_reader_make
     # is infalliable. arrow_odbc_reader_make will truly take ownership of the connection. Even if it
     # should fail, it will be closed correctly.
@@ -170,12 +277,8 @@
     )
 
     # See if we managed to execute the query successfully and return an
     # error if not
     raise_on_error(error)
 
     reader = reader_out[0]
-    if reader == ffi.NULL:
-        # The query ran successfully but did not produce a result set
-        return None
-    else:
-        return BatchReader(reader)
+    return BatchReader(reader)
```

### Comparing `arrow_odbc-0.3.9/src/error.rs` & `arrow_odbc-1.0.0/src/error.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::{ffi::CString, fmt::Display, os::{raw::c_char}, ptr::NonNull};
+use std::{ffi::CString, fmt::Display, os::raw::c_char, ptr::NonNull};
 
 /// Handle to an error emmitted by arrow odbc
 pub struct ArrowOdbcError {
     message: CString,
 }
 
 impl ArrowOdbcError {
@@ -58,17 +58,16 @@
     };
 }
 
 #[cfg(test)]
 mod tests {
     use super::ArrowOdbcError;
 
-
     #[test]
     fn should_truncate_strings_with_interior_nul() {
         let message = "Hello\0World!";
 
         let error = ArrowOdbcError::new(message);
 
         assert_eq!("Hello", error.message.into_string().unwrap())
     }
-}
+}
```

### Comparing `arrow_odbc-0.3.9/src/lib.rs` & `arrow_odbc-1.0.0/src/lib.rs`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 mod error;
 mod parameter;
 mod reader;
 mod writer;
 
 use std::{borrow::Cow, ptr::null_mut, slice, str};
 
-use arrow_odbc::odbc_api::{escape_attribute_value, Connection, Environment};
+use arrow_odbc::odbc_api::{escape_attribute_value, Connection, ConnectionOptions, Environment};
 use lazy_static::lazy_static;
 
 pub use error::{arrow_odbc_error_free, arrow_odbc_error_message, ArrowOdbcError};
 pub use reader::{
     arrow_odbc_reader_free, arrow_odbc_reader_make, arrow_odbc_reader_next, ArrowOdbcReader,
 };
 pub use writer::{
@@ -37,23 +37,33 @@
 pub unsafe extern "C" fn arrow_odbc_connect_with_connection_string(
     connection_string_buf: *const u8,
     connection_string_len: usize,
     user: *const u8,
     user_len: usize,
     password: *const u8,
     password_len: usize,
+    login_timeout_sec_ptr: *const u32,
     connection_out: *mut *mut OdbcConnection,
 ) -> *mut ArrowOdbcError {
     let connection_string = slice::from_raw_parts(connection_string_buf, connection_string_len);
     let mut connection_string = Cow::Borrowed(str::from_utf8(connection_string).unwrap());
 
     append_attribute("UID", &mut connection_string, user, user_len);
     append_attribute("PWD", &mut connection_string, password, password_len);
 
-    let connection = try_!(ENV.connect_with_connection_string(&connection_string));
+    let login_timeout_sec = if login_timeout_sec_ptr.is_null() {
+        None
+    } else {
+        Some(*login_timeout_sec_ptr)
+    };
+
+    let connection = try_!(ENV.connect_with_connection_string(
+        &connection_string,
+        ConnectionOptions { login_timeout_sec }
+    ));
 
     *connection_out = Box::into_raw(Box::new(OdbcConnection(connection)));
     null_mut()
 }
 
 /// Append attribute like user and value to connection string
 unsafe fn append_attribute(
@@ -66,9 +76,9 @@
     if ptr.is_null() {
         return;
     }
 
     let bytes = slice::from_raw_parts(ptr, len);
     let text = str::from_utf8(bytes).unwrap();
     let escaped = escape_attribute_value(text);
-    *connection_string = format!("{}{}={};", connection_string, attribute_name, escaped).into()
+    *connection_string = format!("{connection_string}{attribute_name}={escaped};").into()
 }
```

### Comparing `arrow_odbc-0.3.9/src/parameter.rs` & `arrow_odbc-1.0.0/src/parameter.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-use std::slice;
-
-use arrow_odbc::odbc_api::parameter::VarCharSlice;
-
-/// Opaque type holding a parameter intended to be bound to a placeholder (`?`) in an SQL query.
-pub struct ArrowOdbcParameter<'a>(VarCharSlice<'a>);
-
-impl<'a> ArrowOdbcParameter<'a> {
-    fn from_opt_str(value: Option<&'a [u8]>) -> Self {
-        let inner = if let Some(slice) = value {
-            VarCharSlice::new(slice)
-        } else {
-            VarCharSlice::NULL
-        };
-        Self(inner)
-    }
-}
-
-impl<'a> ArrowOdbcParameter<'a> {
-    pub fn unwrap(self) -> VarCharSlice<'a> {
-        self.0
-    }
-}
-
-/// # Safety
-/// 
-/// `char_buf` may be `NULL`, but if it is not, it must contain a valid utf-8 sequence not shorter
-/// than `char_len`. This function does not take ownership of the parameter. The parameter must at
-/// least be valid until the call make reader is finished.
-#[no_mangle]
-pub unsafe extern "C" fn arrow_odbc_parameter_string_make(
-    char_buf: *const u8,
-    char_len: usize,
-) -> *mut ArrowOdbcParameter<'static> {
-    let opt = if char_buf.is_null() {
-        None
-    } else {
-        Some(slice::from_raw_parts(char_buf, char_len))
-    };
-
-    let param = ArrowOdbcParameter::from_opt_str(opt);
-    Box::into_raw(Box::new(param))
-}
+use std::slice;
+
+use arrow_odbc::odbc_api::parameter::VarCharSlice;
+
+/// Opaque type holding a parameter intended to be bound to a placeholder (`?`) in an SQL query.
+pub struct ArrowOdbcParameter<'a>(VarCharSlice<'a>);
+
+impl<'a> ArrowOdbcParameter<'a> {
+    fn from_opt_str(value: Option<&'a [u8]>) -> Self {
+        let inner = if let Some(slice) = value {
+            VarCharSlice::new(slice)
+        } else {
+            VarCharSlice::NULL
+        };
+        Self(inner)
+    }
+}
+
+impl<'a> ArrowOdbcParameter<'a> {
+    pub fn unwrap(self) -> VarCharSlice<'a> {
+        self.0
+    }
+}
+
+/// # Safety
+///
+/// `char_buf` may be `NULL`, but if it is not, it must contain a valid utf-8 sequence not shorter
+/// than `char_len`. This function does not take ownership of the parameter. The parameter must at
+/// least be valid until the call make reader is finished.
+#[no_mangle]
+pub unsafe extern "C" fn arrow_odbc_parameter_string_make(
+    char_buf: *const u8,
+    char_len: usize,
+) -> *mut ArrowOdbcParameter<'static> {
+    let opt = if char_buf.is_null() {
+        None
+    } else {
+        Some(slice::from_raw_parts(char_buf, char_len))
+    };
+
+    let param = ArrowOdbcParameter::from_opt_str(opt);
+    Box::into_raw(Box::new(param))
+}
```

### Comparing `arrow_odbc-0.3.9/src/reader.rs` & `arrow_odbc-1.0.0/src/reader.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 use std::{
     ffi::c_void,
-    ptr::swap,
+    mem::swap,
     os::raw::c_int,
     ptr::{null_mut, NonNull},
     slice, str,
-    sync::Arc,
 };
 
-use arrow::ffi::ArrowArray;
+use arrow::ffi::{ArrowArray, ArrowArrayRef, FFI_ArrowArray, FFI_ArrowSchema};
 use arrow_odbc::{
     arrow::{
         array::{Array, StructArray},
-        ffi::{FFI_ArrowArray, FFI_ArrowSchema},
         record_batch::RecordBatchReader,
     },
-    odbc_api::{CursorImpl, StatementConnection},
+    odbc_api::{Cursor, CursorImpl, StatementConnection},
     BufferAllocationOptions, OdbcReader,
 };
 
 use crate::{parameter::ArrowOdbcParameter, try_, ArrowOdbcError, OdbcConnection};
 
 /// Opaque type holding all the state associated with an ODBC reader implementation in Rust. This
 /// type also has ownership of the ODBC Connection handle.
@@ -118,56 +116,114 @@
 pub unsafe extern "C" fn arrow_odbc_reader_free(reader: NonNull<ArrowOdbcReader>) {
     drop(Box::from_raw(reader.as_ptr()));
 }
 
 /// # Safety
 ///
 /// * `reader` must be valid non-null reader, allocated by [`arrow_odbc_reader_make`].
-/// * `array_out` and `schema_out` must both point to valid pointers, which themselves may be null.
+/// * `array` and `schema` must both point to valid, but unitialized memory. The memory must be
+///   allocated in the python code, so it can also be deallocated there and the python part can take
+///   ownership of the whole thing.
+/// * In case an error is returned `array` and `schema` remain unchanged.
 #[no_mangle]
 pub unsafe extern "C" fn arrow_odbc_reader_next(
     mut reader: NonNull<ArrowOdbcReader>,
     array: *mut c_void,
     schema: *mut c_void,
     has_next_out: *mut c_int,
 ) -> *mut ArrowOdbcError {
     let schema = schema as *mut FFI_ArrowSchema;
     let array = array as *mut FFI_ArrowArray;
 
     if let Some(result) = reader.as_mut().0.next() {
-        *array = FFI_ArrowArray::empty();
-        *schema = FFI_ArrowSchema::empty();
-
+        // In case of an error fail early, before we change the output paramters.
         let batch = try_!(result);
         let struct_array: StructArray = batch.into();
         let arrow_array = try_!(ArrowArray::try_new(struct_array.data().clone()));
 
-        let (ffi_array_ptr, ffi_schema_ptr) = ArrowArray::into_raw(arrow_array);
+        // Create two empty instances, so array and schema now point to valid instances.
+        *array = FFI_ArrowArray::empty();
+        *schema = FFI_ArrowSchema::empty();
+        // Now that the instances are valid it safe to use them as references rather than pointers
+        // (references must always be valid)
+        let array = &mut *array;
+        let schema = &mut *schema;
+
+        let array_data = arrow_array.to_data().unwrap();
 
-        // In order to avoid memory leaks we must convert both pointers returned by the `into_raw`
-        // method. So we must back to `Arc` again, so they are freed at the end of this function
-        // call in order to avoid memory leaks. Furthermore it is the callers responsibility to
-        // provide us with the FFI_Arrow* structures to fill, and the caller maintains ownership
-        // over them.
-
-        let mut arc_schema = Arc::from_raw(ffi_schema_ptr);
-        let source_schema = Arc::get_mut(&mut arc_schema).unwrap();
-        swap(schema, source_schema);
-
-        let mut arc_array = Arc::from_raw(ffi_array_ptr);
-        let source_array = Arc::get_mut(&mut arc_array).unwrap();
-        swap(array, source_array);
+        let mut ffi_array = FFI_ArrowArray::new(&array_data);
+        let mut ffi_schema = FFI_ArrowSchema::try_from(array_data.data_type()).unwrap();
+
+        swap(array, &mut ffi_array);
+        swap(schema, &mut ffi_schema);
 
         *has_next_out = 1;
     } else {
         *has_next_out = 0;
     }
     null_mut()
 }
 
+/// # Safety
+///
+/// * `reader_in` must point to a valid non-null reader, allocated by [`arrow_odbc_reader_make`].
+///   This function takes ownership of reader_in and will free the associated resources, even in
+///   case of error. After the function call `reader_in` is invalid and must not be dereferenced.
+/// * `reader_out` In case another result set exists, `reader_out` will point to a valid instance of
+///   [`ArrowOdbcReader`]. Otherwise, it will point to `NULL`.
+#[no_mangle]
+pub unsafe extern "C" fn arrow_odbc_reader_more_results(
+    reader_in: NonNull<ArrowOdbcReader>,
+    reader_out: *mut *mut ArrowOdbcReader,
+    batch_size: usize,
+    max_text_size: usize,
+    max_binary_size: usize,
+    fallibale_allocations: bool,
+) -> *mut ArrowOdbcError {
+    // In case we return early, we want the caller to know that reader_out is invalid.
+    *reader_out = null_mut();
+
+    // Dereference reader and take ownership of it.
+    let reader = Box::from_raw(reader_in.as_ptr()).0;
+
+    // Move cursor to the next result set.
+    let cursor = try_!(reader.into_cursor());
+    let next = try_!(cursor.more_results());
+
+    if let Some(cursor) = next {
+        // There is another result set. Let us create an new reader
+        let max_text_size = if max_text_size == 0 {
+            None
+        } else {
+            Some(max_text_size)
+        };
+        let max_binary_size = if max_binary_size == 0 {
+            None
+        } else {
+            Some(max_binary_size)
+        };
+        let buffer_allocation_options = BufferAllocationOptions {
+            max_text_size,
+            max_binary_size,
+            fallibale_allocations,
+        };
+
+        let reader = try_!(OdbcReader::with(
+            cursor,
+            batch_size,
+            None,
+            buffer_allocation_options
+        ));
+        let reader = ArrowOdbcReader(reader);
+        *reader_out = Box::into_raw(Box::new(reader));
+    }
+
+    null_mut()
+}
+
 /// Retrieve the associated schema from a reader.
 #[no_mangle]
 pub unsafe extern "C" fn arrow_odbc_reader_schema(
     mut reader: NonNull<ArrowOdbcReader>,
     out_schema: *mut c_void,
 ) -> *mut ArrowOdbcError {
     let out_schema: *mut FFI_ArrowSchema = out_schema as *mut FFI_ArrowSchema;
```

### Comparing `arrow_odbc-0.3.9/tests/iris.csv` & `arrow_odbc-1.0.0/tests/iris.csv`

 * *Files identical despite different names*

### Comparing `arrow_odbc-0.3.9/tests/test_arrow_odbc.py` & `arrow_odbc-1.0.0/tests/test_arrow_odbc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import gc
 import os
 
 import pyarrow as pa
 import pyarrow.csv as csv
+import pyarrow.parquet as pq
 
 import pytest
 
 from subprocess import run, check_output
 
 from pytest import raises
 
-from arrow_odbc import read_arrow_batches_from_odbc, Error
-from arrow_odbc.writer import insert_into_table
+from arrow_odbc import (
+    insert_into_table,
+    from_table_to_db,
+    read_arrow_batches_from_odbc,
+    Error,
+)
 
 MSSQL = "Driver={ODBC Driver 17 for SQL Server};Server=localhost;UID=SA;PWD=My@Test@Password1;"
 
 
-def test_should_report_error_on_invalid_connection_string():
+def test_should_report_error_on_invalid_connection_string_reading():
     """
     We want to forward the original ODBC errors to the end user. Of course foo
     is not a valid connection string. Therefore we want to see the creation of
     this connection fail, but with a nice error.
     """
     # Error on windows: Data source name not found and no default driver specified
     # Erron on linux: Data source name not found, and no default driver specified
@@ -41,32 +46,91 @@
 
     with raises(Error, match="Invalid object name 'Foo'"):
         read_arrow_batches_from_odbc(
             query=query, batch_size=100, connection_string=MSSQL
         )
 
 
-def test_insert_statement():
+def test_no_result_set():
     """
-    BatchReader should be `None` if statement does not produce a result set.
+    BatchReader should be be empty if no result set can be produced
     """
     table = "EmptyResult"
     os.system(f'odbcsv fetch -c "{MSSQL}" -q "DROP TABLE IF EXISTS {table};"')
     os.system(f'odbcsv fetch -c "{MSSQL}" -q "CREATE TABLE {table} (a int);"')
 
     # This statement does not produce a result set
     query = f"INSERT INTO {table} (a) VALUES (42);"
+    reader = read_arrow_batches_from_odbc(
+        query=query, batch_size=100, connection_string=MSSQL
+    )
 
-    assert (
-        read_arrow_batches_from_odbc(
-            query=query, batch_size=100, connection_string=MSSQL
-        )
-        is None
+    assert reader.schema == pa.schema([])
+    with raises(StopIteration):
+        next(iter(reader))
+
+
+def test_skip_to_second_result_set():
+    """
+    Calling `more_results` should allow to consume the next result set
+    """
+    # This statement produces two result sets
+    query = f"SELECT 1 AS a; SELECT 2 AS b;"
+
+    reader = read_arrow_batches_from_odbc(
+        query=query, batch_size=100, connection_string=MSSQL
     )
 
+    # Skip to second result set
+    reader.more_results(batch_size=100)
+
+    # Process second result
+    schema = pa.schema([pa.field("b", pa.int32(), nullable=False)])
+    assert reader.schema == schema
+    expected = pa.RecordBatch.from_pydict({"b": [2]}, schema)
+    assert expected == next(iter(reader))
+    with raises(StopIteration):
+        next(iter(reader))
+
+
+def test_more_results_return_should_indicate_if_there_is_a_result_set():
+    """
+    Calling `more_results` should return a boolean indicating wether there is another result set or
+    not to be extracted
+    """
+    # This statement produces two result sets
+    query = f"SELECT 1 AS a; SELECT 2 AS b;"
+
+    reader = read_arrow_batches_from_odbc(
+        query=query, batch_size=100, connection_string=MSSQL
+    )
+    
+    assert reader.more_results(batch_size=100)
+    assert not reader.more_results(batch_size=100)
+
+
+def test_advancing_past_last_result_set_leaves_empty_reader():
+    """
+    Moving past the last result set, leaves a reader returning a schema with no columns and no
+    batches.
+    """
+    # This statement produces one result
+    query = f"SELECT 1 AS a;"
+
+    reader = read_arrow_batches_from_odbc(
+        query=query, batch_size=100, connection_string=MSSQL
+    )
+    # Move to a second result set, which does not exist
+    reader.more_results(batch_size=100)
+
+    # Assert schema and batches are empty
+    assert reader.schema == pa.schema([])
+    with raises(StopIteration):
+        next(iter(reader))
+
 
 def test_empty_table():
     """
     Should return an empty iterator querying an empty table.
     """
     table = "Empty"
     os.system(f'odbcsv fetch -c "{MSSQL}" -q "DROP TABLE IF EXISTS {table};"')
@@ -172,22 +236,17 @@
     reader = read_arrow_batches_from_odbc(
         query=query,
         batch_size=100,
         connection_string=connection_string,
         user=user,
         password=password,
     )
-    it = iter(reader)
-
-    actual = next(it)
-
-    schema = pa.schema([("a", pa.int32())])
-    expected = pa.RecordBatch.from_pydict({"a": [42]}, schema)
-    assert expected == actual
 
+    it = iter(reader)
+    _result = next(it)
     with raises(StopIteration):
         next(it)
 
 
 def test_query_char():
     """
     Query a string those UTF-16 representation is larger than the maximum binary column length on
@@ -426,29 +485,53 @@
     Insert should raise on invalid connection string
     """
     # Given
     invalid_connection_string = "FOO"
     schema = pa.schema([("a", pa.int64())])
 
     def iter_record_batches():
-        for i in range(2):
-            yield pa.RecordBatch.from_arrays([pa.array([1, 2, 3])], schema=schema)
+        yield pa.RecordBatch.from_arrays([pa.array([1, 2, 3])], schema=schema)
 
     reader = pa.RecordBatchReader.from_batches(schema, iter_record_batches())
 
     # When / Then
     with raises(Error, match="Data source name not found"):
         insert_into_table(
             connection_string=invalid_connection_string,
             chunk_size=20,
             table="MyTable",
             reader=reader,
         )
 
 
+def test_insert_should_raise_on_unsupported_column_type():
+    """
+    Insert should raise on unsupported column type
+    """
+    # Given
+    schema = pa.schema([("a", pa.dictionary(pa.int32(), pa.int32()))])
+
+    def iter_record_batches():
+        yield pa.RecordBatch.from_arrays([pa.array([(1, 1)])], schema=schema)
+
+    reader = pa.RecordBatchReader.from_batches(schema, iter_record_batches())
+
+    # When / Then
+    with raises(
+        Error,
+        match="The arrow data type Dictionary\(Int32, Int32\) is not supported for insertion.",
+    ):
+        insert_into_table(
+            connection_string=MSSQL,
+            chunk_size=20,
+            table="MyTable",
+            reader=reader,
+        )
+
+
 def test_insert_batches():
     """
     Insert data into database
     """
     # Given
     table = "InsertBatches"
     os.system(f'odbcsv fetch -c "{MSSQL}" -q "DROP TABLE IF EXISTS {table};"')
@@ -471,28 +554,81 @@
     # Then
     actual = check_output(
         ["odbcsv", "fetch", "-c", MSSQL, "-q", f"SELECT a FROM {table} ORDER BY id"]
     )
     assert "a\n1\n2\n3\n1\n2\n3\n" == actual.decode("utf8")
 
 
+def test_insert_from_parquet():
+    """
+    Insert data into database from a parquet file
+    """
+    # Given
+    table = "InsertFromParquet"
+    os.system(f'odbcsv fetch -c "{MSSQL}" -q "DROP TABLE IF EXISTS {table};"')
+    os.system(
+        f'odbcsv fetch -c "{MSSQL}" -q "CREATE TABLE {table} (sepal_length REAL, sepal_width REAL, petal_length REAL, petal_width REAL, variety VARCHAR(20) )"'
+    )
+
+    # When
+    arrow_table = pq.read_table("./tests/iris.parquet")
+    from_table_to_db(source=arrow_table, target=table, connection_string=MSSQL)
+
+    # Then
+    after_roundtrip = read_arrow_batches_from_odbc(
+        query=f"SELECT * FROM {table}", batch_size=1000, connection_string=MSSQL
+    )
+    assert after_roundtrip.schema == arrow_table.schema
+    assert len(next(after_roundtrip)) == 150
+
+
+def test_insert_large_string():
+    """
+    Insert an arrow table whose schema contains a "large string".
+    """
+    # Given
+    table = "InsertLargeString"
+    os.system(f'odbcsv fetch -c "{MSSQL}" -q "DROP TABLE IF EXISTS {table};"')
+    os.system(f'odbcsv fetch -c "{MSSQL}" -q "CREATE TABLE {table} (a Varchar(50))"')
+    schema = pa.schema([("a", pa.large_string())])
+
+    def iter_record_batches():
+        # The string value is not actually large, just the schema information allows it to be
+        yield pa.RecordBatch.from_arrays([pa.array(["Hello"])], schema=schema)
+
+    reader = pa.RecordBatchReader.from_batches(schema, iter_record_batches())
+
+    # When
+    insert_into_table(
+        connection_string=MSSQL, chunk_size=20, table=table, reader=reader
+    )
+
+    # Then
+    actual = check_output(
+        ["odbcsv", "fetch", "-c", MSSQL, "-q", f"SELECT a FROM {table}"]
+    )
+    assert "a\nHello\n" == actual.decode("utf8")
+
+
 @pytest.mark.slow
 def test_should_not_leak_memory_for_each_batch():
     """
     Read a bunch of arrow batches and see if total memory usage went over a
-    threshold after running GC.
+    threshold after running GC. Currently I let this run manually and see if
+    the process takes more memory over time as an assertion.
     """
     # Given
     table = "ShouldNotLeakMemoryForEachBatch"
     os.system(f'odbcsv fetch -c "{MSSQL}" -q "DROP TABLE IF EXISTS {table};"')
     os.system(
         f'odbcsv fetch -c "{MSSQL}" -q "CREATE TABLE {table} (sepal_length REAL, sepal_width REAL, petal_length REAL, petal_width REAL, variety VARCHAR(20) )"'
     )
     os.system(f'odbcsv insert -c "{MSSQL}" -i ./tests/iris.csv {table}')
 
-    # When, create an individual batch for each row
-    reader = read_arrow_batches_from_odbc(
-        query=f"SELECT * FROM {table}", batch_size=1, connection_string=MSSQL
-    )
+    for _ in range(1):
+        # When, create an individual batch for each row
+        reader = read_arrow_batches_from_odbc(
+            query=f"SELECT * FROM {table}", batch_size=1, connection_string=MSSQL
+        )
 
-    for batch in reader:
-        del batch
+        for batch in reader:
+            del batch
```

### Comparing `arrow_odbc-0.3.9/Cargo.lock` & `arrow_odbc-1.0.0/Cargo.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "adler"
-version = "1.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
-
-[[package]]
 name = "ahash"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf6ccdb167abbf410dcb915cabd428929d7f6a04980b54a11f26a39f1c7f7107"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
  "cfg-if",
  "const-random",
  "getrandom",
  "once_cell",
  "version_check",
 ]
@@ -27,128 +21,139 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "android_system_properties"
-version = "0.1.5"
+name = "android-activity"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+checksum = "7c77a0045eda8b888c76ea473c2b0515ba6f471d318f8927c5c72240937035a6"
 dependencies = [
+ "android-properties",
+ "bitflags 1.3.2",
+ "cc",
+ "jni-sys",
  "libc",
+ "log",
+ "ndk",
+ "ndk-context",
+ "ndk-sys",
+ "num_enum",
 ]
 
 [[package]]
-name = "arrayref"
-version = "0.3.6"
+name = "android-properties"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4c527152e37cf757a3f78aae5a06fbeefdb07ccc535c980a3208ee3060dd544"
+checksum = "fc7eb209b1518d6bb87b283c20095f5228ecda460da70b44f0802523dea6da04"
 
 [[package]]
-name = "arrayvec"
-version = "0.5.2"
+name = "android_system_properties"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23b62fc65de8e4e7f52534fb52b0f3ed04746ae267519eef2a83941e8085068b"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
 
 [[package]]
 name = "arrow"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1948f504d736dc6f71ea33773c5c7475998c44925be5321e9d18087a626845f5"
+checksum = "990dfa1a9328504aa135820da1c95066537b69ad94c04881b785f64328e0fa6b"
 dependencies = [
  "ahash",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-ord",
  "arrow-row",
  "arrow-schema",
  "arrow-select",
  "arrow-string",
- "bitflags",
 ]
 
 [[package]]
 name = "arrow-arith"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5984187a7913813ffd5bb034fdc6810bdbe0ae4cff2292f0eb92797342dc02c8"
+checksum = "f2b2e52de0ab54173f9b08232b7184c26af82ee7ab4ac77c83396633c90199fa"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-array"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf71dc342bb42343d331b58c0bcad095dc045e367493d47b7f4c4509e2adfee5"
+checksum = "e10849b60c17dbabb334be1f4ef7550701aa58082b71335ce1ed586601b2f423"
 dependencies = [
  "ahash",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
- "hashbrown",
+ "hashbrown 0.13.2",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7b328d9f3e124cca761ec85a6d3fcea9bf8de1b8531c7a3b6abd367472024df"
+checksum = "b0746ae991b186be39933147117f8339eb1c4bbbea1c8ad37e7bf5851a1a06ba"
 dependencies = [
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-cast"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03976edbf66ac00a582af10a51743f0a9611777adfd68c71799d783344c3bdd2"
+checksum = "b88897802515d7b193e38b27ddd9d9e43923d410a9e46307582d756959ee9595"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "chrono",
  "lexical-core",
  "num",
 ]
 
 [[package]]
 name = "arrow-data"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "174df8602dedcdb9149538809c11bd3c0888af30b915f763c66a3d724391c8b9"
+checksum = "533f937efa1aaad9dc86f6a0e382c2fa736a4943e2090c946138079bdf060cef"
 dependencies = [
  "arrow-buffer",
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-odbc"
-version = "0.26.2"
+version = "0.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72e4711141e40b89d2ca34d3d63ed47aa8e2773ba0df30ed25f35a423c19b10e"
+checksum = "f67c97fff393388a0e128d584a71372ac1d27222ab321e44ff031b2ccd66ffe6"
 dependencies = [
  "arrow",
  "atoi",
  "chrono",
  "odbc-api",
  "thiserror",
 ]
@@ -161,65 +166,69 @@
  "arrow-odbc",
  "lazy_static",
  "log",
 ]
 
 [[package]]
 name = "arrow-ord"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7db83c14ddddf81c1d10ce303670f70b7687c8f52de7425b09ae905e4357fda5"
+checksum = "33d2671eb3793f9410230ac3efb0e6d36307be8a2dac5fad58ac9abde8e9f01e"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
+ "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-row"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db41abdf586f1dba8c2973711d5c69ffb9d63688ffa46354b8c85bf9347a921c"
+checksum = "fc11fa039338cebbf4e29cf709c8ac1d6a65c7540063d4a25f991ab255ca85c8"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half",
- "hashbrown",
+ "hashbrown 0.13.2",
 ]
 
 [[package]]
 name = "arrow-schema"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a99dcc494fe6224e5ece572c5935d5109120a71df06bd8e04c4e23ac14dd8fac"
+checksum = "d04f17f7b86ded0b5baf98fe6123391c4343e031acc3ccc5fa604cc180bff220"
+dependencies = [
+ "bitflags 2.1.0",
+]
 
 [[package]]
 name = "arrow-select"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3a2cde3ea85b28f64704045d7d54e0fcc4b17efffced574d2dd3320218298f"
+checksum = "163e35de698098ff5f5f672ada9dc1f82533f10407c7a11e2cd09f3bcf31d18a"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "num",
 ]
 
 [[package]]
 name = "arrow-string"
-version = "30.0.1"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04cf8d0003ebe0aecc716e0ac8c858c570872a7485c7c6284975f31469703a0d"
+checksum = "bfdfbed1b10209f0dc68e6aa4c43dc76079af65880965c7c3b73f641f23d4aba"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "regex",
@@ -244,112 +253,81 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
-name = "block"
-version = "0.1.6"
+name = "bitflags"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d8c1fef690941d3e7788d328517591fecc684c084084702d6ff1641e993699a"
+checksum = "c70beb79cbb5ce9c4f8e20849978f34225931f665bb49efa6982875a4d5facb3"
 
 [[package]]
-name = "bumpalo"
-version = "3.11.1"
+name = "block-sys"
+version = "0.1.0-beta.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "572f695136211188308f16ad2ca5c851a712c464060ae6974944458eb83880ba"
+checksum = "0fa55741ee90902547802152aaf3f8e5248aab7e21468089560d4c8840561146"
+dependencies = [
+ "objc-sys",
+]
 
 [[package]]
-name = "bytemuck"
-version = "1.12.3"
+name = "block2"
+version = "0.2.0-alpha.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aaa3a8d9a1ca92e282c96a32d6511b695d7d994d1d102ba85d279f9b2756947f"
+checksum = "8dd9e63c1744f755c2f60332b88de39d341e5e86239014ad839bd71c106dec42"
+dependencies = [
+ "block-sys",
+ "objc2-encode",
+]
 
 [[package]]
-name = "calloop"
-version = "0.10.5"
+name = "bumpalo"
+version = "3.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a59225be45a478d772ce015d9743e49e92798ece9e34eda9a6aa2a6a7f40192"
-dependencies = [
- "log",
- "nix 0.25.1",
- "slotmap",
- "thiserror",
- "vec_map",
-]
+checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
 
 [[package]]
 name = "cc"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a20104e2335ce8a659d6dd92a51a767a0c062599c73b343fd152cb401e828c3d"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+dependencies = [
+ "jobserver",
+]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "cfg_aliases"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
+
+[[package]]
 name = "chrono"
-version = "0.4.23"
+version = "0.4.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b0a3d9ed01224b22057780a37bb8c5dbfe1be8ba48678e7bf57ec4b385411f"
+checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
 dependencies = [
  "iana-time-zone",
  "js-sys",
  "num-integer",
  "num-traits",
  "time",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
-name = "cmake"
-version = "0.1.49"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db34956e100b30725f2eb215f90d4871051239535632f84fea3bc92722c66b7c"
-dependencies = [
- "cc",
-]
-
-[[package]]
-name = "cocoa"
-version = "0.24.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f425db7937052c684daec3bd6375c8abe2d146dca4b8b143d6db777c39138f3a"
-dependencies = [
- "bitflags",
- "block",
- "cocoa-foundation",
- "core-foundation",
- "core-graphics",
- "foreign-types 0.3.2",
- "libc",
- "objc",
-]
-
-[[package]]
-name = "cocoa-foundation"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ade49b65d560ca58c403a479bb396592b155c0185eada742ee323d1d68d6318"
-dependencies = [
- "bitflags",
- "block",
- "core-foundation",
- "core-graphics-types",
- "foreign-types 0.3.2",
- "libc",
- "objc",
-]
-
-[[package]]
 name = "codespan-reporting"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
 dependencies = [
  "termcolor",
  "unicode-width",
@@ -385,314 +363,125 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "core-graphics"
 version = "0.22.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2581bbab3b8ffc6fcbd550bf46c355135d16e9ff2a6ea032ad6b9bf1d7efe4fb"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "core-foundation",
  "core-graphics-types",
- "foreign-types 0.3.2",
+ "foreign-types",
  "libc",
 ]
 
 [[package]]
 name = "core-graphics-types"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3a68b68b3446082644c91ac778bf50cd4104bfb002b5a6a7c44cca5a2c70788b"
 dependencies = [
- "bitflags",
- "core-foundation",
- "foreign-types 0.3.2",
- "libc",
-]
-
-[[package]]
-name = "core-text"
-version = "19.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99d74ada66e07c1cefa18f8abfba765b486f250de2e4a999e5727fc0dd4b4a25"
-dependencies = [
- "core-foundation",
- "core-graphics",
- "foreign-types 0.3.2",
- "libc",
-]
-
-[[package]]
-name = "crc32fast"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
-name = "crossfont"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21fd3add36ea31aba1520aa5288714dd63be506106753226d0eb387a93bc9c45"
-dependencies = [
- "cocoa",
+ "bitflags 1.3.2",
  "core-foundation",
- "core-foundation-sys",
- "core-graphics",
- "core-text",
- "dwrote",
- "foreign-types 0.5.0",
- "freetype-rs",
+ "foreign-types",
  "libc",
- "log",
- "objc",
- "once_cell",
- "pkg-config",
- "servo-fontconfig",
- "winapi",
 ]
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
-name = "cty"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b365fabc795046672053e29c954733ec3b05e4be654ab130fe8f1f94d7051f35"
-
-[[package]]
 name = "cxx"
-version = "1.0.86"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "51d1075c37807dcf850c379432f0df05ba52cc30f279c5cfc43cc221ce7f8579"
+checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
 name = "cxx-build"
-version = "1.0.86"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5044281f61b27bc598f2f6647d480aed48d2bf52d6eb0b627d84c0361b17aa70"
+checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
-version = "1.0.86"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61b50bc93ba22c27b0d31128d2d130a0a6b3d267ae27ef7e4fae2167dfe8781c"
+checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
 
 [[package]]
 name = "cxxbridge-macro"
-version = "1.0.86"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e61fda7e62115119469c7b3591fd913ecca96fb766cfd3f2e2502ab7bc87a5"
+checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
-]
-
-[[package]]
-name = "darling"
-version = "0.13.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a01d95850c592940db9b8194bc39f4bc0e89dee5c4265e4b1807c34a9aba453c"
-dependencies = [
- "darling_core",
- "darling_macro",
-]
-
-[[package]]
-name = "darling_core"
-version = "0.13.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "859d65a907b6852c9361e3185c862aae7fafd2887876799fa55f5f99dc40d610"
-dependencies = [
- "fnv",
- "ident_case",
- "proc-macro2",
- "quote",
- "strsim",
- "syn",
-]
-
-[[package]]
-name = "darling_macro"
-version = "0.13.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c972679f83bdf9c42bd905396b6c3588a843a17f0f16dfcfa3e2c5d57441835"
-dependencies = [
- "darling_core",
- "quote",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "dispatch"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd0c93bb4b0c6d9b77f4435b0ae98c24d17f1c45b2ff844c6151a07256ca923b"
 
 [[package]]
-name = "dlib"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac1b7517328c04c2aa68422fc60a41b92208182142ed04a25879c26c8f878794"
-dependencies = [
- "libloading",
-]
-
-[[package]]
-name = "downcast-rs"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ea835d29036a4087793836fa931b08837ad5e957da9e23886b29586fb9b6650"
-
-[[package]]
-name = "dwrote"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "439a1c2ba5611ad3ed731280541d36d2e9c4ac5e7fb818a27b604bdc5a6aa65b"
-dependencies = [
- "lazy_static",
- "libc",
- "serde",
- "serde_derive",
- "winapi",
- "wio",
-]
-
-[[package]]
-name = "expat-sys"
-version = "2.1.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658f19728920138342f68408b7cf7644d90d4784353d8ebc32e7e8663dbe45fa"
-dependencies = [
- "cmake",
- "pkg-config",
-]
-
-[[package]]
-name = "flate2"
-version = "1.0.25"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
-dependencies = [
- "crc32fast",
- "miniz_oxide",
-]
-
-[[package]]
-name = "fnv"
-version = "1.0.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
-
-[[package]]
 name = "force-send-sync"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d9188d4e883c054455b2c7950be30c54b11d7400f0a8562b74a4acd79c495b6"
 
 [[package]]
 name = "foreign-types"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6f339eb8adc052cd2ca78910fda869aefa38d22d5cb648e6485e4d3fc06f3b1"
 dependencies = [
- "foreign-types-shared 0.1.1",
-]
-
-[[package]]
-name = "foreign-types"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d737d9aa519fb7b749cbc3b962edcf310a8dd1f4b67c91c4f83975dbdd17d965"
-dependencies = [
- "foreign-types-macros",
- "foreign-types-shared 0.3.1",
-]
-
-[[package]]
-name = "foreign-types-macros"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8469d0d40519bc608ec6863f1cc88f3f1deee15913f2f3b3e573d81ed38cccc"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
+ "foreign-types-shared",
 ]
 
 [[package]]
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
-name = "foreign-types-shared"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa9a19cbb55df58761df49b23516a86d432839add4af60fc256da840f66ed35b"
-
-[[package]]
-name = "freetype-rs"
-version = "0.26.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74eadec9d0a5c28c54bb9882e54787275152a4e36ce206b45d7451384e5bf5fb"
-dependencies = [
- "bitflags",
- "freetype-sys",
- "libc",
-]
-
-[[package]]
-name = "freetype-sys"
-version = "0.13.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a37d4011c0cc628dfa766fcc195454f4b068d7afdc2adfd28861191d866e731a"
-dependencies = [
- "cmake",
- "libc",
- "pkg-config",
-]
-
-[[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
@@ -703,47 +492,57 @@
 dependencies = [
  "crunchy",
  "num-traits",
 ]
 
 [[package]]
 name = "hashbrown"
+version = "0.12.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+
+[[package]]
+name = "hashbrown"
 version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.53"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64c122667b287044802d6ce17ee2ddf13207ed924c712de9a66a5814d5b64765"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "winapi",
+ "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
-name = "ident_case"
-version = "1.0.1"
+name = "indexmap"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
+dependencies = [
+ "autocfg",
+ "hashbrown 0.12.3",
+]
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
@@ -756,18 +555,27 @@
 [[package]]
 name = "jni-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8eaf4bc02d17cbdd7ff4c7438cafcdf7fb9a4613313ad11b4f8fefe7d3fa0130"
 
 [[package]]
+name = "jobserver"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "js-sys"
-version = "0.3.60"
+version = "0.3.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -836,27 +644,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.139"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
-
-[[package]]
-name = "libloading"
-version = "0.7.4"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
-dependencies = [
- "cfg-if",
- "winapi",
-]
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
@@ -866,186 +664,58 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
-name = "lock_api"
-version = "0.4.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
-dependencies = [
- "autocfg",
- "scopeguard",
-]
-
-[[package]]
 name = "log"
 version = "0.4.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "malloc_buf"
-version = "0.0.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62bb907fe88d54d8d9ce32a3cceab4218ed2f6b7d35617cafe9adf84e43919cb"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
-name = "memmap2"
-version = "0.5.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b182332558b18d807c4ce1ca8ca983b34c3ee32765e47b3f0f69b90355cc1dc"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "memoffset"
-version = "0.6.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "minimal-lexical"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
-
-[[package]]
-name = "miniz_oxide"
-version = "0.6.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
-dependencies = [
- "adler",
-]
-
-[[package]]
-name = "mio"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d732bc30207a6423068df043e3d02e0735b155ad7ce1a6f76fe2baa5b158de"
-dependencies = [
- "libc",
- "log",
- "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys 0.42.0",
-]
-
-[[package]]
 name = "ndk"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "451422b7e4718271c8b5b3aadf5adedba43dc76312454b387e98fae0fc951aa0"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "jni-sys",
  "ndk-sys",
  "num_enum",
- "raw-window-handle 0.5.0",
+ "raw-window-handle",
  "thiserror",
 ]
 
 [[package]]
 name = "ndk-context"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "27b02d87554356db9e9a873add8782d4ea6e3e58ea071a9adb9a2e8ddb884a8b"
 
 [[package]]
-name = "ndk-glue"
-version = "0.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0434fabdd2c15e0aab768ca31d5b7b333717f03cf02037d5a0a3ff3c278ed67f"
-dependencies = [
- "libc",
- "log",
- "ndk",
- "ndk-context",
- "ndk-macro",
- "ndk-sys",
- "once_cell",
- "parking_lot",
-]
-
-[[package]]
-name = "ndk-macro"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0df7ac00c4672f9d5aece54ee3347520b7e20f158656c7db2e6de01902eb7a6c"
-dependencies = [
- "darling",
- "proc-macro-crate",
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
 name = "ndk-sys"
 version = "0.4.1+23.1.7779620"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3cf2aae958bd232cac5069850591667ad422d263686d75b52a065f9badeee5a3"
 dependencies = [
  "jni-sys",
 ]
 
 [[package]]
-name = "nix"
-version = "0.24.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa52e972a9a719cecb6864fb88568781eb706bac2cd1d4f04a648542dbf78069"
-dependencies = [
- "bitflags",
- "cfg-if",
- "libc",
- "memoffset",
-]
-
-[[package]]
-name = "nix"
-version = "0.25.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f346ff70e7dbfd675fe90590b92d59ef2de15a8779ae305ebcbfd3f0caf59be4"
-dependencies = [
- "autocfg",
- "bitflags",
- "cfg-if",
- "libc",
- "memoffset",
-]
-
-[[package]]
-name = "nom"
-version = "7.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5507769c4919c998e69e49c839d9dc6e693ede4cc4290d6ad8b41d4f09c548c"
-dependencies = [
- "memchr",
- "minimal-lexical",
-]
-
-[[package]]
 name = "num"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
 dependencies = [
  "num-bigint",
  "num-complex",
@@ -1064,17 +734,17 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ae39348c8bc5fbd7f40c727a9925f03517afd2ab27d46702108b6a7e5414c19"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.45"
@@ -1116,355 +786,233 @@
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_enum"
-version = "0.5.7"
+version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf5395665662ef45796a4ff5486c5d41d29e0c09640af4c5f17fd94ee2c119c9"
+checksum = "1f646caf906c20226733ed5b1374287eb97e3c2a5c227ce668c1f2ce20ae57c9"
 dependencies = [
  "num_enum_derive",
 ]
 
 [[package]]
 name = "num_enum_derive"
-version = "0.5.7"
+version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b0498641e53dd6ac1a4f22547548caa6864cc4933784319cd1775271c5a46ce"
+checksum = "dcbff9bc912032c62bf65ef1d5aea88983b420f4f839db1e9b0c281a25c9c799"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "objc-sys"
+version = "0.2.0-beta.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df3b9834c1e95694a05a828b59f55fa2afec6288359cda67146126b3f90a55d7"
+
+[[package]]
+name = "objc2"
+version = "0.3.0-beta.3.patch-leaks.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e01640f9f2cb1220bbe80325e179e532cb3379ebcd1bf2279d703c19fe3a468"
+dependencies = [
+ "block2",
+ "objc-sys",
+ "objc2-encode",
 ]
 
 [[package]]
-name = "objc"
-version = "0.2.7"
+name = "objc2-encode"
+version = "2.0.0-pre.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "915b1b472bc21c53464d6c8461c9d3af805ba1ef837e1cac254428f4a77177b1"
+checksum = "abfcac41015b00a120608fdaa6938c44cb983fee294351cc4bac7638b4e50512"
 dependencies = [
- "malloc_buf",
+ "objc-sys",
 ]
 
 [[package]]
 name = "odbc-api"
-version = "0.54.0"
+version = "0.56.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed99ecea03c2a36fa6e1c3dbb3d7c5dd8d170e009502f3097357af698f521164"
+checksum = "c6bf11bd6f82a755c9ab4df0723401ab4f45a0bac9c034466e6e9d2f5c162c8e"
 dependencies = [
  "force-send-sync",
  "log",
  "odbc-sys",
  "thiserror",
  "widestring",
  "winit",
 ]
 
 [[package]]
 name = "odbc-sys"
-version = "0.21.3"
+version = "0.21.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "576c6d6bbba0ffa13888958275b5cb67dba93d2d5ff7d5e69609b90e1d34ab69"
+checksum = "592c5c4ce58f47dde428c52b39904252191d25436b410cc232fae0813ff58f08"
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
-name = "parking_lot"
-version = "0.12.1"
+name = "orbclient"
+version = "0.3.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
-dependencies = [
- "lock_api",
- "parking_lot_core",
-]
-
-[[package]]
-name = "parking_lot_core"
-version = "0.9.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba1ef8814b5c993410bb3adfad7a5ed269563e4a2f90c41f5d85be7fb47133bf"
+checksum = "0e9829e16c5e112e94efb5e2ad1fe17f8c1c99bb0fcdc8c65c44e935d904767d"
 dependencies = [
  "cfg-if",
- "libc",
- "redox_syscall",
- "smallvec",
- "windows-sys 0.42.0",
-]
-
-[[package]]
-name = "percent-encoding"
-version = "2.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
-
-[[package]]
-name = "pkg-config"
-version = "0.3.26"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
-
-[[package]]
-name = "png"
-version = "0.17.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d708eaf860a19b19ce538740d2b4bdeeb8337fa53f7738455e706623ad5c638"
-dependencies = [
- "bitflags",
- "crc32fast",
- "flate2",
- "miniz_oxide",
+ "redox_syscall 0.2.16",
+ "wasm-bindgen",
+ "web-sys",
 ]
 
 [[package]]
 name = "proc-macro-crate"
-version = "1.2.1"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eda0fc3b0fb7c975631757e14d9049da17374063edb6ebbcbc54d880d4fe94e9"
+checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
 dependencies = [
  "once_cell",
- "thiserror",
- "toml",
+ "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.49"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a8eca9f9c4ffde41714334dee777596264c7825420f521abc92b5b5deb63a5"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "raw-window-handle"
-version = "0.4.3"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b800beb9b6e7d2df1fe337c9e3d04e3af22a124460fb4c30fcc22c9117cefb41"
-dependencies = [
- "cty",
-]
+checksum = "f2ff9a1f06a88b01621b7ae906ef0211290d1c8a168a15542486a8f61c0833b9"
 
 [[package]]
-name = "raw-window-handle"
-version = "0.5.0"
+name = "redox_syscall"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed7e3d950b66e19e0c372f3fa3fbbcf85b1746b571f74e0c2af6042a5c93420a"
+checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "cty",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
-
-[[package]]
-name = "safe_arch"
-version = "0.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1ff3d6d9696af502cc3110dacce942840fb06ff4514cad92236ecc455f2ce05"
-dependencies = [
- "bytemuck",
-]
-
-[[package]]
-name = "scoped-tls"
-version = "1.0.1"
+version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1cf6437eb19a8f4a6cc0f7dca544973b0b78843adbfeb3683d1a94a0024a294"
-
-[[package]]
-name = "scopeguard"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "scratch"
-version = "1.0.3"
+version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddccb15bcce173023b3fedd9436f882a0739b8dfb45e4f6b6002bee5929f61b2"
+checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
 
 [[package]]
-name = "sctk-adwaita"
-version = "0.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61270629cc6b4d77ec1907db1033d5c2e1a404c412743621981a871dc9c12339"
-dependencies = [
- "crossfont",
- "log",
- "smithay-client-toolkit",
- "tiny-skia",
-]
-
-[[package]]
-name = "serde"
-version = "1.0.152"
+name = "static_assertions"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
-name = "serde_derive"
-version = "1.0.152"
+name = "syn"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
-]
-
-[[package]]
-name = "servo-fontconfig"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7e3e22fe5fd73d04ebf0daa049d3efe3eae55369ce38ab16d07ddd9ac5c217c"
-dependencies = [
- "libc",
- "servo-fontconfig-sys",
-]
-
-[[package]]
-name = "servo-fontconfig-sys"
-version = "5.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e36b879db9892dfa40f95da1c38a835d41634b825fbd8c4c418093d53c24b388"
-dependencies = [
- "expat-sys",
- "freetype-sys",
- "pkg-config",
-]
-
-[[package]]
-name = "slotmap"
-version = "1.0.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1e08e261d0e8f5c43123b7adf3e4ca1690d655377ac93a03b2c9d3e98de1342"
-dependencies = [
- "version_check",
-]
-
-[[package]]
-name = "smallvec"
-version = "1.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
-
-[[package]]
-name = "smithay-client-toolkit"
-version = "0.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f307c47d32d2715eb2e0ece5589057820e0e5e70d07c247d1063e844e107f454"
-dependencies = [
- "bitflags",
- "calloop",
- "dlib",
- "lazy_static",
- "log",
- "memmap2",
- "nix 0.24.3",
- "pkg-config",
- "wayland-client",
- "wayland-cursor",
- "wayland-protocols",
+ "unicode-ident",
 ]
 
 [[package]]
-name = "static_assertions"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
-
-[[package]]
-name = "strsim"
-version = "0.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
-
-[[package]]
 name = "syn"
-version = "1.0.107"
+version = "2.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "termcolor"
-version = "1.1.3"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
+checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
@@ -1480,66 +1028,43 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
-name = "tiny-skia"
-version = "0.7.0"
+name = "toml_datetime"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642680569bb895b16e4b9d181c60be1ed136fa0c9c7f11d004daf053ba89bf82"
-dependencies = [
- "arrayref",
- "arrayvec",
- "bytemuck",
- "cfg-if",
- "png",
- "safe_arch",
- "tiny-skia-path",
-]
+checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
 
 [[package]]
-name = "tiny-skia-path"
-version = "0.7.0"
+name = "toml_edit"
+version = "0.19.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c114d32f0c2ee43d585367cb013dfaba967ab9f62b90d9af0d696e955e70fa6c"
+checksum = "239410c8609e8125456927e6707163a3b1fdb40561e4b803bc041f466ccfdc13"
 dependencies = [
- "arrayref",
- "bytemuck",
-]
-
-[[package]]
-name = "toml"
-version = "0.5.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1333c76748e868a4d9d1017b5ab53171dfd095f70c712fdb4653a406547f598f"
-dependencies = [
- "serde",
+ "indexmap",
+ "toml_datetime",
+ "winnow",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
 [[package]]
-name = "vec_map"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
-
-[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wasi"
@@ -1551,144 +1076,82 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.83"
+version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.83"
+version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.83"
+version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.83"
+version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.83"
+version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
-
-[[package]]
-name = "wayland-client"
-version = "0.29.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f3b068c05a039c9f755f881dc50f01732214f5685e379829759088967c46715"
-dependencies = [
- "bitflags",
- "downcast-rs",
- "libc",
- "nix 0.24.3",
- "scoped-tls",
- "wayland-commons",
- "wayland-scanner",
- "wayland-sys",
-]
-
-[[package]]
-name = "wayland-commons"
-version = "0.29.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8691f134d584a33a6606d9d717b95c4fa20065605f798a3f350d78dced02a902"
-dependencies = [
- "nix 0.24.3",
- "once_cell",
- "smallvec",
- "wayland-sys",
-]
-
-[[package]]
-name = "wayland-cursor"
-version = "0.29.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6865c6b66f13d6257bef1cd40cbfe8ef2f150fb8ebbdb1e8e873455931377661"
-dependencies = [
- "nix 0.24.3",
- "wayland-client",
- "xcursor",
-]
-
-[[package]]
-name = "wayland-protocols"
-version = "0.29.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b950621f9354b322ee817a23474e479b34be96c2e909c14f7bc0100e9a970bc6"
-dependencies = [
- "bitflags",
- "wayland-client",
- "wayland-commons",
- "wayland-scanner",
-]
+checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
 
 [[package]]
 name = "wayland-scanner"
 version = "0.29.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f4303d8fa22ab852f789e75a967f0a2cdc430a607751c0499bada3e451cbd53"
 dependencies = [
  "proc-macro2",
  "quote",
  "xml-rs",
 ]
 
 [[package]]
-name = "wayland-sys"
-version = "0.29.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be12ce1a3c39ec7dba25594b97b42cb3195d54953ddb9d3d95a7c3902bc6e9d4"
-dependencies = [
- "dlib",
- "lazy_static",
- "pkg-config",
-]
-
-[[package]]
 name = "web-sys"
-version = "0.3.60"
+version = "0.3.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcda906d8be16e728fd5adc5b729afad4e444e106ab28cd1c7256e54fa61510f"
+checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "widestring"
@@ -1724,173 +1187,179 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.36.1"
+name = "windows"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows_aarch64_msvc 0.36.1",
- "windows_i686_gnu 0.36.1",
- "windows_i686_msvc 0.36.1",
- "windows_x86_64_gnu 0.36.1",
- "windows_x86_64_msvc 0.36.1",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.45.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+dependencies = [
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc 0.42.1",
- "windows_i686_gnu 0.42.1",
- "windows_i686_msvc 0.42.1",
- "windows_x86_64_gnu 0.42.1",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc 0.42.1",
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winit"
-version = "0.27.5"
+version = "0.28.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb796d6fbd86b2fd896c9471e6f04d39d750076ebe5680a3958f00f5ab97657c"
+checksum = "4f504e8c117b9015f618774f8d58cd4781f5a479bc41079c064f974cbb253874"
 dependencies = [
- "bitflags",
- "cocoa",
+ "android-activity",
+ "bitflags 1.3.2",
+ "cfg_aliases",
  "core-foundation",
  "core-graphics",
  "dispatch",
  "instant",
  "libc",
  "log",
- "mio",
  "ndk",
- "ndk-glue",
- "objc",
+ "objc2",
  "once_cell",
- "parking_lot",
- "percent-encoding",
- "raw-window-handle 0.4.3",
- "raw-window-handle 0.5.0",
- "sctk-adwaita",
- "smithay-client-toolkit",
+ "orbclient",
+ "raw-window-handle",
+ "redox_syscall 0.3.5",
  "wasm-bindgen",
- "wayland-client",
- "wayland-protocols",
+ "wayland-scanner",
  "web-sys",
- "windows-sys 0.36.1",
- "x11-dl",
+ "windows-sys",
 ]
 
 [[package]]
-name = "wio"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d129932f4644ac2396cb456385cbf9e63b5b30c6e8dc4820bdca4eb082037a5"
-dependencies = [
- "winapi",
-]
-
-[[package]]
-name = "x11-dl"
-version = "2.20.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1536d6965a5d4e573c7ef73a2c15ebcd0b2de3347bdf526c34c297c00ac40f0"
-dependencies = [
- "lazy_static",
- "libc",
- "pkg-config",
-]
-
-[[package]]
-name = "xcursor"
-version = "0.3.4"
+name = "winnow"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "463705a63313cd4301184381c5e8042f0a7e9b4bb63653f216311d4ae74690b7"
+checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
 dependencies = [
- "nom",
+ "memchr",
 ]
 
 [[package]]
 name = "xml-rs"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2d7d3948613f75c98fd9328cfdcc45acc4d360655289d0a7d4ec931392200a3"
```

### Comparing `arrow_odbc-0.3.9/PKG-INFO` & `arrow_odbc-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: arrow-odbc
-Version: 0.3.9
+Version: 1.0.0
 Requires-Dist: cffi
 Requires-Dist: pyarrow
 Requires-Dist: pytest < 8.0.0; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: Read the data of an ODBC data source as sequence of Apache Arrow record batches.
 Author: Markus Klein
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: changelog, https://github.com/pacman82/arrow-odbc-py/blob/main/Changelog.md
 Project-URL: repository, https://github.com/pacman82/arrow-odbc-py
+Project-URL: changelog, https://github.com/pacman82/arrow-odbc-py/blob/main/Changelog.md
 
 # arrow-odbc-py
 
 [![Licence](https://img.shields.io/crates/l/arrow-odbc)](https://github.com/pacman82/arrow-odbc-py/blob/master/License)
 [![PyPI version](https://badge.fury.io/py/arrow-odbc.svg)](https://pypi.org/project/arrow-odbc/)
 [![Documentation Status](https://readthedocs.org/projects/arrow-odbc/badge/?version=latest)](https://arrow-odbc.readthedocs.io/en/latest/?badge=latest)
 
 Fill Apache Arrow arrays from ODBC data sources. This package is build on top of the [`pyarrow`](https://pypi.org/project/arrow/) Python package and [`arrow-odbc`](https://crates.io/crates/arrow-odbc) Rust crate and enables you to read the data of an ODBC data source as sequence of Apache Arrow record batches.
 
 This package can also be used to insert data in Arrow record batches to database tables.
 
 This package has been designed to be easily deployable, so it provides a prebuild many linux wheel which is independent of the specific version of your Python interpreter and the specific Arrow Version you want to use. It will dynamically link against the ODBC driver manager provided by your system.
 
-Users looking for more features than just bulk fetching/inserting data from/into ODBC data sources in Python should also take a look at [`turbodbc`](https://github.com/blue-yonder/turbodbc) which has a helpful community and seen a lot of battle testing. This Python package is more narrow in Scope (which is a fancy way of saying it has less features), as it is only concerned with bulk fetching Arrow Arrays. `turbodbc` may be harder to install using `pip` though, due to it's reliance on C++ API and external dependencies like `boost`.
+Users looking for more features than just bulk fetching/inserting data from/into ODBC data sources in Python should also take a look at [`turbodbc`](https://github.com/blue-yonder/turbodbc) which has a helpful community and seen a lot of battle testing. This Python package is more narrow in Scope (which is a fancy way of saying it has less features), as it is only concerned with bulk fetching Arrow Arrays. `arrow-odbc` may have less features than `turbodbc`, but it is easier to install and more resilient to version changes in `pyarrow`, since it is independent of C++ ABI, system dependencies (with the exeception of your ODBC driver manager of course) and your specific Python ABI. It also offers pre build wheels windows, linux and OS-X on [`pypi`](https://pypi.org/project/arrow-odbc/). In addition to that there is also a conda-forge recipie (thanks to @timkpaine).
 
 ## About Arrow
 
 > [Apache Arrow](https://arrow.apache.org/) defines a language-independent columnar memory format for flat and hierarchical data, organized for efficient analytic operations on modern hardware like CPUs and GPUs. The Arrow memory format also supports zero-copy reads for lightning-fast data access without serialization overhead.
 
 ## About ODBC
```

