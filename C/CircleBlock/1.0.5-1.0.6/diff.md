# Comparing `tmp/CircleBlock-1.0.5.tar.gz` & `tmp/CircleBlock-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircleBlock-1.0.5.tar", last modified: Sun Apr  9 14:20:27 2023, max compression
+gzip compressed data, was "CircleBlock-1.0.6.tar", last modified: Sun Apr  9 16:48:20 2023, max compression
```

## Comparing `CircleBlock-1.0.5.tar` & `CircleBlock-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 14:20:27.279078 CircleBlock-1.0.5/
--rw-r--r--   0 phil       (501) staff       (20)      386 2023-04-09 14:18:40.000000 CircleBlock-1.0.5/CHANGELOG.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 14:20:27.278131 CircleBlock-1.0.5/CircleBlock.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      370 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       45 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/entry_points.txt
--rw-r--r--   0 phil       (501) staff       (20)       25 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)       18 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.5/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 14:19:08.000000 CircleBlock-1.0.5/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 14:20:27.278895 CircleBlock-1.0.5/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-09 09:32:22.000000 CircleBlock-1.0.5/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 14:20:27.278615 CircleBlock-1.0.5/circleblock/
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 08:43:50.000000 CircleBlock-1.0.5/circleblock/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     4958 2023-04-09 09:22:09.000000 CircleBlock-1.0.5/circleblock/changer.py
--rw-r--r--   0 phil       (501) staff       (20)     3156 2023-04-09 14:17:55.000000 CircleBlock-1.0.5/circleblock/cli.py
--rw-r--r--   0 phil       (501) staff       (20)      983 2023-04-09 13:59:02.000000 CircleBlock-1.0.5/circleblock/watcher.py
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 14:20:27.279121 CircleBlock-1.0.5/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     1021 2023-04-09 14:19:24.000000 CircleBlock-1.0.5/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 14:20:27.278736 CircleBlock-1.0.5/tests/
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 13:11:03.000000 CircleBlock-1.0.5/tests/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 16:48:20.226320 CircleBlock-1.0.6/
+-rw-r--r--   0 phil       (501) staff       (20)      411 2023-04-09 16:48:10.000000 CircleBlock-1.0.6/CHANGELOG.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 16:48:20.225623 CircleBlock-1.0.6/CircleBlock.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      328 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       45 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/entry_points.txt
+-rw-r--r--   0 phil       (501) staff       (20)       25 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.6/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 14:19:08.000000 CircleBlock-1.0.6/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 16:48:20.226189 CircleBlock-1.0.6/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-09 09:32:22.000000 CircleBlock-1.0.6/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 16:48:20.226011 CircleBlock-1.0.6/circleblock/
+-rw-r--r--   0 phil       (501) staff       (20)     4729 2023-04-09 16:45:25.000000 CircleBlock-1.0.6/circleblock/changer.py
+-rw-r--r--   0 phil       (501) staff       (20)     3156 2023-04-09 14:52:09.000000 CircleBlock-1.0.6/circleblock/cli.py
+-rw-r--r--   0 phil       (501) staff       (20)      983 2023-04-09 13:59:02.000000 CircleBlock-1.0.6/circleblock/watcher.py
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 16:48:20.226372 CircleBlock-1.0.6/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     1021 2023-04-09 16:47:41.000000 CircleBlock-1.0.6/setup.py
```

### Comparing `CircleBlock-1.0.5/CircleBlock.egg-info/PKG-INFO` & `CircleBlock-1.0.6/CircleBlock.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.5/LICENSE` & `CircleBlock-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.5/PKG-INFO` & `CircleBlock-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.5/README.md` & `CircleBlock-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.5/circleblock/changer.py` & `CircleBlock-1.0.6/circleblock/changer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import importlib.machinery
 import inspect
 from typing import Tuple, List
 
+import typer
 from watchdog.events import FileSystemEvent, FileSystemEventHandler
 
 
 def _is_external(module, obj) -> bool:
     """
     Check if the object is imported from an external module.
 
@@ -33,26 +34,30 @@
 
 def _get_exports(module_path: str) -> Tuple[str, list[str]]:
     """
     Get a list of exportable functions within a module.
 
     모듈 내 내보낼 수 있는 함수 목록을 가져옴.
     """
-    module_name = os.path.basename(module_path).replace('.py', '')
-    loader = importlib.machinery.SourceFileLoader(module_name, module_path)
-    module = loader.load_module()
-
-    exports = [
-        attr for attr in dir(module)
-        if all([
-            not attr.startswith('_'),
-            not _is_external(module, getattr(module, attr)),
-            _is_exportable(getattr(module, attr))
-        ])
-    ]
+    try:
+        module_name = os.path.basename(module_path).replace('.py', '')
+        loader = importlib.machinery.SourceFileLoader(module_name, module_path)
+        module = loader.load_module()
+
+        exports = [
+            attr for attr in dir(module)
+            if all([
+                not attr.startswith('_'),
+                not _is_external(module, getattr(module, attr)),
+                _is_exportable(getattr(module, attr))
+            ])
+        ]
+    except Exception as e:
+        typer.echo(f'Error while importing {module_path}: {e}')
+        return '', []
     return module_name, exports
 
 
 def _get_exports_str(module_name: str, exports: List[str], imports: list) -> None:
     if not exports:
         return
     exports = ',\n'.join([f'    {export} as {module_name}_{export}' for export in exports])
@@ -100,39 +105,25 @@
         Check if the event is valid.
 
         유효한 이벤트인지 확인.
         """
         sl = ['.', '_']
         return all([
             not event.is_directory,
-            not any([*[filename.startswith(i) for i in sl], not event.src_path.endswith('.py')]),
+            not any([*[filename.startswith(i) for i in sl], not filename.endswith('.py')]),
+            dirname != os.path.dirname(os.path.abspath(__file__)),
             dirname != self.project_root,
         ])
 
     def initialize_all_init_files(self):
         """
         Find all the directories and create '__init__.py' files in each directory.
         Also write the import statements for all exportable functions in each package's `__init__.py` file.
 
         모든 디렉토리를 찾아서 각 디렉토리에 '__init__.py' 파일을 생성합니다.
         또한, 각 패키지의 `__init__.py` 파일에 있는 내보낼 수 있는 함수를 import 하는 코드를 작성합니다.
         """
         for root, dirs, files in os.walk(self.project_root):
             for directory in dirs:
                 dir_path = os.path.join(root, directory)
-                init_path = os.path.join(dir_path, '__init__.py')
-                if not os.path.exists(init_path):
-                    open(init_path, 'a').close()
-                imports = self._collect_imports(dir_path, FileSystemEvent(''))
+                imports = self._collect_imports(dir_path, FileSystemEvent(dir_path))
                 _write_imports_to_init_file(dir_path, imports)
-
-    def on_modified(self, event: FileSystemEvent):
-        # TODO: Separate and implement
-        pass
-
-    def on_created(self, event: FileSystemEvent):
-        # TODO: Separate and implement
-        pass
-
-    def on_deleted(self, event: FileSystemEvent):
-        # TODO: Separate and implement
-        pass
```

### Comparing `CircleBlock-1.0.5/circleblock/cli.py` & `CircleBlock-1.0.6/circleblock/cli.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.5/circleblock/watcher.py` & `CircleBlock-1.0.6/circleblock/watcher.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.5/setup.py` & `CircleBlock-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CircleBlock',
-    version='1.0.5',
+    version='1.0.6',
     description='Python package for creating circle-themed block diagrams',
     author='phil',
     author_email='eightynine01@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'watchdog',
```

