# Comparing `tmp/CircleBlock-1.0.2.tar.gz` & `tmp/CircleBlock-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircleBlock-1.0.2.tar", last modified: Sun Apr  9 08:56:21 2023, max compression
+gzip compressed data, was "CircleBlock-1.0.3.tar", last modified: Sun Apr  9 13:17:07 2023, max compression
```

## Comparing `CircleBlock-1.0.2.tar` & `CircleBlock-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 08:56:21.477748 CircleBlock-1.0.2/
--rw-r--r--   0 phil       (501) staff       (20)      364 2023-04-09 05:40:57.000000 CircleBlock-1.0.2/CHANGELOG.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 08:56:21.476822 CircleBlock-1.0.2/CircleBlock.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      603 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      360 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       53 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/entry_points.txt
--rw-r--r--   0 phil       (501) staff       (20)       32 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)       12 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.2/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 08:39:25.000000 CircleBlock-1.0.2/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)      603 2023-04-09 08:56:21.477553 CircleBlock-1.0.2/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1959 2023-04-09 07:29:41.000000 CircleBlock-1.0.2/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 08:56:21.477380 CircleBlock-1.0.2/circleblock/
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 08:43:50.000000 CircleBlock-1.0.2/circleblock/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     4927 2023-04-09 08:42:09.000000 CircleBlock-1.0.2/circleblock/changer.py
--rw-r--r--   0 phil       (501) staff       (20)     4319 2023-04-09 08:53:58.000000 CircleBlock-1.0.2/circleblock/circleblock.py
--rw-r--r--   0 phil       (501) staff       (20)     1209 2023-04-09 08:20:47.000000 CircleBlock-1.0.2/circleblock/watcher.py
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 08:56:21.477791 CircleBlock-1.0.2/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      947 2023-04-09 08:51:09.000000 CircleBlock-1.0.2/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:17:07.350616 CircleBlock-1.0.3/
+-rw-r--r--   0 phil       (501) staff       (20)      386 2023-04-09 09:29:13.000000 CircleBlock-1.0.3/CHANGELOG.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:17:07.349743 CircleBlock-1.0.3/CircleBlock.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      358 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       33 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/entry_points.txt
+-rw-r--r--   0 phil       (501) staff       (20)       32 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)       18 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.3/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      167 2023-04-09 13:11:42.000000 CircleBlock-1.0.3/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 13:17:07.350424 CircleBlock-1.0.3/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-09 09:32:22.000000 CircleBlock-1.0.3/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:17:07.350109 CircleBlock-1.0.3/circleblock/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 08:43:50.000000 CircleBlock-1.0.3/circleblock/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     4958 2023-04-09 09:22:09.000000 CircleBlock-1.0.3/circleblock/changer.py
+-rw-r--r--   0 phil       (501) staff       (20)     1209 2023-04-09 08:20:47.000000 CircleBlock-1.0.3/circleblock/watcher.py
+-rw-r--r--   0 phil       (501) staff       (20)     3351 2023-04-09 13:13:01.000000 CircleBlock-1.0.3/cli.py
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 13:17:07.350659 CircleBlock-1.0.3/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     1027 2023-04-09 13:12:19.000000 CircleBlock-1.0.3/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:17:07.350248 CircleBlock-1.0.3/tests/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 13:11:03.000000 CircleBlock-1.0.3/tests/__init__.py
```

### Comparing `CircleBlock-1.0.2/CircleBlock.egg-info/PKG-INFO` & `CircleBlock-1.0.3/CircleBlock.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 License-File: LICENSE
```

### Comparing `CircleBlock-1.0.2/LICENSE` & `CircleBlock-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.2/PKG-INFO` & `CircleBlock-1.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 License-File: LICENSE
```

### Comparing `CircleBlock-1.0.2/circleblock/changer.py` & `CircleBlock-1.0.3/circleblock/changer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import importlib.machinery
 import inspect
+from typing import Tuple, List
 
 from watchdog.events import FileSystemEvent, FileSystemEventHandler
 
 
 def _is_external(module, obj) -> bool:
     """
     Check if the object is imported from an external module.
@@ -26,15 +27,15 @@
     Check if the object is exportable (function or class).
 
     객체가 내보낼 수 있는지 (함수 또는 클래스) 확인.
     """
     return (inspect.isfunction(obj) or inspect.isclass(obj)) and inspect.getmodule(obj) != obj.__class__
 
 
-def _get_exports(module_path: str) -> tuple[str, list[str]]:
+def _get_exports(module_path: str) -> Tuple[str, list[str]]:
     """
     Get a list of exportable functions within a module.
 
     모듈 내 내보낼 수 있는 함수 목록을 가져옴.
     """
     module_name = os.path.basename(module_path).replace('.py', '')
     loader = importlib.machinery.SourceFileLoader(module_name, module_path)
@@ -47,23 +48,23 @@
             not _is_external(module, getattr(module, attr)),
             _is_exportable(getattr(module, attr))
         ])
     ]
     return module_name, exports
 
 
-def _get_exports_str(module_name: str, exports: list[str], imports: list) -> None:
+def _get_exports_str(module_name: str, exports: List[str], imports: list) -> None:
     if not exports:
         return
     exports = ',\n'.join([f'    {export} as {module_name}_{export}' for export in exports])
     line_templates = f'from .{module_name} import (\n{exports}\n)\n'
     imports.append(line_templates)
 
 
-def _write_imports_to_init_file(dirname, imports: list[str]) -> None:
+def _write_imports_to_init_file(dirname, imports: List[str]) -> None:
     """
     Write importable functions to the circleblock_cli.py file in the given directory.
 
     주어진 디렉토리의 circleblock_cli.py 파일에 가져올 함수들을 작성.
     """
     if not imports:
         return
```

### Comparing `CircleBlock-1.0.2/circleblock/watcher.py` & `CircleBlock-1.0.3/circleblock/watcher.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.2/setup.py` & `CircleBlock-1.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CircleBlock',
-    version='1.0.2',
+    version='1.0.3',
     description='Python package for creating circle-themed block diagrams',
     author='phil',
     author_email='eightynine01@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'watchdog',
         'loguru',
-        'click',
+        'typer',
         'daemonize'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
-            'ccbk=circleblock.circleblock:run'
+            'ccbk=cli:app'
         ]
     }
 )
```

