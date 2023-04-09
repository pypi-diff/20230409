# Comparing `tmp/pytest-emoji-output-0.2.0.tar.gz` & `tmp/pytest-emoji-output-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-emoji-output-0.2.0.tar", last modified: Tue Apr 12 20:22:12 2022, max compression
+gzip compressed data, was "pytest-emoji-output-0.2.1.tar", last modified: Sun Apr  9 07:54:56 2023, max compression
```

## Comparing `pytest-emoji-output-0.2.0.tar` & `pytest-emoji-output-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 fox        (501) staff       (20)        0 2022-04-12 20:22:12.504233 pytest-emoji-output-0.2.0/
--rw-r--r--   0 fox        (501) staff       (20)      153 2021-12-23 16:29:54.000000 pytest-emoji-output-0.2.0/.gitcommit.txt
--rw-r--r--   0 fox        (501) staff       (20)      124 2021-12-23 16:29:54.000000 pytest-emoji-output-0.2.0/AUTHORS.md
--rw-r--r--   0 fox        (501) staff       (20)     1199 2022-04-12 20:15:44.000000 pytest-emoji-output-0.2.0/CHANGELOG.md
--rw-r--r--   0 fox        (501) staff       (20)     1084 2021-12-23 16:29:54.000000 pytest-emoji-output-0.2.0/LICENSE.md
--rw-r--r--   0 fox        (501) staff       (20)      158 2021-12-23 16:29:54.000000 pytest-emoji-output-0.2.0/MANIFEST.in
--rw-r--r--   0 fox        (501) staff       (20)     5471 2022-04-12 20:22:12.503967 pytest-emoji-output-0.2.0/PKG-INFO
--rw-r--r--   0 fox        (501) staff       (20)     4373 2022-04-12 20:21:55.000000 pytest-emoji-output-0.2.0/README.md
-drwxr-xr-x   0 fox        (501) staff       (20)        0 2022-04-12 20:22:12.501785 pytest-emoji-output-0.2.0/plugin/
--rw-r--r--   0 fox        (501) staff       (20)      233 2022-04-12 20:13:58.000000 pytest-emoji-output-0.2.0/plugin/__init__.py
--rw-r--r--   0 fox        (501) staff       (20)     2631 2021-12-23 16:29:54.000000 pytest-emoji-output-0.2.0/plugin/emoji.py
--rw-r--r--   0 fox        (501) staff       (20)      434 2021-12-23 16:29:54.000000 pytest-emoji-output-0.2.0/pyproject.toml
-drwxr-xr-x   0 fox        (501) staff       (20)        0 2022-04-12 20:22:12.503610 pytest-emoji-output-0.2.0/pytest_emoji_output.egg-info/
--rw-r--r--   0 fox        (501) staff       (20)     5471 2022-04-12 20:22:11.000000 pytest-emoji-output-0.2.0/pytest_emoji_output.egg-info/PKG-INFO
--rw-r--r--   0 fox        (501) staff       (20)      428 2022-04-12 20:22:12.000000 pytest-emoji-output-0.2.0/pytest_emoji_output.egg-info/SOURCES.txt
--rw-r--r--   0 fox        (501) staff       (20)        1 2022-04-12 20:22:11.000000 pytest-emoji-output-0.2.0/pytest_emoji_output.egg-info/dependency_links.txt
--rw-r--r--   0 fox        (501) staff       (20)       32 2022-04-12 20:22:12.000000 pytest-emoji-output-0.2.0/pytest_emoji_output.egg-info/entry_points.txt
--rw-r--r--   0 fox        (501) staff       (20)       41 2022-04-12 20:22:12.000000 pytest-emoji-output-0.2.0/pytest_emoji_output.egg-info/requires.txt
--rw-r--r--   0 fox        (501) staff       (20)        7 2022-04-12 20:22:12.000000 pytest-emoji-output-0.2.0/pytest_emoji_output.egg-info/top_level.txt
--rw-r--r--   0 fox        (501) staff       (20)      228 2022-04-12 19:49:06.000000 pytest-emoji-output-0.2.0/requirements-dev.txt
--rw-r--r--   0 fox        (501) staff       (20)       41 2022-04-12 19:47:51.000000 pytest-emoji-output-0.2.0/requirements.txt
--rw-r--r--   0 fox        (501) staff       (20)       38 2022-04-12 20:22:12.504314 pytest-emoji-output-0.2.0/setup.cfg
--rw-r--r--   0 fox        (501) staff       (20)     2427 2022-04-12 19:51:02.000000 pytest-emoji-output-0.2.0/setup.py
+drwxr-xr-x   0 vyahello   (501) staff       (20)        0 2023-04-09 07:54:56.575310 pytest-emoji-output-0.2.1/
+-rw-r--r--   0 vyahello   (501) staff       (20)      153 2022-04-16 22:03:04.000000 pytest-emoji-output-0.2.1/.gitcommit.txt
+-rw-r--r--   0 vyahello   (501) staff       (20)      124 2022-04-16 22:03:04.000000 pytest-emoji-output-0.2.1/AUTHORS.md
+-rw-r--r--   0 vyahello   (501) staff       (20)     1199 2022-04-16 22:03:04.000000 pytest-emoji-output-0.2.1/CHANGELOG.md
+-rw-r--r--   0 vyahello   (501) staff       (20)     1084 2022-04-16 22:03:04.000000 pytest-emoji-output-0.2.1/LICENSE.md
+-rw-r--r--   0 vyahello   (501) staff       (20)      158 2022-04-16 22:03:04.000000 pytest-emoji-output-0.2.1/MANIFEST.in
+-rw-r--r--   0 vyahello   (501) staff       (20)     5392 2023-04-09 07:54:56.575161 pytest-emoji-output-0.2.1/PKG-INFO
+-rw-r--r--   0 vyahello   (501) staff       (20)     4364 2023-04-09 07:50:11.000000 pytest-emoji-output-0.2.1/README.md
+drwxr-xr-x   0 vyahello   (501) staff       (20)        0 2023-04-09 07:54:56.574144 pytest-emoji-output-0.2.1/plugin/
+-rw-r--r--   0 vyahello   (501) staff       (20)      233 2023-04-09 07:52:37.000000 pytest-emoji-output-0.2.1/plugin/__init__.py
+-rw-r--r--   0 vyahello   (501) staff       (20)     2631 2022-04-16 22:03:04.000000 pytest-emoji-output-0.2.1/plugin/emoji.py
+-rw-r--r--   0 vyahello   (501) staff       (20)      434 2022-04-16 22:03:04.000000 pytest-emoji-output-0.2.1/pyproject.toml
+drwxr-xr-x   0 vyahello   (501) staff       (20)        0 2023-04-09 07:54:56.574857 pytest-emoji-output-0.2.1/pytest_emoji_output.egg-info/
+-rw-r--r--   0 vyahello   (501) staff       (20)     5392 2023-04-09 07:54:56.000000 pytest-emoji-output-0.2.1/pytest_emoji_output.egg-info/PKG-INFO
+-rw-r--r--   0 vyahello   (501) staff       (20)      448 2023-04-09 07:54:56.000000 pytest-emoji-output-0.2.1/pytest_emoji_output.egg-info/SOURCES.txt
+-rw-r--r--   0 vyahello   (501) staff       (20)        1 2023-04-09 07:54:56.000000 pytest-emoji-output-0.2.1/pytest_emoji_output.egg-info/dependency_links.txt
+-rw-r--r--   0 vyahello   (501) staff       (20)       32 2023-04-09 07:54:56.000000 pytest-emoji-output-0.2.1/pytest_emoji_output.egg-info/entry_points.txt
+-rw-r--r--   0 vyahello   (501) staff       (20)       41 2023-04-09 07:54:56.000000 pytest-emoji-output-0.2.1/pytest_emoji_output.egg-info/requires.txt
+-rw-r--r--   0 vyahello   (501) staff       (20)        7 2023-04-09 07:54:56.000000 pytest-emoji-output-0.2.1/pytest_emoji_output.egg-info/top_level.txt
+-rw-r--r--   0 vyahello   (501) staff       (20)      228 2022-04-17 00:56:53.000000 pytest-emoji-output-0.2.1/requirements-dev.txt
+-rw-r--r--   0 vyahello   (501) staff       (20)       41 2022-04-16 22:03:04.000000 pytest-emoji-output-0.2.1/requirements.txt
+-rw-r--r--   0 vyahello   (501) staff       (20)       38 2023-04-09 07:54:56.575352 pytest-emoji-output-0.2.1/setup.cfg
+-rw-r--r--   0 vyahello   (501) staff       (20)     2374 2023-04-09 07:48:26.000000 pytest-emoji-output-0.2.1/setup.py
+drwxr-xr-x   0 vyahello   (501) staff       (20)        0 2023-04-09 07:54:56.574964 pytest-emoji-output-0.2.1/tests/
+-rw-r--r--   0 vyahello   (501) staff       (20)     1032 2022-04-16 22:03:04.000000 pytest-emoji-output-0.2.1/tests/test_emoji.py
```

### Comparing `pytest-emoji-output-0.2.0/CHANGELOG.md` & `pytest-emoji-output-0.2.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pytest-emoji-output-0.2.0/LICENSE.md` & `pytest-emoji-output-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytest-emoji-output-0.2.0/PKG-INFO` & `pytest-emoji-output-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: pytest-emoji-output
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pytest plugin to represent test output with emoji support
 Home-page: https://github.com/vyahello/pytest-emoji-output
 Author: Volodymyr Yahello
 Author-email: vyahello@gmail.com
 Maintainer: Volodymyr Yahello
 Maintainer-email: vyahello@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -40,27 +38,25 @@
 # Pytest emoji output
 
 > A pytest plugin that helps to reflect tests output with emoji. 
 
 ## Tools
 
 ### Production
-- python 3.6, 3.7, 3.8, 3.9
+- python 3.7, 3.8, 3.9, 3.10
 - [pytest](https://pypi.org/project/pytest/)
 
 ### Development
 - [travis](https://travis-ci.org/)
 - [black](https://black.readthedocs.io/en/stable/)
 - [mypy](https://mypy.readthedocs.io/en/latest)
 - [pylint](https://www.pylint.org/)
 - [flake8](http://flake8.pycqa.org/en/latest/)
 - [interrogate](https://interrogate.readthedocs.io/en/latest/)
 
-## Usage
-
 ### Installation
 
 Please run following script to obtain latest package from PYPI:
 ```bash
 pip install pytest-emoji-output
 ```
 
@@ -150,9 +146,7 @@
 
 ### What's next
 
 All recent activities and ideas are described at project [issues](https://github.com/vyahello/pytest-emoji-output/issues). 
 If you have ideas you want to change/implement please do not hesitate and create an issue.
 
 **[⬆ back to top](#pytest-emoji-output)**
-
-
```

### Comparing `pytest-emoji-output-0.2.0/README.md` & `pytest-emoji-output-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,27 +11,25 @@
 # Pytest emoji output
 
 > A pytest plugin that helps to reflect tests output with emoji. 
 
 ## Tools
 
 ### Production
-- python 3.6, 3.7, 3.8, 3.9
+- python 3.7, 3.8, 3.9, 3.10
 - [pytest](https://pypi.org/project/pytest/)
 
 ### Development
 - [travis](https://travis-ci.org/)
 - [black](https://black.readthedocs.io/en/stable/)
 - [mypy](https://mypy.readthedocs.io/en/latest)
 - [pylint](https://www.pylint.org/)
 - [flake8](http://flake8.pycqa.org/en/latest/)
 - [interrogate](https://interrogate.readthedocs.io/en/latest/)
 
-## Usage
-
 ### Installation
 
 Please run following script to obtain latest package from PYPI:
 ```bash
 pip install pytest-emoji-output
 ```
```

### Comparing `pytest-emoji-output-0.2.0/plugin/emoji.py` & `pytest-emoji-output-0.2.1/plugin/emoji.py`

 * *Files identical despite different names*

### Comparing `pytest-emoji-output-0.2.0/pytest_emoji_output.egg-info/PKG-INFO` & `pytest-emoji-output-0.2.1/pytest_emoji_output.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: pytest-emoji-output
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pytest plugin to represent test output with emoji support
 Home-page: https://github.com/vyahello/pytest-emoji-output
 Author: Volodymyr Yahello
 Author-email: vyahello@gmail.com
 Maintainer: Volodymyr Yahello
 Maintainer-email: vyahello@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -40,27 +38,25 @@
 # Pytest emoji output
 
 > A pytest plugin that helps to reflect tests output with emoji. 
 
 ## Tools
 
 ### Production
-- python 3.6, 3.7, 3.8, 3.9
+- python 3.7, 3.8, 3.9, 3.10
 - [pytest](https://pypi.org/project/pytest/)
 
 ### Development
 - [travis](https://travis-ci.org/)
 - [black](https://black.readthedocs.io/en/stable/)
 - [mypy](https://mypy.readthedocs.io/en/latest)
 - [pylint](https://www.pylint.org/)
 - [flake8](http://flake8.pycqa.org/en/latest/)
 - [interrogate](https://interrogate.readthedocs.io/en/latest/)
 
-## Usage
-
 ### Installation
 
 Please run following script to obtain latest package from PYPI:
 ```bash
 pip install pytest-emoji-output
 ```
 
@@ -150,9 +146,7 @@
 
 ### What's next
 
 All recent activities and ideas are described at project [issues](https://github.com/vyahello/pytest-emoji-output/issues). 
 If you have ideas you want to change/implement please do not hesitate and create an issue.
 
 **[⬆ back to top](#pytest-emoji-output)**
-
-
```

### Comparing `pytest-emoji-output-0.2.0/setup.py` & `pytest-emoji-output-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         install_requires=__requirements(),
         classifiers=[
             "Development Status :: 4 - Beta",
             "Framework :: Pytest",
             "Intended Audience :: Developers",
             "Topic :: Software Development :: Testing",
             "Programming Language :: Python",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: Implementation :: CPython",
             "Operating System :: OS Independent",
             f"License :: OSI Approved :: {__license__} License",
```

