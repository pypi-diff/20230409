# Comparing `tmp/PyMemoryEditor-1.3.2.tar.gz` & `tmp/PyMemoryEditor-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.3.2.tar", last modified: Sun Apr  9 02:46:06 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.4.0.tar", last modified: Sun Apr  9 04:38:51 2023, max compression
```

## Comparing `PyMemoryEditor-1.3.2.tar` & `PyMemoryEditor-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 02:46:06.264742 PyMemoryEditor-1.3.2/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     2976 2023-04-09 02:46:06.264742 PyMemoryEditor-1.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 02:46:06.216359 PyMemoryEditor-1.3.2/PyMemoryEditor/
--rw-rw-rw-   0        0        0      426 2023-04-09 02:33:01.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     3685 2023-04-08 01:24:36.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-09 02:46:06.250602 PyMemoryEditor-1.3.2/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-03 04:40:51.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-03 04:41:38.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-03 04:42:49.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 02:46:06.264742 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/
--rw-rw-rw-   0        0        0    13571 2023-04-03 05:07:05.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/constants.py
--rw-rw-rw-   0        0        0    14385 2023-04-03 05:07:48.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/enum.py
--rw-rw-rw-   0        0        0     4590 2023-04-09 02:32:36.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1795 2023-04-09 02:15:47.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      905 2023-04-08 05:11:54.000000 PyMemoryEditor-1.3.2/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 02:46:06.232622 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     2976 2023-04-09 02:46:06.000000 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-04-09 02:46:06.000000 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 02:46:06.000000 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 02:46:06.000000 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 02:46:06.000000 PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2025 2023-04-03 04:59:56.000000 PyMemoryEditor-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 02:46:06.264742 PyMemoryEditor-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:38:51.644738 PyMemoryEditor-1.4.0/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     2976 2023-04-09 04:38:51.644738 PyMemoryEditor-1.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 04:38:51.631229 PyMemoryEditor-1.4.0/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      426 2023-04-09 03:26:04.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     3737 2023-04-09 03:43:03.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:38:51.644738 PyMemoryEditor-1.4.0/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:38:51.644738 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/
+-rw-rw-rw-   0        0        0    13571 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/constants.py
+-rw-rw-rw-   0        0        0    14385 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/enum.py
+-rw-rw-rw-   0        0        0     4705 2023-04-09 03:42:05.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1795 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      928 2023-04-09 03:40:32.000000 PyMemoryEditor-1.4.0/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:38:51.631229 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     2976 2023-04-09 04:38:51.000000 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-04-09 04:38:51.000000 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 04:38:51.000000 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 04:38:51.000000 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 04:38:51.000000 PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2025 2023-04-03 04:59:56.000000 PyMemoryEditor-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 04:38:51.644738 PyMemoryEditor-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.4.0/setup.py
```

### Comparing `PyMemoryEditor-1.3.2/LICENSE` & `PyMemoryEditor-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.2/PKG-INFO` & `PyMemoryEditor-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.3.2
+Version: 1.4.0
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.4.0/PyMemoryEditor/open_process.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         pytype: Type[T],
         bufflength: int
     ) -> T:
         """
         Return a value from a memory address.
 
         :param address: target memory address (ex: 0x006A9EC0).
-        :param pytype: type of the value to be received (str, int or float).
+        :param pytype: type of the value to be received (bool, int, float, str or bytes).
         :param bufflength: value size in bytes (1, 2, 4, 8).
         """
         valid_permissions = [
             ProcessOperations.PROCESS_ALL_ACCESS.value,
             ProcessOperations.PROCESS_VM_READ.value
         ]
         if self.__permission.value not in valid_permissions:
@@ -85,23 +85,23 @@
         return ReadProcessMemory(self.__process_handle, address, pytype, bufflength)
 
     def write_process_memory(
         self,
         address: int,
         pytype: Type[T],
         bufflength: int,
-        value: Union[str, int, float]
+        value: Union[bool, int, float, str, bytes]
     ) -> T:
         """
         Write a value to a memory address.
 
         :param address: target memory address (ex: 0x006A9EC0).
-        :param pytype: type of value to be written into memory (str, int or float).
+        :param pytype: type of value to be written into memory (bool, int, float, str or bytes).
         :param bufflength: value size in bytes (1, 2, 4, 8).
-        :param value: value to be written (str, int or float).
+        :param value: value to be written (bool, int, float, str or bytes).
         """
         valid_permissions = [
             ProcessOperations.PROCESS_ALL_ACCESS.value,
             ProcessOperations.PROCESS_VM_OPERATION.value | ProcessOperations.PROCESS_VM_WRITE.value
         ]
         if self.__permission.value not in valid_permissions:
             raise PermissionError("The handle does not have permission to write to the process memory.")
```

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.4.0/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.4.0/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.4.0/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor/win32/constants.py` & `PyMemoryEditor-1.4.0/PyMemoryEditor/win32/constants.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor/win32/enum.py` & `PyMemoryEditor-1.4.0/PyMemoryEditor/win32/enum.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor/win32/functions.py` & `PyMemoryEditor-1.4.0/PyMemoryEditor/win32/functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,33 +103,35 @@
     address: int,
     pytype: Type[T],
     bufflength: int
 ) -> T:
     """
     Return a value from a memory address.
     """
-    if pytype not in [str, int, float]: raise ValueError("The type must be string, int or float.")
+    if pytype not in [bool, int, float, str, bytes]:
+        raise ValueError("The type must be bool, int, float, str or bytes.")
 
     data = get_c_type_of(pytype, int(bufflength))
     kernel32.ReadProcessMemory(process_handle, c_void_p(address), byref(data), bufflength, None)
 
-    return data.value
+    return str(data.value) if pytype is str else data.value
 
 
 def WriteProcessMemory(
     process_handle: int,
     address: int,
     pytype: Type[T],
     bufflength: int,
-    value: Union[int, float, str]
+    value: Union[bool, int, float, str, bytes]
 ) -> T:
     """
     Write a value to a memory address.
     """
-    if pytype not in [str, int, float]: raise ValueError("The type must be string, int or float.")
+    if pytype not in [bool, int, float, str, bytes]:
+        raise ValueError("The type must be bool, int, float, str or bytes.")
 
     data = get_c_type_of(pytype, int(bufflength))
     data.value = value.encode() if isinstance(value, str) else value
 
     kernel32.WriteProcessMemory(process_handle, c_void_p(address), byref(data), bufflength, None)
 
     return value
```

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.4.0/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.4.0/PyMemoryEditor/win32/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import ctypes
 
 
 def get_c_type_of(pytype: Type, length: int = 1) -> ctypes._SimpleCData:
     """
     Return a C type of a primitive type of the Python language.
     """
-    if pytype is str: return ctypes.create_string_buffer(length)
+    if pytype is str or pytype is bytes: return ctypes.create_string_buffer(length)
 
     elif pytype is int:
 
         if length == 1: return ctypes.c_int8()      # 1 Byte
         if length == 2: return ctypes.c_int16()     # 2 Bytes
         if length <= 4: return ctypes.c_int32()     # 4 Bytes
         return ctypes.c_int64()                     # 8 Bytes
 
     # Float values lose their precision when converted to c_float. For that reason,
     # any float value will be converted to double.
     elif pytype is float: return ctypes.c_double()  # 8 Bytes
 
     elif pytype is bool: return ctypes.c_bool()
 
-    else: raise ValueError("The type must be string, int, float or bool.")
+    else: raise ValueError("The type must be bool, int, float, str or bytes.")
```

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.3.2
+Version: 1.4.0
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `PyMemoryEditor-1.3.2/PyMemoryEditor.egg-info/SOURCES.txt` & `PyMemoryEditor-1.4.0/PyMemoryEditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.2/README.md` & `PyMemoryEditor-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.3.2/setup.py` & `PyMemoryEditor-1.4.0/setup.py`

 * *Files identical despite different names*

