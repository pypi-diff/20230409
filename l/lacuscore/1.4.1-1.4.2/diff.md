# Comparing `tmp/lacuscore-1.4.1.tar.gz` & `tmp/lacuscore-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.4.1.tar", max compression
+gzip compressed data, was "lacuscore-1.4.2.tar", max compression
```

## Comparing `lacuscore-1.4.1.tar` & `lacuscore-1.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.1/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.1/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.1/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.1/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    27963 2023-04-08 12:04:00.137154 lacuscore-1.4.1/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.1/lacuscore/py.typed
--rw-r--r--   0        0        0     1475 2023-04-08 12:04:14.661245 lacuscore-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 lacuscore-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.2/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.2/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.2/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.2/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    27998 2023-04-08 16:48:20.490890 lacuscore-1.4.2/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.2/lacuscore/py.typed
+-rw-r--r--   0        0        0     1475 2023-04-09 10:56:54.694290 lacuscore-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 lacuscore-1.4.2/PKG-INFO
```

### Comparing `lacuscore-1.4.1/LICENSE` & `lacuscore-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.1/README.md` & `lacuscore-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.1/lacuscore/lacus_monitoring.py` & `lacuscore-1.4.2/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.1/lacuscore/lacuscore.py` & `lacuscore-1.4.2/lacuscore/lacuscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -533,15 +533,15 @@
                 logger.exception(f'Invalid parameters for the capture of {url} - {e}')
                 result = {'error': 'Invalid parameters for the capture of {url} - {e}'}
                 raise CaptureError
             except asyncio.CancelledError:
                 logger.warning(f'The capture of {url} has been cancelled.')
                 result = {'error': f'The capture of {url} has been cancelled.'}
                 raise CaptureError
-            except TimeoutError:
+            except (TimeoutError, asyncio.exceptions.TimeoutError):
                 logger.warning(f'The capture of {url} took longer than the allowed max capture time ({self.max_capture_time}s)')
                 result = {'error': f'The capture of {url} took longer than the allowed max capture time ({self.max_capture_time}s)'}
                 raise CaptureError
             except Exception as e:
                 logger.exception(f'Something went poorly {url} - {e}')
                 result = {'error': f'Something went poorly {url} - {e}'}
                 raise CaptureError
```

### Comparing `lacuscore-1.4.1/pyproject.toml` & `lacuscore-1.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.4.1"
+version = "1.4.2"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -40,12 +40,12 @@
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
 types-redis = {version = "^4.5.4.1"}
 mypy = "^1.2.0"
 types-requests = "^2.28.11.17"
 ipython = "^8.12.0"
-pytest = "^7.2.2"
+pytest = "^7.3.0"
 
 [build-system]
 requires = ["poetry_core>=1.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lacuscore-1.4.1/PKG-INFO` & `lacuscore-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.4.1
+Version: 1.4.2
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

