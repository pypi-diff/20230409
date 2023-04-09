# Comparing `tmp/gigapixel-1.2.0.tar.gz` & `tmp/gigapixel-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigapixel-1.2.0.tar", last modified: Tue Mar 28 10:42:22 2023, max compression
+gzip compressed data, was "gigapixel-1.3.0.tar", last modified: Sun Apr  9 11:47:45 2023, max compression
```

## Comparing `gigapixel-1.2.0.tar` & `gigapixel-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:42:22.945087 gigapixel-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-28 10:42:01.000000 gigapixel-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-28 10:42:22.945087 gigapixel-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-28 10:42:01.000000 gigapixel-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:42:22.945087 gigapixel-1.2.0/gigapixel/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-28 10:42:01.000000 gigapixel-1.2.0/gigapixel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-28 10:42:01.000000 gigapixel-1.2.0/gigapixel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-03-28 10:42:01.000000 gigapixel-1.2.0/gigapixel/gigapixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-28 10:42:01.000000 gigapixel-1.2.0/gigapixel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:42:22.945087 gigapixel-1.2.0/gigapixel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-28 10:42:22.000000 gigapixel-1.2.0/gigapixel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-28 10:42:22.000000 gigapixel-1.2.0/gigapixel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 10:42:22.000000 gigapixel-1.2.0/gigapixel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-28 10:42:22.000000 gigapixel-1.2.0/gigapixel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-28 10:42:22.000000 gigapixel-1.2.0/gigapixel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-28 10:42:01.000000 gigapixel-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-28 10:42:22.945087 gigapixel-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-28 10:42:01.000000 gigapixel-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:47:45.346704 gigapixel-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 11:47:35.000000 gigapixel-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-09 11:47:45.346704 gigapixel-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-09 11:47:35.000000 gigapixel-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:47:45.346704 gigapixel-1.3.0/gigapixel/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 11:47:35.000000 gigapixel-1.3.0/gigapixel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-09 11:47:35.000000 gigapixel-1.3.0/gigapixel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-09 11:47:35.000000 gigapixel-1.3.0/gigapixel/gigapixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-09 11:47:35.000000 gigapixel-1.3.0/gigapixel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:47:45.346704 gigapixel-1.3.0/gigapixel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-09 11:47:45.000000 gigapixel-1.3.0/gigapixel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-09 11:47:45.000000 gigapixel-1.3.0/gigapixel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:47:45.000000 gigapixel-1.3.0/gigapixel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-09 11:47:45.000000 gigapixel-1.3.0/gigapixel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 11:47:45.000000 gigapixel-1.3.0/gigapixel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-09 11:47:35.000000 gigapixel-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 11:47:45.346704 gigapixel-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-09 11:47:35.000000 gigapixel-1.3.0/setup.py
```

### Comparing `gigapixel-1.2.0/LICENSE` & `gigapixel-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gigapixel-1.2.0/PKG-INFO` & `gigapixel-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigapixel
-Version: 1.2.0
+Version: 1.3.0
 Summary: Topaz Gigapixel AI automation tool
 Home-page: https://github.com/TimNekk/Gigapixel
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -61,30 +61,30 @@
 
 ## Usage
 
 1. Create `Gigapixel` instance
 2. Use `.process()` method to enhance image
 
 ```python
-from gigapixel import Gigapixel, Scale, Mode
+from gigapixel import Gigapixel, Scale, Mode, OutputFormat
 from pathlib import Path
 
 # Path to Gigapixel executable file.
 exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz Gigapixel AI.exe')
 
 # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg)
 # You should set same value inside Gigapixel (File -> Preferences -> Default filename suffix).
 output_suffix = '-gigapixel'
 
 # Create Gigapixel instance.
 app = Gigapixel(exe_path, output_suffix)
 
 # Process image.
 image = Path('path/to/image.jpg')
-output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True)
+output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
 
 # Print output path.
 print(output_path)
 ```
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gigapixel Version: 1.2.0 Summary: Topaz Gigapixel
+Metadata-Version: 2.1 Name: gigapixel Version: 1.3.0 Summary: Topaz Gigapixel
 AI automation tool Home-page: https://github.com/TimNekk/Gigapixel Author:
 TimNekk Author-email: herew26@gmail.com License: Apache License, Version 2.0,
 see LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
@@ -19,19 +19,20 @@
                   *** Topaz Gigapixel AI automation tool ***
                            [PyPI] [Python 3] [Tests]
      Requirements â¢ Installation â¢ Usage â¢ Contributing â¢ License
 ## Requirements [Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)
 **v6** of **newer** required ## Installation Install the current version with
 [PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -U gigapixel
 ``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()` method to
-enhance image ```python from gigapixel import Gigapixel, Scale, Mode from
-pathlib import Path # Path to Gigapixel executable file. exe_path = Path('C:
-\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz Gigapixel AI.exe') #
-Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) # You should set same
-value inside Gigapixel (File -> Preferences -> Default filename suffix).
-output_suffix = '-gigapixel' # Create Gigapixel instance. app = Gigapixel
-(exe_path, output_suffix) # Process image. image = Path('path/to/image.jpg')
-output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD,
-delete_from_history=True) # Print output path. print(output_path) ``` ##
-Contributing Bug reports and/or pull requests are welcome ## License The module
-is available as open source under the terms of the [Apache License, Version
-2.0](https://opensource.org/licenses/Apache-2.0)
+enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
+OutputFormat from pathlib import Path # Path to Gigapixel executable file.
+exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz
+Gigapixel AI.exe') # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) #
+You should set same value inside Gigapixel (File -> Preferences -> Default
+filename suffix). output_suffix = '-gigapixel' # Create Gigapixel instance. app
+= Gigapixel(exe_path, output_suffix) # Process image. image = Path('path/to/
+image.jpg') output_path = app.process(image, scale=Scale.X2,
+mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG) #
+Print output path. print(output_path) ``` ## Contributing Bug reports and/or
+pull requests are welcome ## License The module is available as open source
+under the terms of the [Apache License, Version 2.0](https://opensource.org/
+licenses/Apache-2.0)
```

### Comparing `gigapixel-1.2.0/README.md` & `gigapixel-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,30 +36,30 @@
 
 ## Usage
 
 1. Create `Gigapixel` instance
 2. Use `.process()` method to enhance image
 
 ```python
-from gigapixel import Gigapixel, Scale, Mode
+from gigapixel import Gigapixel, Scale, Mode, OutputFormat
 from pathlib import Path
 
 # Path to Gigapixel executable file.
 exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz Gigapixel AI.exe')
 
 # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg)
 # You should set same value inside Gigapixel (File -> Preferences -> Default filename suffix).
 output_suffix = '-gigapixel'
 
 # Create Gigapixel instance.
 app = Gigapixel(exe_path, output_suffix)
 
 # Process image.
 image = Path('path/to/image.jpg')
-output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True)
+output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
 
 # Print output path.
 print(output_path)
 ```
 
 ## Contributing
```

#### html2text {}

```diff
@@ -5,19 +5,20 @@
                   *** Topaz Gigapixel AI automation tool ***
                            [PyPI] [Python 3] [Tests]
      Requirements â¢ Installation â¢ Usage â¢ Contributing â¢ License
 ## Requirements [Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)
 **v6** of **newer** required ## Installation Install the current version with
 [PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -U gigapixel
 ``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()` method to
-enhance image ```python from gigapixel import Gigapixel, Scale, Mode from
-pathlib import Path # Path to Gigapixel executable file. exe_path = Path('C:
-\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz Gigapixel AI.exe') #
-Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) # You should set same
-value inside Gigapixel (File -> Preferences -> Default filename suffix).
-output_suffix = '-gigapixel' # Create Gigapixel instance. app = Gigapixel
-(exe_path, output_suffix) # Process image. image = Path('path/to/image.jpg')
-output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD,
-delete_from_history=True) # Print output path. print(output_path) ``` ##
-Contributing Bug reports and/or pull requests are welcome ## License The module
-is available as open source under the terms of the [Apache License, Version
-2.0](https://opensource.org/licenses/Apache-2.0)
+enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
+OutputFormat from pathlib import Path # Path to Gigapixel executable file.
+exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz
+Gigapixel AI.exe') # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) #
+You should set same value inside Gigapixel (File -> Preferences -> Default
+filename suffix). output_suffix = '-gigapixel' # Create Gigapixel instance. app
+= Gigapixel(exe_path, output_suffix) # Process image. image = Path('path/to/
+image.jpg') output_path = app.process(image, scale=Scale.X2,
+mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG) #
+Print output path. print(output_path) ``` ## Contributing Bug reports and/or
+pull requests are welcome ## License The module is available as open source
+under the terms of the [Apache License, Version 2.0](https://opensource.org/
+licenses/Apache-2.0)
```

### Comparing `gigapixel-1.2.0/gigapixel/gigapixel.py` & `gigapixel-1.3.0/gigapixel/gigapixel.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,14 +24,24 @@
     STANDARD = "Standard"
     Lines = "Lines"
     ART_AND_CG = "Art & CG"
     LOW_RESOLUTION = "Low Resolution"
     VERY_COMPRESSED = "Very Compressed"
 
 
+class OutputFormat(Enum):
+    PRESERVE_SOURCE_FORMAT = "Preserve Source Format"
+    JPG = "JPG"
+    JPEG = "JPEG"
+    TIF = "TIF"
+    TIFF = "TIFF"
+    PNG = "PNG"
+    DNG = "DNG"
+
+
 class Gigapixel:
     def __init__(self,
                  executable_path: Path,
                  output_suffix: str):
         self._executable_path = executable_path
         self._output_suffix = output_suffix
 
@@ -52,30 +62,57 @@
                 logger.debug("Trying to open photo")
                 self._main_window.set_focus()
                 send_keys('{ESC}^o')
                 clipboard.copy(str(photo_path))
                 send_keys('^v {ENTER}')
 
         @log("Saving photo", "Photo saved", level=Level.DEBUG)
-        def save_photo(self) -> None:
-            send_keys('^S {ENTER}')
+        def save_photo(self, output_format: OutputFormat) -> None:
+            send_keys('^S')
+            self._set_output_format(output_format)
+            send_keys('{ENTER}')
             self._main_window.child_window(title="Cancel Processing", control_type="Button").wait_not('visible',
                                                                                                       timeout=60)
 
         @log("Deleting photo from history", "Photo deleted", level=Level.DEBUG)
         def delete_photo(self) -> None:
             self._main_window.Pane.Button2.click_input()
 
         @log("Setting processing options", "Processing options set", level=Level.DEBUG)
         def set_processing_options(self, scale: Optional[Scale] = None, mode: Optional[Mode] = None) -> None:
             if scale:
                 self._set_scale(scale)
             if mode:
                 self._set_mode(mode)
 
+        def _set_output_format(self, save_format: OutputFormat) -> None:
+            self._main_window.ComboBox.click_input()
+
+            if save_format == OutputFormat.PRESERVE_SOURCE_FORMAT:
+                self._main_window.ListItem.click_input()
+                send_keys('{TAB}')
+            elif save_format == OutputFormat.JPG:
+                self._main_window.ListItem2.click_input()
+                send_keys('{TAB}')
+            elif save_format == OutputFormat.JPEG:
+                self._main_window.ListItem3.click_input()
+                send_keys('{TAB}')
+            elif save_format == OutputFormat.TIF:
+                self._main_window.ListItem4.click_input()
+                send_keys('{TAB} {TAB} {TAB}')
+            elif save_format == OutputFormat.TIFF:
+                self._main_window.ListItem5.click_input()
+                send_keys('{TAB} {TAB} {TAB}')
+            elif save_format == OutputFormat.PNG:
+                self._main_window.ListItem6.click_input()
+                send_keys('{TAB}')
+            elif save_format == OutputFormat.DNG:
+                self._main_window.ListItem7.click_input()
+                send_keys('{TAB}')
+
         def _set_scale(self, scale: Scale):
             if self.scale == scale:
                 return
 
             try:
                 self._main_window.child_window(title=scale.value).click_input()
             except ElementNotFoundError:
@@ -110,36 +147,44 @@
 
     @log("Starting new Gigapixel instance...", "Started new Gigapixel instance: {}", format=(-1,), level=Level.DEBUG)
     def _open_topaz(self) -> Application:
         instance = Application(backend="uia").start(str(self._executable_path)).connect(path=self._executable_path)
         return instance
 
     @log("Checking path: {}", "Path is valid", format=(1,), level=Level.DEBUG)
-    def _check_path(self, path: Path) -> None:
+    def _check_path(self, path: Path, output_format: OutputFormat) -> None:
         if not path.is_file():
             raise NotFile(f"Path is not a file: {path}")
 
-        save_path = self._get_save_path(path)
+        save_path = self._get_save_path(path, output_format)
         if save_path.name in os.listdir(path.parent):
             raise FileAlreadyExists(f"Output file already exists: {save_path}")
 
     @staticmethod
     def _remove_suffix(input_string: str, suffix: str) -> str:
         if suffix and input_string.endswith(suffix):
             return input_string[:-len(suffix)]
         return input_string
 
-    def _get_save_path(self, path: Path) -> Path:
-        return path.parent / (Gigapixel._remove_suffix(path.name, path.suffix) + self._output_suffix + path.suffix)
+    def _get_save_path(self, path: Path, output_format: OutputFormat) -> Path:
+        extension = path.suffix if output_format == OutputFormat.PRESERVE_SOURCE_FORMAT else f".{output_format.value.lower()}"
+        return path.parent / (Gigapixel._remove_suffix(path.name, path.suffix) + self._output_suffix + extension)
 
     @log(start="Starting processing: {}", format=(1,))
     @log(end="Finished processing: {}", format=(1,), level=Level.SUCCESS)
-    def process(self, photo_path: Path, scale: Scale = Scale.X2, mode: Mode = Mode.STANDARD, delete_from_history: bool = True) -> Path:
-        self._check_path(photo_path)
+    def process(self,
+                photo_path: Path,
+                scale: Scale = Scale.X2,
+                mode: Mode = Mode.STANDARD,
+                delete_from_history: bool = True,
+                output_format: OutputFormat = OutputFormat.PRESERVE_SOURCE_FORMAT
+                ) -> Path:
+        self._check_path(photo_path, output_format)
 
         self._app.open_photo(photo_path)
         self._app.set_processing_options(scale, mode)
-        self._app.save_photo()
+        self._app.save_photo(output_format)
+
         if delete_from_history:
             self._app.delete_photo()
 
-        return self._get_save_path(photo_path)
+        return self._get_save_path(photo_path, output_format)
```

### Comparing `gigapixel-1.2.0/gigapixel/logging.py` & `gigapixel-1.3.0/gigapixel/logging.py`

 * *Files identical despite different names*

### Comparing `gigapixel-1.2.0/gigapixel.egg-info/PKG-INFO` & `gigapixel-1.3.0/gigapixel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigapixel
-Version: 1.2.0
+Version: 1.3.0
 Summary: Topaz Gigapixel AI automation tool
 Home-page: https://github.com/TimNekk/Gigapixel
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -61,30 +61,30 @@
 
 ## Usage
 
 1. Create `Gigapixel` instance
 2. Use `.process()` method to enhance image
 
 ```python
-from gigapixel import Gigapixel, Scale, Mode
+from gigapixel import Gigapixel, Scale, Mode, OutputFormat
 from pathlib import Path
 
 # Path to Gigapixel executable file.
 exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz Gigapixel AI.exe')
 
 # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg)
 # You should set same value inside Gigapixel (File -> Preferences -> Default filename suffix).
 output_suffix = '-gigapixel'
 
 # Create Gigapixel instance.
 app = Gigapixel(exe_path, output_suffix)
 
 # Process image.
 image = Path('path/to/image.jpg')
-output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True)
+output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
 
 # Print output path.
 print(output_path)
 ```
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gigapixel Version: 1.2.0 Summary: Topaz Gigapixel
+Metadata-Version: 2.1 Name: gigapixel Version: 1.3.0 Summary: Topaz Gigapixel
 AI automation tool Home-page: https://github.com/TimNekk/Gigapixel Author:
 TimNekk Author-email: herew26@gmail.com License: Apache License, Version 2.0,
 see LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
@@ -19,19 +19,20 @@
                   *** Topaz Gigapixel AI automation tool ***
                            [PyPI] [Python 3] [Tests]
      Requirements â¢ Installation â¢ Usage â¢ Contributing â¢ License
 ## Requirements [Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)
 **v6** of **newer** required ## Installation Install the current version with
 [PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -U gigapixel
 ``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()` method to
-enhance image ```python from gigapixel import Gigapixel, Scale, Mode from
-pathlib import Path # Path to Gigapixel executable file. exe_path = Path('C:
-\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz Gigapixel AI.exe') #
-Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) # You should set same
-value inside Gigapixel (File -> Preferences -> Default filename suffix).
-output_suffix = '-gigapixel' # Create Gigapixel instance. app = Gigapixel
-(exe_path, output_suffix) # Process image. image = Path('path/to/image.jpg')
-output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD,
-delete_from_history=True) # Print output path. print(output_path) ``` ##
-Contributing Bug reports and/or pull requests are welcome ## License The module
-is available as open source under the terms of the [Apache License, Version
-2.0](https://opensource.org/licenses/Apache-2.0)
+enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
+OutputFormat from pathlib import Path # Path to Gigapixel executable file.
+exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz
+Gigapixel AI.exe') # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) #
+You should set same value inside Gigapixel (File -> Preferences -> Default
+filename suffix). output_suffix = '-gigapixel' # Create Gigapixel instance. app
+= Gigapixel(exe_path, output_suffix) # Process image. image = Path('path/to/
+image.jpg') output_path = app.process(image, scale=Scale.X2,
+mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG) #
+Print output path. print(output_path) ``` ## Contributing Bug reports and/or
+pull requests are welcome ## License The module is available as open source
+under the terms of the [Apache License, Version 2.0](https://opensource.org/
+licenses/Apache-2.0)
```

### Comparing `gigapixel-1.2.0/setup.py` & `gigapixel-1.3.0/setup.py`

 * *Files identical despite different names*

