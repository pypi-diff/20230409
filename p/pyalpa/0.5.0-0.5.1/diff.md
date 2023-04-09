# Comparing `tmp/pyalpa-0.5.0.tar.gz` & `tmp/pyalpa-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.5.0.tar", max compression
+gzip compressed data, was "pyalpa-0.5.1.tar", max compression
```

## Comparing `pyalpa-0.5.0.tar` & `pyalpa-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-04-09 14:32:24.639143 pyalpa-0.5.0/LICENSE
--rw-r--r--   0        0        0     1631 2023-04-09 14:32:24.639143 pyalpa-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/cli/__init__.py
--rw-r--r--   0        0        0      710 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1230 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/cli/base.py
--rw-r--r--   0        0        0     6330 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/cli/local_repo.py
--rw-r--r--   0        0        0        0 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/config/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/config/local_config.py
--rw-r--r--   0        0        0     2673 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/config/packit.py
--rw-r--r--   0        0        0      813 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/constants.py
--rw-r--r--   0        0        0      111 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/exceptions.py
--rw-r--r--   0        0        0     3579 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/gh.py
--rw-r--r--   0        0        0     1447 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/messages.py
--rw-r--r--   0        0        0    12949 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/repository.py
--rw-r--r--   0        0        0     3858 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/upstream_integration.py
--rw-r--r--   0        0        0      762 2023-04-09 14:32:24.639143 pyalpa-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 pyalpa-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 14:49:39.981480 pyalpa-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1631 2023-04-09 14:49:39.981480 pyalpa-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      710 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1230 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/cli/base.py
+-rw-r--r--   0        0        0     6330 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0        0 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1015 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/config/local_config.py
+-rw-r--r--   0        0        0     2673 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/config/packit.py
+-rw-r--r--   0        0        0      813 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/constants.py
+-rw-r--r--   0        0        0      111 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/exceptions.py
+-rw-r--r--   0        0        0     3579 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/gh.py
+-rw-r--r--   0        0        0     1447 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/messages.py
+-rw-r--r--   0        0        0    12955 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/repository.py
+-rw-r--r--   0        0        0     3858 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      762 2023-04-09 14:49:39.981480 pyalpa-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 pyalpa-0.5.1/PKG-INFO
```

### Comparing `pyalpa-0.5.0/LICENSE` & `pyalpa-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/README.md` & `pyalpa-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/alpa/cli/alpa_repo.py` & `pyalpa-0.5.1/alpa/cli/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/alpa/cli/base.py` & `pyalpa-0.5.1/alpa/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/alpa/cli/local_repo.py` & `pyalpa-0.5.1/alpa/cli/local_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/alpa/config/local_config.py` & `pyalpa-0.5.1/alpa/config/local_config.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/alpa/config/packit.py` & `pyalpa-0.5.1/alpa/config/packit.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/alpa/constants.py` & `pyalpa-0.5.1/alpa/constants.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/alpa/gh.py` & `pyalpa-0.5.1/alpa/gh.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/alpa/messages.py` & `pyalpa-0.5.1/alpa/messages.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/alpa/repository.py` & `pyalpa-0.5.1/alpa/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         if packit_conf.packit_config_file_exists() and not override:
             return False
 
         packit_conf.create_packit_config()
         return True
 
     def get_git_root(self) -> Optional[Path]:
-        return self.local_repo.working_tree_dir
+        return Path(self.local_repo.working_tree_dir)
 
 
 class AlpaRepo(LocalRepo):
     def __init__(self, repo_path: Path, gh_api: Optional[GithubAPI] = None) -> None:
         super().__init__(repo_path)
 
         self.gh_api = gh_api or GithubAPI(self.repo_name)
```

### Comparing `pyalpa-0.5.0/alpa/upstream_integration.py` & `pyalpa-0.5.1/alpa/upstream_integration.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.0/pyproject.toml` & `pyalpa-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.5.0"
+version = "0.5.1"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
```

### Comparing `pyalpa-0.5.0/PKG-INFO` & `pyalpa-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.5.0
+Version: 0.5.1
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
```

