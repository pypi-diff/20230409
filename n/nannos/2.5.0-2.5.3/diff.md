# Comparing `tmp/nannos-2.5.0.tar.gz` & `tmp/nannos-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nannos-2.5.0.tar", last modified: Wed Jun 29 23:10:50 2022, max compression
+gzip compressed data, was "nannos-2.5.3.tar", last modified: Sun Apr  9 01:16:12 2023, max compression
```

## Comparing `nannos-2.5.0.tar` & `nannos-2.5.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 bench     (1000) bench     (1000)        0 2022-06-29 23:10:50.628390 nannos-2.5.0/
--rw-r--r--   0 bench     (1000) bench     (1000)    35147 2021-07-09 10:13:11.000000 nannos-2.5.0/LICENSE.txt
--rw-r--r--   0 bench     (1000) bench     (1000)        0 2021-07-10 13:43:01.000000 nannos-2.5.0/MANIFEST.in
--rw-r--r--   0 bench     (1000) bench     (1000)     4642 2022-06-29 23:10:50.628390 nannos-2.5.0/PKG-INFO
--rw-r--r--   0 bench     (1000) bench     (1000)     3520 2022-06-12 15:41:41.000000 nannos-2.5.0/README.rst
--rw-r--r--   0 bench     (1000) bench     (1000)       94 2022-02-03 17:01:40.000000 nannos-2.5.0/pyproject.toml
--rw-r--r--   0 bench     (1000) bench     (1000)     1540 2022-06-29 23:10:50.628390 nannos-2.5.0/setup.cfg
-drwxr-xr-x   0 bench     (1000) bench     (1000)        0 2022-06-29 23:10:50.625056 nannos-2.5.0/src/
-drwxr-xr-x   0 bench     (1000) bench     (1000)        0 2022-06-29 23:10:50.628390 nannos-2.5.0/src/nannos/
--rw-r--r--   0 bench     (1000) bench     (1000)      790 2022-06-29 23:00:23.000000 nannos-2.5.0/src/nannos/__about__.py
--rw-r--r--   0 bench     (1000) bench     (1000)     7360 2022-06-29 22:10:42.000000 nannos-2.5.0/src/nannos/__init__.py
--rw-r--r--   0 bench     (1000) bench     (1000)      253 2021-09-03 16:30:27.000000 nannos-2.5.0/src/nannos/constants.py
--rw-r--r--   0 bench     (1000) bench     (1000)     2431 2022-06-11 14:48:48.000000 nannos-2.5.0/src/nannos/excitation.py
-drwxr-xr-x   0 bench     (1000) bench     (1000)        0 2022-06-29 23:10:50.628390 nannos-2.5.0/src/nannos/formulations/
--rw-r--r--   0 bench     (1000) bench     (1000)      161 2021-09-03 16:30:27.000000 nannos-2.5.0/src/nannos/formulations/__init__.py
--rw-r--r--   0 bench     (1000) bench     (1000)     1278 2022-04-20 21:38:15.000000 nannos-2.5.0/src/nannos/formulations/fft.py
--rw-r--r--   0 bench     (1000) bench     (1000)      631 2022-04-02 03:06:07.000000 nannos-2.5.0/src/nannos/formulations/jones.py
--rw-r--r--   0 bench     (1000) bench     (1000)     5437 2022-06-11 14:48:48.000000 nannos-2.5.0/src/nannos/formulations/tangent.py
--rw-r--r--   0 bench     (1000) bench     (1000)     4910 2022-06-11 14:48:48.000000 nannos-2.5.0/src/nannos/geometry.py
--rw-r--r--   0 bench     (1000) bench     (1000)     8518 2022-06-28 09:53:28.000000 nannos-2.5.0/src/nannos/lattice.py
--rw-r--r--   0 bench     (1000) bench     (1000)     8651 2022-06-29 23:03:13.000000 nannos-2.5.0/src/nannos/layers.py
--rw-r--r--   0 bench     (1000) bench     (1000)     1168 2022-04-20 15:55:28.000000 nannos-2.5.0/src/nannos/log.py
--rw-r--r--   0 bench     (1000) bench     (1000)     6774 2022-06-11 14:48:48.000000 nannos-2.5.0/src/nannos/optimize.py
--rw-r--r--   0 bench     (1000) bench     (1000)      675 2022-04-07 21:26:21.000000 nannos-2.5.0/src/nannos/parallel.py
--rw-r--r--   0 bench     (1000) bench     (1000)     7618 2022-06-11 14:48:48.000000 nannos-2.5.0/src/nannos/plot.py
--rw-r--r--   0 bench     (1000) bench     (1000)     3254 2022-01-25 11:39:24.000000 nannos-2.5.0/src/nannos/sample.py
--rw-r--r--   0 bench     (1000) bench     (1000)    32000 2022-06-29 21:05:25.000000 nannos-2.5.0/src/nannos/simulation.py
-drwxr-xr-x   0 bench     (1000) bench     (1000)        0 2022-06-29 23:10:50.628390 nannos-2.5.0/src/nannos/utils/
--rwxr-xr-x   0 bench     (1000) bench     (1000)      351 2021-12-21 13:17:16.000000 nannos-2.5.0/src/nannos/utils/__init__.py
--rw-r--r--   0 bench     (1000) bench     (1000)     3502 2022-06-11 14:48:48.000000 nannos-2.5.0/src/nannos/utils/helpers.py
--rw-r--r--   0 bench     (1000) bench     (1000)     2902 2022-06-29 21:24:06.000000 nannos-2.5.0/src/nannos/utils/jupyter.py
--rw-r--r--   0 bench     (1000) bench     (1000)      356 2021-10-12 22:02:28.000000 nannos-2.5.0/src/nannos/utils/time.py
-drwxr-xr-x   0 bench     (1000) bench     (1000)        0 2022-06-29 23:10:50.628390 nannos-2.5.0/src/nannos.egg-info/
--rw-r--r--   0 bench     (1000) bench     (1000)     4642 2022-06-29 23:10:50.000000 nannos-2.5.0/src/nannos.egg-info/PKG-INFO
--rw-r--r--   0 bench     (1000) bench     (1000)      764 2022-06-29 23:10:50.000000 nannos-2.5.0/src/nannos.egg-info/SOURCES.txt
--rw-r--r--   0 bench     (1000) bench     (1000)       62 2022-06-29 23:10:50.000000 nannos-2.5.0/src/nannos.egg-info/dependency_links.txt
--rw-r--r--   0 bench     (1000) bench     (1000)      228 2022-06-29 23:10:50.000000 nannos-2.5.0/src/nannos.egg-info/requires.txt
--rw-r--r--   0 bench     (1000) bench     (1000)        7 2022-06-29 23:10:50.000000 nannos-2.5.0/src/nannos.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 01:16:12.594500 nannos-2.5.3/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-04-09 01:15:52.000000 nannos-2.5.3/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 01:15:52.000000 nannos-2.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-04-09 01:16:12.595500 nannos-2.5.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2023-04-09 01:15:52.000000 nannos-2.5.3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-09 01:15:52.000000 nannos-2.5.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2023-04-09 01:16:12.596500 nannos-2.5.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 01:16:12.582499 nannos-2.5.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 01:16:12.589499 nannos-2.5.3/src/nannos/
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/__about__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7789 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/excitation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 01:16:12.593500 nannos-2.5.3/src/nannos/formulations/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/formulations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/formulations/fft.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/formulations/jones.py
+-rw-rw-rw-   0 root         (0) root         (0)     5612 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/formulations/tangent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     8477 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/lattice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8317 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/layers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     6749 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/optimize.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)     7618 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)    31936 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/simulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 01:16:12.594500 nannos-2.5.3/src/nannos/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      351 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3848 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/utils/jupyter.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-04-09 01:15:52.000000 nannos-2.5.3/src/nannos/utils/time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 01:16:12.591499 nannos-2.5.3/src/nannos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-04-09 01:16:12.000000 nannos-2.5.3/src/nannos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      764 2023-04-09 01:16:12.000000 nannos-2.5.3/src/nannos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-09 01:16:12.000000 nannos-2.5.3/src/nannos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-09 01:16:12.000000 nannos-2.5.3/src/nannos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-09 01:16:12.000000 nannos-2.5.3/src/nannos.egg-info/top_level.txt
```

### Comparing `nannos-2.5.0/LICENSE.txt` & `nannos-2.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nannos-2.5.0/PKG-INFO` & `nannos-2.5.3/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,118 @@
-Metadata-Version: 2.1
-Name: nannos
-Version: 2.5.0
-Summary: Fourier Modal Method for multilayer metamaterials
-Home-page: https://gitlab.com/nannos/nannos
-Author: Benjamin Vial
-License: GPL-3.0-or-later
-Project-URL: Code, https://gitlab.com/nannos/nannos
-Project-URL: Documentation, https://nannos.gitlab.io
-Project-URL: Issues, https://gitlab.com/nannos/nannos/issues
-Keywords: fourier modal method,diffraction,optics,photonics,metamaterials
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: gpu
-Provides-Extra: magma
-License-File: LICENSE.txt
 
-
-.. image:: https://img.shields.io/endpoint?url=https://gitlab.com/nannos/nannos/-/jobs/artifacts/master/file/logobadge.json?job=badge
+.. |release_badge| image:: https://img.shields.io/endpoint?url=https://gitlab.com/nannos/nannos/-/jobs/artifacts/master/raw/logobadge.json?job=badge
   :target: https://gitlab.com/nannos/nannos/-/releases
   :alt: Release
 
-
-.. image:: https://img.shields.io/gitlab/pipeline/nannos/nannos/master?logo=gitlab&labelColor=dedede&logoColor=ffffff&style=for-the-badge
+.. |GL_CI| image:: https://img.shields.io/gitlab/pipeline/nannos/nannos/master?logo=gitlab&labelColor=grey&style=for-the-badge
   :target: https://gitlab.com/nannos/nannos/commits/master
   :alt: pipeline status
 
+.. |conda| image:: https://img.shields.io/conda/vn/conda-forge/nannos?logo=conda-forge&color=CD5C5C&logoColor=white&style=for-the-badge   
+  :target: https://anaconda.org/conda-forge/nannos
+  :alt: Conda (channel only)
 
-.. image:: https://img.shields.io/gitlab/coverage/nannos/nannos/master?logo=python&logoColor=e9d672&style=for-the-badge
- :target: https://gitlab.com/nannos/nannos/commits/master
- :alt: coverage report
-
-
-.. image:: https://img.shields.io/badge/code%20style-black-dedede.svg?logo=python&logoColor=e9d672&style=for-the-badge
-  :alt: Code style: black
-
-
-.. image:: https://img.shields.io/badge/license-GPLv3-blue?color=dd7d54&logo=open-access&logoColor=dd7d54&style=for-the-badge
-  :target: https://gitlab.com/nannos/nannos/-/blob/master/LICENCE.txt
-  :alt: license
-
+.. |conda_dl| image:: https://img.shields.io/conda/dn/conda-forge/nannos?logo=conda-forge&logoColor=white&style=for-the-badge
+  :alt: Conda
 
+.. |conda_platform| image:: https://img.shields.io/conda/pn/conda-forge/nannos?logo=conda-forge&logoColor=white&style=for-the-badge
+  :alt: Conda
 
-----------------------
 
-.. image:: https://img.shields.io/pypi/v/nannos?color=blue&logo=pypi&logoColor=e9d672&style=for-the-badge
+.. |pip| image:: https://img.shields.io/pypi/v/nannos?color=blue&logo=pypi&logoColor=e9d672&style=for-the-badge
   :target: https://pypi.org/project/nannos/
   :alt: PyPI
-
-
-.. image:: https://img.shields.io/pypi/dm/nannos?logo=pypi&logoColor=e9d672&style=for-the-badge
+  
+.. |pip_dl| image:: https://img.shields.io/pypi/dm/nannos?logo=pypi&logoColor=e9d672&style=for-the-badge   
   :alt: PyPI - Downloads
-
-
-.. image:: https://img.shields.io/pypi/status/nannos?logo=pypi&logoColor=e9d672&style=for-the-badge
+   
+.. |pip_status| image:: https://img.shields.io/pypi/status/nannos?logo=pypi&logoColor=e9d672&style=for-the-badge   
   :alt: PyPI - Status
 
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?logo=python&logoColor=e9d672&style=for-the-badge
+  :alt: Code style: black
+ 
+.. |coverage| image:: https://img.shields.io/gitlab/coverage/nannos/nannos/master?logo=python&logoColor=e9d672&style=for-the-badge
+  :target: https://gitlab.com/nannos/nannos/commits/master
+  :alt: coverage report 
+  
+.. |zenodo| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.6490098-dd7d54?logo=google-scholar&logoColor=dd7d54&style=for-the-badge
+  :target: https://doi.org/10.5281/zenodo.6490098
+ 
+.. |licence| image:: https://img.shields.io/badge/license-GPLv3-blue?color=dd7d54&logo=open-access&logoColor=dd7d54&style=for-the-badge
+  :target: https://gitlab.com/nannos/nannos/-/blob/master/LICENCE.txt
+  :alt: license
 
-.. .. image:: https://img.shields.io/codeclimate/maintainability/benvial/nannos?logo=code-climate&style=for-the-badge
-..    :target: https://codeclimate.com/github/benvial/nannos
-..    :alt: Code Climate maintainability
-
-
-.. image:: https://img.shields.io/badge/DOI-10.5281/zenodo.6490098-dd7d54?logo=google-scholar&logoColor=dd7d54&style=for-the-badge
- :target: https://doi.org/10.5281/zenodo.6490098
-
-
-.. ------------------------------------------------------------------------------------------
-..
-..
-.. .. image:: https://img.shields.io/conda/vn/conda-forge/nannos?logo=conda-forge&color=CD5C5C&logoColor=white&style=for-the-badge
-..    :target: https://anaconda.org/conda-forge/nannos
-..    :alt: Conda (channel only)
-..
-.. .. image:: https://img.shields.io/conda/dn/conda-forge/nannos?logo=conda-forge&logoColor=white&style=for-the-badge
-..    :alt: Conda
-..
-.. .. image:: https://img.shields.io/conda/pn/conda-forge/nannos?logo=conda-forge&logoColor=white&style=for-the-badge
-..    :alt: Conda
++----------------------+----------------------+----------------------+
+| Release              |            |release_badge|                  |
++----------------------+----------------------+----------------------+
+| Deployment           | |pip|                |        |conda|       |
++----------------------+----------------------+----------------------+
+| Build Status         |            |GL_CI|                          |
++----------------------+----------------------+----------------------+
+| Metrics              |                |coverage|                   |
++----------------------+----------------------+----------------------+
+| Activity             |     |pip_dl|         |      |conda_dl|      |
++----------------------+----------------------+----------------------+
+| Citation             |           |zenodo|                          |
++----------------------+----------------------+----------------------+
+| License              |           |licence|                         |
++----------------------+----------------------+----------------------+
+| Formatter            |           |black|                           |
++----------------------+----------------------+----------------------+
 
 
-----------------------------
 
 .. inclusion-marker-badges
 
 =============================================================
 nannos: Fourier Modal Method for multilayer metamaterials
 =============================================================
 
 
 .. inclusion-marker-install-start
 
 Installation
 ============
 
+From conda
+----------
+
+If using `conda <https://www.anaconda.com/>`_, first, add conda-forge to your channels with:
+
+.. code-block:: bash
+    
+    conda config --add channels conda-forge
+    conda config --set channel_priority strict
+
+Once the conda-forge channel has been enabled, nannos can be installed with:
+
+.. code-block:: bash
+  
+  conda install nannos
+
+
+Alternatively, we provide an `environment.yml <https://gitlab.com/nannos/nannos/-/blob/master/environment.yml>`_ 
+file with all the dependencies for the master branch. First create the environment:
+
+.. code-block:: bash
+
+  conda env create -f environment.yml
+
+and then activate it with 
+
+.. code-block:: bash
+
+  conda activate nannos
+  
+
+See the `github repository <https://github.com/conda-forge/nannos-feedstock/>`_ 
+where development happens for conda-forge.
+  
+
 From pypi
 ---------
 
 The package is available on `pypi <https://pypi.org/project/nannos>`_.
 To install, simply use:
 
 .. code-block:: bash
```

### Comparing `nannos-2.5.0/setup.cfg` & `nannos-2.5.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nannos
-version = 2.5.0
+version = 2.5.3
 author = Benjamin Vial
 email = benjamin.vial84@gmail.com
 description = Fourier Modal Method for multilayer metamaterials
 url = https://gitlab.com/nannos/nannos
 project_urls = 
 	Code=https://gitlab.com/nannos/nannos
 	Documentation=https://nannos.gitlab.io
@@ -47,17 +47,17 @@
 	joblib
 	colorlog
 	shapely
 	psutil
 	nlopt
 	ipython
 	pyvista
-	pythreejs
-	ipyvtklink
-	panel
+	trame
+	nest-asyncio
+	ipywidgets
 python_requires = >=3.6
 setup_requires = 
 	setuptools>=42
 	wheel
 dependency_links = https://storage.googleapis.com/jax-releases/jax_releases.html
 
 [options.packages.find]
```

### Comparing `nannos-2.5.0/src/nannos/__about__.py` & `nannos-2.5.3/src/nannos/__about__.py`

 * *Files identical despite different names*

### Comparing `nannos-2.5.0/src/nannos/__init__.py` & `nannos-2.5.3/src/nannos/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,50 +61,49 @@
     available_backends.append("jax")
 
 
 def use_gpu(boolean):
     global DEVICE
     global _CPU_DEVICE
     global _GPU_DEVICE
+    global _FORCE_GPU
+    _FORCE_GPU = 1
 
     if boolean:
-
-        if BACKEND not in ["torch"]:
+        if BACKEND not in ["torch", "jax"]:
             logger.debug(f"Cannot use GPU with {BACKEND} backend.")
             _delvar("_GPU_DEVICE")
             _CPU_DEVICE = True
+        elif BACKEND == "torch" and not HAS_TORCH:
+            logger.warning("pytorch not found. Cannot use GPU.")
+            _delvar("_GPU_DEVICE")
+            _CPU_DEVICE = True
+        elif BACKEND == "torch" and not HAS_CUDA:
+            logger.warning("cuda not found. Cannot use GPU.")
+            _delvar("_GPU_DEVICE")
+            _CPU_DEVICE = True
+        elif BACKEND == "jax" and not HAS_JAX:
+            logger.warning("jax not found. Cannot use GPU.")
+            _delvar("_GPU_DEVICE")
+            _CPU_DEVICE = True
         else:
-            if not HAS_TORCH:
-                logger.warning("pytorch not found. Cannot use GPU.")
-                _delvar("_GPU_DEVICE")
-                _CPU_DEVICE = True
-            elif not HAS_CUDA:
-                logger.warning("cuda not found. Cannot use GPU.")
-                _delvar("_GPU_DEVICE")
-                _CPU_DEVICE = True
-            else:
-                DEVICE = "cuda"
-                logger.debug("Using GPU.")
-                _delvar("_CPU_DEVICE")
-                _GPU_DEVICE = True
+            DEVICE = "cuda"
+            logger.debug("Using GPU.")
+            _delvar("_CPU_DEVICE")
+            _GPU_DEVICE = True
     else:
         _CPU_DEVICE = True
         _delvar("_GPU_DEVICE")
         DEVICE = "cpu"
         logger.debug("Using CPU.")
     _reload_package()
 
 
 def jit(fun, **kwargs):
-    if BACKEND == "jax":
-        from jax import jit
-
-        return jit(fun, **kwargs)
-    else:
-        return fun
+    return fun
 
 
 def _delvar(VAR):
     if VAR in globals():
         del globals()[VAR]
 
 
@@ -175,29 +174,27 @@
         raise ValueError(
             f"Unknown backend '{backend}'. Please choose between 'numpy', 'scipy', 'jax', 'torch' and 'autograd'."
         )
     _reload_package()
 
 
 def _reload_package():
-
     import importlib
     import sys
 
     import nannos
 
     importlib.reload(nannos)
 
     its = [s for s in sys.modules.items() if s[0].startswith("nannos")]
     for k, v in its:
         importlib.reload(v)
 
 
 def get_backend():
-
     if "_SCIPY" in globals():
         return "scipy"
     elif "_AUTOGRAD" in globals():
         return "autograd"
     elif "_JAX" in globals():
         return "jax"
     elif "_TORCH" in globals():
@@ -207,43 +204,44 @@
 
 
 def _grad(f):
     raise NotImplementedError(f"grad is not implemented for {BACKEND} backend.")
 
 
 if "_SCIPY" in globals():
-
     import numpy
 
     grad = _grad
     backend = numpy
 elif "_AUTOGRAD" in globals():
     from autograd import grad, numpy
 
     backend = numpy
 elif "_JAX" in globals():
     if HAS_JAX:
+        import jax
 
-        from jax.config import config
+        if DEVICE == "cpu":
+            os.environ["CUDA_VISIBLE_DEVICES"] = ""
+            jax.config.update("jax_platform_name", "cpu")
+        else:
+            # os.environ.pop("CUDA_VISIBLE_DEVICES", None)
+            os.environ["CUDA_VISIBLE_DEVICES"] = "0"
+            jax.config.update("jax_platform_name", "gpu")
 
-        config.update("jax_platform_name", "cpu")
-        config.update("jax_enable_x64", True)
+        jax.config.update("jax_enable_x64", True)
 
         # TODO: jax eig not implemented on GPU
         # see https://github.com/google/jax/issues/1259
 
         # TODO: support jax properly (is it faster than autograd? use jit?)
         # jax does not support eig
         # for autodif wrt eigenvectors yet.
         # see: https://github.com/google/jax/issues/2748
 
-        # if DEVICE == "cpu":
-        #     config.update("jax_platform_name", "cpu")
-        # else:
-        #     config.update("jax_platform_name", "gpu")
         # from jax import grad, numpy
         from jax import numpy
 
         grad = _grad
         backend = numpy
 
     else:
@@ -290,22 +288,34 @@
 def get_device():
     return "cuda" if "_GPU_DEVICE" in globals() else "cpu"
 
 
 BACKEND = get_backend()
 DEVICE = get_device()
 
+
 _backend_env_var = os.environ.get("NANNOS_BACKEND")
+_gpu_env_var = os.environ.get("NANNOS_GPU")
 
-if _backend_env_var in available_backends and _backend_env_var is not None:
-    if BACKEND != _backend_env_var and "_FORCE_BACKEND" not in globals():
-        logger.debug(f"Found environment variable NANNOS_BACKEND={_backend_env_var}")
-        set_backend(_backend_env_var)
+if (
+    _backend_env_var in available_backends
+    and _backend_env_var is not None
+    and BACKEND != _backend_env_var
+    and "_FORCE_BACKEND" not in globals()
+):
+    logger.debug(f"Found environment variable NANNOS_BACKEND={_backend_env_var}")
+    set_backend(_backend_env_var)
+
+if _gpu_env_var is not None and "_FORCE_GPU" not in globals():
+    logger.debug(f"Found environment variable NANNOS_GPU={_gpu_env_var}")
+    use_gpu(True)
 
 from . import optimize
 from .constants import *
 from .excitation import *
 from .lattice import *
 from .parallel import *
 from .sample import *
 from .simulation import *
 from .utils import *
+
+array = backend.array
```

### Comparing `nannos-2.5.0/src/nannos/excitation.py` & `nannos-2.5.3/src/nannos/excitation.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,21 +25,19 @@
         :math:`\\theta`: polar angle,
         :math:`\phi`: azimuthal angle,
         :math:`\psi`: polarization angle.
 
     """
 
     def __init__(self, wavelength=1, angles=(0, 0, 0)):
-        self.wavelength = bk.array(wavelength)
+        self.wavelength = bk.array(wavelength, dtype=bk.float64)
         self.angles_deg = bk.array(angles, dtype=bk.float64)
         self.angles = self.angles_deg * _deg2rad
-        self.theta = bk.array(self.angles[0], dtype=bk.float64)
-        self.phi = bk.array(self.angles[1], dtype=bk.float64)
-        self.psi = bk.array(self.angles[2], dtype=bk.float64)
-        self.frequency_scaled = bk.array(1 / self.wavelength)
+        self.theta, self.phi, self.psi = self.angles
+        self.frequency_scaled = 1 / self.wavelength
 
         k0 = 2 * pi * self.frequency_scaled
 
         self.wavenumber = k0
         self.wavevector = k0 * bk.array(
             [
                 bk.sin(self.theta) * bk.cos(self.phi),
```

### Comparing `nannos-2.5.0/src/nannos/formulations/fft.py` & `nannos-2.5.3/src/nannos/formulations/fft.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     if BACKEND == "scipy":
         uft = _fft2_scipy(u, shape=s, axes=axes)
     elif BACKEND == "torch":
         uft = _fft2_torch(u, s=s, dim=axes)
     else:
         uft = bk.fft.fft2(u, s=s, axes=axes)
     nx, ny = uft.shape[axes[0]], uft.shape[axes[1]]
-    return uft / (nx * ny)
+    return bk.array(uft) / (nx * ny)
 
 
 def inverse_fourier_transform(uft, s=None, axes=(-2, -1)):
     if BACKEND == "scipy":
         u = _ifft2_scipy(uft, shape=s, axes=axes)
     elif BACKEND == "torch":
         u = _ifft2_torch(uft, s=s, dim=axes)
     else:
         u = bk.fft.ifft2(uft, s=s, axes=axes)
     nx, ny = uft.shape[axes[0]], uft.shape[axes[1]]
-    return u * (nx * ny)
+    return bk.array(u) * (nx * ny)
 
 
 fourier_transform = jit(fourier_transform, static_argnums=(1, 2))
 inverse_fourier_transform = jit(inverse_fourier_transform, static_argnums=(1, 2))
```

### Comparing `nannos-2.5.0/src/nannos/formulations/jones.py` & `nannos-2.5.3/src/nannos/formulations/jones.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,11 +16,10 @@
 
 def get_jones_field(t):
     norm_t = norm(t)
     n = [-t[1], t[0]]
     theta = _arctan2(t[1], t[0])
     phi = pi / 8 * (1 + bk.cos(pi * norm_t))
     expo = bk.exp(1j * theta)
-    J = [
+    return [
         expo / norm_t * (t[i] * bk.cos(phi) + 1j * n[i] * bk.sin(phi)) for i in range(2)
     ]
-    return J
```

### Comparing `nannos-2.5.0/src/nannos/formulations/tangent.py` & `nannos-2.5.3/src/nannos/formulations/tangent.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
         t = [t[i] / bk.max(norm(t)) for i in range(2)]
     return t
 
 
 def _get_tangent_field_min(
     grid, harmonics, normalize=False, rfilt=4, opt_backend="autograd"
 ):
-
     if opt_backend == "jax":
         from jax import grad
         from jax import numpy as npg
         from jax.config import config
 
         # config.update("jax_platform_name", "cpu")
         config.update("jax_enable_x64", True)
@@ -102,14 +101,20 @@
     shape_small = (Nx_ds, Ny_ds)
 
     nh = len(harmonics[0])
     nh = min(nh, 51)
     harmonics = harmonics[:, :nh]
 
     xf = apply_filter(grid, rfilt=rfilt)
+
+    try:
+        xf = xf.detach().cpu().numpy()
+    except:
+        pass
+
     dgrid_f = npg.array(npg.gradient(xf))
 
     normdgrid_f = norm(dgrid_f)
     # maxi = npg.max(normdgrid_f)
     # dgrid_f = npg.array([dgrid_f[i] /maxi for i in range(2)])
     dgrid_f = npg.array([_normalize(dgrid_f[i], normdgrid_f) for i in range(2)])
 
@@ -167,15 +172,19 @@
     a = _get_amps(coef, (Nx, Ny))
     n = npg.array(npg.gradient(a))
     t = [n[1], -n[0]]
 
     t = bk.array(t).real
 
     if normalize:
-        norm_t = norm(t)
+        try:
+            t1 = t.detach().cpu().numpy()
+        except:
+            t1 = t
+        norm_t = bk.array(norm(t1))
         t = _normalize_vec(t, norm_t)
     else:
         t = [t[i] / bk.max(norm(t)) for i in range(2)]
 
     return t
```

### Comparing `nannos-2.5.0/src/nannos/geometry.py` & `nannos-2.5.3/src/nannos/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,20 +72,18 @@
     elif shp.contains(rect):
         m = set_index_2d(m, True)
 
     else:
         lx, ly = m.shape
 
         if lx == 1 and ly == 1:
-
             val = shp.contains(sg.Point(x[0], y[0]))
             m = set_index_2d(m, val)
 
         elif lx == 1:
-
             val = shape_mask(shp, x[: ly // 2], y, m[:, : ly // 2])
             m = set_index_2d(m, val, idx2=(None, ly // 2))
             val = shape_mask(shp, x[ly // 2 :], y, m[:, ly // 2 :])
             m = set_index_2d(m, val, idx2=(ly // 2, None))
 
         elif ly == 1:
             val = shape_mask(shp, x, y[: lx // 2], m[: lx // 2])
@@ -112,16 +110,15 @@
     y0 = bk.linspace(0, 1.0, Ny)
     x_, y_ = bk.meshgrid(x0, y0, indexing="ij")
     grid = bk.stack([x_, y_])
     x, y = grid[0][:, 0], grid[1][0, :]
     invM = bk.linalg.inv(lattice.matrix)
     matrix = invM.ravel().tolist() + [0, 0]
     geom = sa.affine_transform(geom, matrix)
-    mask = shape_mask(geom, x, y).T
-    return mask
+    return shape_mask(geom, x, y).T
 
 
 def polygon(vertices, lattice, Nx, Ny):
     polygon = sg.Polygon(vertices)
     return geometry_mask(polygon, lattice, Nx, Ny)
 
 
@@ -137,18 +134,20 @@
     ell = sa.scale(circ, xfact=1.0, yfact=radius_y / radius_x, zfact=1.0, origin=cent)
     if rotate != 0:
         ell = sa.rotate(ell, rotate, origin=cent, use_radians=False)
     return geometry_mask(ell, lattice, Nx, Ny)
 
 
 def rectangle(center, widths, lattice, Nx, Ny, rotate=0):
-    vertices = [[center[0] - widths[0] / 2, center[1] - widths[1] / 2]]
-    vertices.append([center[0] + widths[0] / 2, center[1] - widths[1] / 2])
-    vertices.append([center[0] + widths[0] / 2, center[1] + widths[1] / 2])
-    vertices.append([center[0] - widths[0] / 2, center[1] + widths[1] / 2])
+    vertices = [
+        [center[0] - widths[0] / 2, center[1] - widths[1] / 2],
+        [center[0] + widths[0] / 2, center[1] - widths[1] / 2],
+        [center[0] + widths[0] / 2, center[1] + widths[1] / 2],
+        [center[0] - widths[0] / 2, center[1] + widths[1] / 2],
+    ]
     rect = sg.Polygon(vertices)
     cent = sg.Point(*center)
     if rotate != 0:
         rect = sa.rotate(rect, rotate, origin=cent, use_radians=False)
     return geometry_mask(rect, lattice, Nx, Ny)
```

### Comparing `nannos-2.5.0/src/nannos/lattice.py` & `nannos-2.5.3/src/nannos/lattice.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,16 @@
             self.basis_vectors = basis_vectors
             self.discretization = tuple(discretization)
 
     @property
     def area(self):
         if self.is_1D:
             return self.basis_vectors[0][0]
-        else:
-            v = self.basis_vectors
-            return bk.linalg.norm(bk.cross(v[0], v[1]))
+        v = self.basis_vectors
+        return bk.linalg.norm(bk.cross(v[0], v[1]))
 
     @property
     def matrix(self):
         """Basis matrix.
 
         Returns
         -------
@@ -101,15 +100,15 @@
         -------
         G : list of tuple of integers of length 2
             Harmonics (i1, i2).
         nh : int
             The number of harmonics after truncation.
 
         """
-        if not int(nh) == nh:
+        if int(nh) != nh:
             raise ValueError("nh must be integer.")
         if self.truncation == "circular":
             return _circular_truncation(nh, self.reciprocal)
         elif self.truncation == "parallelogrammic":
             return _parallelogramic_truncation(nh, self.reciprocal)
         else:
             return _one_dim_truncation(nh)
@@ -131,19 +130,18 @@
         Returns
         -------
         array like
             The unit grid of size equal to the attribute `discretization`.
 
         """
         Nx, Ny = self.discretization
-        x0 = bk.linspace(0, 1.0, Nx)
-        y0 = bk.linspace(0, 1.0, Ny)
+        x0 = bk.array(bk.linspace(0, 1.0, Nx))
+        y0 = bk.array(bk.linspace(0, 1.0, Ny))
         x_, y_ = bk.meshgrid(x0, y0, indexing="ij")
-        grid = bk.stack([x_, y_])
-        return grid
+        return bk.stack([x_, y_])
 
     @property
     def grid(self):
         """Grid in lattice vectors basis.
 
         Returns
         -------
@@ -243,16 +241,15 @@
         )
 
 
 def _one_dim_truncation(nh):
     n = int((nh - 1) / 2)
     G = [(0, 0)]
     for i in range(1, n + 1):
-        G.append((i, 0))
-        G.append((-i, 0))
+        G.extend(((i, 0), (-i, 0)))
     return bk.array(G).T, len(G)
 
 
 def _parallelogramic_truncation(nh, Lk):
     u = bk.array([bk.linalg.norm(value) for value in Lk])
     udot = bk.dot(Lk[0], Lk[1])
```

### Comparing `nannos-2.5.0/src/nannos/layers.py` & `nannos-2.5.3/src/nannos/layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 
 
 __all__ = ["Layer"]
 
 
 from copy import copy
 
+from . import BACKEND, DEVICE
 from . import backend as bk
 from . import jit
 from .formulations.jones import get_jones_field
 from .formulations.tangent import get_tangent_field
 from .plot import *
 from .utils import block
-from .utils.helpers import _reseter
+from .utils.helpers import _reseter, is_anisotropic, is_uniform
 
 
 class Layer:
     """A layer object.
 
     Parameters
     ----------
@@ -43,17 +44,16 @@
         thickness=0,
         epsilon=1,
         mu=1,
         lattice=None,
         tangent_field=None,
         tangent_field_type="fft",
     ):
-        if thickness is not None:
-            if thickness < 0:
-                raise ValueError("thickness must be positive.")
+        if thickness is not None and thickness < 0:
+            raise ValueError("thickness must be positive.")
         self.name = name
         self.thickness = thickness
         self.epsilon = bk.array(epsilon, dtype=bk.complex128)
         self.mu = bk.array(mu, dtype=bk.complex128)
         self.lattice = lattice
         self.tangent_field = tangent_field
         self.tangent_field_type = tangent_field_type
@@ -158,16 +158,16 @@
             bk.array(
                 _epsilon * _mu * omega**2 - kx**2 - ky**2,
                 dtype=bk.complex128,
             )
             ** 0.5
         )
         # q = bk.where(bk.imag(q) < 0.0, -q, q)
-        self.eigenvalues = bk.hstack((q, q))
-        self.eigenvectors = bk.eye(2 * len(kx), dtype=bk.complex128)
+        self.eigenvalues = bk.array(bk.hstack((q, q)))
+        self.eigenvectors = bk.array(bk.eye(2 * len(kx), dtype=bk.complex128))
         return self.eigenvalues, self.eigenvectors
 
     def solve_eigenproblem(self, matrix):
         """Solve the eigenproblem for a patterned layer.
 
         Parameters
         ----------
@@ -183,30 +183,29 @@
         if self.iscopy:
             self.eigenvalues, self.eigenvectors = (
                 self.original.eigenvalues,
                 self.original.eigenvectors,
             )
 
         else:
-            # # TODO: implement custom autodiff rules for the evp with jax
-            # if BACKEND == "jax":
-            #     # from ._jax_eig_workaround import eig_jax
-            #     eig_func = bk.linalg.eig
-            # elif BACKEND == "torch":
-            #     from . import torch
-            #
-            #     def eig_func(u):
-            #         u = torch.tensor(u)#.to(_device)
-            #         return torch.linalg.eig(u)
-            #
-            # else:
-            #     eig_func = bk.linalg.eig
-            eig_func = jit(bk.linalg.eig)
+            # TODO: implement custom autodiff rules for the evp with jax
+            # if get_backend() == "jax" and get_device()=="cuda":
+            if BACKEND == "jax" and DEVICE == "cuda":
+                # fix for GPU
+                # from ._jax_eig_workaround import eig_jax
+                import jax
+
+                w, v = jax.jit(jax.numpy.linalg.eig, backend="cpu")(matrix)
+                w = jax.device_put(w, jax.devices("gpu")[0])
+                v = jax.device_put(v, jax.devices("gpu")[0])
 
-            w, v = eig_func(matrix)
+            else:
+                eig_func = bk.linalg.eig
+                eig_func = jit(bk.linalg.eig)
+                w, v = eig_func(matrix)
             q = w**0.5
             q = bk.where(bk.imag(q) < 0.0, -q, q)
             self.eigenvalues, self.eigenvectors = q, v
         return self.eigenvalues, self.eigenvectors
 
     def copy(self, name=None):
         """Copy a layer.
@@ -240,51 +239,33 @@
 
         Returns
         -------
         bool
             ``True`` if the layer is uniform, ``False`` if not.
 
         """
-        if self.is_epsilon_anisotropic:
-            e = self.epsilon.shape == (3, 3)
-        else:
-            e = self.epsilon.shape == ()
-        if self.is_mu_anisotropic:
-            m = self.mu.shape == (3, 3)
-        else:
-            m = self.mu.shape == ()
-
-        return e and m
+        return is_uniform(self.epsilon) and is_uniform(self.mu)
 
     def get_tangent_field(self, harmonics, normalize=False, type=None):
-        type = type or self.tangent_field_type
         if self.is_uniform:
             return None
-        else:
-            if self.tangent_field is not None:
-                return self.tangent_field
-            else:
-                epsilon = self.epsilon
-                epsilon_zz = epsilon[2, 2] if self.is_epsilon_anisotropic else epsilon
-                return get_tangent_field(
-                    epsilon_zz,
-                    harmonics,
-                    normalize=normalize,
-                    type=self.tangent_field_type,
-                )
+        if self.tangent_field is not None:
+            return self.tangent_field
+        epsilon = self.epsilon
+        epsilon_zz = epsilon[2, 2] if self.is_epsilon_anisotropic else epsilon
+        type = type or self.tangent_field_type
+        return get_tangent_field(
+            epsilon_zz,
+            harmonics,
+            normalize=normalize,
+            type=self.tangent_field_type,
+        )
 
     def get_jones_field(self, t):
-        if self.is_uniform:
-            return None
-        else:
-            return get_jones_field(t)
-
-
-def is_anisotropic(f):
-    return f.shape[:2] == (3, 3)
+        return None if self.is_uniform else get_jones_field(t)
 
 
 def _get_layer(id, layers, layer_names):
     """Helper to get layer index and name.
 
     Parameters
     ----------
@@ -299,20 +280,19 @@
     -------
     layer : nannos.Layer
         The layer object.
     index : nannos.Layer
         The layer index in the stack.
     """
     if isinstance(id, str):
-        if id in layer_names:
-            for i, l in enumerate(layers):
-                if l.name == id:
-                    return l, i
-        else:
+        if id not in layer_names:
             raise ValueError(f"Unknown layer name {id}")
+        for i, l in enumerate(layers):
+            if l.name == id:
+                return l, i
     elif isinstance(id, int):
         return layers[id], id
     elif hasattr(id, "name"):
         return _get_layer(id.name, layers, layer_names)
     else:
         raise ValueError(
             f"Wrong id for layer: {id}. Please use an integrer specifying the layer index or a string for the layer name."
```

### Comparing `nannos-2.5.0/src/nannos/log.py` & `nannos-2.5.3/src/nannos/log.py`

 * *Files identical despite different names*

### Comparing `nannos-2.5.0/src/nannos/optimize.py` & `nannos-2.5.3/src/nannos/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,38 +29,35 @@
     return ((tanh(thres * beta)) + tanh(beta * (x - thres))) / (
         tanh(thres * beta) + (tanh((1 - thres) * beta))
     )
 
 
 def multi_project(x, beta=1, Nthres=2):
     thresholds = bk.linspace(0, 1, Nthres + 1)[1:-1]
-    out = 0
-    for thres in thresholds:
-        out += project(x, beta, thres)
+    out = sum(project(x, beta, thres) for thres in thresholds)
     return out / len(thresholds)
 
 
 def multi_simp(x, epsilons, p=1):
     epsilons = bk.array(epsilons) + 0j
     nthres = len(epsilons)
     npts = nthres
     if nthres == 2:
         return simp(x, epsilons[0], epsilons[1], p)
-    else:
-        pts = bk.linspace(0, 1, npts)
+    pts = bk.linspace(0, 1, npts)
 
-        def pol(coefs, x):
-            return sum(c * x ** (n * p) for n, c in enumerate(coefs))
+    def pol(coefs, x):
+        return sum(c * x ** (n * p) for n, c in enumerate(coefs))
 
-        def mat(pts):
-            return bk.array([[_x ** (n * p) + 0j for n in range(npts)] for _x in pts])
+    def mat(pts):
+        return bk.array([[_x ** (n * p) + 0j for n in range(npts)] for _x in pts])
 
-        M = mat(pts)
-        coefs = bk.linalg.inv(M) @ epsilons
-        return pol(coefs, x)
+    M = mat(pts)
+    coefs = bk.linalg.inv(M) @ epsilons
+    return pol(coefs, x)
 
 
 class StopFunError(Exception):
     """Raised when stop value reached"""
 
     pass
 
@@ -68,17 +65,16 @@
 class StopFun:
     def __init__(self, fun, stopval=None):
         self.fun_in = fun
         self.stopval = stopval
 
     def fun(self, x, *args):
         self.f = self.fun_in(x, *args)
-        if self.stopval is not None:
-            if self.f < self.stopval:
-                raise StopFunError("Stop value reached.")
+        if self.stopval is not None and self.f < self.stopval:
+            raise StopFunError("Stop value reached.")
         self.x = x
         return self.f
 
 
 class TopologyOptimizer:
     def __init__(
         self,
@@ -87,16 +83,18 @@
         method="scipy",
         threshold=(0, 8),
         maxiter=10,
         stopval=None,
         args=None,
         callback=None,
         verbose=False,
-        options={},
+        options=None,
     ):
+        if options is None:
+            options = {}
         self.fun = fun
         self.x0 = x0
         self.nvar = len(x0)
         self.method = method
         self.threshold = threshold
         self.maxiter = maxiter
         self.stopval = stopval
@@ -109,15 +107,14 @@
         self.current_iteration = 0
 
     def print(self, s):
         if self.verbose:
             return print(s)
 
     def minimize(self):
-
         self.print("#################################################")
         self.print(f"Topology optimization with {self.nvar} variables")
         self.print("#################################################")
         self.print("")
         x0 = (
             self.x0.cpu()
             if (get_backend() == "torch" and DEVICE == "cuda")
@@ -183,15 +180,15 @@
                             dy.cpu()
                             if (get_backend() == "torch" and DEVICE == "cuda")
                             else dy
                         )
                         gradn[:] = npo.array(dy, dtype=npo.float64)
 
                     self.current_iteration += 1
-                    return npo.float(y)
+                    return float(y)
 
                 lb = npo.zeros(self.nvar, dtype=npo.float64)
                 ub = npo.ones(self.nvar, dtype=npo.float64)
 
                 self.opt = nlopt.opt(nlopt.LD_MMA, self.nvar)
                 self.opt.set_lower_bounds(lb)
                 self.opt.set_upper_bounds(ub)
```

### Comparing `nannos-2.5.0/src/nannos/parallel.py` & `nannos-2.5.3/src/nannos/parallel.py`

 * *Files identical despite different names*

### Comparing `nannos-2.5.0/src/nannos/plot.py` & `nannos-2.5.3/src/nannos/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import matplotlib.pyplot as plt
 import matplotlib.transforms as mtransforms
 import pyvista
 
 from . import backend as bk
 
-pyvista.set_jupyter_backend("pythreejs")
+pyvista.set_jupyter_backend("trame")
 pyvista.set_plot_theme("document")
 pyvista.global_theme.background = "white"
 # pyvista.global_theme.window_size = [600, 400]
 pyvista.global_theme.axes.show = True
 # pyvista.global_theme.smooth_shading = True
 # pyvista.global_theme.antialiasing = True
 # pyvista.global_theme.axes.box = True
@@ -76,32 +76,31 @@
                 mtransforms.Affine2D()
                 .translate(i * bv[0][0], i * bv[0][1])
                 .translate(j * bv[1][0], j * bv[1][1])
             )
             trans_data = transform + ax.transData
             im.set_transform(trans_data)
             ims.append(im)
-    lx, ly = [bk.linalg.norm(v) for v in lattice.basis_vectors]
+    lx, ly = [
+        bk.linalg.norm(bk.array(v, dtype=bk.float64)) for v in lattice.basis_vectors
+    ]
     lmax = max(lx, ly)
     delta = 0.1 * lmax
     ax.set_xlim(-delta, nperx * bv[0][0] + npery * bv[1][0] + delta)
     ax.set_ylim(-delta, nperx * bv[0][1] + npery * bv[1][1] + delta)
     if show_cell:
         plot_unit_cell(ax, bv, cellstyle)
     ax.set_aspect("equal")
     return ims
 
 
 def plot_structure(
     sim, plotter=None, nper=(1, 1), dz=0.0, null_thickness=None, **kwargs
 ):
-    if "layer_colors" in kwargs:
-        layer_colors = kwargs.pop("layer_colors")
-    else:
-        layer_colors = None
+    layer_colors = kwargs.pop("layer_colors") if "layer_colors" in kwargs else None
     if "layer_metallic" in kwargs:
         layer_metallic = kwargs.pop("layer_metallic")
     else:
         layer_metallic = None
     if "layer_roughness" in kwargs:
         layer_roughness = kwargs.pop("layer_roughness")
     else:
@@ -117,15 +116,14 @@
             [bvs[0][0], bvs[1][0], 0, 0],
             [bvs[0][1], bvs[1][1], 0, 0],
             [0, 0, 1, 0],
             [0, 0, 0, 1],
         ]
     )
     for jx in range(nper[0]):
-
         for jy in range(nper[1]):
             z = 0
             x0, y0 = jx, jy
 
             for ilayer, layer in enumerate(sim.layers):
                 thickness = layer.thickness
                 if thickness == 0:
```

### Comparing `nannos-2.5.0/src/nannos/simulation.py` & `nannos-2.5.3/src/nannos/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         self.bN = bk.array(bk.zeros(2 * self.nh, dtype=bk.complex128))
 
         # This is a boolean checking that the eigenproblems are solved for all layers
         # TODO: This is to avoid solving again, but could be confusing
         self.is_solved = False
         # dictionary to store intermediate S-matrices
         # TODO: check memory consumption of doing that, maybe make it optional.
-        self._intermediate_S = dict()
+        self._intermediate_S = {}
 
     def get_layer(self, id):
         """Helper to get layer index and name.
 
         Parameters
         ----------
         id : int or str
@@ -233,15 +233,14 @@
         else:
             stack = range(indices[0], indices[1])
             logger.info(f"Computing S-matrix for indices {indices}")
 
         try:
             S = self._intermediate_S[f"{stack[0]},{stack[-1]}"]
         except Exception:
-
             for i in stack:
                 layer, layer_next = self.layers[i], self.layers[i + 1]
                 z = layer.thickness or 0
                 z_next = layer_next.thickness or 0
                 f, f_next = bk.diag(phasor(layer.eigenvalues, z)), bk.diag(
                     phasor(layer_next.eigenvalues, z_next)
                 )
@@ -321,42 +320,41 @@
         u = bk.array(u)
         s = 0
         for i in range(self.nh):
             f = bk.zeros(shape, dtype=bk.complex128)
             f = set_index(f, [self.harmonics[0, i], self.harmonics[1, i]], 1.0)
             a = u[i]
             s += a * f
-        ft = fft.inverse_fourier_transform(s, axes=axes)
-        return ft
+        return fft.inverse_fourier_transform(s, axes=axes)
 
     def get_ifft_amplitudes(self, amplitudes, shape, axes=(0, 1)):
         _t0 = timer.tic()
         logger.info("Inverse Fourier transforming amplitudes")
 
         amplitudes = bk.array(amplitudes)
         if len(amplitudes.shape) == 1:
             amplitudes = bk.reshape(amplitudes, amplitudes.shape + (1,))
 
         s = 0
         for i in range(self.nh):
             f = bk.zeros(shape + (amplitudes.shape[0],), dtype=bk.complex128)
+            f = bk.array(f)
             f = set_index(f, [self.harmonics[0, i], self.harmonics[1, i]], 1.0)
             # f[self.harmonics[0, i], self.harmonics[1, i], :] = 1.0
             a = amplitudes[:, i]
             s += a * f
 
         ft = fft.inverse_fourier_transform(s, axes=axes)
         _t1 = timer.toc(_t0, verbose=False)
         logger.info(f"Done inverse Fourier transforming amplitudes in {_t1:0.3e}s")
         return ft
 
     def get_field_grid(
         self, layer_index, z=0, shape=None, field="all", component="all"
     ):
-
         if field not in ["all", "E", "H"]:
             raise ValueError("Wrong field argument, must be `all`, `E` or `H`")
         if component not in ["all", "x", "y", "z"]:
             raise ValueError("Wrong component argument, must be `all`, `x`, `y` or `z`")
 
         layer, layer_index = self.get_layer(layer_index)
         _t0 = timer.tic()
@@ -474,15 +472,15 @@
         norma_r2 = nin**2 * (gamma_in / gamma_in0)
 
         norma_t = (norma_t2.real) ** 0.5
         norma_r = (norma_r2.real) ** 0.5
 
         t = self.get_field_fourier("Substrate")[0, 0] * norma_t
         bx0 = self.get_field_fourier("Superstrate")[0, 0] * norma_r
-        o0 = bk.zeros(self.nh)
+        o0 = bk.array(bk.zeros(self.nh))
         o0 = set_index(o0, [0], 1)
         r = bk.stack([b - o0 * c for b, c in zip(bx0, self.excitation.amplitude)])
         return r, t
 
     def get_z_stress_tensor_integral(self, layer_index, z=0):
         layer, layer_index = self.get_layer(layer_index)
         fields_fourier = self.get_field_fourier(layer_index, z=z)
@@ -523,39 +521,38 @@
             ).real
         )
         return Tx, Ty, Tz
 
     def get_order_index(self, order):
         try:
             len(order) == 2
-        except Exception:
+        except Exception as e:
             if self.lattice.is_1D and isinstance(order, int):
                 order = (order, 0)
             else:
                 raise ValueError(
                     "order must be a tuple of integers length 2 for bi-periodic gratings"
-                )
+                ) from e
         return [
             k for k, i in enumerate(self.harmonics.T) if bk.allclose(i, bk.array(order))
         ][0]
 
     def get_order(self, A, order):
         return A[self.get_order_index(order)]
 
     def _get_toeplitz_matrix(self, u, transverse=False):
         if transverse:
             return [
                 [self._get_toeplitz_matrix(u[i, j]) for j in range(2)] for i in range(2)
             ]
-        else:
-            uft = fft.fourier_transform(u)
-            ix = bk.arange(self.nh)
-            jx, jy = bk.meshgrid(ix, ix, indexing="ij")
-            delta = self.harmonics[:, jx] - self.harmonics[:, jy]
-            return uft[delta[0, :], delta[1, :]]
+        uft = fft.fourier_transform(u)
+        ix = bk.array(bk.arange(self.nh))
+        jx, jy = bk.meshgrid(ix, ix, indexing="ij")
+        delta = self.harmonics[:, jx] - self.harmonics[:, jy]
+        return uft[delta[0], delta[1]]
 
     def build_matrix(self, layer):
         _t0 = timer.tic()
         layer, layer_index = self.get_layer(layer)
         logger.info(f"Building matrix for layer {layer}")
         if layer.iscopy:
             layer.matrix = layer.original.matrix
@@ -565,20 +562,16 @@
             layer.mu_hat = layer.original.mu_hat
             layer.mu_hat_inv = layer.original.mu_hat_inv
             layer.Keps = layer.original.Keps
             layer.Peps = layer.original.Peps
             layer.Qeps = layer.original.Qeps
             return layer
         Kx, Ky = self.Kx, self.Ky
-        if layer.is_uniform:
-            epsilon = layer.epsilon
-            mu = layer.mu
-        else:
-            epsilon = layer.epsilon
-            mu = layer.mu
+        mu = layer.mu
+        epsilon = layer.epsilon
         if layer.is_uniform:
             # if layer.is_epsilon_anisotropic:
             #     _epsilon = block(
             #         [
             #             [epsilon[0, 0] * self.IdG, epsilon[0, 1] * self.IdG],
             #             [epsilon[1, 0] * self.IdG, epsilon[1, 1] * self.IdG],
             #         ]
@@ -675,31 +668,32 @@
         if layer.is_uniform:
             return layer.epsilon
 
         epsilon_zz = (
             layer.epsilon[2, 2] if layer.is_epsilon_anisotropic else layer.epsilon
         )
         eps_hat = self._get_toeplitz_matrix(epsilon_zz)
-        out = self.get_ifft(eps_hat[:, 0], shape=self.lattice.discretization, axes=axes)
-        return out
+        return self.get_ifft(
+            eps_hat[:, 0], shape=self.lattice.discretization, axes=axes
+        )
         # if inv:
         #     u = layer.eps_hat_inv ## nu_hat
         #     out = self.get_ifft(u[0,:], shape=self.lattice.discretization, axes=axes)
         #     return _inv(out)
 
     def _get_amplitudes(self, layer_index, z=0, translate=True):
         _t0 = timer.tic()
         logger.info("Retrieving amplitudes")
 
         layer, layer_index = self.get_layer(layer_index)
         n_interfaces = len(self.layers) - 1
         if layer_index == 0:
             aN, b0 = self._solve_ext()
             ai, bi = self.a0, b0
-        elif layer_index == n_interfaces or layer_index == -1:
+        elif layer_index in [n_interfaces, -1]:
             aN, b0 = self._solve_ext()
             ai, bi = aN, self.bN
         else:
             ai, bi = self._solve_int(layer_index)
         if translate:
             ai, bi = _translate_amplitudes(self.layers[layer_index], z, ai, bi)
         _t1 = timer.toc(_t0, verbose=False)
@@ -742,27 +736,28 @@
             nuhat_inv = _inv((nuhat))
         return N, nuhat_inv
 
     def _get_Peps(self, layer, eps_hat, t, direct=False):
         N, nuhat_inv = self._get_nu_hat_inv(layer)
 
         if direct:
-
             T = block([[t[1], bk.conj(t[0])], [-t[0], bk.conj(t[1])]])
 
             invT = inv2by2block(T, N)
             # invT = _inv(T)
-            if layer.is_epsilon_anisotropic:
-                Q = block(
-                    [[eps_hat[0][0], nuhat_inv[0][1]], [eps_hat[1][0], nuhat_inv[1][1]]]
+            Q = (
+                block(
+                    [
+                        [eps_hat[0][0], nuhat_inv[0][1]],
+                        [eps_hat[1][0], nuhat_inv[1][1]],
+                    ]
                 )
-
-            else:
-                Q = block([[eps_hat[0][0], self.ZeroG], [self.ZeroG, nuhat_inv]])
-
+                if layer.is_epsilon_anisotropic
+                else block([[eps_hat[0][0], self.ZeroG], [self.ZeroG, nuhat_inv]])
+            )
             That = block(
                 [
                     [self._get_toeplitz_matrix(get_block(T, i, j, N)) for j in range(2)]
                     for i in range(2)
                 ]
             )
             invThat = block(
@@ -770,15 +765,15 @@
                     [
                         self._get_toeplitz_matrix(get_block(invT, i, j, N))
                         for j in range(2)
                     ]
                     for i in range(2)
                 ]
             )
-            Peps = That @ Q @ invThat
+            return That @ Q @ invThat
 
         else:
             norm_t = norm(t)
             nt2 = bk.abs(norm_t) ** 2
             Pxx = t[0] * bk.conj(t[0]) / nt2
             Pyy = t[1] * bk.conj(t[1]) / nt2
             Pxy = t[0] * bk.conj(t[1]) / nt2
@@ -797,16 +792,15 @@
             if layer.is_epsilon_anisotropic:
                 D = eps_para_hat - block(nuhat_inv)
             else:
                 D = eps_para_hat - block(
                     [[nuhat_inv, self.ZeroG], [self.ZeroG, nuhat_inv]]
                 )
 
-            Peps = eps_para_hat - D @ Pi
-        return Peps
+            return eps_para_hat - D @ Pi
 
     def plot_structure(
         self, plotter=None, nper=(1, 1), dz=0.0, null_thickness=None, **kwargs
     ):
         return plot_structure(self, plotter, nper, dz, null_thickness, **kwargs)
```

### Comparing `nannos-2.5.0/src/nannos/utils/helpers.py` & `nannos-2.5.3/src/nannos/utils/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,26 +16,55 @@
     "get_block",
     "blockmatmul",
     "block2list",
     "inv2by2block",
     "apply_filter",
 ]
 
+import numpy as npo
+
 from .. import backend as bk
 from .. import get_backend, jit
 from ..formulations.fft import fourier_transform, inverse_fourier_transform
 
 
+def allclose(a, b, **kwargs):
+    try:
+        a = a.detach().cpu().numpy()
+    except:
+        pass
+
+    try:
+        b = b.detach().cpu().numpy()
+    except:
+        pass
+
+    return npo.allclose(a, b, **kwargs)
+
+
 def unique(x):
-    seen = list()
+    seen = []
     return not any(i in seen or seen.append(i) for i in x)
 
 
-def is_scalar(z):
-    return not hasattr(z, "__len__")
+def is_scalar(x):
+    return not hasattr(x, "__len__")
+
+
+def is_anisotropic(x):
+    return False if is_scalar(x) else x.shape[:2] == (3, 3)
+
+
+def is_uniform(x):
+    if is_scalar(x):
+        return True
+    if is_anisotropic(x):
+        return x.shape == (3, 3)
+    else:
+        return x.shape[0] == 1 if len(x.shape) == 1 else x.shape == ()
 
 
 def set_index(mat, idx, val):
     if get_backend() == "jax":
         mat = mat.at[tuple(idx)].set(val)
     else:
         idx += [None]
@@ -67,15 +96,15 @@
     return M[i * n : (i + 1) * n, j * n : (j + 1) * n]
 
 
 def blockmatmul(A, B, N):
     a = [[get_block(A, i, j, N) for j in range(2)] for i in range(2)]
     b = [[get_block(B, i, j, N) for j in range(2)] for i in range(2)]
     out = [
-        [sum([a[i][k] * b[k][j] for k in range(2)]) for j in range(2)] for i in range(2)
+        [sum(a[i][k] * b[k][j] for k in range(2)) for j in range(2)] for i in range(2)
     ]
     return block(out)
 
 
 def block2list(M, N):
     return [[get_block(M, i, j, N) for j in range(2)] for i in range(2)]
 
@@ -88,50 +117,46 @@
             [M[1][1] / detT, -M[0][1] / detT],
             [-M[1][0] / detT, M[0][0] / detT],
         ]
     )
 
 
 def _reseter(prop, attr=None):
-    if attr is None:
-        try:
+    try:
+        if attr is None:
             del prop
-        except Exception:
-            pass
-    else:
-        try:
+        else:
             delattr(prop, attr)
-        except Exception:
-            pass
+    except Exception:
+        pass
 
 
 def _apply_filter(x, rfilt, vectors=None):
-    if rfilt == 0 or rfilt == (0, 0):
+    if is_scalar(rfilt):
+        rfilt = (rfilt, rfilt)
+
+    if rfilt == (0, 0):
         return x
-    else:
+    Nx, Ny = x.shape
 
-        if is_scalar(rfilt):
-            rfilt = (rfilt, rfilt)
-        Nx, Ny = x.shape
-
-        if vectors is not None:
-            tx = bk.array(bk.linspace(-0.5 * vectors[0][0], 0.5 * vectors[0][0], Nx))
-            ty = bk.array(bk.linspace(-0.5 * vectors[1][1], 0.5 * vectors[1][1], Ny))
-        else:
-            tx = bk.array(bk.linspace(-Nx / 2, Nx / 2, Nx))
-            ty = bk.array(bk.linspace(-Ny / 2, Ny / 2, Ny))
+    if vectors is None:
+        tx = bk.array(bk.linspace(-Nx / 2, Nx / 2, Nx))
+        ty = bk.array(bk.linspace(-Ny / 2, Ny / 2, Ny))
 
-        bumpx = bk.exp(-(tx**2) / rfilt[0] ** 2)
-        bumpx /= bk.trapz(bumpx)  # normalize the integral to 1
-        bumpy = bk.exp(-(ty**2) / rfilt[1] ** 2)
-        bumpy /= bk.trapz(bumpy)  # normalize the integral to 1
-        # make a 2-D kernel out of it
-        kernel = bumpx[:, None] * bumpy[None, :]
-        kernel_ft = fourier_transform(kernel, s=x.shape[:2], axes=(0, 1))
-        img_ft = fourier_transform(x, axes=(0, 1))
-        # convolve
-        img2_ft = kernel_ft * img_ft
-        out = bk.real(inverse_fourier_transform(img2_ft, axes=(0, 1)))
-        return bk.fft.fftshift(out) * (Nx * Ny)
+    else:
+        tx = bk.array(bk.linspace(-0.5 * vectors[0][0], 0.5 * vectors[0][0], Nx))
+        ty = bk.array(bk.linspace(-0.5 * vectors[1][1], 0.5 * vectors[1][1], Ny))
+    bumpx = bk.exp(-(tx**2) / rfilt[0] ** 2)
+    bumpx /= bk.trapz(bumpx)  # normalize the integral to 1
+    bumpy = bk.exp(-(ty**2) / rfilt[1] ** 2)
+    bumpy /= bk.trapz(bumpy)  # normalize the integral to 1
+    # make a 2-D kernel out of it
+    kernel = bumpx[:, None] * bumpy[None, :]
+    kernel_ft = fourier_transform(kernel, s=x.shape[:2], axes=(0, 1))
+    img_ft = fourier_transform(x, axes=(0, 1))
+    # convolve
+    img2_ft = kernel_ft * img_ft
+    out = bk.real(inverse_fourier_transform(img2_ft, axes=(0, 1)))
+    return bk.fft.fftshift(out) * (Nx * Ny)
 
 
 apply_filter = jit(_apply_filter, static_argnums=(1))
```

### Comparing `nannos-2.5.0/src/nannos/utils/jupyter.py` & `nannos-2.5.3/src/nannos/utils/jupyter.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,70 +26,63 @@
 def local_hardware_info():
     """Basic hardware information about the local machine.
     Gives actual number of CPU's in the machine, even when hyperthreading is
     turned on. CPU count defaults to 1 when true count can't be determined.
     Returns:
         dict: The hardware information.
     """
-    results = {
+    return {
         "python_compiler": platform.python_compiler(),
         "python_build": ", ".join(platform.python_build()),
         "python_version": platform.python_version(),
         "os": platform.system(),
         "memory": psutil.virtual_memory().total / (1024**3),
         "cpus": psutil.cpu_count(logical=False) or 1,
     }
-    return results
 
 
 @magics_class
 class VersionTable(Magics):
     """A class of status magic functions."""
 
     @line_magic
     def nannos_version_table(self, line="", cell=None):
         """
         Print an HTML-formatted table with version numbers for Nannos and its
         dependencies. This should make it possible to reproduce the environment
         and the calculation later on.
         """
 
-        html = "<h3>Version Information</h3>"
-        html += "<table>"
+        html = "<h3>Version Information</h3>" + "<table>"
         html += "<tr><th>Package</th></tr>"
 
         packages = []
 
-        packages_names = ["nannos", "numpy", "scipy", "matplotlib"]
+        packages_names = ["nannos", "numpy", "scipy", "autograd", "jax", "torch"]
 
         for pkg in packages_names:
             ver = pkg_resources.get_distribution(pkg).version
 
             packages.append((f"<code>{pkg}</code>", ver))
 
-        ver = pkg_resources.get_distribution("autograd").version
-        packages.append(("<code>autograd</code>", ver))
-
         for name, version in packages:
             html += f"<tr><td>{name}</td><td>{version}</td></tr>"
 
         html += "<tr><th>System information</th></tr>"
 
         local_hw_info = local_hardware_info()
         sys_info = [
             ("Python version", local_hw_info["python_version"]),
             ("Python compiler", local_hw_info["python_compiler"]),
             ("Python build", local_hw_info["python_build"]),
-            ("OS", "%s" % local_hw_info["os"]),
-            ("CPUs", "%s" % local_hw_info["cpus"]),
-            ("Memory (Gb)", "%s" % local_hw_info["memory"]),
+            ("OS", f'{local_hw_info["os"]}'),
+            ("CPUs", f'{local_hw_info["cpus"]}'),
+            ("Memory (Gb)", f'{local_hw_info["memory"]}'),
         ]
 
         for name, version in sys_info:
             html += f"<tr><td>{name}</td><td>{version}</td></tr>"
 
-        html += "<tr><td colspan='2'>%s</td></tr>" % time.strftime(
-            "%a %b %d %H:%M:%S %Y %Z"
-        )
+        html += f"""<tr><td colspan='2'>{time.strftime("%a %b %d %H:%M:%S %Y %Z")}</td></tr>"""
         html += "</table>"
 
         return display(HTML(html))
```

### Comparing `nannos-2.5.0/src/nannos.egg-info/SOURCES.txt` & `nannos-2.5.3/src/nannos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

