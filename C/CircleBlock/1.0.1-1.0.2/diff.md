# Comparing `tmp/CircleBlock-1.0.1.tar.gz` & `tmp/CircleBlock-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircleBlock-1.0.1.tar", last modified: Sun Apr  9 07:57:31 2023, max compression
+gzip compressed data, was "CircleBlock-1.0.2.tar", last modified: Sun Apr  9 08:56:21 2023, max compression
```

## Comparing `CircleBlock-1.0.1.tar` & `CircleBlock-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 07:57:31.293069 CircleBlock-1.0.1/
--rw-r--r--   0 phil       (501) staff       (20)      364 2023-04-09 05:40:57.000000 CircleBlock-1.0.1/CHANGELOG.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 07:57:31.292235 CircleBlock-1.0.1/CircleBlock.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      603 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      355 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       36 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/entry_points.txt
--rw-r--r--   0 phil       (501) staff       (20)       22 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.1/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 06:09:13.000000 CircleBlock-1.0.1/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)      603 2023-04-09 07:57:31.292940 CircleBlock-1.0.1/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1959 2023-04-09 07:29:41.000000 CircleBlock-1.0.1/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 07:57:31.292771 CircleBlock-1.0.1/circleblock/
--rw-r--r--   0 phil       (501) staff       (20)     4904 2023-04-09 07:03:29.000000 CircleBlock-1.0.1/circleblock/changer.py
--rw-r--r--   0 phil       (501) staff       (20)     3421 2023-04-09 07:02:41.000000 CircleBlock-1.0.1/circleblock/circleblock.py
--rw-r--r--   0 phil       (501) staff       (20)      833 2023-04-09 07:49:56.000000 CircleBlock-1.0.1/circleblock/cli.py
--rw-r--r--   0 phil       (501) staff       (20)     1197 2023-04-09 06:12:22.000000 CircleBlock-1.0.1/circleblock/watcher.py
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 07:57:31.293113 CircleBlock-1.0.1/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      909 2023-04-09 07:55:28.000000 CircleBlock-1.0.1/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 08:56:21.477748 CircleBlock-1.0.2/
+-rw-r--r--   0 phil       (501) staff       (20)      364 2023-04-09 05:40:57.000000 CircleBlock-1.0.2/CHANGELOG.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 08:56:21.476822 CircleBlock-1.0.2/CircleBlock.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      603 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      360 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       53 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/entry_points.txt
+-rw-r--r--   0 phil       (501) staff       (20)       32 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)       12 2023-04-09 08:56:21.000000 CircleBlock-1.0.2/CircleBlock.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.2/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 08:39:25.000000 CircleBlock-1.0.2/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)      603 2023-04-09 08:56:21.477553 CircleBlock-1.0.2/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1959 2023-04-09 07:29:41.000000 CircleBlock-1.0.2/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 08:56:21.477380 CircleBlock-1.0.2/circleblock/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 08:43:50.000000 CircleBlock-1.0.2/circleblock/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     4927 2023-04-09 08:42:09.000000 CircleBlock-1.0.2/circleblock/changer.py
+-rw-r--r--   0 phil       (501) staff       (20)     4319 2023-04-09 08:53:58.000000 CircleBlock-1.0.2/circleblock/circleblock.py
+-rw-r--r--   0 phil       (501) staff       (20)     1209 2023-04-09 08:20:47.000000 CircleBlock-1.0.2/circleblock/watcher.py
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 08:56:21.477791 CircleBlock-1.0.2/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      947 2023-04-09 08:51:09.000000 CircleBlock-1.0.2/setup.py
```

### Comparing `CircleBlock-1.0.1/CircleBlock.egg-info/PKG-INFO` & `CircleBlock-1.0.2/CircleBlock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.1/LICENSE` & `CircleBlock-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.1/PKG-INFO` & `CircleBlock-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.1/README.md` & `CircleBlock-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.1/circleblock/changer.py` & `CircleBlock-1.0.2/circleblock/changer.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,17 @@
     exports = ',\n'.join([f'    {export} as {module_name}_{export}' for export in exports])
     line_templates = f'from .{module_name} import (\n{exports}\n)\n'
     imports.append(line_templates)
 
 
 def _write_imports_to_init_file(dirname, imports: list[str]) -> None:
     """
-    Write importable functions to the cli.py file in the given directory.
+    Write importable functions to the circleblock_cli.py file in the given directory.
 
-    주어진 디렉토리의 cli.py 파일에 가져올 함수들을 작성.
+    주어진 디렉토리의 circleblock_cli.py 파일에 가져올 함수들을 작성.
     """
     if not imports:
         return
     with open(os.path.join(dirname, '__init__.py'), 'w', encoding='UTF8') as f:
         f.writelines(imports)
 
 
@@ -103,15 +103,15 @@
         sl = ['.', '_']
         return all([
             not event.is_directory,
             not any([*[filename.startswith(i) for i in sl], not event.src_path.endswith('.py')]),
             dirname != self.project_root,
         ])
 
-    def _initialize_all_init_files(self):
+    def initialize_all_init_files(self):
         """
         Find all the directories and create '__init__.py' files in each directory.
         Also write the import statements for all exportable functions in each package's `__init__.py` file.
 
         모든 디렉토리를 찾아서 각 디렉토리에 '__init__.py' 파일을 생성합니다.
         또한, 각 패키지의 `__init__.py` 파일에 있는 내보낼 수 있는 함수를 import 하는 코드를 작성합니다.
         """
```

### Comparing `CircleBlock-1.0.1/circleblock/circleblock.py` & `CircleBlock-1.0.2/circleblock/circleblock.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import os
 import sys
 from typing import Optional
 
+import click
+from daemonize import Daemonize
 from loguru import logger
 
-from changer import InitFileUpdater
-from watcher import FileWatcher
+from .changer import InitFileUpdater
+from .watcher import FileWatcher
 
 
 class CircleBlock:
     """
     CircleBlock은 프로젝트 루트 디렉토리 내의 파일 시스템을 감시하는 클래스입니다.
     CircleBlock is a class that monitors the file system in the project root directory.
     """
@@ -21,15 +24,15 @@
         :param project_root: 프로젝트 루트 디렉토리 경로 (Project root directory path)
         """
         self.project_root = project_root
         self.updater = InitFileUpdater(project_root)
         self.watcher = FileWatcher(project_root, self.updater)
         if not init:
             return
-        self.updater._initialize_all_init_files()
+        self.updater.initialize_all_init_files()
 
     def start_watching(self):
         """
         파일 시스템 감시를 시작합니다.
         Start monitoring the file system.
         """
         self.watcher.start_watching()
@@ -63,23 +66,65 @@
         format=default_msg_fmt
     )
     circleblock = CircleBlock(project_root)
     logger.info('CircleBlock 시작합니다. Start CircleBlock.')
     logger.info(f'프로젝트 루트 디렉토리 경로: {project_root} Project root directory path: {project_root}')
     circleblock.start_watching()
 
-#
-# def init_circleblock(project_root: str):
-#     """
-#     Add import statements for all exportable functions in each package's `__init__.py` file.
-#
-#     모든 패키지의 `__init__.py` 파일에 있는 내보낼 수 있는 함수를 import 하는 코드를 추가합니다.
-#     """
-#     for dirpath, dirnames, filenames in os.walk(project_root):
-#         if '__init__.py' in filenames:
-#             init_file = os.path.join(dirpath, '__init__.py')
-#             if os.path.exists(os.path.join(dirpath, 'circleblock')):
-#                 updater = InitFileUpdater(project_root)
-#                 imports = updater._collect_imports(dirpath, None)
-#                 if imports:
-#                     with open(init_file, 'a', encoding='UTF8') as f:
-#                         f.write('\n'.join(imports))
+
+@click.group(name='ccbk')
+@click.option(
+    '--project-root',
+    '-p',
+    default=os.getcwd(),
+    help='Project root directory path (default: current directory) | 프로젝트 루트 디렉토리 경로 (default: 실행위치)'
+)
+@click.option(
+    '--log-level',
+    '-l',
+    default='INFO',
+    help='Log level (default: INFO) | 로그 레벨 (default: INFO)'
+)
+@click.option(
+    '--init',
+    '-i',
+    is_flag=True,
+    default=False,
+    help='Initialize and update all __init__.py files in the project | 프로젝트 내 모든 __init__.py 파일을 초기화 및 업데이트'
+)
+@click.pass_context
+def cli(ctx, project_root, log_level, init):
+    msg_left = '[<level>{level}|</level><green>{time:YYYY-MM-DD HH:mm:ss}</green>]'
+    msg_center = '[<cyan>{name}</cyan>:<cyan>{function}</cyan>:<red>{line}</red>]'
+    msg_right = '<level>{message}</level>'
+    default_msg_fmt = f'{msg_left}{msg_center} {msg_right}'
+    logger.remove()
+    logger.add(
+        sink=sys.stderr if log_level == 'DEBUG' else sys.stdout,
+        level=log_level,
+        format=default_msg_fmt
+    )
+    ctx.obj = CircleBlock(project_root, init)
+
+
+@click.command()
+@click.pass_obj
+def run(cb: CircleBlock, daemon: bool = True):
+    if daemon:
+        def start():
+            cb.start_watching()
+
+        logger.info(f"Starting CircleBlock in daemon mode")
+        daemon = Daemonize(
+            app="CircleBlock",
+            pid=os.path.join(cb.project_root, "CircleBlock.pid"),
+            action=start
+        )
+        daemon.start()
+    else:
+        cb.start_watching()
+
+
+@click.command()
+@click.pass_obj
+def stop(cb: CircleBlock):
+    cb.stop_watching()
```

### Comparing `CircleBlock-1.0.1/circleblock/watcher.py` & `CircleBlock-1.0.2/circleblock/watcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.project_root = project_root
         self.changer = changer
         self.observer = Observer()
         atexit.register(log_exit_message)
 
     def start_watching(self):
         """
-        변경 사항을 감시하기 위해 루트 디렉토리를 감시하고 cli.py 파일을 생성/업데이트합니다.
+        변경 사항을 감시하기 위해 루트 디렉토리를 감시하고 circleblock_cli.py 파일을 생성/업데이트합니다.
         """
         logger.debug('변경 사항 감시 시작...')
         logger.debug(f'프로젝트 루트: {self.project_root}')
 
         self.observer.schedule(self.changer, self.project_root, recursive=True)
         self.observer.start()
         signal.signal(signal.SIGINT, lambda *args, **kwargs: self.stop_watching())
```

### Comparing `CircleBlock-1.0.1/setup.py` & `CircleBlock-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CircleBlock',
-    version='1.0.1',
+    version='1.0.2',
     description='Python package for creating circle-themed block diagrams',
     author='phil',
     author_email='eightynine01@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'watchdog',
         'loguru',
-        'click'
+        'click',
+        'daemonize'
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
     ],
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
-            'ccbk=.cli:start'
+            'ccbk=circleblock.circleblock:run'
         ]
     }
 )
```

