# Comparing `tmp/devcontainer_manager-1.3.0.tar.gz` & `tmp/devcontainer_manager-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcontainer_manager-1.3.0.tar", last modified: Sun Dec 11 13:18:59 2022, max compression
+gzip compressed data, was "devcontainer_manager-1.3.1.tar", last modified: Sun Apr  9 12:59:38 2023, max compression
```

## Comparing `devcontainer_manager-1.3.0.tar` & `devcontainer_manager-1.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 13:18:59.655528 devcontainer_manager-1.3.0/
--rw-rw-r--   0 root         (0) root         (0)     1061 2022-01-06 15:44:11.000000 devcontainer_manager-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      156 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6285 2022-12-11 13:18:59.655528 devcontainer_manager-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5996 2022-12-11 12:49:42.000000 devcontainer_manager-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 13:18:59.651528 devcontainer_manager-1.3.0/devcontainer_manager/
--rw-r--r--   0 root         (0) root         (0)       22 2022-12-11 13:17:58.000000 devcontainer_manager-1.3.0/devcontainer_manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/devcontainer_manager/__main__.py
--rw-r--r--   0 root         (0) root         (0)      880 2022-12-11 13:16:32.000000 devcontainer_manager-1.3.0/devcontainer_manager/alias.py
--rw-r--r--   0 root         (0) root         (0)     3872 2022-12-11 13:13:57.000000 devcontainer_manager-1.3.0/devcontainer_manager/base_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 13:18:59.651528 devcontainer_manager-1.3.0/devcontainer_manager/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/devcontainer_manager/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1896 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/devcontainer_manager/cli/alias.py
--rw-r--r--   0 root         (0) root         (0)     4284 2022-12-11 13:16:43.000000 devcontainer_manager-1.3.0/devcontainer_manager/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     8427 2022-12-11 13:13:28.000000 devcontainer_manager-1.3.0/devcontainer_manager/config.py
--rw-r--r--   0 root         (0) root         (0)      336 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/devcontainer_manager/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1673 2022-12-11 13:13:18.000000 devcontainer_manager-1.3.0/devcontainer_manager/global_config.py
--rw-r--r--   0 root         (0) root         (0)      412 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/devcontainer_manager/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 13:18:59.651528 devcontainer_manager-1.3.0/devcontainer_manager/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 13:18:59.651528 devcontainer_manager-1.3.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 13:18:59.655528 devcontainer_manager-1.3.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/
--rw-rw-r--   0 root         (0) root         (0)      233 2022-01-07 00:28:25.000000 devcontainer_manager-1.3.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/build.sh
--rw-r--r--   0 root         (0) root         (0)      240 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1662 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)     1834 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/devcontainer_manager/types.py
--rw-r--r--   0 root         (0) root         (0)     1203 2022-11-13 22:15:55.000000 devcontainer_manager-1.3.0/devcontainer_manager/util.py
--rw-r--r--   0 root         (0) root         (0)     2691 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/devcontainer_manager/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 13:18:59.651528 devcontainer_manager-1.3.0/devcontainer_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6285 2022-12-11 13:18:59.000000 devcontainer_manager-1.3.0/devcontainer_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1061 2022-12-11 13:18:59.000000 devcontainer_manager-1.3.0/devcontainer_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-11 13:18:59.000000 devcontainer_manager-1.3.0/devcontainer_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2022-12-11 13:18:59.000000 devcontainer_manager-1.3.0/devcontainer_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2022-12-11 13:18:59.000000 devcontainer_manager-1.3.0/devcontainer_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-11 13:18:59.000000 devcontainer_manager-1.3.0/devcontainer_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      408 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-11 13:18:59.655528 devcontainer_manager-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      991 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/
+-rw-rw-r--   0 root         (0) root         (0)     1061 2022-01-06 15:44:11.000000 devcontainer_manager-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-09 12:27:48.000000 devcontainer_manager-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-04-09 12:55:25.000000 devcontainer_manager-1.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/devcontainer_manager/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-09 12:54:42.000000 devcontainer_manager-1.3.1/devcontainer_manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-04-09 12:25:48.000000 devcontainer_manager-1.3.1/devcontainer_manager/alias.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-04-09 12:14:41.000000 devcontainer_manager-1.3.1/devcontainer_manager/base_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/devcontainer_manager/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/cli/alias.py
+-rw-r--r--   0 root         (0) root         (0)     4303 2023-04-09 12:51:56.000000 devcontainer_manager-1.3.1/devcontainer_manager/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8497 2023-04-09 12:52:29.000000 devcontainer_manager-1.3.1/devcontainer_manager/config.py
+-rw-r--r--   0 root         (0) root         (0)      336 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2022-12-11 13:13:18.000000 devcontainer_manager-1.3.1/devcontainer_manager/global_config.py
+-rw-r--r--   0 root         (0) root         (0)      412 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.316182 devcontainer_manager-1.3.1/devcontainer_manager/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.316182 devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/
+-rw-rw-r--   0 root         (0) root         (0)      233 2022-01-07 00:28:25.000000 devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/build.sh
+-rw-r--r--   0 root         (0) root         (0)      240 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)     1834 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/types.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2022-11-13 22:15:55.000000 devcontainer_manager-1.3.1/devcontainer_manager/util.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      991 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/setup.py
```

### Comparing `devcontainer_manager-1.3.0/LICENSE` & `devcontainer_manager-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.0/PKG-INFO` & `devcontainer_manager-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devcontainer_manager
-Version: 1.3.0
+Version: 1.3.1
 Summary: UNKNOWN
 Home-page: https://github.com/gnox/devcontainer-manager
 Author: gnox
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `devcontainer_manager-1.3.0/README.md` & `devcontainer_manager-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager/alias.py` & `devcontainer_manager-1.3.1/devcontainer_manager/alias.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,16 +15,20 @@
             "aliases for templates, can be added using,\n" "`devcontainer_manager alias --help`"
         ),
     )
 
     _not_none = validator("*", pre=True, allow_reuse=True)(default_if_none)
 
     def is_alias(self, alias: str):
+        if isinstance(alias, Path):
+            alias = alias.as_posix()
         return alias in self.aliases
 
     def resolve(self, alias: str):
+        if isinstance(alias, Path):
+            alias = alias.as_posix()
         return self.aliases.get(alias, alias)
 
     def path_to_alias(self, path: Path):
         path = path.resolve()
         ret = [k for k, p in self.aliases.items() if p.resolve() == path][0]
         return path if not ret else ret
```

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager/base_config.py` & `devcontainer_manager-1.3.1/devcontainer_manager/base_config.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager/cli/alias.py` & `devcontainer_manager-1.3.1/devcontainer_manager/cli/alias.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager/cli/cli.py` & `devcontainer_manager-1.3.1/devcontainer_manager/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,26 +47,25 @@
     configs = [Config.parse_file(t).merge_bases() for t in templates]
     merged_config = global_config.merge_bases().defaults | reduce(lambda a, b: a | b, configs)
 
     if print_config:
         typer.echo(merged_config.yaml())
         raise typer.Exit()
 
+    config_path = global_config.defaults.project_path / global_config.override_config_path
     COOKIECUTTER_CONFIG.write_text(
-        merged_config.resolve().json(indent=4, exclude={"base_config": True})
+        merged_config.resolve(config_path).json(indent=4, exclude={"base_config": True})
     )
     cookiecutter(TEMPLATE_DIR.as_posix(), no_input=True, overwrite_if_exists=True)
 
     if not from_override:
         config_paths = [alias_config.path_to_alias(cfg.config_path) for cfg in configs]
         override_config = Config.none()
         override_config.base_config = config_paths
-        override_config.write_yaml(
-            global_config.defaults.project_path / global_config.override_config_path
-        )
+        override_config.write_yaml(config_path)
 
     devcontainer_dir = merged_config.project_path / ".devcontainer"
     if not merged_config.docker.file:
         (devcontainer_dir / "devcontainer.Dockerfile").unlink()
         (devcontainer_dir / "build.sh").unlink()
 
     if build:
```

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager/config.py` & `devcontainer_manager-1.3.1/devcontainer_manager/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,29 +173,29 @@
     )
     devcontainer: Optional[DevcontainerConfig] = DevcontainerConfig()
     # vscode: Optional[VSCodeConfig] = VSCodeConfig()
     docker: Optional[DockerConfig] = DockerConfig()
 
     _not_none = validator("*", pre=True, allow_reuse=True)(default_if_none)
 
-    def resolve(self) -> "ResolvedConfig":
+    def resolve(self, config_path: Path = None) -> "ResolvedConfig":
         values = self.dict()
         values.update(GlobalVariables().dict())
 
         cfg_copy: Config = self.copy(deep=True)
         cfg_copy.devcontainer.workspace_mount = (
             self.devcontainer.workspace_mount.to_devcontainer_format()
         )
         cfg_copy.devcontainer.mounts = [
             mount.to_devcontainer_format() for mount in cfg_copy.devcontainer.mounts
         ]
 
         rendered_template = render_recursive_template(cfg_copy.json(), values)
         new_config = Config.parse_raw(rendered_template)
-        new_config.config_path = self.config_path
+        new_config.config_path = config_path if config_path is not None else self.config_path
         return ResolvedConfig.parse_obj(new_config.dict(exclude={"config_path": {}}))
 
     @classmethod
     def none(cls):
         return Config.construct(
             base_config=None,
             devcontainer=DevcontainerConfig.none(),
```

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager/global_config.py` & `devcontainer_manager-1.3.1/devcontainer_manager/global_config.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json` & `devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager/types.py` & `devcontainer_manager-1.3.1/devcontainer_manager/types.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager/util.py` & `devcontainer_manager-1.3.1/devcontainer_manager/util.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager/yaml.py` & `devcontainer_manager-1.3.1/devcontainer_manager/yaml.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager.egg-info/PKG-INFO` & `devcontainer_manager-1.3.1/devcontainer_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devcontainer-manager
-Version: 1.3.0
+Version: 1.3.1
 Summary: UNKNOWN
 Home-page: https://github.com/gnox/devcontainer-manager
 Author: gnox
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `devcontainer_manager-1.3.0/devcontainer_manager.egg-info/SOURCES.txt` & `devcontainer_manager-1.3.1/devcontainer_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.0/setup.py` & `devcontainer_manager-1.3.1/setup.py`

 * *Files identical despite different names*

