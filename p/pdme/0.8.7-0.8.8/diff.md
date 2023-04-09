# Comparing `tmp/pdme-0.8.7.tar.gz` & `tmp/pdme-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdme-0.8.7.tar", max compression
+gzip compressed data, was "pdme-0.8.8.tar", max compression
```

## Comparing `pdme-0.8.7.tar` & `pdme-0.8.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1229 2022-09-17 21:19:13.344450 pdme-0.8.7/README.md
--rw-r--r--   0        0        0      154 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/__init__.py
--rw-r--r--   0        0        0      184 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/inputs/__init__.py
--rw-r--r--   0        0        0      688 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/inputs/dot_inputs.py
--rw-r--r--   0        0        0      536 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/measurement/__init__.py
--rw-r--r--   0        0        0      984 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/measurement/dot_measure.py
--rw-r--r--   0        0        0     1224 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/measurement/dot_pair_measure.py
--rw-r--r--   0        0        0     1131 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/measurement/input_types.py
--rw-r--r--   0        0        0     5219 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/measurement/oscillating_dipole.py
--rw-r--r--   0        0        0       70 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/meta.py
--rw-r--r--   0        0        0     1066 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/model/__init__.py
--rw-r--r--   0        0        0     2367 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/model/fixed_magnitude_model.py
--rw-r--r--   0        0        0     3721 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
--rw-r--r--   0        0        0     3372 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/model/log_spaced_random_choice_model.py
--rw-r--r--   0        0        0     3176 2022-09-17 21:19:13.348450 pdme-0.8.7/pdme/model/log_spaced_random_choice_xy_model.py
--rw-r--r--   0        0        0     1076 2022-09-17 21:19:13.352450 pdme-0.8.7/pdme/model/model.py
--rw-r--r--   0        0        0     2560 2022-09-17 21:19:13.352450 pdme-0.8.7/pdme/model/multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0     3076 2022-09-17 21:19:13.352450 pdme-0.8.7/pdme/model/random_count_multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0        0 2022-09-17 21:19:13.352450 pdme-0.8.7/pdme/py.typed
--rw-r--r--   0        0        0        0 2022-09-17 21:19:13.352450 pdme-0.8.7/pdme/util/__init__.py
--rw-r--r--   0        0        0     2952 2022-09-17 21:19:13.352450 pdme-0.8.7/pdme/util/fast_nonlocal_spectrum.py
--rw-r--r--   0        0        0     2258 2022-09-17 21:19:13.352450 pdme-0.8.7/pdme/util/fast_v_calc.py
--rw-r--r--   0        0        0      838 2022-09-17 21:19:13.352450 pdme-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     1935 2022-09-17 21:20:25.163471 pdme-0.8.7/setup.py
--rw-r--r--   0        0        0     1766 2022-09-17 21:20:25.163985 pdme-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1229 2023-04-09 21:35:05.220972 pdme-0.8.8/README.md
+-rw-r--r--   0        0        0      154 2023-04-09 21:35:05.220972 pdme-0.8.8/pdme/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-09 21:35:05.220972 pdme-0.8.8/pdme/inputs/__init__.py
+-rw-r--r--   0        0        0      688 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/inputs/dot_inputs.py
+-rw-r--r--   0        0        0      536 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/measurement/__init__.py
+-rw-r--r--   0        0        0      984 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/measurement/dot_measure.py
+-rw-r--r--   0        0        0     1224 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/measurement/dot_pair_measure.py
+-rw-r--r--   0        0        0     1131 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/measurement/input_types.py
+-rw-r--r--   0        0        0     5219 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/measurement/oscillating_dipole.py
+-rw-r--r--   0        0        0       70 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/meta.py
+-rw-r--r--   0        0        0     1066 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/__init__.py
+-rw-r--r--   0        0        0     2367 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/fixed_magnitude_model.py
+-rw-r--r--   0        0        0     3721 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
+-rw-r--r--   0        0        0     3372 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/log_spaced_random_choice_model.py
+-rw-r--r--   0        0        0     3176 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/log_spaced_random_choice_xy_model.py
+-rw-r--r--   0        0        0     1076 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/model.py
+-rw-r--r--   0        0        0     2560 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0     3076 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/random_count_multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/py.typed
+-rw-r--r--   0        0        0        0 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/util/__init__.py
+-rw-r--r--   0        0        0     2952 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/util/fast_nonlocal_spectrum.py
+-rw-r--r--   0        0        0     3604 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/util/fast_v_calc.py
+-rw-r--r--   0        0        0      839 2023-04-09 21:35:05.224972 pdme-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0     1937 2023-04-09 21:36:06.738076 pdme-0.8.8/setup.py
+-rw-r--r--   0        0        0     1768 2023-04-09 21:36:06.738456 pdme-0.8.8/PKG-INFO
```

### Comparing `pdme-0.8.7/README.md` & `pdme-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/inputs/dot_inputs.py` & `pdme-0.8.8/pdme/inputs/dot_inputs.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/measurement/__init__.py` & `pdme-0.8.8/pdme/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/measurement/dot_measure.py` & `pdme-0.8.8/pdme/measurement/dot_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/measurement/dot_pair_measure.py` & `pdme-0.8.8/pdme/measurement/dot_pair_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/measurement/input_types.py` & `pdme-0.8.8/pdme/measurement/input_types.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/measurement/oscillating_dipole.py` & `pdme-0.8.8/pdme/measurement/oscillating_dipole.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/model/__init__.py` & `pdme-0.8.8/pdme/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/model/fixed_magnitude_model.py` & `pdme-0.8.8/pdme/model/fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/model/log_spaced_random_choice_fixed_orientation_model.py` & `pdme-0.8.8/pdme/model/log_spaced_random_choice_fixed_orientation_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/model/log_spaced_random_choice_model.py` & `pdme-0.8.8/pdme/model/log_spaced_random_choice_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/model/log_spaced_random_choice_xy_model.py` & `pdme-0.8.8/pdme/model/log_spaced_random_choice_xy_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/model/model.py` & `pdme-0.8.8/pdme/model/model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/model/multidipole_fixed_magnitude_model.py` & `pdme-0.8.8/pdme/model/multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/model/random_count_multidipole_fixed_magnitude_model.py` & `pdme-0.8.8/pdme/model/random_count_multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pdme/util/fast_nonlocal_spectrum.py` & `pdme-0.8.8/pdme/util/fast_nonlocal_spectrum.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.7/pyproject.toml` & `pdme-0.8.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pdme"
-version = "0.8.7"
+version = "0.8.8"
 description = "Python dipole model evaluator"
 authors = ["Deepak <dmallubhotla+github@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.10"
 numpy = "^1.22.3"
-scipy = "~1.8"
+scipy = "~1.10"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6"
 flake8 = "^4.0.0"
 pytest-cov = "^3.0.0"
 mypy = "^0.961"
 ipython = "^8.2.0"
```

### Comparing `pdme-0.8.7/setup.py` & `pdme-0.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pdme', 'pdme.inputs', 'pdme.measurement', 'pdme.model', 'pdme.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.22.3,<2.0.0', 'scipy>=1.8,<1.9']
+['numpy>=1.22.3,<2.0.0', 'scipy>=1.10,<1.11']
 
 setup_kwargs = {
     'name': 'pdme',
-    'version': '0.8.7',
+    'version': '0.8.8',
     'description': 'Python dipole model evaluator',
     'long_description': '# pdme - the python dipole model evaluator\n\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-green.svg?style=flat-square)](https://conventionalcommits.org)\n[![PyPI](https://img.shields.io/pypi/v/pdme?style=flat-square)](https://pypi.org/project/pdme/)\n[![Jenkins](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster&style=flat-square)](https://jenkins.deepak.science/job/gitea-physics/job/pdme/job/master/)\n![Jenkins tests](https://img.shields.io/jenkins/tests?compact_message&jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)\n![Jenkins Coverage](https://img.shields.io/jenkins/coverage/cobertura?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)\n![Maintenance](https://img.shields.io/maintenance/yes/2022?style=flat-square)\n\nThis repo has library code for evaluating dipole models.\n\n## Getting started\n\n`poetry install` to start locally\n\nCommit using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), and when commits are on master, release with `doo release`.\n',
     'author': 'Deepak',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `pdme-0.8.7/PKG-INFO` & `pdme-0.8.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pdme
-Version: 0.8.7
+Version: 0.8.8
 Summary: Python dipole model evaluator
 License: GPL-3.0-only
 Author: Deepak
 Author-email: dmallubhotla+github@gmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
-Requires-Dist: scipy (>=1.8,<1.9)
+Requires-Dist: scipy (>=1.10,<1.11)
 Description-Content-Type: text/markdown
 
 # pdme - the python dipole model evaluator
 
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-green.svg?style=flat-square)](https://conventionalcommits.org)
 [![PyPI](https://img.shields.io/pypi/v/pdme?style=flat-square)](https://pypi.org/project/pdme/)
 [![Jenkins](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster&style=flat-square)](https://jenkins.deepak.science/job/gitea-physics/job/pdme/job/master/)
```

