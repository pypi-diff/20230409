# Comparing `tmp/nutikacompile-0.11.tar.gz` & `tmp/nutikacompile-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutikacompile-0.11.tar", last modified: Sun Apr  9 13:33:15 2023, max compression
+gzip compressed data, was "nutikacompile-0.12.tar", last modified: Sun Apr  9 14:08:53 2023, max compression
```

## Comparing `nutikacompile-0.11.tar` & `nutikacompile-0.12.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 13:33:15.342618 nutikacompile-0.11/
--rw-rw-rw-   0        0        0     1148 2023-04-09 13:33:10.000000 nutikacompile-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      141 2023-04-09 13:33:10.000000 nutikacompile-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     3963 2023-04-09 13:33:15.342618 nutikacompile-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     3202 2023-04-09 08:41:19.000000 nutikacompile-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 13:33:15.337632 nutikacompile-0.11/nutikacompile/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 nutikacompile-0.11/nutikacompile/LICENSE
--rw-rw-rw-   0        0        0     3202 2023-04-09 08:41:19.000000 nutikacompile-0.11/nutikacompile/README.MD
--rw-rw-rw-   0        0        0     6634 2023-04-09 13:32:32.000000 nutikacompile-0.11/nutikacompile/__init__.py
--rw-rw-rw-   0        0        0       32 2023-04-09 13:33:14.000000 nutikacompile-0.11/nutikacompile/requirements.txt
--rw-rw-rw-   0        0        0    58415 2023-04-09 13:33:14.000000 nutikacompile-0.11/nutikacompile/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-09 13:33:15.341620 nutikacompile-0.11/nutikacompile.egg-info/
--rw-rw-rw-   0        0        0     3963 2023-04-09 13:33:15.000000 nutikacompile-0.11/nutikacompile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-04-09 13:33:15.000000 nutikacompile-0.11/nutikacompile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 13:33:15.000000 nutikacompile-0.11/nutikacompile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-09 13:33:15.000000 nutikacompile-0.11/nutikacompile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-09 13:33:15.000000 nutikacompile-0.11/nutikacompile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-09 13:33:15.343615 nutikacompile-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1300 2023-04-09 13:33:14.000000 nutikacompile-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:08:53.170939 nutikacompile-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-04-09 14:08:50.000000 nutikacompile-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      141 2023-04-09 14:08:50.000000 nutikacompile-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     4043 2023-04-09 14:08:53.170939 nutikacompile-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     3273 2023-04-09 14:06:28.000000 nutikacompile-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 14:08:53.166950 nutikacompile-0.12/nutikacompile/
+-rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 nutikacompile-0.12/nutikacompile/LICENSE
+-rw-rw-rw-   0        0        0     3273 2023-04-09 14:06:28.000000 nutikacompile-0.12/nutikacompile/README.MD
+-rw-rw-rw-   0        0        0     6708 2023-04-09 14:05:33.000000 nutikacompile-0.12/nutikacompile/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-04-09 14:08:52.000000 nutikacompile-0.12/nutikacompile/requirements.txt
+-rw-rw-rw-   0        0        0    58415 2023-04-09 14:08:52.000000 nutikacompile-0.12/nutikacompile/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-09 14:08:53.169942 nutikacompile-0.12/nutikacompile.egg-info/
+-rw-rw-rw-   0        0        0     4043 2023-04-09 14:08:53.000000 nutikacompile-0.12/nutikacompile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-04-09 14:08:53.000000 nutikacompile-0.12/nutikacompile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 14:08:53.000000 nutikacompile-0.12/nutikacompile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-09 14:08:53.000000 nutikacompile-0.12/nutikacompile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-09 14:08:53.000000 nutikacompile-0.12/nutikacompile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-04-09 14:08:53.170939 nutikacompile-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2023-04-09 14:08:52.000000 nutikacompile-0.12/setup.py
```

### Comparing `nutikacompile-0.11/LICENSE.rst` & `nutikacompile-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `nutikacompile-0.11/PKG-INFO` & `nutikacompile-0.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutikacompile
-Version: 0.11
+Version: 0.12
 Summary: A function that creates the cmd line for nuitka and executes it
 Home-page: https://github.com/hansalemaos/nutikacompile
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: nuitka,exe,compile
 Classifier: Development Status :: 4 - Beta
@@ -43,29 +43,38 @@
 )
 print(wholecommand)
 
 # The function creates and executes this command: 
 start "" "C:\ProgramData\anaconda3\envs\adda\python.exe" -m nuitka C:/ProgramData/anaconda3/envs/adda/secretsubprocess.py --assume-yes-for-downloads --output-dir=c:/compiledapptest --windows-disable-console --onefile --windows-icon-from-ico=C:/Users/hansc/AppData/Local/Temp/tmpb4w1z8d9.ico --include-data-files=C:/Users/hansc/AppData/Local/Temp/tmpb4i48w8_=.//=**/*.* --windows-uac-admin --file-version=1.0.0.0 --onefile-tempdir-spec=%CACHE_DIR%/nutikacompile/1.0.0.0
 
 
-
-compile_with_nuitka(pyfile: str, icon: Optional[str] = None, disable_console: bool = True, onefile: bool = True, file_version: str = '1', outputdir: Optional[str] = None, addfiles: Optional[list] = None, delete_onefile_temp=False, needs_admin=False) -> str
+compile_with_nuitka(
+    pyfile: str,
+    icon: Union[str, None] = None,
+    disable_console: bool = True,
+    onefile: bool = True,
+    file_version: str = "1",
+    outputdir: Union[str, None] = None,
+    addfiles: Union[list, None] = None,
+    delete_onefile_temp: bool = False,
+    needs_admin: bool = False,
+    relativefolderinapps: Union[None, str] = None,
+    arguments2add: str = "",
+) -> str
     Compiles a Python file using Nuitka.
-    
+
     Args:
         pyfile (str): The path to the Python file to be compiled.
-        icon (Union[str, None], optional): The path to the icon file to be used for the compiled executable, all formats that PIL can read are fine. Defaults to None.
+        icon (Union[str, None], optional): The path to the icon file to be used for the compiled executable. Defaults to None.
         disable_console (bool, optional): Whether to disable the console window for the compiled executable. Defaults to True.
         onefile (bool, optional): Whether to create a single executable file. Defaults to True.
-        file_version (str, optional): The version number to be assigned to the compiled executable.
-                                       File version to use in version information. Must be a
-                                        sequence of up to 4 numbers, e.g. 1.0 or 1.0.0.0, no
-                                        more digits are allowed, no strings are allowed. Defaults to "1".
-    
+        file_version (str, optional): The version number to be assigned to the compiled executable. Defaults to "1".
         outputdir (Union[str, None], optional): The path to the directory where the compiled executable will be saved. Defaults to None.
         addfiles (Union[list, None], optional): A list of files to be included in the compiled executable. Defaults to None.
-        delete_onefile_temp (bool, optional): Whether to delete the temporary directory created for the single executable file. Defaults to False.
+        delete_onefile_temp (bool, optional): Whether to delete the temporary directory for the single executable file. Defaults to False.
         needs_admin (bool, optional): Whether the compiled executable requires administrative privileges to run. Defaults to False.
-    
+        relativefolderinapps (Union[None, str], optional): The relative folder path to be used for the compiled executable. Defaults to None.
+        arguments2add (str, optional): Additional arguments to be passed to the Nuitka compiler. Defaults to "".
+
     Returns:
         str: The command used to compile the Python file.
 ```
```

### Comparing `nutikacompile-0.11/README.md` & `nutikacompile-0.12/nutikacompile.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,80 @@
-# A function that creates the cmd line for nuitka and executes it 
-
-
-```python
-pip install nutikacompile
+Metadata-Version: 2.1
+Name: nutikacompile
+Version: 0.12
+Summary: A function that creates the cmd line for nuitka and executes it
+Home-page: https://github.com/hansalemaos/nutikacompile
+Author: Johannes Fischer
+Author-email: <aulasparticularesdealemaosp@gmail.com>
+License: MIT
+Keywords: nuitka,exe,compile
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE.rst
+
+
+# A function that creates the cmd line for nuitka and executes it 
+
+
+```python
+pip install nutikacompile
+```
+
+```python
+from nutikacompile import compile_with_nuitka
+# creates the command line and executes it in a new console
+wholecommand = compile_with_nuitka(
+    pyfile=r"C:\ProgramData\anaconda3\envs\adda\secretsubprocess.py",
+    icon=r"C:\Users\hansc\Pictures\radiobutton.png",
+    disable_console=True,
+    file_version="1.0.0.0",
+    onefile=True,
+    outputdir="c:\\compiledapptest",
+    addfiles=[
+        r"C:\ProgramData\anaconda3\envs\adda\convertpic2ico.exe",  # output: compiledapptest/convertpic2ico.exe
+        r"C:\ProgramData\anaconda3\envs\adda\pi2\README.MD",  # output: compiledapptest/pi2/README.MD
+    ],
+    delete_onefile_temp=False,  # creates a permanent cache folder
+    needs_admin=True,
+)
+print(wholecommand)
+
+# The function creates and executes this command: 
+start "" "C:\ProgramData\anaconda3\envs\adda\python.exe" -m nuitka C:/ProgramData/anaconda3/envs/adda/secretsubprocess.py --assume-yes-for-downloads --output-dir=c:/compiledapptest --windows-disable-console --onefile --windows-icon-from-ico=C:/Users/hansc/AppData/Local/Temp/tmpb4w1z8d9.ico --include-data-files=C:/Users/hansc/AppData/Local/Temp/tmpb4i48w8_=.//=**/*.* --windows-uac-admin --file-version=1.0.0.0 --onefile-tempdir-spec=%CACHE_DIR%/nutikacompile/1.0.0.0
+
+
+compile_with_nuitka(
+    pyfile: str,
+    icon: Union[str, None] = None,
+    disable_console: bool = True,
+    onefile: bool = True,
+    file_version: str = "1",
+    outputdir: Union[str, None] = None,
+    addfiles: Union[list, None] = None,
+    delete_onefile_temp: bool = False,
+    needs_admin: bool = False,
+    relativefolderinapps: Union[None, str] = None,
+    arguments2add: str = "",
+) -> str
+    Compiles a Python file using Nuitka.
+
+    Args:
+        pyfile (str): The path to the Python file to be compiled.
+        icon (Union[str, None], optional): The path to the icon file to be used for the compiled executable. Defaults to None.
+        disable_console (bool, optional): Whether to disable the console window for the compiled executable. Defaults to True.
+        onefile (bool, optional): Whether to create a single executable file. Defaults to True.
+        file_version (str, optional): The version number to be assigned to the compiled executable. Defaults to "1".
+        outputdir (Union[str, None], optional): The path to the directory where the compiled executable will be saved. Defaults to None.
+        addfiles (Union[list, None], optional): A list of files to be included in the compiled executable. Defaults to None.
+        delete_onefile_temp (bool, optional): Whether to delete the temporary directory for the single executable file. Defaults to False.
+        needs_admin (bool, optional): Whether the compiled executable requires administrative privileges to run. Defaults to False.
+        relativefolderinapps (Union[None, str], optional): The relative folder path to be used for the compiled executable. Defaults to None.
+        arguments2add (str, optional): Additional arguments to be passed to the Nuitka compiler. Defaults to "".
+
+    Returns:
+        str: The command used to compile the Python file.
 ```
-
-```python
-from nutikacompile import compile_with_nuitka
-# creates the command line and executes it in a new console
-wholecommand = compile_with_nuitka(
-    pyfile=r"C:\ProgramData\anaconda3\envs\adda\secretsubprocess.py",
-    icon=r"C:\Users\hansc\Pictures\radiobutton.png",
-    disable_console=True,
-    file_version="1.0.0.0",
-    onefile=True,
-    outputdir="c:\\compiledapptest",
-    addfiles=[
-        r"C:\ProgramData\anaconda3\envs\adda\convertpic2ico.exe",  # output: compiledapptest/convertpic2ico.exe
-        r"C:\ProgramData\anaconda3\envs\adda\pi2\README.MD",  # output: compiledapptest/pi2/README.MD
-    ],
-    delete_onefile_temp=False,  # creates a permanent cache folder
-    needs_admin=True,
-)
-print(wholecommand)
-
-# The function creates and executes this command: 
-start "" "C:\ProgramData\anaconda3\envs\adda\python.exe" -m nuitka C:/ProgramData/anaconda3/envs/adda/secretsubprocess.py --assume-yes-for-downloads --output-dir=c:/compiledapptest --windows-disable-console --onefile --windows-icon-from-ico=C:/Users/hansc/AppData/Local/Temp/tmpb4w1z8d9.ico --include-data-files=C:/Users/hansc/AppData/Local/Temp/tmpb4i48w8_=.//=**/*.* --windows-uac-admin --file-version=1.0.0.0 --onefile-tempdir-spec=%CACHE_DIR%/nutikacompile/1.0.0.0
-
-
-
-compile_with_nuitka(pyfile: str, icon: Optional[str] = None, disable_console: bool = True, onefile: bool = True, file_version: str = '1', outputdir: Optional[str] = None, addfiles: Optional[list] = None, delete_onefile_temp=False, needs_admin=False) -> str
-    Compiles a Python file using Nuitka.
-    
-    Args:
-        pyfile (str): The path to the Python file to be compiled.
-        icon (Union[str, None], optional): The path to the icon file to be used for the compiled executable, all formats that PIL can read are fine. Defaults to None.
-        disable_console (bool, optional): Whether to disable the console window for the compiled executable. Defaults to True.
-        onefile (bool, optional): Whether to create a single executable file. Defaults to True.
-        file_version (str, optional): The version number to be assigned to the compiled executable.
-                                       File version to use in version information. Must be a
-                                        sequence of up to 4 numbers, e.g. 1.0 or 1.0.0.0, no
-                                        more digits are allowed, no strings are allowed. Defaults to "1".
-    
-        outputdir (Union[str, None], optional): The path to the directory where the compiled executable will be saved. Defaults to None.
-        addfiles (Union[list, None], optional): A list of files to be included in the compiled executable. Defaults to None.
-        delete_onefile_temp (bool, optional): Whether to delete the temporary directory created for the single executable file. Defaults to False.
-        needs_admin (bool, optional): Whether the compiled executable requires administrative privileges to run. Defaults to False.
-    
-    Returns:
-        str: The command used to compile the Python file.
-```
```

### Comparing `nutikacompile-0.11/nutikacompile/LICENSE` & `nutikacompile-0.12/nutikacompile/LICENSE`

 * *Files identical despite different names*

### Comparing `nutikacompile-0.11/nutikacompile/README.MD` & `nutikacompile-0.12/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,29 +24,38 @@
 )
 print(wholecommand)
 
 # The function creates and executes this command: 
 start "" "C:\ProgramData\anaconda3\envs\adda\python.exe" -m nuitka C:/ProgramData/anaconda3/envs/adda/secretsubprocess.py --assume-yes-for-downloads --output-dir=c:/compiledapptest --windows-disable-console --onefile --windows-icon-from-ico=C:/Users/hansc/AppData/Local/Temp/tmpb4w1z8d9.ico --include-data-files=C:/Users/hansc/AppData/Local/Temp/tmpb4i48w8_=.//=**/*.* --windows-uac-admin --file-version=1.0.0.0 --onefile-tempdir-spec=%CACHE_DIR%/nutikacompile/1.0.0.0
 
 
-
-compile_with_nuitka(pyfile: str, icon: Optional[str] = None, disable_console: bool = True, onefile: bool = True, file_version: str = '1', outputdir: Optional[str] = None, addfiles: Optional[list] = None, delete_onefile_temp=False, needs_admin=False) -> str
+compile_with_nuitka(
+    pyfile: str,
+    icon: Union[str, None] = None,
+    disable_console: bool = True,
+    onefile: bool = True,
+    file_version: str = "1",
+    outputdir: Union[str, None] = None,
+    addfiles: Union[list, None] = None,
+    delete_onefile_temp: bool = False,
+    needs_admin: bool = False,
+    relativefolderinapps: Union[None, str] = None,
+    arguments2add: str = "",
+) -> str
     Compiles a Python file using Nuitka.
-    
+
     Args:
         pyfile (str): The path to the Python file to be compiled.
-        icon (Union[str, None], optional): The path to the icon file to be used for the compiled executable, all formats that PIL can read are fine. Defaults to None.
+        icon (Union[str, None], optional): The path to the icon file to be used for the compiled executable. Defaults to None.
         disable_console (bool, optional): Whether to disable the console window for the compiled executable. Defaults to True.
         onefile (bool, optional): Whether to create a single executable file. Defaults to True.
-        file_version (str, optional): The version number to be assigned to the compiled executable.
-                                       File version to use in version information. Must be a
-                                        sequence of up to 4 numbers, e.g. 1.0 or 1.0.0.0, no
-                                        more digits are allowed, no strings are allowed. Defaults to "1".
-    
+        file_version (str, optional): The version number to be assigned to the compiled executable. Defaults to "1".
         outputdir (Union[str, None], optional): The path to the directory where the compiled executable will be saved. Defaults to None.
         addfiles (Union[list, None], optional): A list of files to be included in the compiled executable. Defaults to None.
-        delete_onefile_temp (bool, optional): Whether to delete the temporary directory created for the single executable file. Defaults to False.
+        delete_onefile_temp (bool, optional): Whether to delete the temporary directory for the single executable file. Defaults to False.
         needs_admin (bool, optional): Whether the compiled executable requires administrative privileges to run. Defaults to False.
-    
+        relativefolderinapps (Union[None, str], optional): The relative folder path to be used for the compiled executable. Defaults to None.
+        arguments2add (str, optional): Additional arguments to be passed to the Nuitka compiler. Defaults to "".
+
     Returns:
         str: The command used to compile the Python file.
 ```
```

### Comparing `nutikacompile-0.11/nutikacompile/__init__.py` & `nutikacompile-0.12/nutikacompile/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,35 +98,34 @@
     pyfile: str,
     icon: Union[str, None] = None,
     disable_console: bool = True,
     onefile: bool = True,
     file_version: str = "1",
     outputdir: Union[str, None] = None,
     addfiles: Union[list, None] = None,
-    delete_onefile_temp=False,
-    needs_admin=False,
-    relativefolderinapps=None,
+    delete_onefile_temp: bool = False,
+    needs_admin: bool = False,
+    relativefolderinapps: Union[None, str] = None,
+    arguments2add: str = "",
 ) -> str:
-    r"""
+    """
     Compiles a Python file using Nuitka.
 
     Args:
         pyfile (str): The path to the Python file to be compiled.
-        icon (Union[str, None], optional): The path to the icon file to be used for the compiled executable, all formats that PIL can read are fine. Defaults to None.
+        icon (Union[str, None], optional): The path to the icon file to be used for the compiled executable. Defaults to None.
         disable_console (bool, optional): Whether to disable the console window for the compiled executable. Defaults to True.
         onefile (bool, optional): Whether to create a single executable file. Defaults to True.
-        file_version (str, optional): The version number to be assigned to the compiled executable.
-                                       File version to use in version information. Must be a
-                                        sequence of up to 4 numbers, e.g. 1.0 or 1.0.0.0, no
-                                        more digits are allowed, no strings are allowed. Defaults to "1".
-
+        file_version (str, optional): The version number to be assigned to the compiled executable. Defaults to "1".
         outputdir (Union[str, None], optional): The path to the directory where the compiled executable will be saved. Defaults to None.
         addfiles (Union[list, None], optional): A list of files to be included in the compiled executable. Defaults to None.
-        delete_onefile_temp (bool, optional): Whether to delete the temporary directory created for the single executable file. Defaults to False.
+        delete_onefile_temp (bool, optional): Whether to delete the temporary directory for the single executable file. Defaults to False.
         needs_admin (bool, optional): Whether the compiled executable requires administrative privileges to run. Defaults to False.
+        relativefolderinapps (Union[None, str], optional): The relative folder path to be used for the compiled executable. Defaults to None.
+        arguments2add (str, optional): Additional arguments to be passed to the Nuitka compiler. Defaults to "".
 
     Returns:
         str: The command used to compile the Python file.
     """
     addtocmd = ""
 
     if outputdir:
@@ -157,15 +156,16 @@
     if not delete_onefile_temp:
         if not relativefolderinapps:
             basename = ".".join(os.path.basename(pyfile).split(".")[:-1])
         else:
             basename = relativefolderinapps.strip('\\" ')
         cdi = f"%CACHE_DIR%/{basename}/{file_version}"
         addtocmd = addtocmd + f" --onefile-tempdir-spec={cdi}"
-
+    if arguments2add:
+        addtocmd = addtocmd + " " + arguments2add.strip()
     backs = "\\"
     forw = "/"
     wholecommand = (
         f'start "" "{sys.executable}" -m nuitka {pyfile.replace(backs, forw)} --standalone --assume-yes-for-downloads'
         + addtocmd
     )
     p = subprocess.Popen(wholecommand, shell=True)
```

### Comparing `nutikacompile-0.11/nutikacompile/thirdparty.json` & `nutikacompile-0.12/nutikacompile/thirdparty.json`

 * *Files identical despite different names*

### Comparing `nutikacompile-0.11/setup.py` & `nutikacompile-0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #change to dict
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.11'
+VERSION = '0.12'
 DESCRIPTION = "A function that creates the cmd line for nuitka and executes it"
 
 # Setting up
 setup(
     name="nutikacompile",
     version=VERSION,
     license='MIT',
```

