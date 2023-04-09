# Comparing `tmp/symbolicmode-0.9.tar.gz` & `tmp/symbolicmode-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolicmode-0.9.tar", last modified: Sat Apr  8 04:37:59 2023, max compression
+gzip compressed data, was "symbolicmode-0.9.1.tar", last modified: Sun Apr  9 17:33:46 2023, max compression
```

## Comparing `symbolicmode-0.9.tar` & `symbolicmode-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:37:59.904573 symbolicmode-0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-08 04:37:50.000000 symbolicmode-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-08 04:37:59.904573 symbolicmode-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-08 04:37:50.000000 symbolicmode-0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-08 04:37:50.000000 symbolicmode-0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 04:37:59.908573 symbolicmode-0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:37:59.904573 symbolicmode-0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:37:59.904573 symbolicmode-0.9/src/symbolicmode/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6340 2023-04-08 04:37:50.000000 symbolicmode-0.9/src/symbolicmode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:37:59.904573 symbolicmode-0.9/src/symbolicmode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-08 04:37:59.000000 symbolicmode-0.9/src/symbolicmode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-08 04:37:59.000000 symbolicmode-0.9/src/symbolicmode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 04:37:59.000000 symbolicmode-0.9/src/symbolicmode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-08 04:37:59.000000 symbolicmode-0.9/src/symbolicmode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:37:59.904573 symbolicmode-0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-08 04:37:50.000000 symbolicmode-0.9/tests/test_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:33:46.158565 symbolicmode-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-09 17:33:34.000000 symbolicmode-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-09 17:33:46.158565 symbolicmode-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-09 17:33:34.000000 symbolicmode-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-09 17:33:34.000000 symbolicmode-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 17:33:46.158565 symbolicmode-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:33:46.154564 symbolicmode-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:33:46.154564 symbolicmode-0.9.1/src/symbolicmode/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9017 2023-04-09 17:33:34.000000 symbolicmode-0.9.1/src/symbolicmode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:33:46.154564 symbolicmode-0.9.1/src/symbolicmode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-09 17:33:46.000000 symbolicmode-0.9.1/src/symbolicmode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-09 17:33:46.000000 symbolicmode-0.9.1/src/symbolicmode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:33:46.000000 symbolicmode-0.9.1/src/symbolicmode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-09 17:33:46.000000 symbolicmode-0.9.1/src/symbolicmode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:33:46.154564 symbolicmode-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-09 17:33:34.000000 symbolicmode-0.9.1/tests/test_chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-09 17:33:34.000000 symbolicmode-0.9.1/tests/test_modes.py
```

### Comparing `symbolicmode-0.9/LICENSE` & `symbolicmode-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9/PKG-INFO` & `symbolicmode-0.9.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-Metadata-Version: 2.1
-Name: symbolicmode
-Version: 0.9
-Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
-Author-email: Sean Reifschneider <jafo00@gmail.com>
-Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
-Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # SymbolicMode -- Code to handle symbolic file permissions
 
 This python library parses symbolic file permission modes as used by GNU chmod, part
 of the coreutils package.  For example:
 
     >>> from symbolicmode import *
     >>> oct(symbolic_to_numeric_permissions('a=rx,u+w'))
     '0o755'   
 
+It also has a "chmod" function:
+
+    >>> chmod('a=rx,u+w', '/tmp/foo')
+    >>> chmod('755', '/tmp/foo')
+    >>> chmod(0o755, '/tmp/foo')
+
+For convenience it can take permissions in the form of an integer, a numeric string
+or the symbolic permissions.
+
 ## Status
 
 This library is fully compatible with GNU Coreutils "chmod" command. It fully implements
 all mode specifiers except for the purely numeric versions ("755") that chmod does,
 as verified by manual, unit, and extensive fuzz testing.
 
 My fuzz testing was against version 8.32-4.1ubuntu1).  Fuzz testing tools are in the
 "fuzzchmod" directory.
 
-## Docstring
+## Docstring - symbolic\_to\_numeric\_permissions
 
 Convert a symbolic file permission string to its numeric equivalent.
 
 The function takes a symbolic permission description string in the format of
 `user[=,+,-]permissions,group[=,+,-]permissions,other[=,+,-]permissions`.
 The available permission characters are `r` (read), `w` (write), `x` (execute),
 `X` (execute if a directory), `s` (setuid/setgid), and `t` (sticky bit), or a single
@@ -62,18 +57,55 @@
     >>> symbolic_to_numeric_permissions("u=rwX", is_directory=True)
     0o700
     >>> symbolic_to_numeric_permissions("u=rws,g=rx,o=r")
     0o4754
     >>> symbolic_to_numeric_permissions("=rw", initial_mode=0o4777, is_directory=False, umask=0o027)
     0o640
 
+## Docstring - chmod
+
+Change the mode (permissions) of a specified file or directory.
+
+The mode can be specified as an integer, a string representing an octal integer
+or as a string representing symbolic permissions (e.g., 'u=rwx,g=r,o=r').
+
+Parameters:
+- mode : int or str
+    The mode (permissions) to be applied to the file or directory. The mode can
+    be specified either as an integer, a string of digits (which are parsed as
+    an octal integer), or as a string representing symbolic permissions (e.g.,
+    'u=rwx,g=r,o=r').
+- path : str or Path
+    The path to the file or directory whose mode is to be changed.
+
+Returns: None
+
+Raises:
+- FileNotFoundError
+    If the specified file or directory does not exist.
+- PermissionError
+    If the user does not have sufficient privileges to change the mode.
+- ValueError
+    If the specified mode is invalid.
+
+Examples:
+
+    # Change the mode of a file using an octal integer:
+    chmod(0o755, '/path/to/file')
+
+    # Change the mode of a file using a digit string:
+    chmod('755', '/path/to/file')
+
+    # Change the mode of a directory using symbolic permissions
+    chmod('u=rwx,g=rx,o=r', '/path/to/directory')
+
 ## Permissions Instructions
 
 Permission instructions are 1 or more comma separated values of the form:
-"[USERS][=+-][PERMS]".
+"[ugoa...][[=+-][PERMS...]...]".
 
 USERS can be:
 
 - u: Set permissions for the owner.
 - g: Set permissions for group access.
 - o: Set permissions for all others.
 - a: All of the above.
```

### Comparing `symbolicmode-0.9/README.md` & `symbolicmode-0.9.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,49 @@
+Metadata-Version: 2.1
+Name: symbolicmode
+Version: 0.9.1
+Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
+Author-email: Sean Reifschneider <jafo00@gmail.com>
+Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
+Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SymbolicMode -- Code to handle symbolic file permissions
 
 This python library parses symbolic file permission modes as used by GNU chmod, part
 of the coreutils package.  For example:
 
     >>> from symbolicmode import *
     >>> oct(symbolic_to_numeric_permissions('a=rx,u+w'))
     '0o755'   
 
+It also has a "chmod" function:
+
+    >>> chmod('a=rx,u+w', '/tmp/foo')
+    >>> chmod('755', '/tmp/foo')
+    >>> chmod(0o755, '/tmp/foo')
+
+For convenience it can take permissions in the form of an integer, a numeric string
+or the symbolic permissions.
+
 ## Status
 
 This library is fully compatible with GNU Coreutils "chmod" command. It fully implements
 all mode specifiers except for the purely numeric versions ("755") that chmod does,
 as verified by manual, unit, and extensive fuzz testing.
 
 My fuzz testing was against version 8.32-4.1ubuntu1).  Fuzz testing tools are in the
 "fuzzchmod" directory.
 
-## Docstring
+## Docstring - symbolic\_to\_numeric\_permissions
 
 Convert a symbolic file permission string to its numeric equivalent.
 
 The function takes a symbolic permission description string in the format of
 `user[=,+,-]permissions,group[=,+,-]permissions,other[=,+,-]permissions`.
 The available permission characters are `r` (read), `w` (write), `x` (execute),
 `X` (execute if a directory), `s` (setuid/setgid), and `t` (sticky bit), or a single
@@ -48,18 +71,55 @@
     >>> symbolic_to_numeric_permissions("u=rwX", is_directory=True)
     0o700
     >>> symbolic_to_numeric_permissions("u=rws,g=rx,o=r")
     0o4754
     >>> symbolic_to_numeric_permissions("=rw", initial_mode=0o4777, is_directory=False, umask=0o027)
     0o640
 
+## Docstring - chmod
+
+Change the mode (permissions) of a specified file or directory.
+
+The mode can be specified as an integer, a string representing an octal integer
+or as a string representing symbolic permissions (e.g., 'u=rwx,g=r,o=r').
+
+Parameters:
+- mode : int or str
+    The mode (permissions) to be applied to the file or directory. The mode can
+    be specified either as an integer, a string of digits (which are parsed as
+    an octal integer), or as a string representing symbolic permissions (e.g.,
+    'u=rwx,g=r,o=r').
+- path : str or Path
+    The path to the file or directory whose mode is to be changed.
+
+Returns: None
+
+Raises:
+- FileNotFoundError
+    If the specified file or directory does not exist.
+- PermissionError
+    If the user does not have sufficient privileges to change the mode.
+- ValueError
+    If the specified mode is invalid.
+
+Examples:
+
+    # Change the mode of a file using an octal integer:
+    chmod(0o755, '/path/to/file')
+
+    # Change the mode of a file using a digit string:
+    chmod('755', '/path/to/file')
+
+    # Change the mode of a directory using symbolic permissions
+    chmod('u=rwx,g=rx,o=r', '/path/to/directory')
+
 ## Permissions Instructions
 
 Permission instructions are 1 or more comma separated values of the form:
-"[USERS][=+-][PERMS]".
+"[ugoa...][[=+-][PERMS...]...]".
 
 USERS can be:
 
 - u: Set permissions for the owner.
 - g: Set permissions for group access.
 - o: Set permissions for all others.
 - a: All of the above.
```

### Comparing `symbolicmode-0.9/pyproject.toml` & `symbolicmode-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 
 [project]
 name = "symbolicmode"
-version = "0.9"
+version = "0.9.1"
 authors = [
   { name="Sean Reifschneider", email="jafo00@gmail.com" },
 ]
 description = "Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `symbolicmode-0.9/src/symbolicmode/__init__.py` & `symbolicmode-0.9.1/src/symbolicmode.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,155 +1,172 @@
-#!/usr/bin/env python3
+Metadata-Version: 2.1
+Name: symbolicmode
+Version: 0.9.1
+Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
+Author-email: Sean Reifschneider <jafo00@gmail.com>
+Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
+Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SymbolicMode -- Code to handle symbolic file permissions
+
+This python library parses symbolic file permission modes as used by GNU chmod, part
+of the coreutils package.  For example:
+
+    >>> from symbolicmode import *
+    >>> oct(symbolic_to_numeric_permissions('a=rx,u+w'))
+    '0o755'   
+
+It also has a "chmod" function:
+
+    >>> chmod('a=rx,u+w', '/tmp/foo')
+    >>> chmod('755', '/tmp/foo')
+    >>> chmod(0o755, '/tmp/foo')
+
+For convenience it can take permissions in the form of an integer, a numeric string
+or the symbolic permissions.
+
+## Status
+
+This library is fully compatible with GNU Coreutils "chmod" command. It fully implements
+all mode specifiers except for the purely numeric versions ("755") that chmod does,
+as verified by manual, unit, and extensive fuzz testing.
+
+My fuzz testing was against version 8.32-4.1ubuntu1).  Fuzz testing tools are in the
+"fuzzchmod" directory.
+
+## Docstring - symbolic\_to\_numeric\_permissions
+
+Convert a symbolic file permission string to its numeric equivalent.
+
+The function takes a symbolic permission description string in the format of
+`user[=,+,-]permissions,group[=,+,-]permissions,other[=,+,-]permissions`.
+The available permission characters are `r` (read), `w` (write), `x` (execute),
+`X` (execute if a directory), `s` (setuid/setgid), and `t` (sticky bit), or a single
+character from: 'u', 'g', 'o'.
+
+Args:
+- `symbolic_perm` (str): The symbolic permission description string.
+- `initial_mode` (int, optional): The mode to start off with.  If changing mode of an
+        existing file, this is it's current mode, and can also impact 'X'.
+- `is_directory` (bool, optional): A boolean indicating whether the file is a directory.
+        This affects the behavior of the `X` permission. Defaults to False.
+- `umask` (int, optional): Umask to use for "=[modes]" operation.  If not specified, the
+        system umask will be used.
+
+Returns:
+- int: The numeric (octal) representation of the file permissions.
+
+Raises:
+- ValueError: When the permissions contain some invalid instruction.
+
+Examples:
+
+    >>> symbolic_to_numeric_permissions("u=rwx,g=rx,o=r")
+    0o754
+    >>> symbolic_to_numeric_permissions("u=rwX", is_directory=True)
+    0o700
+    >>> symbolic_to_numeric_permissions("u=rws,g=rx,o=r")
+    0o4754
+    >>> symbolic_to_numeric_permissions("=rw", initial_mode=0o4777, is_directory=False, umask=0o027)
+    0o640
+
+## Docstring - chmod
+
+Change the mode (permissions) of a specified file or directory.
+
+The mode can be specified as an integer, a string representing an octal integer
+or as a string representing symbolic permissions (e.g., 'u=rwx,g=r,o=r').
+
+Parameters:
+- mode : int or str
+    The mode (permissions) to be applied to the file or directory. The mode can
+    be specified either as an integer, a string of digits (which are parsed as
+    an octal integer), or as a string representing symbolic permissions (e.g.,
+    'u=rwx,g=r,o=r').
+- path : str or Path
+    The path to the file or directory whose mode is to be changed.
+
+Returns: None
+
+Raises:
+- FileNotFoundError
+    If the specified file or directory does not exist.
+- PermissionError
+    If the user does not have sufficient privileges to change the mode.
+- ValueError
+    If the specified mode is invalid.
+
+Examples:
+
+    # Change the mode of a file using an octal integer:
+    chmod(0o755, '/path/to/file')
+
+    # Change the mode of a file using a digit string:
+    chmod('755', '/path/to/file')
+
+    # Change the mode of a directory using symbolic permissions
+    chmod('u=rwx,g=rx,o=r', '/path/to/directory')
+
+## Permissions Instructions
+
+Permission instructions are 1 or more comma separated values of the form:
+"[ugoa...][[=+-][PERMS...]...]".
+
+USERS can be:
+
+- u: Set permissions for the owner.
+- g: Set permissions for group access.
+- o: Set permissions for all others.
+- a: All of the above.
+- "": The empty string, only allowed with "=" for the operator.  Applies to all (like
+  "a"), but applies the umask to the permissions set.
+
+Operators are:
+
+- -: Remove the PERMS to the file permissions.
+- +: Add the PERMS to the file permissions.
+- =: Set the permissions to exactly PERMS.
+
+PERMS can be a combination of the following (except for u/g/o which if specified must
+be the only, single, PERM provided:
+
+- r: Allow read access, if a directory allow reading files within.
+- w: Allow write access, if a directory allow writing or creating files.
+- x: Allow execute, or list contents if a directory.
+- X: Set "x" but only if file permissions already had an "x" set for any user, or if
+  the object is a directory.
+- s: Set UID/GID on execution, allows a program to take on the user/group permissions
+  of the executable file.
+- t: Sticky bit or restrict deletion to the file owner if a directory.  Note that
+  some system settings may prevent root from writing to non-root files in a
+  restricted deletion directory.  See "fs.protected\_regular" sysctl setting.
+- u: Take on the permissions granted to the user ("go=u").  Must be the only PERM if
+  specified.
+- g: Take on the group permissions.  Must be the only PERM if specified.
+- o: Take on the permissions granted to others.  Must be the only PERM if specified.
+
+Notes on instructions:
+
+- "=[PERMS]" sets the permissions based on the umask.  This acts like "a" was
+  specified for the USER, the PERMS are masked with the umask when applied for u/g/o.
+- "-[PERMS]" and "+[PERMS]" are not defined as meaning anything in the chmod manpage.
+  If given to chmod, chmod will make a permissions change and then error out saying
+  that the change was not the expected change.  Because of this, SymbolicMode will
+  raise a ValueError on either of these instructions.
+
+## Fuzz Testing
+
+In the "fuzzchmod" directory is a set of programs for fuzz testing SymbolicMode
+against the system "chmod" to try to ensure correctness for even unusual inputs.
 
-"""
-This module implements code for handling symbolic permissions in the way that GNU
-chmod from coreutils does.  For example: "a=rx,u+w" for 755
-
-Written by Sean Reifschneider and ChatGPT, 2023-03
-"""
-
-import os
-import re
-from typing import Union, Iterator, Tuple
-
-
-def symbolic_to_numeric_permissions(
-    symbolic_perm: str,
-    initial_mode: int = 0,
-    is_directory: bool = False,
-    umask: Union[int, None] = None,
-) -> int:
-    """
-    Convert a symbolic file permission string to its numeric equivalent.
-
-    The function takes a symbolic permission description string in the format of
-    `user[=,+,-]permissions,group[=,+,-]permissions,other[=,+,-]permissions`.
-    The available permission characters are `r` (read), `w` (write), `x` (execute),
-    `X` (execute if a directory), `s` (setuid/setgid), and `t` (sticky bit), or a single
-    character from: 'u', 'g', 'o'.
-
-    Args:
-        symbolic_perm (str): The symbolic permission description string.
-        initial_mode (int, optional): The mode to start off with.  If changing mode of an
-                existing file, this is it's current mode, and can also impact 'X'.
-        is_directory (bool, optional): A boolean indicating whether the file is a directory.
-                This affects the behavior of the `X` permission. Defaults to False.
-        umask (int, optional): Umask to use for "=[modes]" operation.  If not specified, the
-                system umask will be used.
-
-    Returns:
-        int: The numeric (octal) representation of the file permissions.
-
-    Raises:
-        ValueError: When the permissions contain some invalid instruction.
-
-    Examples:
-        >>> symbolic_to_numeric_permissions("u=rwx,g=rx,o=r")
-        0o754
-        >>> symbolic_to_numeric_permissions("u=rwX", is_directory=True)
-        0o700
-        >>> symbolic_to_numeric_permissions("u=rws,g=rx,o=r")
-        0o4754
-        >>> symbolic_to_numeric_permissions("=rw", initial_mode=0o4777, is_directory=False, umask=0o027)
-        0o640
-    """
-
-    def update_perm(operation: str, instruction_perms: int, current_perm: int) -> int:
-        "Helper function to apply `operation` to the current perms and the instruction_perms"
-        if operation == "=":
-            return instruction_perms
-        if operation == "+":
-            return current_perm | instruction_perms
-        return current_perm & ~instruction_perms
-
-    def parse_instructions(permstr: str) -> Iterator[Tuple[str, str, str]]:
-        """Helper to parse the instruction into (lhs, op, rhs).  This also expands
-        multi-operation expressions into multiple u/op/perm tuples."""
-        rx = re.compile(r"([=+-][rwxXstugo]*)")
-        for instruction in permstr.split(","):
-            m = rx.split(instruction)
-            if not m:
-                raise ValueError(f"Invalid instruction: {instruction}")
-            user = m[0]
-            for op, perm in [(op_perm[0], op_perm[1:]) for op_perm in m[1::2]]:
-                yield ((user, op, perm))
-
-    # Define a mapping of symbolic permission characters to their corresponding numeric values
-    perm_values = {"r": 4, "w": 2, "x": 1, "X": 1 if is_directory else 0, "-": 0}
-
-    #  bits to shift based on u/g/o
-    shift_by_user = {"u": 6, "g": 3, "o": 0}
-
-    # Extract initial permissions and special bits
-    user_perms = (initial_mode >> 6) & 0o7
-    group_perms = (initial_mode >> 3) & 0o7
-    other_perms = (initial_mode >> 0) & 0o7
-    perms = {"u": user_perms, "g": group_perms, "o": other_perms}
-    setuid_bit = 4 if initial_mode & 0o4000 else 0
-    setgid_bit = 2 if initial_mode & 0o2000 else 0
-    sticky_bit = 1 if initial_mode & 0o1000 else 0
-
-    if umask is None:
-        umask = os.umask(0)
-        os.umask(umask)
-
-    for users, operation, perms_str in parse_instructions(symbolic_perm):
-        #  set X value for executable based on current perms
-        if not is_directory:
-            perm_values["X"] = (
-                1 if perms["u"] & 1 or perms["g"] & 1 or perms["o"] & 1 else 0
-            )
-
-        # calculate PERMS value
-        perm_set = set(perms_str)
-        if "x" in perm_set and "X" in perm_set:
-            perm_set.remove("X")  # prevent doubling "x" bit
-        perm_sum = sum(
-            perm_values.get(p, perm_values.get(p.upper(), 0)) for p in perm_set
-        )
-
-        #  handle u/g/o in PERMS
-        if ("u" in perms_str or "g" in perms_str or "o" in perms_str) and len(
-            perms_str
-        ) != 1:
-            raise ValueError(
-                "If u/g/o specified on RHS, only a single letter of u/g/o can be specified"
-            )
-        perm_sum = perms["u"] if perms_str == "u" else perm_sum
-        perm_sum = perms["g"] if perms_str == "g" else perm_sum
-        perm_sum = perms["o"] if perms_str == "o" else perm_sum
-
-        # Update the numeric file mode variables based on the users and operation
-        effective_users = ("u", "g", "o") if users == "" or "a" in users else users
-        for user in effective_users:
-            apply_mask = (~umask if users == "" else 0o7777) >> shift_by_user[user]
-            perms[user] = update_perm(operation, perm_sum & apply_mask, perms[user])
-            if user == "u":
-                if "s" in perms_str:
-                    setuid_bit = 4 if operation in "+=" else 0
-                setuid_bit = (
-                    0
-                    if "s" not in perms_str and operation == "=" and not is_directory
-                    else setuid_bit
-                )
-            if user == "g":
-                if "s" in perms_str:
-                    setgid_bit = 2 if operation in "+=" else 0
-                setgid_bit = (
-                    0
-                    if "s" not in perms_str and operation == "=" and not is_directory
-                    else setgid_bit
-                )
-            if user == "o":
-                if "t" in perms_str:
-                    sticky_bit = 1 if operation in "+=" else 0
-                sticky_bit = (
-                    0 if "t" not in perms_str and operation == "=" else sticky_bit
-                )
-
-    # Combine the numeric file modes for the owner, group, and others into a single numeric file mode
-    return (
-        ((setuid_bit + setgid_bit + sticky_bit) << 9)
-        | (perms["u"] << 6)
-        | (perms["g"] << 3)
-        | (perms["o"])
-    )
+## License
+
+CC0 1.0 Universal, see LICENSE file for more information.
+
+<!-- vim: ts=4 sw=4 ai et tw=85
+-->
```

### Comparing `symbolicmode-0.9/tests/test_modes.py` & `symbolicmode-0.9.1/tests/test_modes.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,20 @@
     def test_basic_permissions(self):
         self.assertEqual(symbolic_to_numeric_permissions("u=rwx,g=rx,o=r"), 0o754)
         self.assertEqual(symbolic_to_numeric_permissions("u=rw,g=r,o="), 0o640)
         self.assertEqual(symbolic_to_numeric_permissions("u=rwx,g=,o="), 0o700)
         self.assertEqual(symbolic_to_numeric_permissions("a=r"), 0o444)
         self.assertEqual(symbolic_to_numeric_permissions("a=-,ug+r,u+w"), 0o640)
         self.assertEqual(symbolic_to_numeric_permissions("+X", 0o500), 0o511)
+        self.assertEqual(
+            symbolic_to_numeric_permissions("u+rwx,g+rwx,o=rwx", 0o000), 0o777
+        )
+        self.assertEqual(
+            symbolic_to_numeric_permissions("u+rwx,g+rwx,o=rwx", 0o000, True), 0o777
+        )
 
     def test_add_permissions(self):
         self.assertEqual(symbolic_to_numeric_permissions("u=rw,g=r,o=,ug+w"), 0o660)
         self.assertEqual(symbolic_to_numeric_permissions("u=rwx,g=rx,o=r,u+w"), 0o754)
 
     def test_remove_permissions(self):
         self.assertEqual(symbolic_to_numeric_permissions("u=rw,g=r,o=,ug-w"), 0o440)
```

