# Comparing `tmp/pyalpa-0.4.0.tar.gz` & `tmp/pyalpa-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.4.0.tar", max compression
+gzip compressed data, was "pyalpa-0.5.0.tar", max compression
```

## Comparing `pyalpa-0.4.0.tar` & `pyalpa-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-04-07 22:30:15.199819 pyalpa-0.4.0/LICENSE
--rw-r--r--   0        0        0     1631 2023-04-07 22:30:15.199819 pyalpa-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/cli/__init__.py
--rw-r--r--   0        0        0      710 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1230 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/cli/base.py
--rw-r--r--   0        0        0     6330 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/cli/local_repo.py
--rw-r--r--   0        0        0        0 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/config/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/config/local_config.py
--rw-r--r--   0        0        0     2243 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/config/packit.py
--rw-r--r--   0        0        0      813 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/constants.py
--rw-r--r--   0        0        0      111 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/exceptions.py
--rw-r--r--   0        0        0     3579 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/gh.py
--rw-r--r--   0        0        0     1447 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/messages.py
--rw-r--r--   0        0        0    12804 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/repository.py
--rw-r--r--   0        0        0     3858 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/upstream_integration.py
--rw-r--r--   0        0        0      762 2023-04-07 22:30:15.199819 pyalpa-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 pyalpa-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 14:32:24.639143 pyalpa-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1631 2023-04-09 14:32:24.639143 pyalpa-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      710 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1230 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/cli/base.py
+-rw-r--r--   0        0        0     6330 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0        0 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1015 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/config/local_config.py
+-rw-r--r--   0        0        0     2673 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/config/packit.py
+-rw-r--r--   0        0        0      813 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/constants.py
+-rw-r--r--   0        0        0      111 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/exceptions.py
+-rw-r--r--   0        0        0     3579 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/gh.py
+-rw-r--r--   0        0        0     1447 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/messages.py
+-rw-r--r--   0        0        0    12949 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/repository.py
+-rw-r--r--   0        0        0     3858 2023-04-09 14:32:24.639143 pyalpa-0.5.0/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      762 2023-04-09 14:32:24.639143 pyalpa-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 pyalpa-0.5.0/PKG-INFO
```

### Comparing `pyalpa-0.4.0/LICENSE` & `pyalpa-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.4.0/README.md` & `pyalpa-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyalpa-0.4.0/alpa/cli/alpa_repo.py` & `pyalpa-0.5.0/alpa/cli/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.4.0/alpa/cli/base.py` & `pyalpa-0.5.0/alpa/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.4.0/alpa/cli/local_repo.py` & `pyalpa-0.5.0/alpa/cli/local_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.4.0/alpa/config/local_config.py` & `pyalpa-0.5.0/alpa/config/local_config.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.4.0/alpa/config/packit.py` & `pyalpa-0.5.0/alpa/config/packit.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,41 +12,54 @@
     def __init__(self, package_name: str) -> None:
         self.package_name = package_name
         self.working_dir = Path(getcwd())
         self.metadata = MetadataConfig.get_config(self.working_dir)
         self.alpa_repo_config = AlpaRepoConfig.get_config()
 
     def get_packit_config(self) -> dict:
+        jobs = [
+            {
+                "job": "copr_build",
+                "trigger": "pull_request",
+                "targets": list(self.metadata.targets),
+                "owner": self.alpa_repo_config.copr_owner,
+                "project": f"{self.alpa_repo_config.copr_repo}-pull-requests",
+            },
+            {
+                "job": "copr_build",
+                "trigger": "commit",
+                "branch": self.package_name,
+                "targets": list(self.metadata.targets),
+                "owner": self.alpa_repo_config.copr_owner,
+                "project": self.alpa_repo_config.copr_repo,
+            },
+        ]
+
+        if self.metadata.autoupdate is not None:
+            autoupdate_dict = {
+                "job": "copr_build",
+                "trigger": "commit",
+                "branch": f"__alpa_autoupdate_{self.package_name}",
+                "targets": list(self.metadata.targets),
+                "owner": self.alpa_repo_config.copr_owner,
+                "project": f"{self.alpa_repo_config.copr_repo}-pull-requests",
+            }
+            jobs.append(autoupdate_dict)
+
         return {
             "specfile_path": f"{self.package_name}.spec",
             "srpm_build_deps": ["pip"],
             "actions": {
                 "create-archive": [
                     "pip install pyalpa",
                     'bash -c "alpa get-pkg-archive"',
                     f'bash -c "ls -1 ./{self.package_name}-*.tar.gz"',
                 ],
             },
-            "jobs": [
-                {
-                    "job": "copr_build",
-                    "trigger": "pull_request",
-                    "targets": list(self.metadata.targets),
-                    "owner": self.alpa_repo_config.copr_owner,
-                    "project": f"{self.alpa_repo_config.copr_repo}-pull-requests",
-                },
-                {
-                    "job": "copr_build",
-                    "trigger": "commit",
-                    "branch": self.package_name,
-                    "targets": list(self.metadata.targets),
-                    "owner": self.alpa_repo_config.copr_owner,
-                    "project": self.alpa_repo_config.copr_repo,
-                },
-            ],
+            "jobs": jobs,
         }
 
     def packit_config_file_exists(self) -> bool:
         for packit_config_name in PACKIT_CONFIG_NAMES:
             files_in_dir = [
                 file.name for file in self.working_dir.iterdir() if file.is_file()
             ]
```

### Comparing `pyalpa-0.4.0/alpa/constants.py` & `pyalpa-0.5.0/alpa/constants.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.4.0/alpa/gh.py` & `pyalpa-0.5.0/alpa/gh.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.4.0/alpa/messages.py` & `pyalpa-0.5.0/alpa/messages.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.4.0/alpa/repository.py` & `pyalpa-0.5.0/alpa/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 class LocalRepo:
     def __init__(self, repo_path: Path) -> None:
         self.repo_path = repo_path
         # TODO: this will differ in the future with repo_path
         self.repo_root_path = repo_path
-        self.local_repo = Repo(str(self.repo_path))
+        self.local_repo = Repo(str(self.repo_path), search_parent_directories=True)
         self.git_cmd = self.local_repo.git
 
         if not self._is_repo_in_predefined_state():
             raise ClickException(NOT_IN_PREDEFINED_STATE)
 
         # do it after predefined state is checked since this depends on it
         # (see comment in the _should_be_fork)
@@ -59,15 +59,15 @@
 
     @property
     def branch(self) -> str:
         return self.local_repo.active_branch.name
 
     @property
     def package(self) -> str:
-        return self.branch.lstrip(ALPA_FEAT_BRANCH_PREFIX)
+        return self.branch.removeprefix(ALPA_FEAT_BRANCH_PREFIX)
 
     @staticmethod
     def get_feat_branch_of_package(package: str) -> str:
         return ALPA_FEAT_BRANCH.format(pkgname=package)
 
     @property
     def feat_branch(self) -> str:
@@ -282,26 +282,29 @@
     def push(self, branch: str) -> None:
         # you always want to push to origin, even from a fork
         click.echo(self.git_cmd.push(ORIGIN_NAME, branch))
 
     def full_reponame(self) -> str:
         for remote in self.local_repo.remotes:
             if remote.name == self.remote_name:
-                return remote.url.split(":")[-1].rstrip(".git")
+                return remote.url.split(":")[-1].removesuffix(".git")
 
         return ""
 
     def create_packit_config(self, override: bool) -> bool:
         packit_conf = PackitConfig(self.package)
         if packit_conf.packit_config_file_exists() and not override:
             return False
 
         packit_conf.create_packit_config()
         return True
 
+    def get_git_root(self) -> Optional[Path]:
+        return self.local_repo.working_tree_dir
+
 
 class AlpaRepo(LocalRepo):
     def __init__(self, repo_path: Path, gh_api: Optional[GithubAPI] = None) -> None:
         super().__init__(repo_path)
 
         self.gh_api = gh_api or GithubAPI(self.repo_name)
         self.gh_repo = self.gh_api.get_repo(self.namespace, self.repo_name)
@@ -338,15 +341,15 @@
         if not gh_repo.is_fork:
             return
 
         Remote.create(local_repo, UPSTREAM_NAME, gh_repo.upstream_clone_url)
 
     @staticmethod
     def _get_repo_name_from_url(repo_url: str) -> str:
-        return repo_url.split("/")[-1].rstrip(".git")
+        return repo_url.split("/")[-1].removesuffix(".git")
 
     @staticmethod
     def _check_for_permission_and_fork(
         clone_fork: bool, gh_repo: GithubRepo
     ) -> tuple[bool, str]:
         if clone_fork and not gh_repo.is_fork:
             return False, CLONED_REPO_IS_NOT_FORK
```

### Comparing `pyalpa-0.4.0/alpa/upstream_integration.py` & `pyalpa-0.5.0/alpa/upstream_integration.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.4.0/pyproject.toml` & `pyalpa-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.4.0"
+version = "0.5.0"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = ">=8.0.0"
 gitpython = ">=3.0"
 pygithub = ">=1.4"
 pyyaml = ">=5.0"
-alpa-conf = ">=0.3.2"
+alpa-conf = ">=0.4.0"
 specfile = ">=0.13.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.0.0"
```

### Comparing `pyalpa-0.4.0/PKG-INFO` & `pyalpa-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.4.0
+Version: 0.5.0
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: alpa-conf (>=0.3.2)
+Requires-Dist: alpa-conf (>=0.4.0)
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: gitpython (>=3.0)
 Requires-Dist: pygithub (>=1.4)
 Requires-Dist: pyyaml (>=5.0)
 Requires-Dist: specfile (>=0.13.0)
 Project-URL: Repository, https://github.com/alpa-team/alpa
 Description-Content-Type: text/markdown
```

