# Comparing `tmp/gpush-1.0.4.tar.gz` & `tmp/gpush-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpush-1.0.4.tar", last modified: Sat Apr  1 20:36:09 2023, max compression
+gzip compressed data, was "gpush-1.1.0.tar", last modified: Sun Apr  9 09:17:00 2023, max compression
```

## Comparing `gpush-1.0.4.tar` & `gpush-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 20:36:09.765000 gpush-1.0.4/
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-01 20:36:09.765000 gpush-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-04-01 20:36:06.000000 gpush-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 20:36:09.765000 gpush-1.0.4/gpush.egg-info/
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-01 20:36:09.000000 gpush-1.0.4/gpush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2023-04-01 20:36:09.000000 gpush-1.0.4/gpush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 20:36:09.000000 gpush-1.0.4/gpush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-01 20:36:09.000000 gpush-1.0.4/gpush.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1770 2023-04-01 20:36:06.000000 gpush-1.0.4/gpush.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-01 20:36:06.000000 gpush-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-01 20:36:09.765000 gpush-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      144 2023-04-01 20:36:07.000000 gpush-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:17:00.449565 gpush-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-09 09:17:00.445564 gpush-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      574 2023-04-09 09:16:57.000000 gpush-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:17:00.445564 gpush-1.1.0/gpush.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-09 09:17:00.000000 gpush-1.1.0/gpush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2023-04-09 09:17:00.000000 gpush-1.1.0/gpush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 09:17:00.000000 gpush-1.1.0/gpush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-09 09:17:00.000000 gpush-1.1.0/gpush.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-04-09 09:16:57.000000 gpush-1.1.0/gpush.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-09 09:16:57.000000 gpush-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 09:17:00.449565 gpush-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      144 2023-04-09 09:16:58.000000 gpush-1.1.0/setup.py
```

### Comparing `gpush-1.0.4/gpush.py` & `gpush-1.1.0/gpush.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     Function to push commit up to Git on the current branch for the repository
     :param commit_message: String containing the conventional commit message formatted commit
     message
     :return: True/False
     """
     try:
         repo = Repo(search_parent_directories=True)
-        repo.index.commit(commit_message)
+        repo.index.write()
+        repo.git.commit("-m" + commit_message)
         repo.git.push("--set-upstream", "origin", repo.active_branch)
         print("pushing commit: " + commit_message)
         print("Pushed successfully")
     except Exception as error_message:
         print("Some error occured while pushing the code:")
         print(str(error_message))
```

