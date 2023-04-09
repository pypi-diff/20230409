# Comparing `tmp/curldl-0.1.0.tar.gz` & `tmp/curldl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curldl-0.1.0.tar", last modified: Sat Apr  1 20:00:26 2023, max compression
+gzip compressed data, was "curldl-1.0.0.tar", last modified: Sun Apr  9 19:47:10 2023, max compression
```

## Comparing `curldl-0.1.0.tar` & `curldl-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:00:26.941835 curldl-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-01 19:59:08.000000 curldl-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-01 20:00:26.941835 curldl-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-01 19:59:08.000000 curldl-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-01 19:59:08.000000 curldl-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 20:00:26.941835 curldl-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:00:26.933834 curldl-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:00:26.937834 curldl-0.1.0/src/curldl/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-01 19:59:08.000000 curldl-0.1.0/src/curldl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-01 19:59:08.000000 curldl-0.1.0/src/curldl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-01 19:59:08.000000 curldl-0.1.0/src/curldl/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-04-01 19:59:08.000000 curldl-0.1.0/src/curldl/curldl.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-01 19:59:08.000000 curldl-0.1.0/src/curldl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:00:26.941835 curldl-0.1.0/src/curldl/util/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-01 19:59:08.000000 curldl-0.1.0/src/curldl/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-01 19:59:08.000000 curldl-0.1.0/src/curldl/util/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-01 19:59:08.000000 curldl-0.1.0/src/curldl/util/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-01 19:59:08.000000 curldl-0.1.0/src/curldl/util/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-01 19:59:08.000000 curldl-0.1.0/src/curldl/util/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:00:26.937834 curldl-0.1.0/src/curldl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-01 20:00:26.000000 curldl-0.1.0/src/curldl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-01 20:00:26.000000 curldl-0.1.0/src/curldl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 20:00:26.000000 curldl-0.1.0/src/curldl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-01 20:00:26.000000 curldl-0.1.0/src/curldl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-01 20:00:26.000000 curldl-0.1.0/src/curldl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-01 20:00:26.000000 curldl-0.1.0/src/curldl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.297367 curldl-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-09 19:45:54.000000 curldl-1.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-09 19:45:54.000000 curldl-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-09 19:47:10.297367 curldl-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-04-09 19:45:54.000000 curldl-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.289367 curldl-1.0.0/misc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/misc/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-09 19:45:54.000000 curldl-1.0.0/misc/conda/test-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/misc/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-04-09 19:45:54.000000 curldl-1.0.0/misc/scripts/run-bandit.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      184 2023-04-09 19:45:54.000000 curldl-1.0.0/misc/scripts/run-mypy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-04-09 19:45:54.000000 curldl-1.0.0/misc/scripts/run-pylint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-09 19:45:54.000000 curldl-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:47:10.297367 curldl-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/src/curldl/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/curldl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/src/curldl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/util/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/util/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/util/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/src/curldl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.297367 curldl-1.0.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/functional/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/functional/test_curldl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.297367 curldl-1.0.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/test_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/test_curldl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/test_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3554 2023-04-09 19:45:54.000000 curldl-1.0.0/venv.sh
```

### Comparing `curldl-0.1.0/LICENSE.md` & `curldl-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `curldl-0.1.0/pyproject.toml` & `curldl-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PEP 518/517, 621
 
 [project]
 name = "curldl"
-version = "0.1.0"
+dynamic = ["version"]
 description = "Safely and reliably download files with PycURL"
 keywords = ["cURL", "PycURL", "download"]
 
 readme = "README.md"
 license = {text = "LGPL-3.0-or-later"}
 
 authors = [{name = "Michael Orlov", email = "orlovm@noexec.org"}]
@@ -32,79 +32,92 @@
     "tenacity>=6.2.0",      # retry policies
     "tqdm>=4.50.0"          # console progress bar
 ]
 
 [project.optional-dependencies]
 minimal = [
     "pycurl==7.44.0",       # need CURLINFO_CONDITION_UNMET
-    "tenacity==6.2.0",      # need type hinting and no-warnings asyncio (also requires six, but it must be recent)
+    "tenacity==6.2.0",      # need type hinting and no-warnings asyncio (also requires six)
     "tqdm==4.50.0"          # need colour parameter (also requires colorama on win32)
 ]
 
 test = [
     "bandit[toml]",         # security issues checks
     "pytest",               # pytest testing framework
     "pytest-cov",           # code coverage (--cov)
     "pytest-httpserver",    # HTTP server fixture
     "pytest-mock",          # mocker fixtures for monkey patching
     "pytest-mypy",          # type hinting verifier (--mypy)
     "pytest-pylint",        # static code analysis (--pylint)
     "pytest-repeat",        # repeating tests (@pytest.mark.repeat)
     "pytest-sugar",         # look-and-feel for pytest progress
     "pytest-xdist[psutil]", # distributed tests (-n logical --no-pylint)
-    "toml",                 # reading project.version from this file
+    "setuptools-scm[toml]", # git tags-based versioning in editable install
     "types-pycurl",         # external type annotations: pycurl
-    "types-toml",           # external type annotations: toml
     "types-tqdm"            # external type annotations: tqdm
 ]
 
-environment = [
+dev = [
     "build",                # packaging build frontend
     "ipython",              # interactive Python environment
     "pipdeptree",           # show packages dependency tree
     "pip-autoremove",       # remove unused package dependencies
     "pip-review",           # upgrade outdated packages
+    "sphinx",               # documentation generator
+    "twine",                # PyPI package publishing
     "wheel"                 # build system, support PEP 518 installs
 ]
 
 [project.urls]
-repository = "https://github.com/noexec/curldl"
+"Homepage" = "https://github.com/noexec/curldl"
+"Documentation" = "https://pypi.org/project/curldl/"
+"Bug Tracker" = "https://github.com/noexec/curldl/issues"
 
 [project.scripts]
 curldl = "curldl.cli:main"
 
 
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=45", "setuptools-scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [tool.setuptools.package-data]
 "curldl" = ["py.typed"]         # PIP 561
 
 
+[tool.setuptools_scm]
+version_scheme = "no-guess-dev"
+write_to = "src/curldl/_version.py"
+
+
 [tool.pytest.ini_options]
 addopts = "--maxfail=10 --mypy --pylint --cov --cov-report=term --cov-report=html"
 testpaths = ["tests", "src"]    # "src" required for pylint and mypy (whereas cov considers imported files)
 cache_dir = "build/tests/pytest_cache"
 
 filterwarnings = [
     "default",
     "ignore::DeprecationWarning:pytest_pylint.plugin",          # pytest-pylint 0.19.0
     "ignore::DeprecationWarning:pytest_pylint.pylint_util"      # pytest-pylint 0.19.0
 ]
 
 
 [tool.pylint.main]
 py-version = "3.8"
+ignore-paths = ["src/curldl/_version.py"]
+extension-pkg-allow-list = ["pycurl"]
 
 [tool.pylint.format]
 expected-line-ending-format = "LF"
 max-line-length = 120
 
+[tool.pylint.basic]
+good-names-rgxs = "^(dl)$"
+
 [tool.pylint.design]
 min-public-methods = 1
 max-args = 10
 max-attributes = 15
 max-locals = 20
 
 [tool.pylint.miscellaneous]
@@ -144,9 +157,8 @@
 [tool.coverage.html]
 directory = "build/tests/htmlcov"
 show_contexts = true
 skip_covered = false
 
 
 [tool.bandit]
-exclude_dirs = ["venv", "build"]
 skips = ["B101"]
```

### Comparing `curldl-0.1.0/src/curldl/cli.py` & `curldl-1.0.0/src/curldl/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,46 +2,51 @@
 import argparse
 import logging
 import os
 import sys
 import urllib.parse
 from importlib import metadata
 
-import curldl
-from curldl import Downloader
+from curldl import Curldl
 from curldl.util import Log, Cryptography
 
 log = logging.getLogger(__name__)
 
 
 class CommandLine:
-    """Command-line interface"""
+    """Command-line interface, exposed via module entry point"""
 
     def __init__(self) -> None:
         """Initialize argument parser and unhandled exception hook"""
         sys.excepthook = Log.trace_unhandled_exception
         self.args = self._parse_arguments()
         log.debug('Configured: %s', self.args)
 
     @staticmethod
     def _configure_logger(args: argparse.Namespace) -> None:
+        """Configure logger according to command-line arguments.
+        Specifying `verbose` argument raises the log level to `debug`.
+        :param args: command-line arguments
+        """
         debug_log_level = 'debug'
         if args.verbose and args.log != debug_log_level:
             args.log = debug_log_level.capitalize()
 
         loglevel = getattr(logging, args.log.upper())
         assert isinstance(loglevel, int)
         logging.basicConfig(level=loglevel)
 
         if args.log == debug_log_level.capitalize():
             log.debug('Raising logging level to DEBUG')
 
     @classmethod
     def _parse_arguments(cls) -> argparse.Namespace:
-        """Parse command-line arguments"""
+        """Parse command-line arguments
+        :return: arguments after configuring the logger and possibly inferring other arguments
+        """
         parser = argparse.ArgumentParser(prog=__package__, formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
         log_choices = ['debug', 'info', 'warning', 'error', 'critical']
         hash_algos = Cryptography.get_available_digests()
         version = '%(prog)s ' + cls._get_package_version()
 
         parser.add_argument('-V', '--version', action='version', version=version, help='show program version and exit')
@@ -65,39 +70,50 @@
         args = parser.parse_args()
         cls._configure_logger(args)
 
         return cls._infer_arguments(output_arg, args)
 
     @classmethod
     def _infer_arguments(cls, output_arg: argparse.Action, args: argparse.Namespace) -> argparse.Namespace:
-        """Infer missing arguments"""
+        """Infer missing arguments
+        :param output_arg: `output` argument to infer
+        :param args: arguments to extend
+        :return: input arguments after inferring missing ones
+        :raises argparse.ArgumentError: multiple URLs are specified with ``output`` argument
+        """
         if not args.output:
             args.output = [os.path.basename(urllib.parse.unquote(urllib.parse.urlparse(url).path)) for url in args.url]
             log.info('Saving download(s) to: %s', ', '.join(args.output))
 
         elif len(args.output) != len(args.url):
             raise argparse.ArgumentError(output_arg, 'Cannot specify output file when downloading multiple URLs')
 
         return args
 
     def main(self) -> object:
-        """Command-line program entry point"""
-        downloader = Downloader(self.args.basedir, progress=self.args.progress, verbose=self.args.verbose)
+        """Command-line program entry point
+        :return: program exit status
+        """
+        dl = Curldl(self.args.basedir, progress=self.args.progress, verbose=self.args.verbose)
         for url, output in zip(self.args.url, self.args.output):
-            downloader.download(url, rel_path=output, size=self.args.size,
-                                digests=self.args.digest and {self.args.algo: self.args.digest})
+            dl.get(url, rel_path=output, size=self.args.size,
+                   digests=self.args.digest and {self.args.algo: self.args.digest})
         return 0
 
     @staticmethod
     def _get_package_version() -> str:
-        """Retrieve package version from metadata, with support for uninstalled development sources"""
+        """Retrieve package version from metadata, raising error for uninstalled development sources
+        :return: package version string
+        :raises metadata.PackageNotFoundError: version is not available, e.g. when package is not installed
+        """
         try:
             return metadata.version(__package__)
         except metadata.PackageNotFoundError:
-            import toml     # pylint: disable=import-outside-toplevel
-            pyproject = os.path.join(curldl.ROOT_DIR, os.path.pardir, os.path.pardir, 'pyproject.toml')
-            return str(toml.load(pyproject)['project']['version'])
+            log.error('Generated version not available, install package as usual or in editable mode')
+            raise
 
 
 def main() -> object:
-    """Command-line static entry point, suitable for install-time script generation"""
+    """Command-line static entry point, suitable for install-time script generation
+    :return: program exit status
+    """
     return CommandLine().main()
```

### Comparing `curldl-0.1.0/src/curldl/curldl.py` & `curldl-1.0.0/src/curldl/curldl.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,53 +14,81 @@
 from tqdm import tqdm
 
 from curldl.util import FileSystem, Time
 
 log = logging.getLogger(__name__)
 
 
-class Downloader:
-    """Interface for downloading functionality of PycURL"""
+class Curldl:
+    """Interface for downloading functionality of PycURL.
+    Basic usage example::
+
+        import curldl, os
+        dl = curldl.Curldl(basedir='downloads', progress=True)
+        dl.get('https://kernel.org/pub/linux/kernel/Historic/linux-0.01.tar.gz', 'linux-0.01.tar.gz',
+               size=73091, digests={'sha1': '566b6fb6365e25f47b972efa1506932b87d3ca7d'})
+        assert os.path.exists('downloads/linux-0.01.tar.gz')
+
+    For a more in-depth guide, refer to the package documentation.
+    """
 
     DOWNLOAD_RETRY_ERRORS = {
         pycurl.E_COULDNT_RESOLVE_PROXY, pycurl.E_COULDNT_RESOLVE_HOST, pycurl.E_COULDNT_CONNECT,
         pycurl.E_FTP_ACCEPT_FAILED, pycurl.E_FTP_ACCEPT_TIMEOUT, pycurl.E_FTP_CANT_GET_HOST,
         pycurl.E_HTTP2, pycurl.E_PARTIAL_FILE, pycurl.E_FTP_PARTIAL_FILE, pycurl.E_HTTP_RETURNED_ERROR,
         pycurl.E_OPERATION_TIMEDOUT, pycurl.E_FTP_PORT_FAILED, pycurl.E_SSL_CONNECT_ERROR,
         pycurl.E_TOO_MANY_REDIRECTS, pycurl.E_GOT_NOTHING, pycurl.E_SEND_ERROR, pycurl.E_RECV_ERROR, pycurl.E_SSH,
         # TODO: Add once available: E_HTTP2_STREAM, E_HTTP3, E_QUIC_CONNECT_ERROR, E_PROXY, E_UNRECOVERABLE_POLL
     }
-    """libcurl errors accepted by download retry policy"""
+    """``libcurl`` errors accepted by download retry policy"""
 
     DEFAULT_ALLOWED_PROTOCOLS = {
         pycurl.PROTO_HTTP, pycurl.PROTO_HTTPS,
         pycurl.PROTO_FTP, pycurl.PROTO_FTPS,
         pycurl.PROTO_SFTP
     }
-    """Allowed URL schemes"""
+    """URL schemes allowed by default, can be changed with ``allowed_protocols_bitmask`` constructor parameter"""
 
     RESUME_FROM_SCHEMES = {'http', 'https', 'ftp', 'ftps', 'file'}
-    """URL schemes supported by RESUME_FROM. SFTP is not included because its implementation is buggy
-    (total download size is reduced twice by initial size). Scheme is extracted via urllib from initial URL,
+    """URL schemes supported by :attr:`pycurl.RESUME_FROM`. SFTP is not included because its implementation is buggy
+    (total download size is reduced twice by initial size). Scheme is extracted via :mod:`urllib` from initial URL,
     but there are no security implications since it is only used for removing partial downloads."""
 
     VERBOSE_LOGGING = {
         pycurl.INFOTYPE_TEXT: 'TEXT',
         pycurl.INFOTYPE_HEADER_IN: 'IHDR',
         pycurl.INFOTYPE_HEADER_OUT: 'OHDR',
     }
+    """Info types logged by :attr:`pycurl.DEBUGFUNCTION` callback during verbose logging"""
 
     def __init__(self, basedir: str | os.PathLike[str], *, progress: bool = False, verbose: bool = False,
                  user_agent: str = 'curl', retry_attempts: int = 3, retry_wait_sec: int | float = 2,
                  timeout_sec: int | float = 120, max_redirects: int = 5, allowed_protocols_bitmask: int = 0,
                  min_part_bytes: int = 64 * 1024, always_keep_part_bytes: int = 64 * 1024 ** 2,
                  curl_config_callback: Callable[[pycurl.Curl], None] | None = None) -> None:
-        """Initialize a PycURL-based downloader with a single pycurl.Curl instance
+        """Initialize a PycURL-based downloader with a single :class:`pycurl.Curl` instance
         that is reused and reconfigured for each download. The resulting downloader
-        object should be therefore not shared between several threads."""
+        object should be therefore not shared among several threads.
+        :param basedir: base directory path for downloaded file
+        :param progress: show progress bar on :attr:`sys.stderr`
+        :param verbose: enable verbose logging information from ``libcurl`` at ``DEBUG`` level
+        :param user_agent: ``User-Agent`` header for HTTP(S) protocols
+        :param retry_attempts: number of download retry attempts in case of failure in :attr:`DOWNLOAD_RETRY_ERRORS`
+        :param retry_wait_sec: seconds to wait between download retry attempts
+        :param timeout_sec: timeout seconds for ``libcurl`` operation
+        :param max_redirects: maximum number of redirects allowed in HTTP(S) protocols
+        :param allowed_protocols_bitmask: bitmask of allowed protocols, e.g. :attr:`pycurl.PROTO_HTTP`; default is
+            `or` of values in :attr:`DEFAULT_ALLOWED_PROTOCOLS`
+        :param min_part_bytes: partial downloads below this size are removed after unsuccessful download attempt;
+            set to ``0`` to disable removal of unsuccessful partial downloads
+        :param always_keep_part_bytes: do not remove partial downloads of this size or larger when resuming download
+            even if no size or digest is provided for verification; set to ``0`` to never remove existing partial
+            downloads
+        :param curl_config_callback: pass a callback to further configure a :class:`pycurl.Curl` object
+        """
         self._basedir = basedir
 
         self._progress = progress
         self._verbose = verbose
         self._user_agent = user_agent
 
         self._retry_attempts = retry_attempts
@@ -75,16 +103,24 @@
         self._always_keep_part_bytes = always_keep_part_bytes
 
         self._curl_config_callback = curl_config_callback
         self._unconfigured_curl = pycurl.Curl()
 
     def _get_configured_curl(self, url: str, path: str, *,
                              timestamp: int | float | None = None) -> tuple[pycurl.Curl, int]:
-        """Reconfigure pycurl.Curl instance for requested download and return the instance.
-        Methods should not work with unconfigured instance directly, only with this one."""
+        """Reconfigure :class:`pycurl.Curl` instance for requested download and return the instance.
+        Methods should not work with :attr:`_unconfigured_curl` directly, only with instance returned
+        by this method.
+        :param url: URL to download
+        :param path: resolved download file path
+        :param timestamp: last-modified timestamp of an already downloaded ``path``, if it exists;
+            used for skipping not-modified-since downloads with HTTP(S), FTP(S), FILE and RTSP protocols
+        :return: :class:`pycurl.Curl` instance configured for requested download and initial download offset
+            (i.e., file size to resume)
+        """
         curl = self._unconfigured_curl
         curl.reset()
 
         curl.setopt(pycurl.URL, url)
         curl.setopt(pycurl.USERAGENT, self._user_agent)
 
         curl.setopt(pycurl.FAILONERROR, True)
@@ -117,47 +153,74 @@
 
         if self._curl_config_callback:
             self._curl_config_callback(curl)
 
         return curl, initial_size
 
     def _perform_curl_download(self, curl: pycurl.Curl, write_stream: BinaryIO, progress_bar: tqdm[NoReturn]) -> None:
-        """Complete pycurl.Curl configuration and start downloading"""
+        """Complete pycurl.Curl configuration and start downloading
+        :param curl: configured :class:`pycurl.Curl` instance
+        :param write_stream: output stream to write to (a file opened in binary write mode)
+        :param progress_bar: progress bar to use; :attr:`pycurl.XFERINFOFUNCTION` is configured if enabled
+        """
         curl.setopt(pycurl.WRITEDATA, write_stream)
 
         # disable is already finalized after tty detection
         if not progress_bar.disable:
             curl.setopt(pycurl.XFERINFOFUNCTION, self._get_curl_progress_callback(progress_bar))
             curl.setopt(pycurl.NOPROGRESS, False)
 
         curl.perform()
 
     @staticmethod
     def _get_curl_progress_callback(progress_bar: tqdm[NoReturn]) -> Callable[[int, int, int, int], None]:
-        """Constructs a callback for XFERINFOFUNCTION"""
+        """Constructs a progress bar-updating callback for :attr:`pycurl.XFERINFOFUNCTION`
+        :param progress_bar: progress bar to use, must be enabled
+        :return: :attr:`pycurl.XFERINFOFUNCTION` callback
+        """
         def curl_progress_cb(download_total: int, downloaded: int, upload_total: int, uploaded: int) -> None:
-            """Progress callback for XFERINFOFUNCTION, only called if NOPROGRESS=0"""
+            """Progress callback for :attr:`pycurl.XFERINFOFUNCTION`, only called if :attr:`pycurl.NOPROGRESS` is ``0``
+            :param download_total: total bytes to download; initial file size is not included if resuming;
+                equal to ``0`` when download is just being started and download size is not yet available
+            :param downloaded: bytes downloaded so far; initial file size is not included if resuming
+            :param upload_total: unused
+            :param uploaded: unused
+            """
             if download_total != 0:
                 progress_bar.total = download_total + progress_bar.initial
             progress_bar.update(downloaded + progress_bar.initial - progress_bar.n)
         return curl_progress_cb
 
     @classmethod
     def _curl_debug_cb(cls, debug_type: int, debug_msg: bytes) -> None:
-        """Callback for DEBUGFUNCTION"""
+        """Callback for :attr:`pycurl.DEBUGFUNCTION` that logs ``libcurl`` messages at ``DEBUG`` level
+        :param debug_type: :class:`pycurl.Curl`-supplied info type, e.g. :attr:`pycurl.INFOTYPE_HEADER_IN`
+        :param debug_msg: :class:`pycurl.Curl`-supplied debug message
+        """
         debug_type = cls.VERBOSE_LOGGING.get(debug_type)
         if not debug_type:
             return
         debug_msg = debug_msg[:-1].decode('ascii', 'replace')
         log.debug('curl: [%s] %s', debug_type, debug_msg)
 
-    def download(self, url: str, rel_path: str, *, size: int | None = None,
-                 digests: dict[str, str] | None = None) -> None:
-        """Download a URL to basedir-relative path and verify its expected size and digests.
-        See Utilities.verify_size_and_digests() for format of expected digests."""
+    def get(self, url: str, rel_path: str, *, size: int | None = None, digests: dict[str, str] | None = None) -> None:
+        """Download a URL to ``basedir``-relative path and verify its expected size and digests.
+        Resume a partial download with ``.part`` extension if exists and supported by protocol,
+        and retry failures according to retry policy. The downloaded file is removed in case of
+        size or digest mismatch, and :class:`ValueError` is raised.
+        :param url: URL to download
+        :param rel_path: ``basedir``-relative output file path
+        :param size: expected file size in bytes, or ``None`` to ignore
+        :param digests: mapping of digest algorithms to expected hexadecimal digest strings, or ``None`` to ignore
+        (see :func:`curldl.util.FileSystem.verify_size_and_digests`)
+        :raises ValueError: relative path escapes base directory or is otherwise unsafe
+        (see :func:`curldl.util.FileSystem.verify_rel_path_is_safe`),
+        or file size mismatch, or one of digests fails verification
+        :raises pycurl.error: PycURL error when downloading after retries are exhausted
+        """
         path, path_partial = [self._prepare_full_path(rel_path + rel_ext) for rel_ext in ('', '.part')]
 
         if FileSystem.get_file_size(path, default=-1) == size:
             log.debug('Skipping update of %s since it has the expected size %s B', path, f'{size:,}')
             return
 
         if_modified_since_timestamp = None
@@ -195,24 +258,30 @@
             raise
 
         log.debug('Moving %s to %s', path_partial, path)
         os.replace(path_partial, path)
 
     def _download_partial(self, url: str, path: str, *,
                           timestamp: int | float | None = None, description: str | None = None) -> None:
-        """Start or resume a partial download of a URL to absolute path.
-
+        """Start or resume a partial download of a URL to resolved path.
         If timestamp of an already downloaded file is provided, remove the partial file
-        if the URL content is not more recent than the timestamp.
-
-        In case of runtime error or unexpected HTTP status, rollback to initial file size."""
+        if the URL content is not more recent than the timestamp. This method should be
+        invoked with a retry policy.
+        :param url: URL to download
+        :param path: resolved path of a partial download file
+        :param timestamp: last-modified timestamp of an already downloaded ``path``, if it exists
+        :param description: description string for progress bar (e.g., base name of downloaded file)
+        :raises pycurl.error: PycURL error when downloading, may result in a retry according to policy
+        """
         curl, initial_size = self._get_configured_curl(url, path, timestamp=timestamp)
 
         def log_partial_download(message_prefix: str, *, error: pycurl.error | None = None) -> None:
-            """Log information about partially downloaded file"""
+            """Log information about partially downloaded file at ``INFO`` or ``ERROR`` log level
+            :param message_prefix: log message prefix
+            :param error: PycURL exception, implies ``ERROR`` log level"""
             if log.isEnabledFor(log_level := logging.ERROR if error else logging.INFO):
                 log.log(log_level, message_prefix + f' {path} {initial_size:,} -> {os.path.getsize(path):,} B'
                         f' ({self._get_response_status(curl, url, error)})'
                         f' [{Time.timestamp_delta(curl.getinfo(pycurl.TOTAL_TIME))}]')
 
         try:
             with open(path, 'ab') as path_stream, \
@@ -231,38 +300,54 @@
             self._discard_file(path, force_remove=True)
             return
 
         log_partial_download('Finished downloading')
         FileSystem.set_file_timestamp(path, curl.getinfo(pycurl.INFO_FILETIME))
 
     def _prepare_full_path(self, rel_path: str) -> str:
-        """Verify that basedir-relative path is safe and create the required directories"""
+        """Verify that ``basedir``-relative path is safe and create the required directories
+        :param rel_path: ``basedir``-relative path
+        :return: resulting complete path
+        :raises ValueError: relative path escapes base directory or is otherwise unsafe
+            (see :func:`curldl.util.FileSystem.verify_rel_path_is_safe`)
+        """
         FileSystem.verify_rel_path_is_safe(self._basedir, rel_path)
         path = os.path.join(self._basedir, rel_path)
         FileSystem.create_directory_for_path(path)
         return path
 
     @classmethod
     def _get_response_status(cls, curl: pycurl.Curl, url: str, error: pycurl.error | None) -> str:
-        """Format response code and description from cURL with a possible error"""
+        """Format response code and description from cURL with a possible error
+        :param curl: :class:`pycurl.Curl` instance to extract response code from
+        :param url: a URL to extract scheme protocol from if :attr:`pycurl.EFFECTIVE_URL` is unavailable
+        :param error: PycURL exception instance
+        :return: formatted string that includes a response code and its meaning, if available
+        """
         scheme = cls._get_url_scheme(curl.getinfo(pycurl.EFFECTIVE_URL) or url)
         descr = 'No Status'
         if code := curl.getinfo(pycurl.RESPONSE_CODE):
             descr = 'No Description'
             if scheme in ['http', 'https']:
                 descr = http.client.responses.get(code, 'Unrecognized HTTP Status Code')
 
         # pylint: disable=consider-using-f-string
         error_descr = '{}: {} / '.format(error.args[0], error.args[1] or 'No Description') if error else ''
         return '{}{} {}{}'.format(error_descr, scheme.upper(), f'{code}: ' if code else '', descr)
 
     @staticmethod
     def _get_url_scheme(url: str) -> str:
-        """Return URL scheme (lowercase)"""
+        """Return URL scheme (lowercase)
+        :param url: a URL to extract URL scheme part from
+        :return: lowercase protocol scheme, e.g. `http`
+        """
         return urllib.parse.urlparse(url).scheme.lower()
 
     def _discard_file(self, path: str, *, force_remove: bool = False) -> None:
-        """If file size is below a threshold, it is removed. This is also done if force_remove is True."""
+        """If file size is below a threshold, it is removed. This is also done if force_remove is True.
+        :param path: file path to remove if its size is below ``min_part_bytes``
+        :param force_remove: unconditionally remove the file
+        """
         file_size = os.path.getsize(path)
         if force_remove or file_size < self._min_part_bytes:
-            log.debug('Removing %s since size of %s B is below threshold', path, f'{file_size:,}')
+            log.debug('Removing %s since size of %s B is below threshold or removal requested', path, f'{file_size:,}')
             os.remove(path)
```

### Comparing `curldl-0.1.0/src/curldl/util/crypt.py` & `curldl-1.0.0/src/curldl/util/crypt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,40 @@
-"""Cryptographic utilities"""
+"""Cryptographic utilities for internal use"""
 from __future__ import annotations
 
 import hashlib
 import logging
 import os
 
 log = logging.getLogger(__name__)
 
 
 class Cryptography:
-    """Filesystem utilities"""
+    """Cryptographic utilities"""
 
     FILE_CHUNK_BYTES = 8 * 1024 ** 2
 
     @staticmethod
     def get_available_digests() -> list[str]:
-        """Returns lists of fixed-size digest algorithms in hashlib"""
+        """Returns list of fixed-size digest algorithms in :mod:`hashlib`.
+        Uses :attr:`hashlib.algorithms_guaranteed` because :attr:`hashlib.algorithms_available` may
+        result in runtime errors due to deprecated algorithms being hidden by OpenSSL.
+        :return: guaranteed algorithms in :mod:`hashlib` that produce a fixed-size digest
+        """
         return sorted(algo for algo in hashlib.algorithms_guaranteed
                       if hashlib.new(algo).digest_size != 0)
 
     @classmethod
     def verify_digest(cls, path: str | os.PathLike[str], algo: str, digest: str) -> None:
-        """Verify file digest and raise ValueError in case of mismatch.
-        :param path: file path
-        :param algo: hash algorithm name accepted by hashlib.new()
-        :param digest: hexadecimal string"""
+        """Verify file digest and raise :class:`ValueError` in case of mismatch.
+        :param path: input file path
+        :param algo: hash algorithm name accepted by :func:`hashlib.new`
+        :param digest: hexadecimal digest string to verify
+        :raises ValueError: ``digest`` has incorrect length or fails verification
+        """
         hash_obj = hashlib.new(algo)
         digest_name = hash_obj.name.upper()
 
         log.debug('Computing %s-bit %s for %s', hash_obj.digest_size * 8, digest_name, path)
         if hash_obj.digest_size*2 != len(digest):
             raise ValueError(f'Expected {digest_name} for {path} has length != {hash_obj.digest_size} B')
```

### Comparing `curldl-0.1.0/src/curldl/util/fs.py` & `curldl-1.0.0/src/curldl/util/fs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-"""Filesystem utilities"""
+"""Filesystem utilities for internal use"""
 from __future__ import annotations
 
 import logging
 import os
 
 from curldl.util.crypt import Cryptography
 from curldl.util.time import Time
 
 log = logging.getLogger(__name__)
 
 
 class FileSystem:
-    """Filesystem utilities"""
+    """Filesystem utilities, include cryptographic digest verification wrappers"""
 
     @staticmethod
     def verify_rel_path_is_safe(basedir: str | os.PathLike[str], rel_path: str | os.PathLike[str]) -> None:
         """Verify that a relative path does not escape base directory
-        and either does not exist or is a file or a symlink to one"""
+        and either does not exist or is a file or a symlink to one
+        :param basedir: base directory path
+        :param rel_path: path relative to base directory
+        :raises ValueError: relative path escapes base directory before or after symlink resolution,
+        resulting path is a dangling symlink, is not a file or a symlink to file
+        """
         base = os.path.abspath(basedir)
         path = os.path.abspath(os.path.join(basedir, rel_path))
         base_real, path_real = os.path.realpath(base), os.path.realpath(path)
 
         # os.path.commonpath() also raises ValueError for different-drive paths on Windows
         if base != os.path.commonpath((base, path)):
             raise ValueError(f'Relative path {rel_path} escapes base path {base}')
@@ -35,47 +40,66 @@
             raise ValueError(f'Exists and not a file or symlink to file: {path}')
 
         if str(rel_path).endswith(os.path.sep) or (os.path.altsep and str(rel_path).endswith(os.path.altsep)):
             raise ValueError(f'Path can only point to a directory: {rel_path}')
 
     @classmethod
     def create_directory_for_path(cls, path: str | os.PathLike[str]) -> None:
-        """Create all path components for path, except for last"""
+        """Create all path components for path, except for last
+        :param path: file path
+        """
         path_dir = os.path.dirname(path)
         if not os.path.exists(path_dir):
             log.info('Creating directory: %s', path_dir)
             os.makedirs(path_dir)
 
     @classmethod
     def verify_size_and_digests(cls, path: str | os.PathLike[str], *, size: int | None = None,
                                 digests: dict[str, str] | None = None) -> None:
-        """Verify file size and digests and raise ValueError in case of mismatch.
-        digests is a dict of hash algorithms and digests to check (see Cryptography.verify_digest())."""
+        """Verify file size and digests and raise :class:`ValueError` in case of mismatch.
+        ``digests`` is a dict of hash algorithms and digests to check
+        (see :func:`curldl.util.crypt.Cryptography.verify_digest`).
+        :param path: input file path
+        :param size: expected file size in bytes, or ``None`` to ignore
+        :param digests: mapping of digest algorithms to expected hexadecimal digest strings, or ``None`` to ignore
+        :raises ValueError: not a file or file size mismatch or one of digests fails verification
+        """
         if size is not None:
             cls.verify_size(path, size=size)
         for algo, digest in digests.items() if digests else {}:
             Cryptography.verify_digest(path, algo=algo, digest=digest)
 
     @classmethod
     def verify_size(cls, path: str | os.PathLike[str], size: int) -> None:
-        """Verify file size and raise ValueError in case of mismatch or if not a file"""
+        """Verify file size and raise :class:`ValueError` in case of mismatch or if not a file
+        :param path: input file path
+        :param size: expected file size in bytes
+        :raises ValueError: not a file or file size mismatch
+        """
         path_size = os.path.getsize(path)
         if not os.path.isfile(path):
             raise ValueError(f'Not a file: {path}')
         if path_size != size:
             raise ValueError(f'Size mismatch for {path}: {path_size:,} instead of {size:,} B')
         log.debug('Successfully verified file size of %s', path)
 
     @staticmethod
     def get_file_size(path: str | os.PathLike[str], default: int = 0) -> int:
-        """Returns file size, or default if it does not exist or is not a file"""
+        """Returns file size, or ``default`` if it does not exist or is not a file
+        :param path: input file path
+        :param default: value to return if ``path`` does not exist or is not a file (e.g., a directory)
+        :return: input file size
+        """
         return os.path.getsize(path) if os.path.isfile(path) else default
 
     @classmethod
     def set_file_timestamp(cls, path: str | os.PathLike[str], timestamp: int | float) -> None:
-        """Sets file timestamp to a POSIX timestamp.
-        If timestamp is negative, does nothing."""
+        """Sets file timestamp to a POSIX timestamp. If timestamp is negative, does nothing.
+        :param path: filesystem path, must exist; symlinks are followed
+        :param timestamp: POSIX UTC-based timestamp to store as last-modified
+        and last-accessed file time if non-negative
+        """
         if timestamp < 0:
             return
         if log.isEnabledFor(logging.DEBUG):
             log.debug('Timestamping %s with %s', path, Time.timestamp_to_dt(timestamp))
         os.utime(path, times=(timestamp, timestamp))
```

### Comparing `curldl-0.1.0/src/curldl/util/log.py` & `curldl-1.0.0/src/curldl/util/log.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Logging and tracing utilities"""
+"""Logging and tracing utilities for internal use"""
 from __future__ import annotations
 
 import logging
 import traceback
 import types
 from typing import Type
 
@@ -11,18 +11,27 @@
 
 class Log:
     """Logging and tracing utilities"""
 
     @classmethod
     def trace_unhandled_exception(cls, exc_type: Type[BaseException], exc: BaseException,
                                   trace_back: types.TracebackType | None) -> None:
-        """Top-level logger for unhandled exceptions, can be assigned to sys.excepthook"""
+        """Top-level logger for unhandled exceptions, can be assigned to ``sys.excepthook``.
+        The exception is logged at ``CRITICAL`` level, ad traceback at ``DEBUG`` level.
+        :param exc_type: exception type (expected: ``exc.__class__``)
+        :param exc: exception object
+        :param trace_back: exception traceback (expected: ``exc.__traceback__``)
+        """
         log.critical('%s: %s', exc_type.__name__, exc)
         if log.isEnabledFor(logging.DEBUG):
             log.debug(''.join(traceback.format_exception(exc_type, value=exc, tb=trace_back)).rstrip('\n'))
 
     @classmethod
     def trace_exception(cls, exc: BaseException, msg: str) -> None:
-        """Logging helper to trace an exception, including traceback at lower level"""
+        """Logging helper to trace an exception.
+        The exception is logged at ``ERROR`` level, ad traceback at ``DEBUG`` level.
+        :param exc: exception object
+        :param msg: message to prepend when logging the exception
+        """
         log.error('%s: %s: %s', msg, exc.__class__.__name__, exc)
         if log.isEnabledFor(logging.DEBUG):
             log.debug(''.join(traceback.format_exception(exc.__class__, value=exc, tb=exc.__traceback__)).rstrip('\n'))
```

### Comparing `curldl-0.1.0/src/curldl/util/time.py` & `curldl-1.0.0/src/curldl/util/time.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-"""Time and timestamp utilities"""
+"""Time and timestamp utilities for internal use"""
 from __future__ import annotations
 
 import datetime
 import email.utils
-import logging
-
-log = logging.getLogger(__name__)
 
 
 class Time:
     """Time and timestamp utilities"""
 
     @staticmethod
     def timestamp_to_dt(timestamp: int | float) -> datetime.datetime:
-        """Convert POSIX timestamp to datetime in UTC timezone"""
+        """Convert POSIX timestamp to datetime in UTC timezone
+        :param timestamp: UTC-based POSIX timestamp
+        :return: :class:`datetime.datetime` in UTC timezone
+        """
         return datetime.datetime.fromtimestamp(timestamp, datetime.timezone.utc)
 
     @staticmethod
     def timestamp_to_http_date(timestamp: int | float) -> str:
-        """Convert POSIX timestamp to HTTP date in GMT timezone"""
+        """Convert POSIX timestamp to HTTP date in GMT timezone
+        :param timestamp: POSIX timestamp
+        :return: RFC-822 date suitable for HTTP headers
+        """
         return email.utils.formatdate(round(timestamp), usegmt=True)
 
     @staticmethod
     def timestamp_delta(timestamp_delta: int | float) -> datetime.timedelta:
-        """Convert POSIX timestamp difference to a printable datetime duration"""
+        """Convert POSIX timestamp difference to a printable datetime duration
+        :param timestamp_delta: time period in seconds
+        :return: :class:`datetime.datetime` duration, rounded to non-fractional seconds
+        """
         return datetime.timedelta(seconds=round(timestamp_delta))
```

