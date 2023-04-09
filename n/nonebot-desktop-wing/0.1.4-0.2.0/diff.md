# Comparing `tmp/nonebot-desktop-wing-0.1.4.tar.gz` & `tmp/nonebot-desktop-wing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-desktop-wing-0.1.4.tar", last modified: Sun Apr  9 11:55:51 2023, max compression
+gzip compressed data, was "nonebot-desktop-wing-0.2.0.tar", last modified: Sun Apr  9 14:04:26 2023, max compression
```

## Comparing `nonebot-desktop-wing-0.1.4.tar` & `nonebot-desktop-wing-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:51.437413 nonebot-desktop-wing-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 11:55:51.437413 nonebot-desktop-wing-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:51.437413 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/hindsight.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/lazylib.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/lazylib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:51.437413 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 11:55:51.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-09 11:55:51.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:55:51.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 11:55:51.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 11:55:51.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:55:51.437413 nonebot-desktop-wing-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:04:26.811494 nonebot-desktop-wing-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 14:04:26.811494 nonebot-desktop-wing-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:04:26.807494 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/hindsight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/lazylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/lazylib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:04:26.811494 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 14:04:26.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-09 14:04:26.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:04:26.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 14:04:26.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 14:04:26.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:04:26.811494 nonebot-desktop-wing-0.2.0/setup.cfg
```

### Comparing `nonebot-desktop-wing-0.1.4/LICENSE` & `nonebot-desktop-wing-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.4/PKG-INFO` & `nonebot-desktop-wing-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.1.4
+Version: 0.2.0
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-wing-0.1.4/README.md` & `nonebot-desktop-wing-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/__init__.py` & `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/constants.py` & `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/constants.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/hindsight.py` & `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/hindsight.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,55 @@
+from queue import Empty, Queue
 from threading import Thread
-from typing import Callable, Generic, ParamSpec, TypeVar
+from typing import IO, Callable, Generic, List, Optional, ParamSpec, TypeVar
 
 T = TypeVar("T")
+AnyStr_T = TypeVar("AnyStr_T", str, bytes)
 P = ParamSpec("P")
 
-bgobject_log_func = print
-"""Function for logging BackgroundObject info."""
-
 
 class BackgroundObject(Generic[P, T]):
     def __init__(
         self,
         func: Callable[P, T],
         *args: P.args,
         **kwargs: P.kwargs
     ) -> None:
         """
         A descriptor for running functions in background.
         """
         self._func = func
         self._thread = Thread(None, self._work, None, args, kwargs)
         self._thread.start()
-        bgobject_log_func(
-            f"[BackgroundObject] '{func.__module__}.{func.__name__}' is "
-            f"running in background with {args=}, {kwargs=}"
-        )
+        # bgobject_log_func(
+        #     f"[BackgroundObject] '{func.__module__}.{func.__name__}' is "
+        #     f"running in background with {args=}, {kwargs=}"
+        # )
 
     def __get__(self, obj, objtype=None) -> T:
         return self.get()
 
     def _work(self, *args: P.args, **kwargs: P.kwargs) -> None:
         self._value = self._func(*args, **kwargs)
-        bgobject_log_func(
-            f"[BackgroundObject] '{self._func.__module__}."
-            f"{self._func.__name__}' is done with {args=}, {kwargs=}"
-        )
+        # bgobject_log_func(
+        #     f"[BackgroundObject] '{self._func.__module__}."
+        #     f"{self._func.__name__}' is done with {args=}, {kwargs=}"
+        # )
 
     def get(self) -> T:
         self._thread.join()
-        return self._value
+        return self._value
+
+
+class RealtimeIOPipe(Generic[AnyStr_T]):
+    def __init__(self, stream: IO[AnyStr_T], writer: Callable[[AnyStr_T], object]) -> None:
+        self.stream = stream
+        self.thread = Thread(target=self._pull)
+        self.writer = writer
+        self.thread.start()
+
+    def _pull(self) -> None:
+        while True:
+            try:
+                self.writer(self.stream.read(1))
+            except ValueError:
+                break
```

### Comparing `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/lazylib.py` & `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/lazylib.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/lazylib.pyi` & `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/lazylib.pyi`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/project.py` & `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,30 +28,32 @@
 def distributions(*fp: str):
     from importlib import metadata
     if fp:
         return metadata.distributions(path=list(fp))
     return metadata.distributions()
 
 
-def getdist(root: str):
+def getdist(root: Union[str, Path]):
     return (
         distributions(
             *(str(Path(root) / si)
             for si in glob(".venv/**/site-packages", root_dir=root, recursive=True))
         )
     )
 
 
 def create(
     fp: str,
     drivers: List[Driver],
     adapters: List[Adapter],
     dev: bool,
     usevenv: bool,
-    index: Optional[str] = None
+    index: Optional[str] = None,
+    new_win: bool = False,
+    catch_output: bool = False
 ):
     p = Path(fp)
     if p.exists():
         p.rmdir()
     nb_cli.handlers.create_project(
         "simple" if dev else "bootstrap",
         {
@@ -71,31 +73,34 @@
 
     if usevenv:
         from venv import create as create_venv
         create_venv(venv_dir, prompt=dir_name, with_pip=True)
 
     pyexec = find_python(p)
 
-    ret = perform_pip_install(
-        str(pyexec), "nonebot2", *dri_real, *adp_real, index=index or ""
+    return perform_pip_install(
+        str(pyexec),
+        "nonebot2",
+        *dri_real,
+        *adp_real,
+        index=index or "",
+        new_win=new_win,  # type: ignore
+        catch_output=catch_output
     )
 
-    if ret.returncode != 0:
-        raise OSError("cannot install packages")
-
 
 def get_builtin_plugins(pypath: str):
     return asyncio.run(nb_cli.handlers.list_builtin_plugins(python_path=pypath))
 
 
 def find_env_file(fp: Union[str, Path]):
     return glob(".env*", root_dir=fp)
 
 
-def get_env_config(ep: Path, config: str):
+def get_env_config(ep: Union[str, Path], config: str):
     return DotEnv(ep).get(config)
 
 
 def recursive_find_env_config(fp: Union[str, Path], config: str):
     pfp = Path(fp)
     cp = pfp / ".env"
     if not cp.is_file():
@@ -107,21 +112,24 @@
     return env and get_env_config(pfp / f".env.{env}", config)
 
 
 def recursive_update_env_config(fp: Union[str, Path], config: str, value: str):
     pfp = Path(fp)
     cp = pfp / ".env"
     if not cp.is_file():
+        # Default profile is 'prod' if main profile does not exist.
         cp = pfp / ".env.prod"
         useenv = DotEnv(cp).dict()
     else:
+        # Use main profile.
         useenv = DotEnv(cp).dict()
         if config not in useenv:
             env = get_env_config(cp, "ENVIRONMENT")
             if env:
+                # Developer specified profile is usable.
                 cenv = DotEnv(pfp / f".env.{env}").dict()
                 if config in cenv:
                     cp = pfp / f".env.{env}"
                     useenv = cenv
 
     useenv.update({config: value})
```

### Comparing `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/resources.py` & `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/resources.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/PKG-INFO` & `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.1.4
+Version: 0.2.0
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/SOURCES.txt` & `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.4/pyproject.toml` & `nonebot-desktop-wing-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-desktop-wing"
-version = "0.1.4"
+version = "0.2.0"
 description = "Wings for NoneBot desktop applications."
 authors = [
     {name = "HivertMoZara", email = "worldmozara@163.com"},
 ]
 license = {text = "MIT"}
 dependencies = ["nb_cli~=1.0.0", "python-dotenv~=1.0.0", "httpx>=0.23"]
 requires-python = ">=3.8"
```

