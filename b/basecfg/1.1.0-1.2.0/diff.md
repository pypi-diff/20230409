# Comparing `tmp/basecfg-1.1.0.tar.gz` & `tmp/basecfg-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basecfg-1.1.0.tar", last modified: Fri Apr  7 16:59:26 2023, max compression
+gzip compressed data, was "basecfg-1.2.0.tar", last modified: Sun Apr  9 19:02:15 2023, max compression
```

## Comparing `basecfg-1.1.0.tar` & `basecfg-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:59:26.946476 basecfg-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-07 16:58:56.000000 basecfg-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-07 16:59:26.942476 basecfg-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-07 16:58:56.000000 basecfg-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-07 16:58:56.000000 basecfg-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:59:26.946476 basecfg-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:59:26.938476 basecfg-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:59:26.942476 basecfg-1.1.0/src/basecfg/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-07 16:58:56.000000 basecfg-1.1.0/src/basecfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-07 16:58:56.000000 basecfg-1.1.0/src/basecfg/basecfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:59:26.942476 basecfg-1.1.0/src/basecfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-07 16:59:26.000000 basecfg-1.1.0/src/basecfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-07 16:59:26.000000 basecfg-1.1.0/src/basecfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:59:26.000000 basecfg-1.1.0/src/basecfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 16:59:26.000000 basecfg-1.1.0/src/basecfg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:02:15.462575 basecfg-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-09 19:01:47.000000 basecfg-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-09 19:02:15.462575 basecfg-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-09 19:01:47.000000 basecfg-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-09 19:01:47.000000 basecfg-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:02:15.462575 basecfg-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:02:15.462575 basecfg-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:02:15.462575 basecfg-1.2.0/src/basecfg/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 19:01:47.000000 basecfg-1.2.0/src/basecfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-04-09 19:01:47.000000 basecfg-1.2.0/src/basecfg/basecfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:02:15.462575 basecfg-1.2.0/src/basecfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-09 19:02:15.000000 basecfg-1.2.0/src/basecfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-09 19:02:15.000000 basecfg-1.2.0/src/basecfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:02:15.000000 basecfg-1.2.0/src/basecfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 19:02:15.000000 basecfg-1.2.0/src/basecfg.egg-info/top_level.txt
```

### Comparing `basecfg-1.1.0/LICENSE` & `basecfg-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basecfg-1.1.0/PKG-INFO` & `basecfg-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basecfg
-Version: 1.1.0
+Version: 1.2.0
 Summary: typed 12-factor app configuration helper
 Author-email: Ben Burke <actualben@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/edencehealth/basecfg
 Project-URL: Bug Tracker, https://github.com/edencehealth/basecfg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `basecfg-1.1.0/pyproject.toml` & `basecfg-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basecfg"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Ben Burke", email="actualben@users.noreply.github.com" },
 ]
 description = "typed 12-factor app configuration helper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `basecfg-1.1.0/src/basecfg/basecfg.py` & `basecfg-1.2.0/src/basecfg/basecfg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 #!/usr/bin/env python3
 """
 module for specifying configuration options as a class with typed members and
 loading the configuration values from json config files, environment variables,
 and command-line arguments
 """
+# pylint: disable=too-many-arguments
 import argparse
 import json
 import os
+import re
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     NamedTuple,
     Optional,
     Sequence,
+    Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
 )
 
 # pylint: disable=invalid-name
 OptType = TypeVar("OptType")
 OptParserInput = Union[str, int, float]
 
+empty_line = re.compile(r"^\s*([#].*|$)")
+
 
 class OptionMetadata(NamedTuple):
     """
     OptionMetadata is a named tuple which encapsulates data captured by OptFunc
     instances
     """
 
@@ -36,98 +41,139 @@
     option_type: Optional[Any]
     default: Any
     doc: str
     required: bool
     parser: Optional[Callable[[OptParserInput], Any]]
     choices: Optional[Any]
     sep: str
-
-
-class OptFunc:
-    """
-    OptFunc is actually a class that lets you specify important metadata for
-    options in a BaseCfg
-    """
-
-    namespace: List[OptionMetadata]
-
-    def __init__(self) -> None:
-        self.namespace = []
-
-    def __call__(
-        self,
-        default: OptType,
-        doc: str,
-        required: bool = False,
-        parser: Optional[Callable[[OptParserInput], OptType]] = None,
-        choices: Optional[Sequence[OptType]] = None,
-        sep: str = ",",
-    ) -> OptType:
-        """
-        opt captures data related to a BaseCfg option and returns the default
-        the annotated type of the return value is determined by the type of the
-        given default argument
-        """
-        self.namespace.append(
-            OptionMetadata(None, None, default, doc, required, parser, choices, sep)
-        )
-        return default
-
-    def link(self, cls: Any):
-        """class decorator which injects the optfunc attr into the wrapped class"""
-        cls.optfunc = self
-        return cls
-
-
-# Type Alias to enable various uses in BaseCfg
-_OptFunc = OptFunc
+    redact: bool
 
 
 class BaseCfg:
     """
     BaseCfg is a base class for typed application configurations with
     automatic support for taking configuration data from config files,
     environment variables, and command-line arguments. Users of BaseCfg
     subclass basecfg.BaseCfg and add typed class attributes, defining
     them with basecfg.opt
     """
 
-    OptFunc = _OptFunc  # this is an alias to enable users to call BaseCfg.OptFunc()
-    optfunc: _OptFunc  # this is an attribute set by OptFunc.link
+    _optmeta: List[OptionMetadata]  # this is an attribute set by opt.link
     _options: Dict[str, OptionMetadata]
+    _prog: Optional[str] = None
+    _prog_description: Optional[str] = None
+    _prog_epilog: Optional[str] = None
 
     def __init__(
         self,
         json_config_path: Optional[str] = None,
         json_required=False,
+        envfile_path: Optional[str] = None,
+        envfile_required: bool = False,
+        secrets_dir: str = "/run/secrets",
         cli_args: Optional[Sequence[str]] = None,
+        prog: Optional[str] = None,
+        prog_description: Optional[str] = None,
+        prog_epilog: Optional[str] = None,
     ) -> None:
-        """parse data from various sources according to options"""
-        # step 1 is to enrich our metadata about the configuration options, at
-        # this point we finally have the names of the fields and are aware of
-        # their resolved type annotations
-        self._options = {}
+        """
+        Creates a new instance of the configuration class; all arguments are optional
+        json_config_path [str]: the path to a json config file to parse
+        json_required [bool]: if True an exception will be raised if the given json
+            config file is missing
+        cli_args List[str]: instead of using sys.argv, this list of arguments will be
+            passed to the command-line argument processing routine
+        prog [str]: sets the name of the program - used while printing usage
+            documentation when the program is invoked with -h or --help
+        prog_description [str]: describes what the program does - used while printing
+            usage documentation when the program is invoked with -h or --help
+        prog_epilog [str]: additional text appearing at the end of the usage
+            documentation that is printed when the program is invoked with -h or --help
+        """
+        self._prog = prog
+        self._prog_description = prog_description
+        self._prog_epilog = prog_epilog
+
+        # step 1: enrich our metadata about the configuration options and load
+        # default values. At this point we finally have the names of the fields
+        # and are aware of their resolved type annotations.
+        option_metadata = iter(self._optmeta)
 
-        option_metadata = iter(self.optfunc.namespace)
+        self._options = {}
         for key, val in self.__class__.__annotations__.items():
             self._options[key] = next(option_metadata)._replace(
-                name=key, option_type=val
+                name=key,
+                option_type=val,
             )
 
+        # step 2: load config data from json config file
         if json_config_path:
             for key, val in self._parse_json_config(
                 json_config_path, json_required
             ).items():
                 setattr(self, key, val)
-        for key, val in self._parse_envvars().items():
-            setattr(self, key, val)
+
+        # step 3: load config data from .env files
+        if envfile_path:
+            envfile_values = self._read_envfile(envfile_path, envfile_required)
+            self._apply_dict(envfile_values)
+
+        # step 4: load config data from environment variables
+        self._apply_dict(self._read_envvars())
+
+        # step 5: load config data from docker secrets
+        self._apply_dict(
+            {
+                name: self._read_docker_secret(secret_path)
+                for name, secret_path in self._list_docker_secrets(secrets_dir).items()
+            }
+        )
+
+        # step 6: load config data from command-line arguments
         for key, val in self._parse_args(cli_args).items():
             if val is not None:
                 setattr(self, key, val)
 
+    @classmethod
+    def optfunc(cls):
+        """
+        helper function which returns a uniquely-namespaced opt function which
+        can  be used to define metadata for BaseCfg option fields
+        """
+        namespace: List[OptionMetadata] = []
+
+        def opt(
+            default: OptType,
+            doc: str,
+            required: bool = False,
+            parser: Optional[Callable[[OptParserInput], OptType]] = None,
+            choices: Optional[Sequence[OptType]] = None,
+            sep: str = ",",
+            redact: bool = False,
+        ) -> OptType:
+            """
+            opt captures data related to a BaseCfg option and returns the default
+            the annotated type of the return value is determined by the type of the
+            given default argument
+            """
+            namespace.append(
+                OptionMetadata(
+                    None, None, default, doc, required, parser, choices, sep, redact
+                )
+            )
+            return default
+
+        def link(cls) -> Type[cls]:
+            setattr(cls, "_optmeta", namespace)
+            return cls
+
+        opt.link = link
+
+        return opt
+
     def _parse_json_config(self, path: str, required: bool = False) -> Dict[str, Any]:
         """parses the configuration from the json file at the given path"""
         result: Dict[str, Any] = {}
         if not os.path.isfile(path):
             if required:
                 raise RuntimeError(f"required json config file {path} was not found")
             # no file, not required
@@ -199,24 +245,26 @@
 
     def _keys(self) -> Sequence[str]:
         """return a list of keys in this configuration"""
         return [key for key in self._options if not key.startswith("_")]
 
     def _parse_args(self, cli_args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         """generate an args parser and call it"""
-        argp = argparse.ArgumentParser()
+        argp = argparse.ArgumentParser(
+            prog=self._prog,
+            description=self._prog_description,
+            epilog=self._prog_epilog,
+        )
         for optname, option in self._options.items():
             arg_name = "--" + optname.replace("_", "-")
             option_type = self._base_type(option.option_type)
 
             # use this for as little as possible (because it doesn't get type checked)
             # it could be good to switch to TypedDict for this
-            arg_config: Dict[str, Any] = {
-                "action": "store",
-            }
+            arg_config: Dict[str, Any] = {"action": "store"}
             if option_type == "bool":
                 arg_config["action"] = argparse.BooleanOptionalAction
             elif option_type == "int":
                 arg_config["type"] = int
             elif option_type == "float":
                 arg_config["type"] = float
             elif option_type == "List[str]":
@@ -238,65 +286,141 @@
                 required=False,
                 choices=option.choices,
                 **arg_config,
             )
 
         return vars(argp.parse_args(args=cli_args))
 
-    def _parse_envvars(self) -> Dict[str, Any]:
-        """parse environment variables for configuration values"""
-        # pylint: disable=too-many-branches
-        result: Dict[str, Any] = {}
-
-        for optname, option in self._options.items():
-            envvar_name: str = optname.upper()
-            envvar_value: str
-            if envvar_name in os.environ:
-                envvar_value = os.environ[envvar_name]
-            elif optname in os.environ:
-                envvar_name = optname
-                envvar_value = os.environ[envvar_name]
-            else:
-                continue
+    def _read_envvars(self) -> Dict[str, str]:
+        """read environment variables for configuration values"""
+        result: Dict[str, str] = {}
+
+        for optname in self._options:
+            for envvar_name in (optname.upper(), optname):
+                if envvar_name in os.environ:
+                    result[optname] = os.environ[envvar_name]
+                    break
+        return result
 
-            coerced_value: Any = envvar_value
+    def _apply_dict(self, inputs: Dict[str, str]) -> bool:
+        """
+        given a dict mapping option names to string input values, convert the values to
+        the selected type
+        """
+        # pylint: disable=too-many-branches
+        for optname, input_value in inputs.items():
+            option = self._options[optname]
             option_type = self._base_type(option.option_type)
-            if option_type == "str":
-                coerced_value = envvar_value
+
+            coerced_value: Any = input_value
+            if option.parser:
+                coerced_value = option.parser(input_value)
+            elif option_type == "str":
+                coerced_value = input_value
             elif option_type == "bool":
-                coerced_value = self._parse_bool(envvar_value)
+                coerced_value = self._parse_bool(input_value)
             elif option_type == "int":
-                coerced_value = int(envvar_value)
+                coerced_value = int(input_value)
             elif option_type == "float":
-                coerced_value = float(envvar_value)
+                coerced_value = float(input_value)
             elif option_type == "List[str]":
-                coerced_value = envvar_value.split(option.sep)
+                coerced_value = input_value.split(option.sep)
             elif option_type == "List[int]":
-                coerced_value = [int(n) for n in envvar_value.split(option.sep)]
+                coerced_value = [int(n) for n in input_value.split(option.sep)]
             elif option_type == "List[float]":
-                coerced_value = [float(f) for f in envvar_value.split(option.sep)]
+                coerced_value = [float(f) for f in input_value.split(option.sep)]
             elif option_type == "List[bool]":
                 coerced_value = [
-                    self._parse_bool(s) for s in envvar_value.split(option.sep)
+                    self._parse_bool(s) for s in input_value.split(option.sep)
                 ]
             else:
                 raise ValueError(
                     f"Don't know how to parse type {option.option_type} "
                     f"({option_type})"
                 )
+
             if option.choices:
                 if coerced_value not in option.choices:
                     raise ValueError(
-                        f"{optname} (envvar: {envvar_name}): "
+                        f"{optname} (envvar: {input_value}): "
                         f'value "{coerced_value}" not in specified '
                         f"choices list ({str(option.choices)})"
                     )
-            result[optname] = coerced_value
+
+            setattr(self, optname, coerced_value)
+
+        return True
+
+    @staticmethod
+    def _read_envfile(path: str, required: bool = False) -> Dict[str, str]:
+        """
+        parse entries in an environment file (aka .env) - the format supported
+        is described in the "docker run" (NOT compose) documentation. Notably
+        no quotation marks nor multi-line values are supported and comments are
+        only valid at the beginning of the line
+        """
+        result: Dict[str, str] = {}
+        try:
+            dotenvfh = open(path, "rt", encoding="utf8")
+        except FileNotFoundError as fnf:
+            if not required:
+                return result
+            raise fnf from None
+        with dotenvfh as dotenv:
+            for i, line in enumerate(dotenv.readlines()):
+                if empty_line.match(line):
+                    continue
+                if "=" not in line:
+                    raise ValueError(
+                        f'envfile parsing error; file:"{path}" line:{i}; data line '
+                        f'contains no "-" character'
+                    )
+                key, value = line.split("=", 1)
+                result[key.lower().strip()] = value.strip()
+        return result
+
+    @staticmethod
+    def _list_docker_secrets(
+        secrets_dir: str = "/run/secrets/",
+    ) -> Dict[str, str]:
+        """
+        return a dict mapping names to full paths for docker secrets found
+        on disk
+        """
+        result: Dict[str, str] = {}
+        try:
+            dircontents = os.listdir(secrets_dir)
+        except FileNotFoundError:
+            return result
+        for name in dircontents:
+            if name.startswith("."):
+                continue
+            path = os.path.abspath(os.path.join(secrets_dir, name))
+            if not os.path.isfile(path):
+                continue
+            result[name] = path
         return result
 
+    @staticmethod
+    def _read_docker_secret(
+        path: str,
+        open_mode: str = "rt",
+        encoding: Optional[str] = "utf-8",
+        strip_whitespace: bool = True,
+    ) -> str:
+        """
+        open the secrets directory, look for a file with the given name; return its
+        contents, optionally stripping whitespace from the value
+        """
+        with open(path, open_mode, encoding=encoding) as secret:
+            contents = secret.read()
+        if strip_whitespace:
+            return contents.strip()
+        return contents
+
     def _base_type(self, type_spec: Any) -> str:
         """returns a string representing the type of object"""
         # print(
         #     f"spec: {type_spec}; "
         #     f"name: {type_spec.__name__}; "
         #     f"origin: {get_origin(type_spec)}; "
         #     f"args: {get_args(type_spec)}"
@@ -316,7 +440,22 @@
         # print(f"result is: {result}")
         return result
 
     @staticmethod
     def _parse_bool(value: str) -> bool:
         """evaluates the string value in a boolean context and returns the result"""
         return value.lower().strip() in ("1", "enable", "on", "true", "t", "y", "yes")
+
+    def __getitem__(self, key):
+        """returns the value for the given configuration variable"""
+        try:
+            return getattr(self, key)
+        except AttributeError:
+            raise KeyError(f'key "{key}" not found') from None
+
+    def __len__(self):
+        """returns the number of configuration options in the class"""
+        return len(self._options)
+
+    def __iter__(self):
+        """returns keys iterator"""
+        return iter(self._options.keys())
```

### Comparing `basecfg-1.1.0/src/basecfg.egg-info/PKG-INFO` & `basecfg-1.2.0/src/basecfg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basecfg
-Version: 1.1.0
+Version: 1.2.0
 Summary: typed 12-factor app configuration helper
 Author-email: Ben Burke <actualben@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/edencehealth/basecfg
 Project-URL: Bug Tracker, https://github.com/edencehealth/basecfg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
```

