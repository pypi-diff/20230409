# Comparing `tmp/PyMemoryEditor-1.4.0.tar.gz` & `tmp/PyMemoryEditor-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.4.0.tar", last modified: Sun Apr  9 04:38:51 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.4.1.tar", last modified: Sun Apr  9 17:20:19 2023, max compression
```

## Comparing `PyMemoryEditor-1.4.0.tar` & `PyMemoryEditor-1.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 04:38:51.644738 PyMemoryEditor-1.4.0/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     2976 2023-04-09 04:38:51.644738 PyMemoryEditor-1.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 04:38:51.631229 PyMemoryEditor-1.4.0/PyMemoryEditor/
--rw-rw-rw-   0        0        0      426 2023-04-09 03:26:04.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     3737 2023-04-09 03:43:03.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-09 04:38:51.644738 PyMemoryEditor-1.4.0/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 04:38:51.644738 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/
--rw-rw-rw-   0        0        0    13571 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/constants.py
--rw-rw-rw-   0        0        0    14385 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/enum.py
--rw-rw-rw-   0        0        0     4705 2023-04-09 03:42:05.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1795 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      928 2023-04-09 03:40:32.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 04:38:51.631229 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     2976 2023-04-09 04:38:51.000000 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-04-09 04:38:51.000000 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 04:38:51.000000 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 04:38:51.000000 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 04:38:51.000000 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2025 2023-04-03 04:59:56.000000 PyMemoryEditor-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 04:38:51.644738 PyMemoryEditor-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:20:19.038568 PyMemoryEditor-1.4.1/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     2976 2023-04-09 17:20:19.038568 PyMemoryEditor-1.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 17:20:19.007305 PyMemoryEditor-1.4.1/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      426 2023-04-09 17:00:46.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     3737 2023-04-09 17:20:10.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:20:19.038568 PyMemoryEditor-1.4.1/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:20:19.038568 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/
+-rw-rw-rw-   0        0        0    13571 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/constants.py
+-rw-rw-rw-   0        0        0    14385 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/enum.py
+-rw-rw-rw-   0        0        0     4922 2023-04-09 17:20:10.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.1/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:20:19.022943 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     2976 2023-04-09 17:20:18.000000 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-04-09 17:20:18.000000 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 17:20:18.000000 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 17:20:18.000000 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 17:20:18.000000 PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2025 2023-04-03 04:59:56.000000 PyMemoryEditor-1.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 17:20:19.038568 PyMemoryEditor-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.4.1/setup.py
```

### Comparing `PyMemoryEditor-1.4.0/LICENSE` & `PyMemoryEditor-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.0/PKG-INFO` & `PyMemoryEditor-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.0
+Version: 1.4.1
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.4.1/PyMemoryEditor/open_process.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.4.1/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.4.1/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.4.1/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor/win32/constants.py` & `PyMemoryEditor-1.4.1/PyMemoryEditor/win32/constants.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor/win32/enum.py` & `PyMemoryEditor-1.4.1/PyMemoryEditor/win32/enum.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor/win32/functions.py` & `PyMemoryEditor-1.4.1/PyMemoryEditor/win32/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,27 @@
 # https://learn.microsoft.com/en-us/windows/win32/api/memoryapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/psapi/
 # ...
 
 from .types import MEMORY_BASIC_INFORMATION, SYSTEM_INFO, WNDENUMPROC
 from .util import get_c_type_of
-from ctypes import byref, c_uint32, c_void_p, create_unicode_buffer, sizeof, windll
+from ctypes import POINTER, byref, c_uint32, c_void_p, create_unicode_buffer, sizeof, windll, wintypes
 from typing import Generator, Type, TypeVar, Union
 
+# Load the libraries.
 kernel32 = windll.LoadLibrary("kernel32.dll")
 user32 = windll.LoadLibrary("user32.dll")
 
+# Set the argtypes to prevent ArgumentError.
+kernel32.VirtualQueryEx.argtypes = (
+    wintypes.HANDLE, wintypes.LPCVOID, POINTER(MEMORY_BASIC_INFORMATION), c_uint32
+)
+
+
 # Get the user's system information.
 system_information = SYSTEM_INFO()
 kernel32.GetSystemInfo(byref(system_information))
 
 
 T = TypeVar("T")
```

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.4.1/PyMemoryEditor/win32/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,12 +39,12 @@
         ("dwProcessorType", wintypes.DWORD),
         ("dwAllocationGranularity", wintypes.DWORD),
         ("wProcessorLevel", wintypes.WORD),
         ("wProcessorRevision", wintypes.WORD),
     ]
 
 
-# The structure changes according to the the Python version (64 or 32 bits).
+# The structure changes according to the Python version (64 or 32 bits).
 MEMORY_BASIC_INFORMATION = MEMORY_BASIC_INFORMATION_64 if sizeof(c_void_p) == 8 else MEMORY_BASIC_INFORMATION_32
 
 # For EnumWindows and EnumDesktopWindows functions.
 WNDENUMPROC = WINFUNCTYPE(c_bool, wintypes.HWND, wintypes.LPARAM)
```

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.4.1/PyMemoryEditor/win32/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.0
+Version: 1.4.1
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/SOURCES.txt` & `PyMemoryEditor-1.4.1/PyMemoryEditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.0/README.md` & `PyMemoryEditor-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.0/setup.py` & `PyMemoryEditor-1.4.1/setup.py`

 * *Files identical despite different names*

