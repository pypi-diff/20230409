# Comparing `tmp/awsslack-0.1.0.tar.gz` & `tmp/awsslack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsslack-0.1.0.tar", max compression
+gzip compressed data, was "awsslack-0.1.1.tar", max compression
```

## Comparing `awsslack-0.1.0.tar` & `awsslack-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1032 2023-03-24 19:56:28.581324 awsslack-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-24 19:56:28.581324 awsslack-0.1.0/awsslack/__init__.py
--rw-r--r--   0        0        0       88 2023-03-24 21:37:10.353893 awsslack-0.1.0/awsslack/__main__.py
--rw-r--r--   0        0        0        0 2023-03-24 20:22:19.163395 awsslack-0.1.0/awsslack/commands/__init__.py
--rw-r--r--   0        0        0     6561 2023-04-09 18:23:23.264850 awsslack-0.1.0/awsslack/commands/config.py
--rw-r--r--   0        0        0     1243 2023-04-09 16:43:43.535461 awsslack-0.1.0/awsslack/main.py
--rw-r--r--   0        0        0        0 2023-03-24 21:41:50.014268 awsslack-0.1.0/awsslack/utils/__init__.py
--rw-r--r--   0        0        0     5859 2023-03-24 19:56:28.581324 awsslack-0.1.0/awsslack/utils/code_build.py
--rw-r--r--   0        0        0    12550 2023-03-24 19:56:28.581324 awsslack-0.1.0/awsslack/utils/code_deploy.py
--rw-r--r--   0        0        0      848 2023-04-09 18:03:49.063015 awsslack-0.1.0/awsslack/utils/yaml.py
--rw-r--r--   0        0        0      693 2023-03-24 20:18:59.355140 awsslack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 awsslack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1032 2023-03-24 19:56:28.581324 awsslack-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/__main__.py
+-rw-r--r--   0        0        0     5859 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/code_build.py
+-rw-r--r--   0        0        0    12550 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/code_deploy.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/commands/__init__.py
+-rw-r--r--   0        0        0     6561 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/commands/config.py
+-rw-r--r--   0        0        0     1243 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/main.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/utils/__init__.py
+-rw-r--r--   0        0        0     5859 2023-03-24 19:56:28.581324 awsslack-0.1.1/awsslack/utils/code_build.py
+-rw-r--r--   0        0        0    12550 2023-03-24 19:56:28.581324 awsslack-0.1.1/awsslack/utils/code_deploy.py
+-rw-r--r--   0        0        0      848 2023-04-09 18:42:34.202655 awsslack-0.1.1/awsslack/utils/yaml.py
+-rw-r--r--   0        0        0      709 2023-04-09 18:44:27.094832 awsslack-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 awsslack-0.1.1/PKG-INFO
```

### Comparing `awsslack-0.1.0/README.md` & `awsslack-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.0/awsslack/commands/config.py` & `awsslack-0.1.1/awsslack/commands/config.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.0/awsslack/main.py` & `awsslack-0.1.1/awsslack/main.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.0/awsslack/utils/code_build.py` & `awsslack-0.1.1/awsslack/code_build.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.0/awsslack/utils/code_deploy.py` & `awsslack-0.1.1/awsslack/code_deploy.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.0/awsslack/utils/yaml.py` & `awsslack-0.1.1/awsslack/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.0/pyproject.toml` & `awsslack-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "awsslack"
-version = "0.1.0"
+version = "0.1.1"
 description = "AWS CodeBuild/CodeDeploy triggers & updates to Slack with a cool Progress Bar!"
 authors = ["Saurabh Chopra <Saurabh.Chopra.2021@live.rhul.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 exclude = ["./scripts", "./tests"]
 
 [tool.poetry.scripts]
 awsslack = "awsslack.main:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 boto3 = "^1.26.91"
 slack-sdk = "^3.20.2"
+pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 pytest = "^7.2.2"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.2.1"
 coverage = "^7.2.2"
```

### Comparing `awsslack-0.1.0/PKG-INFO` & `awsslack-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: awsslack
-Version: 0.1.0
+Version: 0.1.1
 Summary: AWS CodeBuild/CodeDeploy triggers & updates to Slack with a cool Progress Bar!
 License: MIT
 Author: Saurabh Chopra
 Author-email: Saurabh.Chopra.2021@live.rhul.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.91,<2.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: slack-sdk (>=3.20.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 # awslack
 
 How this would look in Slack:
 ```
```

