# Comparing `tmp/CircleBlock-1.0.4.tar.gz` & `tmp/CircleBlock-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircleBlock-1.0.4.tar", last modified: Sun Apr  9 13:30:33 2023, max compression
+gzip compressed data, was "CircleBlock-1.0.5.tar", last modified: Sun Apr  9 14:20:27 2023, max compression
```

## Comparing `CircleBlock-1.0.4.tar` & `CircleBlock-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:30:33.133794 CircleBlock-1.0.4/
--rw-r--r--   0 phil       (501) staff       (20)      386 2023-04-09 13:30:17.000000 CircleBlock-1.0.4/CHANGELOG.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:30:33.132800 CircleBlock-1.0.4/CircleBlock.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      370 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       45 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/entry_points.txt
--rw-r--r--   0 phil       (501) staff       (20)       32 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)       18 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.4/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      167 2023-04-09 13:11:42.000000 CircleBlock-1.0.4/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 13:30:33.133595 CircleBlock-1.0.4/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-09 09:32:22.000000 CircleBlock-1.0.4/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:30:33.133309 CircleBlock-1.0.4/circleblock/
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 08:43:50.000000 CircleBlock-1.0.4/circleblock/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     4958 2023-04-09 09:22:09.000000 CircleBlock-1.0.4/circleblock/changer.py
--rw-r--r--   0 phil       (501) staff       (20)     3297 2023-04-09 13:28:04.000000 CircleBlock-1.0.4/circleblock/cli.py
--rw-r--r--   0 phil       (501) staff       (20)      999 2023-04-09 13:24:51.000000 CircleBlock-1.0.4/circleblock/watcher.py
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 13:30:33.133837 CircleBlock-1.0.4/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     1039 2023-04-09 13:29:51.000000 CircleBlock-1.0.4/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:30:33.133432 CircleBlock-1.0.4/tests/
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 13:11:03.000000 CircleBlock-1.0.4/tests/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 14:20:27.279078 CircleBlock-1.0.5/
+-rw-r--r--   0 phil       (501) staff       (20)      386 2023-04-09 14:18:40.000000 CircleBlock-1.0.5/CHANGELOG.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 14:20:27.278131 CircleBlock-1.0.5/CircleBlock.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      370 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       45 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/entry_points.txt
+-rw-r--r--   0 phil       (501) staff       (20)       25 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)       18 2023-04-09 14:20:27.000000 CircleBlock-1.0.5/CircleBlock.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.5/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 14:19:08.000000 CircleBlock-1.0.5/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 14:20:27.278895 CircleBlock-1.0.5/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-09 09:32:22.000000 CircleBlock-1.0.5/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 14:20:27.278615 CircleBlock-1.0.5/circleblock/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 08:43:50.000000 CircleBlock-1.0.5/circleblock/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     4958 2023-04-09 09:22:09.000000 CircleBlock-1.0.5/circleblock/changer.py
+-rw-r--r--   0 phil       (501) staff       (20)     3156 2023-04-09 14:17:55.000000 CircleBlock-1.0.5/circleblock/cli.py
+-rw-r--r--   0 phil       (501) staff       (20)      983 2023-04-09 13:59:02.000000 CircleBlock-1.0.5/circleblock/watcher.py
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 14:20:27.279121 CircleBlock-1.0.5/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     1021 2023-04-09 14:19:24.000000 CircleBlock-1.0.5/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 14:20:27.278736 CircleBlock-1.0.5/tests/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 13:11:03.000000 CircleBlock-1.0.5/tests/__init__.py
```

### Comparing `CircleBlock-1.0.4/CircleBlock.egg-info/PKG-INFO` & `CircleBlock-1.0.5/CircleBlock.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.4/LICENSE` & `CircleBlock-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.4/PKG-INFO` & `CircleBlock-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.4/README.md` & `CircleBlock-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.4/circleblock/changer.py` & `CircleBlock-1.0.5/circleblock/changer.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.4/circleblock/cli.py` & `CircleBlock-1.0.5/circleblock/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import enum
 import os
 import signal
-from typing import Optional
+import sys
 
 import typer
 
 from daemonize import Daemonize
-from loguru import logger
 
 from .changer import InitFileUpdater
 from .watcher import FileWatcher
 
-app = typer.Typer()
+app = typer.Typer(add_completion=True, help='CircleBlock CLI')
 
 
 class CircleBlock:
     """
     CircleBlock is a class that monitors the file system in the project root directory.
     CircleBlock은 프로젝트 루트 디렉토리 내의 파일 시스템을 감시하는 클래스입니다.
     """
@@ -30,85 +29,73 @@
 
     def watch_file_system(self):
         """
         Start monitoring the file system.
         파일 시스템 감시를 시작합니다.
         """
         self.watcher.start_watching()
-        logger.info(f'Start monitoring the file system in {self.project_root}. {self.project_root}의 파일 시스템 감시를 시작합니다.')
+        typer.echo(f'Start monitoring the file system in {self.project_root}. {self.project_root}의 파일 시스템 감시를 시작합니다.')
 
     def stop_file_system_watch(self):
         """
         Stop monitoring the file system.
         파일 시스템 감시를 종료합니다.
         """
         self.watcher.stop_watching()
-        logger.info(f'Stop monitoring the file system in {self.project_root}. {self.project_root}의 파일 시스템 감시를 종료합니다.')
+        typer.echo(f'Stop monitoring the file system in {self.project_root}. {self.project_root}의 파일 시스템 감시를 종료합니다.')
 
 
 class CommandType(enum.IntEnum):
     RUN = enum.auto()
     STOP = enum.auto()
     INIT = enum.auto()
 
 
 @app.callback()
-def callback(ctx: typer.Context):
-    ctx.obj = {'project_root': os.getcwd(), 'cb': None}
+def callback(
+        ctx: typer.Context,
+        project_root: str = typer.Option(None, '-p', '--project-root', help='Project root directory path')
+):
+    ctx.obj = {'project_root': project_root or os.getcwd(), 'cb': None}
 
 
-@app.command()
+@app.command(help='Start CircleBlock in daemon mode')
 def run(ctx: typer.Context) -> None:
     cb: CircleBlock = ctx.obj['cb'] or CircleBlock(ctx.obj['project_root'])
+    typer.echo(f'project_root::{ctx.obj["project_root"]}')
 
     def start():
         cb.watch_file_system()
 
     typer.echo(f'Starting CircleBlock in daemon mode')
     daemon = Daemonize(
         app='CircleBlock',
         pid=os.path.join(cb.project_root, 'CircleBlock.pid'),
         action=start
     )
     daemon.start()
 
 
-@app.command()
+@app.command(help='Stop CircleBlock daemon')
 def stop(ctx: typer.Context) -> None:
     cb: CircleBlock = ctx.obj['cb'] or CircleBlock(ctx.obj['project_root'])
 
     pid_file = os.path.join(cb.project_root, 'CircleBlock.pid')
     if os.path.exists(pid_file):
         with open(pid_file, 'r') as f:
             pid = int(f.read().strip())
         os.kill(pid, signal.SIGTERM)
         os.remove(pid_file)
         typer.echo(f'CircleBlock daemon with PID {pid} has been terminated.')
     else:
         typer.echo('CircleBlock daemon is not running or PID file is missing.')
 
 
-@app.command()
+@app.command(help='Initialize CircleBlock')
 def init(ctx: typer.Context) -> None:
     cb: CircleBlock = ctx.obj['cb'] or CircleBlock(ctx.obj['project_root'])
     cb.updater.initialize_all_init_files()
 
 
-@app.command()
-def ccbk(
-        ctx: typer.Context,
-        command: Optional[str],
-        project_root: Optional[str] = typer.Argument(None, help='Project root directory path')
-) -> None:
-    if project_root:
-        ctx.obj['project_root'] = project_root
-    if ctx.obj['cb'] is None:
-        ctx.obj['cb'] = CircleBlock(ctx.obj['project_root'])
-    {
-        CommandType.RUN: run,
-        CommandType.STOP: stop,
-        CommandType.INIT: init
-    }[CommandType(command)](ctx)
-
-
 if __name__ == '__main__':
-    app()
+    app(prog_name='circleblock', help_option_names=['--help'])
+
```

### Comparing `CircleBlock-1.0.4/circleblock/watcher.py` & `CircleBlock-1.0.5/circleblock/watcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import signal
 
-from loguru import logger
+import typer
 from watchdog.observers import Observer
 
 
 class FileWatcher:
     def __init__(self, project_root: str, changer=None):
         self.project_root = project_root
         self.changer = changer
         self.observer = Observer()
 
     def start_watching(self):
         """
         변경 사항을 감시하기 위해 루트 디렉토리를 감시하고 circleblock_cli.py 파일을 생성/업데이트합니다.
         """
-        logger.debug('변경 사항 감시 시작...')
-        logger.debug(f'프로젝트 루트: {self.project_root}')
+        typer.echo(f'변경 사항 감시 시작...')
+        typer.echo(f'프로젝트 루트: {self.project_root}')
 
         self.observer.schedule(self.changer, self.project_root, recursive=True)
         self.observer.start()
         signal.signal(signal.SIGINT, lambda *args, **kwargs: self.stop_watching())
         signal.pause()
 
     def stop_watching(self):
```

### Comparing `CircleBlock-1.0.4/setup.py` & `CircleBlock-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CircleBlock',
-    version='1.0.4',
+    version='1.0.5',
     description='Python package for creating circle-themed block diagrams',
     author='phil',
     author_email='eightynine01@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'watchdog',
-        'loguru',
         'typer',
         'daemonize'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

