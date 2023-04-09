# Comparing `tmp/PyMemoryEditor-1.3.1.tar.gz` & `tmp/PyMemoryEditor-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.3.1.tar", last modified: Sat Apr  8 05:53:47 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.3.2.tar", last modified: Sun Apr  9 02:46:06 2023, max compression
```

## Comparing `PyMemoryEditor-1.3.1.tar` & `PyMemoryEditor-1.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 05:53:47.805808 PyMemoryEditor-1.3.1/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     2976 2023-04-08 05:53:47.805808 PyMemoryEditor-1.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-08 05:53:47.758085 PyMemoryEditor-1.3.1/PyMemoryEditor/
--rw-rw-rw-   0        0        0      426 2023-04-08 05:44:05.000000 PyMemoryEditor-1.3.1/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     3685 2023-04-08 01:24:36.000000 PyMemoryEditor-1.3.1/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-08 05:53:47.787919 PyMemoryEditor-1.3.1/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-03 04:40:51.000000 PyMemoryEditor-1.3.1/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-03 04:41:38.000000 PyMemoryEditor-1.3.1/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-03 04:42:49.000000 PyMemoryEditor-1.3.1/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-08 05:53:47.804805 PyMemoryEditor-1.3.1/PyMemoryEditor/win32/
--rw-rw-rw-   0        0        0    13571 2023-04-03 05:07:05.000000 PyMemoryEditor-1.3.1/PyMemoryEditor/win32/constants.py
--rw-rw-rw-   0        0        0    14385 2023-04-03 05:07:48.000000 PyMemoryEditor-1.3.1/PyMemoryEditor/win32/enum.py
--rw-rw-rw-   0        0        0     3229 2023-04-08 05:52:58.000000 PyMemoryEditor-1.3.1/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1650 2023-04-08 05:48:29.000000 PyMemoryEditor-1.3.1/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      905 2023-04-08 05:11:54.000000 PyMemoryEditor-1.3.1/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-08 05:53:47.777117 PyMemoryEditor-1.3.1/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     2976 2023-04-08 05:53:47.000000 PyMemoryEditor-1.3.1/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-04-08 05:53:47.000000 PyMemoryEditor-1.3.1/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 05:53:47.000000 PyMemoryEditor-1.3.1/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-08 05:53:47.000000 PyMemoryEditor-1.3.1/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-08 05:53:47.000000 PyMemoryEditor-1.3.1/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2025 2023-04-03 04:59:56.000000 PyMemoryEditor-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 05:53:47.806805 PyMemoryEditor-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 02:46:06.264742 PyMemoryEditor-1.3.2/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2976 2023-04-09 02:46:06.264742 PyMemoryEditor-1.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 02:46:06.216359 PyMemoryEditor-1.3.2/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      426 2023-04-09 02:33:01.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     3685 2023-04-08 01:24:36.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-09 02:46:06.250602 PyMemoryEditor-1.3.2/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-03 04:40:51.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-03 04:41:38.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-03 04:42:49.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 02:46:06.264742 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/
+-rw-rw-rw-   0        0        0    13571 2023-04-03 05:07:05.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/constants.py
+-rw-rw-rw-   0        0        0    14385 2023-04-03 05:07:48.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/enum.py
+-rw-rw-rw-   0        0        0     4590 2023-04-09 02:32:36.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1795 2023-04-09 02:15:47.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      905 2023-04-08 05:11:54.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 02:46:06.232622 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     2976 2023-04-09 02:46:06.000000 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-04-09 02:46:06.000000 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 02:46:06.000000 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 02:46:06.000000 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 02:46:06.000000 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2025 2023-04-03 04:59:56.000000 PyMemoryEditor-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 02:46:06.264742 PyMemoryEditor-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.3.2/setup.py
```

### Comparing `PyMemoryEditor-1.3.1/LICENSE` & `PyMemoryEditor-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.1/PKG-INFO` & `PyMemoryEditor-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.3.1
+Version: 1.3.2
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.3.2/PyMemoryEditor/open_process.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.3.2/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.3.2/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.3.2/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor/win32/constants.py` & `PyMemoryEditor-1.3.2/PyMemoryEditor/win32/constants.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor/win32/enum.py` & `PyMemoryEditor-1.3.2/PyMemoryEditor/win32/enum.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor/win32/functions.py` & `PyMemoryEditor-1.3.2/PyMemoryEditor/win32/functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 # Read more about operations with processes by win32 api here:
 # https://learn.microsoft.com/en-us/windows/win32/api/memoryapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/psapi/
 # ...
 
-from .types import MEMORY_BASIC_INFORMATION, SYSTEM_INFO
+from .types import MEMORY_BASIC_INFORMATION, SYSTEM_INFO, WNDENUMPROC
 from .util import get_c_type_of
-from ctypes import byref, c_void_p, sizeof, windll
+from ctypes import byref, c_uint32, c_void_p, create_unicode_buffer, sizeof, windll
 from typing import Generator, Type, TypeVar, Union
 
 kernel32 = windll.LoadLibrary("kernel32.dll")
+user32 = windll.LoadLibrary("user32.dll")
 
 # Get the user's system information.
 system_information = SYSTEM_INFO()
 kernel32.GetSystemInfo(byref(system_information))
 
 
 T = TypeVar("T")
@@ -57,14 +58,50 @@
     will inherit the handle. Otherwise, the processes do not inherit this handle.
 
     :param pid: The identifier of the local process to be opened.
     """
     return kernel32.OpenProcess(access_right, inherit, pid)
 
 
+def GetProcessIdByWindowTitle(window_title: str) -> int:
+    """
+    Return the process ID by querying a window title.
+    """
+    result = c_uint32(0)
+
+    string_buffer_size = len(window_title) + 2  # (+2) for the next possible character of a title and the NULL char.
+    string_buffer = create_unicode_buffer(string_buffer_size)
+
+    def callback(hwnd, size):
+        """
+        This callback is used to get a window handle and compare
+        its title with the target window title.
+
+        To continue enumeration, the callback function must return TRUE;
+        to stop enumeration, it must return FALSE.
+        """
+        nonlocal result, string_buffer
+
+        user32.GetWindowTextW(hwnd, string_buffer, size)
+
+        # Compare the window titles and get the process ID.
+        if window_title == string_buffer.value:
+            user32.GetWindowThreadProcessId(hwnd, byref(result))
+            return False
+
+        # Indicate it must continue enumeration.
+        return True
+
+    # Enumerates all top-level windows on the screen by passing the handle to each window,
+    # in turn, to an application-defined callback function.
+    user32.EnumWindows(WNDENUMPROC(callback), string_buffer_size)
+
+    return result.value
+
+
 def ReadProcessMemory(
     process_handle: int,
     address: int,
     pytype: Type[T],
     bufflength: int
 ) -> T:
     """
```

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.3.2/PyMemoryEditor/win32/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ctypes import Structure, c_ulonglong, c_void_p, sizeof, wintypes
+from ctypes import Structure, WINFUNCTYPE, c_bool, c_ulonglong, c_void_p, sizeof, wintypes
 
 
 class MEMORY_BASIC_INFORMATION_32(Structure):
     _fields_ = [
         ("BaseAddress", wintypes.DWORD),
         ("AllocationBase", wintypes.DWORD),
         ("AllocationProtect", wintypes.DWORD),
@@ -40,8 +40,11 @@
         ("dwAllocationGranularity", wintypes.DWORD),
         ("wProcessorLevel", wintypes.WORD),
         ("wProcessorRevision", wintypes.WORD),
     ]
 
 
 # The structure changes according to the the Python version (64 or 32 bits).
-MEMORY_BASIC_INFORMATION = MEMORY_BASIC_INFORMATION_64 if sizeof(c_void_p) == 8 else MEMORY_BASIC_INFORMATION_32
+MEMORY_BASIC_INFORMATION = MEMORY_BASIC_INFORMATION_64 if sizeof(c_void_p) == 8 else MEMORY_BASIC_INFORMATION_32
+
+# For EnumWindows and EnumDesktopWindows functions.
+WNDENUMPROC = WINFUNCTYPE(c_bool, wintypes.HWND, wintypes.LPARAM)
```

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.3.2/PyMemoryEditor/win32/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.3.1
+Version: 1.3.2
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `PyMemoryEditor-1.3.1/PyMemoryEditor.egg-info/SOURCES.txt` & `PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.1/README.md` & `PyMemoryEditor-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.1/setup.py` & `PyMemoryEditor-1.3.2/setup.py`

 * *Files identical despite different names*

