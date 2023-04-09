# Comparing `tmp/CircleBlock-1.0.3.tar.gz` & `tmp/CircleBlock-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircleBlock-1.0.3.tar", last modified: Sun Apr  9 13:17:07 2023, max compression
+gzip compressed data, was "CircleBlock-1.0.4.tar", last modified: Sun Apr  9 13:30:33 2023, max compression
```

## Comparing `CircleBlock-1.0.3.tar` & `CircleBlock-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:17:07.350616 CircleBlock-1.0.3/
--rw-r--r--   0 phil       (501) staff       (20)      386 2023-04-09 09:29:13.000000 CircleBlock-1.0.3/CHANGELOG.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:17:07.349743 CircleBlock-1.0.3/CircleBlock.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      358 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       33 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/entry_points.txt
--rw-r--r--   0 phil       (501) staff       (20)       32 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)       18 2023-04-09 13:17:07.000000 CircleBlock-1.0.3/CircleBlock.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.3/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      167 2023-04-09 13:11:42.000000 CircleBlock-1.0.3/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 13:17:07.350424 CircleBlock-1.0.3/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-09 09:32:22.000000 CircleBlock-1.0.3/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:17:07.350109 CircleBlock-1.0.3/circleblock/
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 08:43:50.000000 CircleBlock-1.0.3/circleblock/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     4958 2023-04-09 09:22:09.000000 CircleBlock-1.0.3/circleblock/changer.py
--rw-r--r--   0 phil       (501) staff       (20)     1209 2023-04-09 08:20:47.000000 CircleBlock-1.0.3/circleblock/watcher.py
--rw-r--r--   0 phil       (501) staff       (20)     3351 2023-04-09 13:13:01.000000 CircleBlock-1.0.3/cli.py
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 13:17:07.350659 CircleBlock-1.0.3/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     1027 2023-04-09 13:12:19.000000 CircleBlock-1.0.3/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:17:07.350248 CircleBlock-1.0.3/tests/
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 13:11:03.000000 CircleBlock-1.0.3/tests/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:30:33.133794 CircleBlock-1.0.4/
+-rw-r--r--   0 phil       (501) staff       (20)      386 2023-04-09 13:30:17.000000 CircleBlock-1.0.4/CHANGELOG.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:30:33.132800 CircleBlock-1.0.4/CircleBlock.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      370 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       45 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/entry_points.txt
+-rw-r--r--   0 phil       (501) staff       (20)       32 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)       18 2023-04-09 13:30:33.000000 CircleBlock-1.0.4/CircleBlock.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.4/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      167 2023-04-09 13:11:42.000000 CircleBlock-1.0.4/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 13:30:33.133595 CircleBlock-1.0.4/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-09 09:32:22.000000 CircleBlock-1.0.4/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:30:33.133309 CircleBlock-1.0.4/circleblock/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 08:43:50.000000 CircleBlock-1.0.4/circleblock/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     4958 2023-04-09 09:22:09.000000 CircleBlock-1.0.4/circleblock/changer.py
+-rw-r--r--   0 phil       (501) staff       (20)     3297 2023-04-09 13:28:04.000000 CircleBlock-1.0.4/circleblock/cli.py
+-rw-r--r--   0 phil       (501) staff       (20)      999 2023-04-09 13:24:51.000000 CircleBlock-1.0.4/circleblock/watcher.py
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 13:30:33.133837 CircleBlock-1.0.4/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     1039 2023-04-09 13:29:51.000000 CircleBlock-1.0.4/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 13:30:33.133432 CircleBlock-1.0.4/tests/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 13:11:03.000000 CircleBlock-1.0.4/tests/__init__.py
```

### Comparing `CircleBlock-1.0.3/CircleBlock.egg-info/PKG-INFO` & `CircleBlock-1.0.4/CircleBlock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.3/LICENSE` & `CircleBlock-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.3/PKG-INFO` & `CircleBlock-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.3/README.md` & `CircleBlock-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.3/circleblock/changer.py` & `CircleBlock-1.0.4/circleblock/changer.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.3/circleblock/watcher.py` & `CircleBlock-1.0.4/circleblock/watcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-import atexit
 import signal
 
 from loguru import logger
 from watchdog.observers import Observer
 
 
-def log_exit_message():
-    """
-    프로그램이 종료될 때 종료 메시지를 기록합니다.
-    """
-    logger.info('파일 감시 종료.')
-
-
 class FileWatcher:
     def __init__(self, project_root: str, changer=None):
         self.project_root = project_root
         self.changer = changer
         self.observer = Observer()
-        atexit.register(log_exit_message)
 
     def start_watching(self):
         """
         변경 사항을 감시하기 위해 루트 디렉토리를 감시하고 circleblock_cli.py 파일을 생성/업데이트합니다.
         """
         logger.debug('변경 사항 감시 시작...')
         logger.debug(f'프로젝트 루트: {self.project_root}')
```

### Comparing `CircleBlock-1.0.3/cli.py` & `CircleBlock-1.0.4/circleblock/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import Optional
 
 import typer
 
 from daemonize import Daemonize
 from loguru import logger
 
-from circleblock.changer import InitFileUpdater
-from circleblock.watcher import FileWatcher
+from .changer import InitFileUpdater
+from .watcher import FileWatcher
 
 app = typer.Typer()
 
 
 class CircleBlock:
     """
     CircleBlock is a class that monitors the file system in the project root directory.
@@ -71,15 +71,14 @@
     )
     daemon.start()
 
 
 @app.command()
 def stop(ctx: typer.Context) -> None:
     cb: CircleBlock = ctx.obj['cb'] or CircleBlock(ctx.obj['project_root'])
-    cb.stop_file_system_watch()
 
     pid_file = os.path.join(cb.project_root, 'CircleBlock.pid')
     if os.path.exists(pid_file):
         with open(pid_file, 'r') as f:
             pid = int(f.read().strip())
         os.kill(pid, signal.SIGTERM)
         os.remove(pid_file)
```

### Comparing `CircleBlock-1.0.3/setup.py` & `CircleBlock-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CircleBlock',
-    version='1.0.3',
+    version='1.0.4',
     description='Python package for creating circle-themed block diagrams',
     author='phil',
     author_email='eightynine01@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'watchdog',
@@ -25,11 +25,11 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
-            'ccbk=cli:app'
+            'ccbk=circleblock.cli:app'
         ]
     }
 )
```

