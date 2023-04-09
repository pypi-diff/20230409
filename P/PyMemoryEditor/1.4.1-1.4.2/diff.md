# Comparing `tmp/PyMemoryEditor-1.4.1.tar.gz` & `tmp/PyMemoryEditor-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.4.1.tar", last modified: Sun Apr  9 17:20:19 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.4.2.tar", last modified: Sun Apr  9 19:49:45 2023, max compression
```

## Comparing `PyMemoryEditor-1.4.1.tar` & `PyMemoryEditor-1.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 17:20:19.038568 PyMemoryEditor-1.4.1/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     2976 2023-04-09 17:20:19.038568 PyMemoryEditor-1.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 17:20:19.007305 PyMemoryEditor-1.4.1/PyMemoryEditor/
--rw-rw-rw-   0        0        0      426 2023-04-09 17:00:46.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     3737 2023-04-09 17:20:10.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-09 17:20:19.038568 PyMemoryEditor-1.4.1/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 17:20:19.038568 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/
--rw-rw-rw-   0        0        0    13571 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/constants.py
--rw-rw-rw-   0        0        0    14385 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/enum.py
--rw-rw-rw-   0        0        0     4922 2023-04-09 17:20:10.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 17:20:19.022943 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     2976 2023-04-09 17:20:18.000000 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-04-09 17:20:18.000000 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 17:20:18.000000 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 17:20:18.000000 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 17:20:18.000000 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2025 2023-04-03 04:59:56.000000 PyMemoryEditor-1.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 17:20:19.038568 PyMemoryEditor-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:49:45.559958 PyMemoryEditor-1.4.2/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     2976 2023-04-09 19:49:45.559958 PyMemoryEditor-1.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 19:49:45.507680 PyMemoryEditor-1.4.2/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      426 2023-04-09 19:49:26.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     4750 2023-04-09 19:48:02.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:49:45.544357 PyMemoryEditor-1.4.2/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:49:45.559958 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/
+-rw-rw-rw-   0        0        0    13242 2023-04-09 18:49:26.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/constants.py
+-rw-rw-rw-   0        0        0     2671 2023-04-09 18:35:56.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/enum.py
+-rw-rw-rw-   0        0        0     6575 2023-04-09 19:43:23.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:49:45.544357 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     2976 2023-04-09 19:49:45.000000 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-04-09 19:49:45.000000 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 19:49:45.000000 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 19:49:45.000000 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 19:49:45.000000 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2025 2023-04-03 04:59:56.000000 PyMemoryEditor-1.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 19:49:45.559958 PyMemoryEditor-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.4.2/setup.py
```

### Comparing `PyMemoryEditor-1.4.1/LICENSE` & `PyMemoryEditor-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.1/PKG-INFO` & `PyMemoryEditor-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.1
+Version: 1.4.2
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `PyMemoryEditor-1.4.1/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.4.2/PyMemoryEditor/open_process.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # -*- coding: utf-8 -*-
 
 from .process import Process
 from .win32.enum import ProcessOperations
-from .win32.functions import CloseProcessHandle, GetProcessHandle, ReadProcessMemory, WriteProcessMemory
 
-from typing import Optional, Type, TypeVar, Union
+from .win32.functions import (
+    CloseProcessHandle,
+    GetProcessHandle,
+    ReadProcessMemory,
+    SearchAllMemory,
+    WriteProcessMemory
+)
+
+from typing import List, Optional, Type, TypeVar, Union
 
 
 T = TypeVar("T")
 
 
 class OpenProcess(object):
     """
@@ -58,14 +65,37 @@
 
     def close(self):
         """
         Close the process handle.
         """
         return CloseProcessHandle(self.__process_handle)
 
+    def search_by_value(
+        self,
+        pytype: Type[T],
+        bufflength: int,
+        value: Union[bool, int, float, str, bytes]
+    ) -> List[int]:
+        """
+        Search the whole memory space, accessible to the process,
+        for the provided value, returning the found addresses.
+
+        :param pytype: type of value to be queried (bool, int, float, str or bytes).
+        :param bufflength: value size in bytes (1, 2, 4, 8).
+        :param value: value to be queried (bool, int, float, str or bytes).
+        """
+        valid_permissions = [
+            ProcessOperations.PROCESS_ALL_ACCESS.value,
+            ProcessOperations.PROCESS_VM_READ.value
+        ]
+        if self.__permission.value not in valid_permissions:
+            raise PermissionError("The handle does not have permission to read the process memory.")
+
+        return list(SearchAllMemory(self.__process_handle, pytype, bufflength, value))
+
     def read_process_memory(
         self,
         address: int,
         pytype: Type[T],
         bufflength: int
     ) -> T:
         """
```

### Comparing `PyMemoryEditor-1.4.1/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.4.2/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.1/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.4.2/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.1/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.4.2/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.1/PyMemoryEditor/win32/constants.py` & `PyMemoryEditor-1.4.2/PyMemoryEditor/win32/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 
-# Allocates memory charges (from the overall size of memory and the paging files on disk) for the specified reserved
-# memory pages. The function also guarantees that when the caller later initially accesses the memory, the contents will
-# be zero. Actual physical pages are not allocated unless/until the virtual addresses are actually accessed. To reserve
-# and commit pages in one step, call VirtualAllocEx with MEM_COMMIT | MEM_RESERVE. Attempting to commit a specific
-# address range by specifying MEM_COMMIT without MEM_RESERVE and a non-NULL lpAddress fails unless the entire range has
-# already been reserved. The resulting error code is ERROR_INVALID_ADDRESS. An attempt to commit a page that is already
-# committed does not cause the function to fail. This means that you can commit pages without first determining the
-# current commitment state of each page.
-# If lpAddress specifies an address within an enclave, flAllocationType must be MEM_COMMIT.
+# Indicates committed pages for which physical storage has been allocated, either in memory or in the paging file on disk.
 MEM_COMMIT = 0x00001000
 
-# Reserves a range of the process's virtual address space without allocating any actual physical storage in memory or in
-# the paging file on disk. You commit reserved pages by calling VirtualAllocEx again with MEM_COMMIT. To reserve and
-# commit pages in one step, call VirtualAllocEx with MEM_COMMIT | MEM_RESERVE. Other memory allocation functions, such
-# as malloc and LocalAlloc, cannot use reserved memory until it has been released.
+# Indicates free pages not accessible to the calling process and available to be allocated. For free pages, the
+# information in the AllocationBase, AllocationProtect, Protect, and Type members is undefined.
+MEM_FREE = 0x00010000
+
+# Indicates that the memory pages within the region are mapped into the view of an image section.
+MEM_IMAGE = 0x01000000
+
+# Indicates that the memory pages within the region are mapped into the view of a section.
+MEM_MAPPED = 0x00040000
+
+# Indicates reserved pages where a range of the process's virtual address space is reserved without any physical storage
+# being allocated. For reserved pages, the information in the Protect member is undefined.
 MEM_RESERVE = 0x00002000
 
 # Indicates that data in the memory range specified by lpAddress and dwSize is no longer of interest. The pages should
 # not be read from or written to the paging file. However, the memory block will be used again later, so it should not be
 # decommitted. This value cannot be used with any other value. Using this value does not guarantee that the range operated
 # on with MEM_RESET will contain zeros. If you want the range to contain zeros, decommit the memory and then recommit it.
 # When you use MEM_RESET, the VirtualAllocEx function ignores the value of fProtect. However, you must still set fProtect
@@ -42,14 +42,17 @@
 # If you specify this value, you must also specify MEM_RESERVE and MEM_COMMIT.
 MEM_LARGE_PAGES = 0x20000000
 
 # Reserves an address range that can be used to map Address Windowing Extensions (AWE) pages. This value must be used
 # with MEM_RESERVE and no other values.
 MEM_PHYSICAL = 0x00400000
 
+# Indicates that the memory pages within the region are private (that is, not shared by other processes).
+MEM_PRIVATE = 0x00020000
+
 # Allocates memory at the highest possible address. This can be slower than regular allocations, especially when there
 # are many allocations.
 MEM_TOP_DOWN = 0x00100000
 
 # Enables execute access to the committed region of pages. An attempt to write to the committed
 # region results in an access violation. This flag is not supported by the CreateFileMapping function.
 PAGE_EXECUTE = 0x10
@@ -87,14 +90,17 @@
 # Enables read-only or copy-on-write access to a mapped view of a file mapping object. An attempt to write to a
 # committed copy-on-write page results in a private copy of the page being made for the process. The private page
 # is marked as PAGE_READWRITE, and the change is written to the new page. If Data Execution Prevention is enabled,
 # attempting to execute code in the committed region results in an access violation. This flag is not supported by
 # the VirtualAlloc or VirtualAllocEx functions.
 PAGE_WRITECOPY = 0x08
 
+# Indicates memory page is readble. (Custom constant)
+PAGE_READABLE = PAGE_EXECUTE_READ | PAGE_EXECUTE_READWRITE | PAGE_READWRITE
+
 # Sets all locations in the pages as invalid targets for CFG. Used along with any execute page protection like
 # PAGE_EXECUTE, PAGE_EXECUTE_READ, PAGE_EXECUTE_READWRITE and PAGE_EXECUTE_WRITECOPY. Any indirect call to locations
 # in those pages will fail CFG checks and the process will be terminated. The default behavior for executable pages
 # allocated is to be marked valid call targets for CFG. This flag is not supported by the VirtualProtect or
 # CreateFileMapping functions.
 PAGE_TARGETS_INVALID = 0x40000000
```

### Comparing `PyMemoryEditor-1.4.1/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.4.2/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.1/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.4.2/PyMemoryEditor/win32/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.1
+Version: 1.4.2
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/SOURCES.txt` & `PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.1/README.md` & `PyMemoryEditor-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.1/setup.py` & `PyMemoryEditor-1.4.2/setup.py`

 * *Files identical despite different names*

