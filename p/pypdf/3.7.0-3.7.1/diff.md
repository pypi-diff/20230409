# Comparing `tmp/pypdf-3.7.0.tar.gz` & `tmp/pypdf-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdf-3.7.0.tar", last modified: Sun Mar 26 14:11:18 2023, max compression
+gzip compressed data, was "pypdf-3.7.1.tar", last modified: Sun Apr  9 20:24:56 2023, max compression
```

## Comparing `pypdf-3.7.0.tar` & `pypdf-3.7.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0      488 2022-12-10 23:30:58.176669 pypdf-3.7.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0    34138 2023-03-26 14:11:09.507845 pypdf-3.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     3377 2023-03-19 10:45:11.184383 pypdf-3.7.0/CONTRIBUTORS.md
--rw-r--r--   0        0        0     1605 2022-12-10 23:30:58.184669 pypdf-3.7.0/LICENSE
--rw-r--r--   0        0        0       34 2022-12-10 23:30:58.184669 pypdf-3.7.0/MANIFEST.in
--rw-r--r--   0        0        0     4829 2022-12-31 10:47:18.983493 pypdf-3.7.0/README.md
--rw-r--r--   0        0        0     1234 2023-03-04 08:55:07.145847 pypdf-3.7.0/pypdf/__init__.py
--rw-r--r--   0        0        0    14870 2023-03-18 15:07:48.665105 pypdf-3.7.0/pypdf/_cmap.py
--rw-r--r--   0        0        0     1674 2023-02-28 08:12:53.909178 pypdf-3.7.0/pypdf/_codecs/__init__.py
--rw-r--r--   0        0        0   431492 2022-12-31 10:47:18.999493 pypdf-3.7.0/pypdf/_codecs/adobe_glyphs.py
--rw-r--r--   0        0        0     4269 2022-12-31 10:47:18.999493 pypdf-3.7.0/pypdf/_codecs/pdfdoc.py
--rw-r--r--   0        0        0     2630 2023-02-28 08:12:53.909178 pypdf-3.7.0/pypdf/_codecs/std.py
--rw-r--r--   0        0        0     3734 2022-12-31 10:47:18.999493 pypdf-3.7.0/pypdf/_codecs/symbol.py
--rw-r--r--   0        0        0     3742 2022-12-31 10:47:18.999493 pypdf-3.7.0/pypdf/_codecs/zapfding.py
--rw-r--r--   0        0        0    45635 2023-03-26 14:07:37.382395 pypdf-3.7.0/pypdf/_encryption.py
--rw-r--r--   0        0        0    30650 2023-03-04 11:49:14.882511 pypdf-3.7.0/pypdf/_merger.py
--rw-r--r--   0        0        0    82250 2023-03-18 15:07:48.665105 pypdf-3.7.0/pypdf/_page.py
--rw-r--r--   0        0        0     7186 2023-03-04 08:55:07.145847 pypdf-3.7.0/pypdf/_page_labels.py
--rw-r--r--   0        0        0     1863 2023-02-28 08:12:53.913179 pypdf-3.7.0/pypdf/_protocols.py
--rw-r--r--   0        0        0    85632 2023-03-20 19:14:10.631754 pypdf-3.7.0/pypdf/_reader.py
--rw-r--r--   0        0        0    12788 2023-03-26 14:07:37.382395 pypdf-3.7.0/pypdf/_security.py
--rw-r--r--   0        0        0    10008 2023-03-12 09:43:33.014879 pypdf-3.7.0/pypdf/_text_extraction/__init__.py
--rw-r--r--   0        0        0    14915 2023-03-18 15:53:28.693755 pypdf-3.7.0/pypdf/_utils.py
--rw-r--r--   0        0        0       22 2023-03-26 14:07:43.334345 pypdf-3.7.0/pypdf/_version.py
--rw-r--r--   0        0        0   121777 2023-03-26 14:07:37.386395 pypdf-3.7.0/pypdf/_writer.py
--rw-r--r--   0        0        0    13730 2023-03-26 11:38:56.913817 pypdf-3.7.0/pypdf/constants.py
--rw-r--r--   0        0        0     1631 2023-03-04 08:55:07.149847 pypdf-3.7.0/pypdf/errors.py
--rw-r--r--   0        0        0    24812 2023-03-26 14:07:37.386395 pypdf-3.7.0/pypdf/filters.py
--rw-r--r--   0        0        0     4395 2023-03-26 11:42:39.007648 pypdf-3.7.0/pypdf/generic/__init__.py
--rw-r--r--   0        0        0    17368 2023-03-26 11:42:39.007648 pypdf-3.7.0/pypdf/generic/_annotations.py
--rw-r--r--   0        0        0    24752 2023-03-04 11:49:14.882511 pypdf-3.7.0/pypdf/generic/_base.py
--rw-r--r--   0        0        0    54710 2023-03-26 08:34:42.996994 pypdf-3.7.0/pypdf/generic/_data_structures.py
--rw-r--r--   0        0        0     5427 2023-03-04 08:55:07.149847 pypdf-3.7.0/pypdf/generic/_fit.py
--rw-r--r--   0        0        0     1195 2023-02-28 08:19:03.524706 pypdf-3.7.0/pypdf/generic/_outline.py
--rw-r--r--   0        0        0     8826 2023-03-04 08:55:07.149847 pypdf-3.7.0/pypdf/generic/_rectangle.py
--rw-r--r--   0        0        0     6405 2023-03-04 11:49:14.882511 pypdf-3.7.0/pypdf/generic/_utils.py
--rw-r--r--   0        0        0     6880 2023-03-04 08:55:07.153847 pypdf-3.7.0/pypdf/pagerange.py
--rw-r--r--   0        0        0     1369 2023-02-28 08:12:53.917178 pypdf-3.7.0/pypdf/papersizes.py
--rw-r--r--   0        0        0        0 2022-12-31 10:47:19.003493 pypdf-3.7.0/pypdf/py.typed
--rw-r--r--   0        0        0     2135 2023-03-26 14:07:37.386395 pypdf-3.7.0/pypdf/types.py
--rw-r--r--   0        0        0    17879 2023-03-26 14:07:37.386395 pypdf-3.7.0/pypdf/xmp.py
--rw-r--r--   0        0        0     7370 2023-03-26 14:07:37.386395 pypdf-3.7.0/pyproject.toml
--rw-r--r--   0        0        0     1585 2023-02-05 10:26:02.030123 pypdf-3.7.0/setup.cfg
--rw-r--r--   0        0        0     6863 1970-01-01 00:00:00.000000 pypdf-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0      488 2022-12-10 23:30:58.176669 pypdf-3.7.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      542 2023-03-29 15:43:03.262713 pypdf-3.7.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    34734 2023-04-09 20:24:43.743420 pypdf-3.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3377 2023-03-19 10:45:11.184383 pypdf-3.7.1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     1605 2022-12-10 23:30:58.184669 pypdf-3.7.1/LICENSE
+-rw-r--r--   0        0        0       34 2022-12-10 23:30:58.184669 pypdf-3.7.1/MANIFEST.in
+-rw-r--r--   0        0        0     4729 2023-04-09 16:59:02.663368 pypdf-3.7.1/README.md
+-rw-r--r--   0        0        0     1234 2023-03-04 08:55:07.145847 pypdf-3.7.1/pypdf/__init__.py
+-rw-r--r--   0        0        0    14870 2023-03-18 15:07:48.665105 pypdf-3.7.1/pypdf/_cmap.py
+-rw-r--r--   0        0        0     1674 2023-02-28 08:12:53.909178 pypdf-3.7.1/pypdf/_codecs/__init__.py
+-rw-r--r--   0        0        0   431492 2022-12-31 10:47:18.999493 pypdf-3.7.1/pypdf/_codecs/adobe_glyphs.py
+-rw-r--r--   0        0        0     4269 2022-12-31 10:47:18.999493 pypdf-3.7.1/pypdf/_codecs/pdfdoc.py
+-rw-r--r--   0        0        0     2630 2023-02-28 08:12:53.909178 pypdf-3.7.1/pypdf/_codecs/std.py
+-rw-r--r--   0        0        0     3734 2022-12-31 10:47:18.999493 pypdf-3.7.1/pypdf/_codecs/symbol.py
+-rw-r--r--   0        0        0     3742 2022-12-31 10:47:18.999493 pypdf-3.7.1/pypdf/_codecs/zapfding.py
+-rw-r--r--   0        0        0    45635 2023-03-31 16:21:44.806544 pypdf-3.7.1/pypdf/_encryption.py
+-rw-r--r--   0        0        0    30650 2023-03-04 11:49:14.882511 pypdf-3.7.1/pypdf/_merger.py
+-rw-r--r--   0        0        0    82250 2023-03-31 15:39:30.774654 pypdf-3.7.1/pypdf/_page.py
+-rw-r--r--   0        0        0     7186 2023-03-04 08:55:07.145847 pypdf-3.7.1/pypdf/_page_labels.py
+-rw-r--r--   0        0        0     1920 2023-04-08 20:27:58.305582 pypdf-3.7.1/pypdf/_protocols.py
+-rw-r--r--   0        0        0    86026 2023-04-09 16:59:02.667368 pypdf-3.7.1/pypdf/_reader.py
+-rw-r--r--   0        0        0    12788 2023-03-31 16:21:44.806544 pypdf-3.7.1/pypdf/_security.py
+-rw-r--r--   0        0        0    10008 2023-03-12 09:43:33.014879 pypdf-3.7.1/pypdf/_text_extraction/__init__.py
+-rw-r--r--   0        0        0    14915 2023-04-08 20:27:58.305582 pypdf-3.7.1/pypdf/_utils.py
+-rw-r--r--   0        0        0       22 2023-04-09 20:22:59.891064 pypdf-3.7.1/pypdf/_version.py
+-rw-r--r--   0        0        0   122863 2023-04-08 20:27:58.309582 pypdf-3.7.1/pypdf/_writer.py
+-rw-r--r--   0        0        0    16147 2023-04-09 16:59:02.667368 pypdf-3.7.1/pypdf/constants.py
+-rw-r--r--   0        0        0     1631 2023-03-04 08:55:07.149847 pypdf-3.7.1/pypdf/errors.py
+-rw-r--r--   0        0        0    25921 2023-04-09 16:59:02.667368 pypdf-3.7.1/pypdf/filters.py
+-rw-r--r--   0        0        0     4549 2023-04-09 16:59:02.667368 pypdf-3.7.1/pypdf/generic/__init__.py
+-rw-r--r--   0        0        0    17368 2023-04-08 20:27:58.309582 pypdf-3.7.1/pypdf/generic/_annotations.py
+-rw-r--r--   0        0        0    24854 2023-04-08 20:27:58.309582 pypdf-3.7.1/pypdf/generic/_base.py
+-rw-r--r--   0        0        0    54781 2023-04-08 20:27:58.309582 pypdf-3.7.1/pypdf/generic/_data_structures.py
+-rw-r--r--   0        0        0     5427 2023-03-04 08:55:07.149847 pypdf-3.7.1/pypdf/generic/_fit.py
+-rw-r--r--   0        0        0     1195 2023-02-28 08:19:03.524706 pypdf-3.7.1/pypdf/generic/_outline.py
+-rw-r--r--   0        0        0     8826 2023-03-04 08:55:07.149847 pypdf-3.7.1/pypdf/generic/_rectangle.py
+-rw-r--r--   0        0        0     6405 2023-03-04 11:49:14.882511 pypdf-3.7.1/pypdf/generic/_utils.py
+-rw-r--r--   0        0        0     6880 2023-03-04 08:55:07.153847 pypdf-3.7.1/pypdf/pagerange.py
+-rw-r--r--   0        0        0     1369 2023-02-28 08:12:53.917178 pypdf-3.7.1/pypdf/papersizes.py
+-rw-r--r--   0        0        0        0 2022-12-31 10:47:19.003493 pypdf-3.7.1/pypdf/py.typed
+-rw-r--r--   0        0        0     2135 2023-03-29 15:43:03.266713 pypdf-3.7.1/pypdf/types.py
+-rw-r--r--   0        0        0    17879 2023-03-29 15:43:03.266713 pypdf-3.7.1/pypdf/xmp.py
+-rw-r--r--   0        0        0     7326 2023-04-09 16:59:02.667368 pypdf-3.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1585 2023-02-05 10:26:02.030123 pypdf-3.7.1/setup.cfg
+-rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 pypdf-3.7.1/PKG-INFO
```

### Comparing `pypdf-3.7.0/CHANGELOG.md` & `pypdf-3.7.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # CHANGELOG
 
+## Version 3.7.1, 2023-04-09
+
+### Security (SEC)
+-  Warn about PDF encryption security (#1755)
+
+### Robustness (ROB)
+-  Prevent loop in Cloning (#1770)
+-  Capture UnicodeDecodeError at PdfReader.pdf_header (#1768)
+
+### Documentation (DOC)
+-  Add .readthedocs.yaml and bump docs dependencies using `tox -e deps` (#1750, #1752)
+
+### Developer Experience (DEV)
+-  Make make_changelog.py idempotent
+
+### Maintenance (MAINT)
+-  Move generation of file identifiers to a method (#1760)
+
+### Testing (TST)
+-  Add xmp test (#1775)
+
+[Full Changelog](https://github.com/py-pdf/pypdf/compare/3.7.0...3.7.1)
+
 ## Version 3.7.0, 2023-03-26
 
 ### Security (SEC)
 -  Use Python's secrets module instead of random module (#1748)
 
 ### New Features (ENH)
 -  Add AnnotationBuilder.highlight text markup annotation (#1740)
```

### Comparing `pypdf-3.7.0/CONTRIBUTORS.md` & `pypdf-3.7.1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/LICENSE` & `pypdf-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/README.md` & `pypdf-3.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,57 +17,55 @@
 and
 [metadata](https://pypdf.readthedocs.io/en/stable/user/metadata.html)
 from PDFs as well.
 
 
 ## Installation
 
-You can install pypdf via pip:
+Install pypdf using pip:
 
 ```
 pip install pypdf
 ```
 
-If you plan to use pypdf for encrypting or decrypting PDFs that use AES, you
-will need to install some extra dependencies. Encryption using RC4 is supported
-using the regular installation.
+For using pypdf with AES encryption or decryption, install extra dependencies:
 
 ```
 pip install pypdf[crypto]
 ```
 
-> **NOTE**: `pypdf>=3.1.0` improved a lot compared to `pyPdf<2.0.0` and compared to
-> `PyPDF2 < 2.0.0`. Please
-> read [the migration guide](https://pypdf.readthedocs.io/en/latest/user/migration-1-to-2.html).
+> **NOTE**: `pypdf` 3.1.0 and above include significant improvements compared to
+> previous versions. Please refer to [the migration
+> guide](https://pypdf.readthedocs.io/en/latest/user/migration-1-to-2.html) for
+> more information.
 
 ## Usage
 
 ```python
 from pypdf import PdfReader
 
 reader = PdfReader("example.pdf")
 number_of_pages = len(reader.pages)
 page = reader.pages[0]
 text = page.extract_text()
 ```
 
 pypdf can do a lot more, e.g. splitting, merging, reading and creating
-annotations, decrypting and encrypting, and more.
-
-Please see [the documentation](https://pypdf.readthedocs.io/en/stable/)
-for more usage examples!
-
-A lot of questions are asked and answered
-[on StackOverflow](https://stackoverflow.com/questions/tagged/pypdf)
-(formerly tagged with [PyPDF2](https://stackoverflow.com/questions/tagged/pypdf2)).
+annotations, decrypting and encrypting, and more. Check out [the
+documentation](https://pypdf.readthedocs.io/en/stable/) for additional usage
+examples!
+
+For questions and answers, visit
+[StackOverflow](https://stackoverflow.com/questions/tagged/pypdf)
+(tagged with [pypdf](https://stackoverflow.com/questions/tagged/pypdf)).
 
 ## Contributions
 
-Maintaining pypdf is a collaborative effort. You can support pypdf by writing
-documentation, helping to narrow down issues, and adding code.
+Maintaining pypdf is a collaborative effort. You can support the project by
+writing documentation, helping to narrow down issues, and submitting code.
 
 ### Q&A
 
 The experience pypdf users have covers the whole range from beginners who
 want to make their live easier to experts who developed software before PDF
 existed. You can contribute to the pypdf community by answering questions
 on [StackOverflow](https://stackoverflow.com/questions/tagged/pypdf),
```

### Comparing `pypdf-3.7.0/pypdf/__init__.py` & `pypdf-3.7.1/pypdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_cmap.py` & `pypdf-3.7.1/pypdf/_cmap.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_codecs/__init__.py` & `pypdf-3.7.1/pypdf/_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_codecs/adobe_glyphs.py` & `pypdf-3.7.1/pypdf/_codecs/adobe_glyphs.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_codecs/pdfdoc.py` & `pypdf-3.7.1/pypdf/_codecs/pdfdoc.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_codecs/std.py` & `pypdf-3.7.1/pypdf/_codecs/std.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_codecs/symbol.py` & `pypdf-3.7.1/pypdf/_codecs/symbol.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_codecs/zapfding.py` & `pypdf-3.7.1/pypdf/_codecs/zapfding.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_encryption.py` & `pypdf-3.7.1/pypdf/_encryption.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_merger.py` & `pypdf-3.7.1/pypdf/_merger.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_page.py` & `pypdf-3.7.1/pypdf/_page.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_page_labels.py` & `pypdf-3.7.1/pypdf/_page_labels.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_protocols.py` & `pypdf-3.7.1/pypdf/_protocols.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 
     def get_object(self, indirect_reference: Any) -> Optional[PdfObjectProtocol]:
         ...
 
     def write(self, stream: Union[Path, StrByteType]) -> Tuple[bool, IO]:
         ...
 
+    def _add_object(self, obj: Any) -> Any:
+        ...
+
     @property
     def pages(self) -> List[Any]:
         ...
 
     @property
     def pdf_header(self) -> bytes:
         ...
```

### Comparing `pypdf-3.7.0/pypdf/_reader.py` & `pypdf-3.7.1/pypdf/_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import re
 import struct
 import zlib
 from datetime import datetime
-from io import BytesIO
+from io import BytesIO, UnsupportedOperation
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     Iterator,
@@ -356,15 +356,15 @@
         This is typically something like ``'%PDF-1.6'`` and can be used to
         detect if the file is actually a PDF file and which version it is.
         """
         # TODO: Make this return a bytes object for consistency
         #       but that needs a deprecation
         loc = self.stream.tell()
         self.stream.seek(0, 0)
-        pdf_file_version = self.stream.read(8).decode("utf-8")
+        pdf_file_version = self.stream.read(8).decode("utf-8", "backslashreplace")
         self.stream.seek(loc, 0)  # return to where it was
         return pdf_file_version
 
     @property
     def metadata(self) -> Optional[DocumentInformation]:
         """
         Retrieve the PDF file's document information dictionary, if it exists.
@@ -1269,16 +1269,16 @@
     def _get_indirect_object(self, num: int, gen: int) -> Optional[PdfObject]:
         """
         Used to ease development.
 
         This is equivalent to generic.IndirectObject(num,gen,self).get_object()
 
         Args:
-            num:
-            gen:
+            num: The object number of the indirect object.
+            gen: The generation number of the indirect object.
 
         Returns:
             A PdfObject
         """
         return IndirectObject(num, gen, self).get_object()
 
     def get_object(
@@ -1537,41 +1537,47 @@
                         del self.xref[gen][id]
                     # if not, then either it's just plain wrong, or the
                     # non-zero-index is actually correct
             stream.seek(loc, 0)  # return to where it was
 
     def _basic_validation(self, stream: StreamType) -> None:
         """Ensure file is not empty. Read at most 5 bytes."""
-        # start at the end:
-        stream.seek(0, os.SEEK_END)
-        if not stream.tell():
-            raise EmptyFileError("Cannot read an empty file")
-        if self.strict:
-            stream.seek(0, os.SEEK_SET)
+        stream.seek(0, os.SEEK_SET)
+        try:
             header_byte = stream.read(5)
-            if header_byte != b"%PDF-":
+        except UnicodeDecodeError:
+            raise UnsupportedOperation("cannot read header")
+        if header_byte == b"":
+            raise EmptyFileError("Cannot read an empty file")
+        elif header_byte != b"%PDF-":
+            if self.strict:
                 raise PdfReadError(
                     f"PDF starts with '{header_byte.decode('utf8')}', "
                     "but '%PDF-' expected"
                 )
-            stream.seek(0, os.SEEK_END)
+            else:
+                logger_warning(f"invalid pdf header: {header_byte}", __name__)
+        stream.seek(0, os.SEEK_END)
 
     def _find_eof_marker(self, stream: StreamType) -> None:
         """
         Jump to the %%EOF marker.
 
         According to the specs, the %%EOF marker should be at the very end of
         the file. Hence for standard-compliant PDF documents this function will
         read only the last part (DEFAULT_BUFFER_SIZE).
         """
         HEADER_SIZE = 8  # to parse whole file, Header is e.g. '%PDF-1.6'
         line = b""
         while line[:5] != b"%%EOF":
             if stream.tell() < HEADER_SIZE:
-                raise PdfReadError("EOF marker not found")
+                if self.strict:
+                    raise PdfReadError("EOF marker not found")
+                else:
+                    logger_warning("EOF marker not found", __name__)
             line = read_previous_line(stream)
 
     def _find_startxref_pos(self, stream: StreamType) -> int:
         """
         Find startxref entry - the location of the xref table.
 
         Args:
```

### Comparing `pypdf-3.7.0/pypdf/_security.py` & `pypdf-3.7.1/pypdf/_security.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_text_extraction/__init__.py` & `pypdf-3.7.1/pypdf/_text_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_utils.py` & `pypdf-3.7.1/pypdf/_utils.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/_writer.py` & `pypdf-3.7.1/pypdf/_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,18 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import codecs
 import collections
 import decimal
 import enum
+import hashlib
 import logging
 import re
-import secrets
 import struct
-import time
 import uuid
 import warnings
 from hashlib import md5
 from io import BytesIO, FileIO, IOBase
 from pathlib import Path
 from types import TracebackType
 from typing import (
@@ -140,14 +139,21 @@
     IMAGES = enum.auto()
     LINKS = enum.auto()
     ATTACHMENTS = enum.auto()
     OBJECTS_3D = enum.auto()
     ALL_ANNOTATIONS = enum.auto()
 
 
+def _rolling_checksum(stream: BytesIO, blocksize: int = 65536) -> str:
+    hash = hashlib.md5()
+    for block in iter(lambda: stream.read(blocksize), b""):
+        hash.update(block)
+    return hash.hexdigest()
+
+
 class PdfWriter:
     """
     Write a PDF file out, given pages produced by another class.
 
     Typically data is added from a :class:`PdfReader<pypdf.PdfReader>`.
     """
 
@@ -970,15 +976,15 @@
                 (delegates to append_pages_from_reader). The single parameter of
                 the callback is a reference to the page just appended to the
                 document.
         """
         self.clone_reader_document_root(reader)
         self._info = reader.trailer[TK.INFO].clone(self).indirect_reference  # type: ignore
         try:
-            self._ID = reader.trailer[TK.ID].clone(self)  # type: ignore
+            self._ID = cast(ArrayObject, reader.trailer[TK.ID].clone(self))  # type: ignore
         except KeyError:
             pass
         if callable(after_page_append):
             for page in cast(
                 ArrayObject, cast(DictionaryObject, self._pages.get_object())["/Kids"]
             ):
                 after_page_append(page.get_object())
@@ -994,14 +1000,34 @@
         .. deprecated:: 1.28.0
         """
         deprecation_with_replacement(
             "cloneDocumentFromReader", "clone_document_from_reader", "3.0.0"
         )
         self.clone_document_from_reader(reader, after_page_append)
 
+    def _compute_document_identifier_from_content(self) -> ByteStringObject:
+        stream = BytesIO()
+        self._write_pdf_structure(stream)
+        stream.seek(0)
+        return ByteStringObject(_rolling_checksum(stream).encode("utf8"))
+
+    def generate_file_identifiers(self) -> None:
+        """
+        Generate an identifier for the PDF that will be written.
+
+        The only point of this is ensuring uniqueness. Reproducibility is not
+        required; see 14.4 "File Identifiers".
+        """
+        if hasattr(self, "_ID") and self._ID and len(self._ID) == 2:
+            ID_1 = self._ID[0]
+        else:
+            ID_1 = self._compute_document_identifier_from_content()
+        ID_2 = self._compute_document_identifier_from_content()
+        self._ID = ArrayObject((ID_1, ID_2))
+
     def encrypt(
         self,
         user_password: Optional[str] = None,
         owner_password: Optional[str] = None,
         use_128bit: bool = True,
         permissions_flag: UserAccessPermissions = ALL_DOCUMENT_PERMISSIONS,
         user_pwd: Optional[str] = None,  # deprecated
@@ -1023,14 +1049,20 @@
                 TABLE 3.20 of the PDF 1.7 specification. A bit value of 1 means
                 the permission is grantend.
                 Hence an integer value of -1 will set all flags.
                 Bit position 3 is for printing, 4 is for modifying content,
                 5 and 6 control annotations, 9 for form fields,
                 10 for extraction of text and graphics.
         """
+        warnings.warn(
+            "pypdf only implements RC4 encryption so far. "
+            "The RC4 algorithm is insecure. Either use a library that supports "
+            "AES for encryption or put the PDF in an encrypted container, "
+            "for example an encrypted ZIP file."
+        )
         if user_pwd is not None:
             if user_password is not None:
                 raise ValueError(
                     "Please only set 'user_password'. "
                     "The 'user_pwd' argument is deprecated."
                 )
             else:
@@ -1068,27 +1100,22 @@
             V = 2
             rev = 3
             keylen = int(128 / 8)
         else:
             V = 1
             rev = 2
             keylen = int(40 / 8)
-        secrets_generator = secrets.SystemRandom()
         P = permissions_flag
         O = ByteStringObject(_alg33(owner_password, user_password, rev, keylen))  # type: ignore[arg-type]  # noqa
-        ID_1 = ByteStringObject(md5((repr(time.time())).encode("utf8")).digest())
-        ID_2 = ByteStringObject(
-            md5((repr(secrets_generator.uniform(0, 1))).encode("utf8")).digest()
-        )
-        self._ID = ArrayObject((ID_1, ID_2))
+        self.generate_file_identifiers()
         if rev == 2:
-            U, key = _alg34(user_password, O, P, ID_1)
+            U, key = _alg34(user_password, O, P, self._ID[0])
         else:
             assert rev == 3
-            U, key = _alg35(user_password, rev, keylen, O, P, ID_1, False)  # type: ignore[arg-type]
+            U, key = _alg35(user_password, rev, keylen, O, P, self._ID[0], False)  # type: ignore[arg-type]
         encrypt = DictionaryObject()
         encrypt[NameObject(SA.FILTER)] = NameObject("/Standard")
         encrypt[NameObject("/V")] = NumberObject(V)
         if V == 2:
             encrypt[NameObject(SA.LENGTH)] = NumberObject(keylen * 8)
         encrypt[NameObject(ED.R)] = NumberObject(rev)
         encrypt[NameObject(ED.O)] = ByteStringObject(O)
@@ -1114,15 +1141,15 @@
         # address this problem, PageObject's store their original object
         # reference number, and we add it to the external reference map before
         # we sweep for indirect references.  This forces self-page-referencing
         # trees to reference the correct new object location, rather than
         # copying in a new copy of the page object.
         self._sweep_indirect_references(self._root)
 
-        object_positions = self._write_header(stream)
+        object_positions = self._write_pdf_structure(stream)
         xref_location = self._write_xref_table(stream, object_positions)
         self._write_trailer(stream)
         stream.write(b_(f"\nstartxref\n{xref_location}\n%%EOF\n"))  # eof
 
     def write(self, stream: Union[Path, StrByteType]) -> Tuple[bool, IO]:
         """
         Write the collection of pages added to this object out as a PDF file.
@@ -1149,15 +1176,15 @@
         self.write_stream(stream)
 
         if self.with_as_usage:
             stream.close()
 
         return my_file, stream
 
-    def _write_header(self, stream: StreamType) -> List[int]:
+    def _write_pdf_structure(self, stream: StreamType) -> List[int]:
         object_positions = []
         stream.write(self.pdf_header + b"\n")
         stream.write(b"%\xE2\xE3\xCF\xD3\n")
         for i, obj in enumerate(self._objects):
             obj = self._objects[i]
             # If the obj is None we can't write anything
             if obj is not None:
```

### Comparing `pypdf-3.7.0/pypdf/constants.py` & `pypdf-3.7.1/pypdf/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -302,14 +302,25 @@
     Ff = "/Ff"  # integer, optional
     V = "/V"  # text string, optional
     DV = "/DV"  # text string, optional
     AA = "/AA"  # dictionary, optional
 
     @classmethod
     def attributes(cls) -> Tuple[str, ...]:
+        """
+        Get a tuple of all the attributes present in a Field Dictionary.
+
+        This method returns a tuple of all the attribute constants defined in
+        the FieldDictionaryAttributes class. These attributes correspond to the
+        entries that are common to all field dictionaries as specified in the
+        PDF 1.7 reference.
+
+        Returns:
+            A tuple containing all the attribute constants.
+        """
         return (
             cls.TM,
             cls.T,
             cls.FT,
             cls.Parent,
             cls.TU,
             cls.Ff,
@@ -317,14 +328,26 @@
             cls.DV,
             cls.Kids,
             cls.AA,
         )
 
     @classmethod
     def attributes_dict(cls) -> Dict[str, str]:
+        """
+        Get a dictionary of attribute keys and their human-readable names.
+
+        This method returns a dictionary where the keys are the attribute
+        constants defined in the FieldDictionaryAttributes class and the values
+        are their corresponding human-readable names. These attributes
+        correspond to the entries that are common to all field dictionaries as
+        specified in the PDF 1.7 reference.
+
+        Returns:
+            A dictionary containing attribute keys and their names.
+        """
         return {
             cls.FT: "Field Type",
             cls.Parent: "Parent",
             cls.T: "Field Name",
             cls.TU: "Alternate Field Name",
             cls.TM: "Mapping Name",
             cls.Ff: "Field Flags",
@@ -336,18 +359,41 @@
 class CheckboxRadioButtonAttributes:
     """TABLE 8.76 Field flags common to all field types."""
 
     Opt = "/Opt"  # Options, Optional
 
     @classmethod
     def attributes(cls) -> Tuple[str, ...]:
+        """
+        Get a tuple of all the attributes present in a Field Dictionary.
+
+        This method returns a tuple of all the attribute constants defined in
+        the CheckboxRadioButtonAttributes class. These attributes correspond to
+        the entries that are common to all field dictionaries as specified in
+        the PDF 1.7 reference.
+
+        Returns:
+            A tuple containing all the attribute constants.
+        """
         return (cls.Opt,)
 
     @classmethod
     def attributes_dict(cls) -> Dict[str, str]:
+        """
+        Get a dictionary of attribute keys and their human-readable names.
+
+        This method returns a dictionary where the keys are the attribute
+        constants defined in the CheckboxRadioButtonAttributes class and the
+        values are their corresponding human-readable names. These attributes
+        correspond to the entries that are common to all field dictionaries as
+        specified in the PDF 1.7 reference.
+
+        Returns:
+            A dictionary containing attribute keys and their names.
+        """
         return {
             cls.Opt: "Options",
         }
 
 
 class FieldFlag(IntFlag):
     """TABLE 8.70 Field flags common to all field types."""
@@ -377,21 +423,43 @@
     SINGLE_PAGE = "/SinglePage"
     ONE_COLUMN = "/OneColumn"
     TWO_COLUMN_LEFT = "/TwoColumnLeft"
     TWO_COLUMN_RIGHT = "/TwoColumnRight"
 
 
 class GraphicsStateParameters:
-    """Table 4.8 of the 1.7 reference."""
+    """Table 58 – Entries in a Graphics State Parameter Dictionary"""
 
     TYPE = "/Type"  # name, optional
     LW = "/LW"  # number, optional
-    # TODO: Many more!
+    LC = "/LC"  # integer, optional
+    LJ = "/LJ"  # integer, optional
+    ML = "/ML"  # number, optional
+    D = "/D"  # array, optional
+    RI = "/RI"  # name, optional
+    OP = "/OP"
+    op = "/op"
+    OPM = "/OPM"
     FONT = "/Font"  # array, optional
+    BG = "/BG"
+    BG2 = "/BG2"
+    UCR = "/UCR"
+    UCR2 = "/UCR2"
+    TR = "/TR"
+    TR2 = "/TR2"
+    HT = "/HT"
+    FL = "/FL"
+    SM = "/SM"
+    SA = "/SA"
+    BM = "/BM"
     S_MASK = "/SMask"  # dictionary or name, optional
+    CA = "/CA"
+    ca = "/ca"
+    AIS = "/AIS"
+    TK = "/TK"
 
 
 class CatalogDictionary:
     """Table 3.25 in the 1.7 reference."""
 
     TYPE = "/Type"  # name, required; must be /Catalog
     VERSION = "/Version"  # name
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypdf-3.7.0/pypdf/errors.py` & `pypdf-3.7.1/pypdf/errors.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/filters.py` & `pypdf-3.7.1/pypdf/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,27 @@
     except ImportError:
         # PEP 586 introduced typing.Literal with Python 3.8
         # For older Python versions, the backport typing_extensions is necessary:
         from typing_extensions import Literal  # type: ignore[misc, assignment]
 
 
 def decompress(data: bytes) -> bytes:
+    """
+    Decompress the given data using zlib.
+
+    This function attempts to decompress the input data using zlib. If the
+    decompression fails due to a zlib error, it falls back to using a
+    decompression object with a larger window size.
+
+    Args:
+        data: The input data to be decompressed.
+
+    Returns:
+        The decompressed data.
+    """
     try:
         return zlib.decompress(data)
     except zlib.error:
         d = zlib.decompressobj(zlib.MAX_WBITS | 32)
         result_str = b""
         for b in [data[i : i + 1] for i in range(len(data))]:
             try:
@@ -191,14 +204,23 @@
                 raise PdfReadError(f"Unsupported PNG filter {filter_byte!r}")
             prev_rowdata = tuple(rowdata)
             output.write(bytearray(rowdata[1:]))
         return output.getvalue()
 
     @staticmethod
     def encode(data: bytes) -> bytes:
+        """
+        Compress the input data using zlib.
+
+        Args:
+            data: The data to be compressed.
+
+        Returns:
+            The compressed data.
+        """
         return zlib.compress(data)
 
 
 class ASCIIHexDecode:
     """
     The ASCIIHexDecode filter decodes data that has been encoded in ASCII
     hexadecimal form into a base-7 ASCII format.
@@ -372,15 +394,15 @@
             deprecate_with_replacement("decodeParms", "parameters", "4.0.0")
             decode_parms = kwargs["decodeParms"]  # noqa: F841
         if isinstance(data, str):
             data = data.encode("ascii")
         group_index = b = 0
         out = bytearray()
         for char in data:
-            if ord("!") <= char and char <= ord("u"):
+            if ord("!") <= char <= ord("u"):
                 group_index += 1
                 b = b * 85 + (char - 33)
                 if group_index == 5:
                     out += struct.pack(b">L", b)
                     group_index = b = 0
             elif char == ord("z"):
                 assert group_index == 0
@@ -532,14 +554,31 @@
             0,  # last IFD
         )
 
         return tiff_header + data
 
 
 def decode_stream_data(stream: Any) -> Union[str, bytes]:  # utils.StreamObject
+    """
+    Decode the stream data based on the specified filters.
+
+    This function decodes the stream data using the filters provided in the
+    stream. It supports various filter types, including FlateDecode,
+    ASCIIHexDecode, LZWDecode, ASCII85Decode, DCTDecode, JPXDecode, and
+    CCITTFaxDecode.
+
+    Args:
+        stream: The input stream object containing the data and filters.
+
+    Returns:
+        The decoded stream data.
+
+    Raises:
+        NotImplementedError: If an unsupported filter type is encountered.
+    """
     filters = stream.get(SA.FILTER, ())
     if isinstance(filters, IndirectObject):
         filters = cast(ArrayObject, filters.get_object())
     if not isinstance(filters, ArrayObject):
         # we have a single filter instance
         filters = (filters,)
     decodparms = stream.get(SA.DECODE_PARMS, ({},) * len(filters))
@@ -576,14 +615,15 @@
             else:
                 # Unsupported filter
                 raise NotImplementedError(f"unsupported filter {filter_type}")
     return data
 
 
 def decodeStreamData(stream: Any) -> Union[str, bytes]:  # deprecated
+    """Deprecated. Use decode_stream_data."""
     deprecate_with_replacement("decodeStreamData", "decode_stream_data", "4.0.0")
     return decode_stream_data(stream)
 
 
 def _xobj_to_image(x_object_obj: Dict[str, Any]) -> Tuple[Optional[str], bytes]:
     """
     Users need to have the pillow package installed.
```

### Comparing `pypdf-3.7.0/pypdf/generic/__init__.py` & `pypdf-3.7.1/pypdf/generic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,34 +69,37 @@
     read_string_from_stream,
 )
 
 
 def readHexStringFromStream(
     stream: StreamType,
 ) -> Union["TextStringObject", "ByteStringObject"]:  # deprecated
+    """Deprecated, use read_hex_string_from_stream."""
     deprecate_with_replacement(
         "readHexStringFromStream", "read_hex_string_from_stream", "4.0.0"
     )
     return read_hex_string_from_stream(stream)
 
 
 def readStringFromStream(
     stream: StreamType,
     forced_encoding: Union[None, str, List[str], Dict[int, str]] = None,
 ) -> Union["TextStringObject", "ByteStringObject"]:  # deprecated
+    """Deprecated, use read_string_from_stream."""
     deprecate_with_replacement(
         "readStringFromStream", "read_string_from_stream", "4.0.0"
     )
     return read_string_from_stream(stream, forced_encoding)
 
 
 def createStringObject(
     string: Union[str, bytes],
     forced_encoding: Union[None, str, List[str], Dict[int, str]] = None,
 ) -> Union[TextStringObject, ByteStringObject]:  # deprecated
+    """Deprecated, use create_string_object."""
     deprecate_with_replacement("createStringObject", "create_string_object", "4.0.0")
     return create_string_object(string, forced_encoding)
 
 
 PAGE_FIT = Fit.fit()
```

### Comparing `pypdf-3.7.0/pypdf/generic/_annotations.py` & `pypdf-3.7.1/pypdf/generic/_annotations.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/generic/_base.py` & `pypdf-3.7.1/pypdf/generic/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,18 @@
             obj = self.get_object()
             # case observed : a pointed object can not be found
             if obj is None:
                 # this normally
                 obj = NullObject()
                 assert isinstance(self, (IndirectObject,))
                 obj.indirect_reference = self
-            dup = obj.clone(pdf_dest, force_duplicate, ignore_fields)
+            dup = pdf_dest._add_object(
+                obj.clone(pdf_dest, force_duplicate, ignore_fields)
+            )
+        # asserts added to prevent errors in mypy
         assert dup is not None
         assert dup.indirect_reference is not None
         return dup.indirect_reference
 
     @property
     def indirect_reference(self) -> "IndirectObject":  # type: ignore[override]
         return self
```

### Comparing `pypdf-3.7.0/pypdf/generic/_data_structures.py` & `pypdf-3.7.1/pypdf/generic/_data_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -746,15 +746,18 @@
         """
         self._data = cast("StreamObject", src)._data
         try:
             decoded_self = cast("StreamObject", src).decoded_self
             if decoded_self is None:
                 self.decoded_self = None
             else:
-                self.decoded_self = decoded_self.clone(pdf_dest, True, ignore_fields)  # type: ignore[assignment]
+                self.decoded_self = cast(
+                    "DecodedStreamObject",
+                    decoded_self.clone(pdf_dest, force_duplicate, ignore_fields),
+                )
         except Exception:
             pass
         super()._clone(src, pdf_dest, force_duplicate, ignore_fields)
 
     def hash_value_data(self) -> bytes:
         data = super().hash_value_data()
         data += b_(self._data)
```

### Comparing `pypdf-3.7.0/pypdf/generic/_fit.py` & `pypdf-3.7.1/pypdf/generic/_fit.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/generic/_outline.py` & `pypdf-3.7.1/pypdf/generic/_outline.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/generic/_rectangle.py` & `pypdf-3.7.1/pypdf/generic/_rectangle.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/generic/_utils.py` & `pypdf-3.7.1/pypdf/generic/_utils.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/pagerange.py` & `pypdf-3.7.1/pypdf/pagerange.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/papersizes.py` & `pypdf-3.7.1/pypdf/papersizes.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/types.py` & `pypdf-3.7.1/pypdf/types.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pypdf/xmp.py` & `pypdf-3.7.1/pypdf/xmp.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/pyproject.toml` & `pypdf-3.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,14 @@
     "A",  # Variable is shadowing a built-in
     "B028",  # No explicit `stacklevel` keyword argument found
     "B904", # Within an `except` clause, raise exceptions with
     "B905",  # `zip()` without an explicit `strict=` parameter
     "C901",
     "D101",  # Missing docstring in public class
     "D102", # Missing docstring in public method
-    "D103",  # Missing docstring in public function
     "D417",  # Missing argument descriptions in the docstring
     "FBT001", # Boolean positional arg in function definition
     "FBT002", # Boolean default value in function definition
     "FBT003", # Boolean positional value in function call
     "PGH", # Use specific error messages
     "PLE",  # too many arguments for logging
     "PLR0911",  # Too many return statements
@@ -173,15 +172,15 @@
     "PT012",  # `pytest.raises()` block should contain a single simple statement
     "PTH123", # `open()` should be replaced by `Path.open()`
     "S101",  # Use of `assert` detected
     "SLF001",  # Private member accessed
 ]
 
 [tool.ruff.per-file-ignores]
-"tests/*" = ["S101", "ANN001", "ANN201","D104", "S105", "S106"]
+"tests/*" = ["S101", "ANN001", "ANN201","D104", "S105", "S106", "D103"]
 "sample-files/*" = ["D100", "INP001"]
 "_encryption.py" = ["S324", "S311"]
 "_security.py" = ["S324"]
 "_writer.py" = ["S324"]
 "make_changelog.py" = ["T201"]
 "json_consistency.py" = ["T201"]
 "tests/test_workflows.py" =  ["T201"]
```

### Comparing `pypdf-3.7.0/setup.cfg` & `pypdf-3.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.0/PKG-INFO` & `pypdf-3.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdf
-Version: 3.7.0
+Version: 3.7.1
 Summary: A pure-python PDF library capable of splitting, merging, cropping, and transforming PDF files
 Author-email: Mathieu Fenniak <biziqe@mathieu.fenniak.net>
 Maintainer-email: Martin Thoma <info@martin-thoma.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -63,57 +63,55 @@
 and
 [metadata](https://pypdf.readthedocs.io/en/stable/user/metadata.html)
 from PDFs as well.
 
 
 ## Installation
 
-You can install pypdf via pip:
+Install pypdf using pip:
 
 ```
 pip install pypdf
 ```
 
-If you plan to use pypdf for encrypting or decrypting PDFs that use AES, you
-will need to install some extra dependencies. Encryption using RC4 is supported
-using the regular installation.
+For using pypdf with AES encryption or decryption, install extra dependencies:
 
 ```
 pip install pypdf[crypto]
 ```
 
-> **NOTE**: `pypdf>=3.1.0` improved a lot compared to `pyPdf<2.0.0` and compared to
-> `PyPDF2 < 2.0.0`. Please
-> read [the migration guide](https://pypdf.readthedocs.io/en/latest/user/migration-1-to-2.html).
+> **NOTE**: `pypdf` 3.1.0 and above include significant improvements compared to
+> previous versions. Please refer to [the migration
+> guide](https://pypdf.readthedocs.io/en/latest/user/migration-1-to-2.html) for
+> more information.
 
 ## Usage
 
 ```python
 from pypdf import PdfReader
 
 reader = PdfReader("example.pdf")
 number_of_pages = len(reader.pages)
 page = reader.pages[0]
 text = page.extract_text()
 ```
 
 pypdf can do a lot more, e.g. splitting, merging, reading and creating
-annotations, decrypting and encrypting, and more.
-
-Please see [the documentation](https://pypdf.readthedocs.io/en/stable/)
-for more usage examples!
-
-A lot of questions are asked and answered
-[on StackOverflow](https://stackoverflow.com/questions/tagged/pypdf)
-(formerly tagged with [PyPDF2](https://stackoverflow.com/questions/tagged/pypdf2)).
+annotations, decrypting and encrypting, and more. Check out [the
+documentation](https://pypdf.readthedocs.io/en/stable/) for additional usage
+examples!
+
+For questions and answers, visit
+[StackOverflow](https://stackoverflow.com/questions/tagged/pypdf)
+(tagged with [pypdf](https://stackoverflow.com/questions/tagged/pypdf)).
 
 ## Contributions
 
-Maintaining pypdf is a collaborative effort. You can support pypdf by writing
-documentation, helping to narrow down issues, and adding code.
+Maintaining pypdf is a collaborative effort. You can support the project by
+writing documentation, helping to narrow down issues, and submitting code.
 
 ### Q&A
 
 The experience pypdf users have covers the whole range from beginners who
 want to make their live easier to experts who developed software before PDF
 existed. You can contribute to the pypdf community by answering questions
 on [StackOverflow](https://stackoverflow.com/questions/tagged/pypdf),
```

