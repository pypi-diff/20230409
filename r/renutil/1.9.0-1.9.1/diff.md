# Comparing `tmp/renutil-1.9.0.tar.gz` & `tmp/renutil-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renutil-1.9.0.tar", last modified: Sat May  2 14:08:44 2020, max compression
+gzip compressed data, was "renutil-1.9.1.tar", last modified: Sat May  2 15:56:16 2020, max compression
```

## Comparing `renutil-1.9.0.tar` & `renutil-1.9.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2020-05-02 14:08:41.083632 renutil-1.9.0/LICENSE
--rw-r--r--   0        0        0     2105 2020-05-02 14:08:41.083632 renutil-1.9.0/README.md
--rw-r--r--   0        0        0      695 2020-05-02 14:08:41.083632 renutil-1.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2020-05-02 14:08:41.083632 renutil-1.9.0/renutil/__init__.py
--rw-r--r--   0        0        0    20112 2020-05-02 14:08:41.083632 renutil-1.9.0/renutil/renutil.py
--rw-r--r--   0        0        0     3066 2020-05-02 14:08:44.942270 renutil-1.9.0/setup.py
--rw-r--r--   0        0        0     3019 2020-05-02 14:08:44.942592 renutil-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2020-05-02 15:56:12.540942 renutil-1.9.1/LICENSE
+-rw-r--r--   0        0        0     2105 2020-05-02 15:56:12.540942 renutil-1.9.1/README.md
+-rw-r--r--   0        0        0      695 2020-05-02 15:56:12.540942 renutil-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-05-02 15:56:12.540942 renutil-1.9.1/renutil/__init__.py
+-rw-r--r--   0        0        0    20114 2020-05-02 15:56:12.540942 renutil-1.9.1/renutil/renutil.py
+-rw-r--r--   0        0        0     3066 2020-05-02 15:56:16.723357 renutil-1.9.1/setup.py
+-rw-r--r--   0        0        0     3019 2020-05-02 15:56:16.723667 renutil-1.9.1/PKG-INFO
```

### Comparing `renutil-1.9.0/LICENSE` & `renutil-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `renutil-1.9.0/README.md` & `renutil-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `renutil-1.9.0/pyproject.toml` & `renutil-1.9.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "renutil"
-version = "1.9.0"
+version = "1.9.1"
 description = "A toolkit for managing Ren'Py instances via the command line"
 authors = ["CobaltCore <cobaltcore@yandex.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/kobaltcore/renutil"
 homepage = "https://github.com/kobaltcore/renutil"
```

### Comparing `renutil-1.9.0/renutil/renutil.py` & `renutil-1.9.1/renutil/renutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,26 +274,26 @@
     For example:
         clean -> c
         la -> launch
         li -> list
     """
     global CACHE, REGISTRY
 
+    logzero.loglevel(logging.DEBUG if debug else logging.INFO)
+
     if registry:
         registry = os.path.abspath(registry)
         os.makedirs(registry, exist_ok=True)
         CACHE = registry
     else:
         CACHE = os.path.join(os.path.expanduser("~"), ".renutil")
     REGISTRY = Registry(os.path.join(CACHE, "index.bin"))
 
     logger.debug("Registry Location: {}".format(CACHE))
 
-    logzero.loglevel(logging.DEBUG if debug else logging.INFO)
-
 
 @cli.command()
 @click.option("-a/-l", "--all/--local", "show_all", default=False,
               help="Show all versions available to download or just the local ones")
 @click.option("-n", "--num-versions", "count", default=5, type=int,
               help="Amount of versions to show, sorted in descending order")
 def list(show_all, count):
@@ -408,16 +408,16 @@
         if force:
             logger.info("Uninstalling {} before reinstalling...".format(version))
             instance = REGISTRY.get_instance(version)
             REGISTRY.remove_instance(instance)
             shutil.rmtree(os.path.join(CACHE, instance.path))
             logger.info("Done uninstalling")
         else:
-            logger.error("{} is already installed!".format(version))
-            sys.exit(1)
+            logger.warning("{} is already installed!".format(version))
+            sys.exit(0)
     if not valid_version(version):
         logger.error("Invalid version specifier!")
         sys.exit(1)
 
     logger.info("Downloading necessary files...")
     sdk_filename = "renpy-{}-sdk.zip".format(version)
     rapt_filename = "renpy-{}-rapt.zip".format(version)
```

### Comparing `renutil-1.9.0/setup.py` & `renutil-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'tqdm>=4.45.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['renutil = renutil.renutil:cli']}
 
 setup_kwargs = {
     'name': 'renutil',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': "A toolkit for managing Ren'Py instances via the command line",
     'long_description': "# renUtil\n[![CircleCI](https://circleci.com/gh/kobaltcore/renutil.svg?style=svg)](https://circleci.com/gh/kobaltcore/renutil)\n[![Downloads](https://pepy.tech/badge/renutil)](https://pepy.tech/project/renutil)\n\nA toolkit for managing Ren'Py instances via the command line.\n\nrenUtil can install, update, launch and remove instances of Ren'Py. The instances are completely independent from each other. It automatically sets up and configures RAPT so new instances are instantly ready to deploy to many different platforms. Best of all, renUtil automatically configures Ren'Py in such a way that you can run it headless, making it well suited for build servers and continuous integration pipelines.\n\n## Installation\nrenUtil can be installed via pip:\n```bash\n$ pip install renutil\n```\n\nPlease note that renUtil requires Python 3 and will not provide backwards compatibility for Python 2 for the foreseeable future.\n\n## Usage\n```bash\nUsage: renutil [OPTIONS] COMMAND [ARGS]...\n\n  Commands can be abbreviated by the shortest unique string.\n\n  For example:\n      clean -> c\n      la -> launch\n      li -> list\n\nOptions:\n  -d, --debug / -nd, --no-debug  Print debug information or only regular\n                                 output\n\n  --help                         Show this message and exit.\n\nCommands:\n  cleanup    Clean temporary files of the specified Ren'Py version.\n  install    Install the specified version of Ren'Py (including RAPT).\n  launch     Launch the specified version of Ren'Py.\n  list       List all available versions of Ren'Py.\n  uninstall  Uninstall the specified Ren'Py version.\n```\n\n# Disclaimer\nrenUtil is a hobby project and not in any way affiliated with Ren'Py. This means that there is no way I can guarantee that it will work at all, or continue to work once it does. Commands are mostly relayed to the Ren'Py CLI, so any issues with distribution building or startup are likely the fault of Ren'Py and not mine. renUtil is not likely to break on subsequent updates of Ren'Py, but it is not guaranteed that any available version will work correctly. Use this at your own discretion.\n",
     'author': 'CobaltCore',
     'author_email': 'cobaltcore@yandex.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/kobaltcore/renutil',
```

### Comparing `renutil-1.9.0/PKG-INFO` & `renutil-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renutil
-Version: 1.9.0
+Version: 1.9.1
 Summary: A toolkit for managing Ren'Py instances via the command line
 Home-page: https://github.com/kobaltcore/renutil
 License: MIT
 Author: CobaltCore
 Author-email: cobaltcore@yandex.com
 Requires-Python: >=3.5,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

