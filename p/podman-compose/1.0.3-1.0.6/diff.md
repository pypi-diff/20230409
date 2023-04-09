# Comparing `tmp/podman-compose-1.0.3.tar.gz` & `tmp/podman-compose-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podman-compose-1.0.3.tar", last modified: Tue Dec 21 21:17:16 2021, max compression
+gzip compressed data, was "podman-compose-1.0.6.tar", last modified: Sun Apr  9 11:06:25 2023, max compression
```

## Comparing `podman-compose-1.0.3.tar` & `podman-compose-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 alsadi    (1000) alsadi    (1000)        0 2021-12-21 21:17:16.853515 podman-compose-1.0.3/
--rw-rw-r--   0 alsadi    (1000) alsadi    (1000)     4946 2021-12-21 21:17:16.854515 podman-compose-1.0.3/PKG-INFO
--rw-rw-r--   0 alsadi    (1000) alsadi    (1000)     3205 2021-12-21 21:16:51.000000 podman-compose-1.0.3/README.md
-drwxrwxr-x   0 alsadi    (1000) alsadi    (1000)        0 2021-12-21 21:17:16.853515 podman-compose-1.0.3/podman_compose.egg-info/
--rw-rw-r--   0 alsadi    (1000) alsadi    (1000)     4946 2021-12-21 21:17:16.000000 podman-compose-1.0.3/podman_compose.egg-info/PKG-INFO
--rw-rw-r--   0 alsadi    (1000) alsadi    (1000)      276 2021-12-21 21:17:16.000000 podman-compose-1.0.3/podman_compose.egg-info/SOURCES.txt
--rw-rw-r--   0 alsadi    (1000) alsadi    (1000)        1 2021-12-21 21:17:16.000000 podman-compose-1.0.3/podman_compose.egg-info/dependency_links.txt
--rw-rw-r--   0 alsadi    (1000) alsadi    (1000)       56 2021-12-21 21:17:16.000000 podman-compose-1.0.3/podman_compose.egg-info/entry_points.txt
--rw-rw-r--   0 alsadi    (1000) alsadi    (1000)       21 2021-12-21 21:17:16.000000 podman-compose-1.0.3/podman_compose.egg-info/requires.txt
--rw-rw-r--   0 alsadi    (1000) alsadi    (1000)       15 2021-12-21 21:17:16.000000 podman-compose-1.0.3/podman_compose.egg-info/top_level.txt
--rwxrwxr-x   0 alsadi    (1000) alsadi    (1000)    73250 2021-12-21 21:16:51.000000 podman-compose-1.0.3/podman_compose.py
--rw-rw-r--   0 alsadi    (1000) alsadi    (1000)      122 2021-12-21 21:17:16.854515 podman-compose-1.0.3/setup.cfg
--rw-rw-r--   0 alsadi    (1000) alsadi    (1000)     1440 2021-12-21 21:11:48.000000 podman-compose-1.0.3/setup.py
+drwxr-xr-x   0 alsadi    (1000) alsadi    (1000)        0 2023-04-09 11:06:25.758990 podman-compose-1.0.6/
+-rw-rw-r--   0 alsadi    (1000) alsadi    (1000)    18092 2021-12-21 21:11:48.000000 podman-compose-1.0.6/LICENSE
+-rw-r--r--   0 alsadi    (1000) alsadi    (1000)     5139 2023-04-09 11:06:25.758990 podman-compose-1.0.6/PKG-INFO
+-rw-r--r--   0 alsadi    (1000) alsadi    (1000)     4094 2023-04-09 11:04:42.000000 podman-compose-1.0.6/README.md
+drwxr-xr-x   0 alsadi    (1000) alsadi    (1000)        0 2023-04-09 11:06:25.758990 podman-compose-1.0.6/podman_compose.egg-info/
+-rw-rw-r--   0 alsadi    (1000) alsadi    (1000)     5139 2023-04-09 11:06:25.000000 podman-compose-1.0.6/podman_compose.egg-info/PKG-INFO
+-rw-rw-r--   0 alsadi    (1000) alsadi    (1000)      284 2023-04-09 11:06:25.000000 podman-compose-1.0.6/podman_compose.egg-info/SOURCES.txt
+-rw-rw-r--   0 alsadi    (1000) alsadi    (1000)        1 2023-04-09 11:06:25.000000 podman-compose-1.0.6/podman_compose.egg-info/dependency_links.txt
+-rw-rw-r--   0 alsadi    (1000) alsadi    (1000)       56 2023-04-09 11:06:25.000000 podman-compose-1.0.6/podman_compose.egg-info/entry_points.txt
+-rw-rw-r--   0 alsadi    (1000) alsadi    (1000)       61 2023-04-09 11:06:25.000000 podman-compose-1.0.6/podman_compose.egg-info/requires.txt
+-rw-rw-r--   0 alsadi    (1000) alsadi    (1000)       15 2023-04-09 11:06:25.000000 podman-compose-1.0.6/podman_compose.egg-info/top_level.txt
+-rwxr-xr-x   0 alsadi    (1000) alsadi    (1000)   101409 2023-04-09 11:04:42.000000 podman-compose-1.0.6/podman_compose.py
+-rw-rw-r--   0 alsadi    (1000) alsadi    (1000)      122 2023-04-09 11:06:25.759990 podman-compose-1.0.6/setup.cfg
+-rw-r--r--   0 alsadi    (1000) alsadi    (1000)     1699 2023-04-09 11:04:42.000000 podman-compose-1.0.6/setup.py
```

### Comparing `podman-compose-1.0.3/README.md` & `podman-compose-1.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # Podman Compose
+## [![Pylint Test: ](https://github.com/containers/podman-compose/actions/workflows/pylint.yml/badge.svg)](https://github.com/containers/podman-compose/actions/workflows/pylint.yml) [![Unit tests  PyTest](https://github.com/containers/podman-compose/actions/workflows/pytest.yml/badge.svg)](https://github.com/containers/podman-compose/actions/workflows/pytest.yml)
+
 
 An implementation of [Compose Spec](https://compose-spec.io/) with [Podman](https://podman.io/) backend.
-This project focus on:
+This project focuses on:
 
 * rootless
 * daemon-less process model, we directly execute podman, no running daemon.
 
-This project only depend on:
+This project only depends on:
 
 * `podman`
+* [podman dnsname plugin](https://github.com/containers/dnsname): It is usually found in the `podman-plugins` or `podman-dnsname` distro packages, those packages are not pulled by default and you need to install them. This allows containers to be able to resolve each other if they are on the same CNI network.
 * Python3
 * [PyYAML](https://pyyaml.org/)
 * [python-dotenv](https://pypi.org/project/python-dotenv/)
 
-And it's formed as a single python file script that you can drop into your PATH and run.
+And it's formed as a single Python file script that you can drop into your PATH and run.
 
 ## References:
 
 * [spec.md](https://github.com/compose-spec/compose-spec/blob/master/spec.md)
 * [docker-compose compose-file-v3](https://docs.docker.com/compose/compose-file/compose-file-v3/)
 * [docker-compose compose-file-v2](https://docs.docker.com/compose/compose-file/compose-file-v2/)
 
@@ -34,55 +37,48 @@
 OpenShift/Kubernetes distribution like [OKD](https://www.okd.io/).
 
 ## Versions
 
 If you have legacy version of `podman` (before 3.1.0) you might need to stick with legacy `podman-compose` `0.1.x` branch.
 The legacy branch 0.1.x uses mappings and workarounds to compensate for rootless limitations.
 
-Modern podman versions (>=3.4) do not have those limitations and thus you can use latest and stable 1.x branch.
+Modern podman versions (>=3.4) do not have those limitations, and thus you can use latest and stable 1.x branch.
+
+If you are upgrading from `podman-compose` version `0.1.x` then we no longer have global option `-t` to set mapping type
+like `hostnet`. If you desire that behavior, pass it the standard way like `network_mode: host` in the YAML.
+
 
 ## Installation
 
-Install latest stable version from PyPI:
+Install the latest stable version from PyPI:
 
 ```
 pip3 install podman-compose
 ```
 
 pass `--user` to install inside regular user home without being root.
 
 Or latest development version from GitHub:
 
 ```
 pip3 install https://github.com/containers/podman-compose/archive/devel.tar.gz
 ```
 
-or
-
-```
-curl -o /usr/local/bin/podman-compose https://raw.githubusercontent.com/containers/podman-compose/devel/podman_compose.py
-chmod +x /usr/local/bin/podman-compose
-```
-
-or inside your home
-
-```
-curl -o ~/.local/bin/podman-compose https://raw.githubusercontent.com/containers/podman-compose/devel/podman_compose.py
-chmod +x ~/.local/bin/podman-compose
-```
 
 or install from Fedora (starting from f31) repositories:
 
 ```
 sudo dnf install podman-compose
 ```
 
 ## Basic Usage
 
 We have included fully functional sample stacks inside `examples/` directory.
+You can get more examples from [awesome-compose](https://github.com/docker/awesome-compose).
+
 
 A quick example would be
 
 ```
 cd examples/busybox
 podman-compose --help
 podman-compose up --help
@@ -95,16 +91,25 @@
 - A Postgres Database
 - RabbitMQ server
 - MemCached server
 - a django web server
 - a django tasks
 
 
-When testing the `AWX3` example, if you got errors just wait for db migrations to end. 
+When testing the `AWX3` example, if you got errors, just wait for db migrations to end.
 There is also AWX 17.1.0
 
 ## Tests
 
 Inside `tests/` directory we have many useless docker-compose stacks
-that are meant to test as much cases as we can to make sure we are compatible
+that are meant to test as many cases as we can to make sure we are compatible
+
+### Unit tests with pytest
+run a pytest with following command
+
+```shell
+python -m pytest pytests
+```
 
+# Contributing guide
 
+If you are a user or a developer and want to contribute please check the [CONTRIBUTING](CONTRIBUTING.md) section
```

### Comparing `podman-compose-1.0.3/setup.py` & `podman-compose-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 import os
 from setuptools import setup
 
 try:
-    readme = open(os.path.join(os.path.dirname(__file__), 'README.md')).read()
+    readme = open(os.path.join(os.path.dirname(__file__), "README.md")).read()
 except:
-    readme = ''
+    readme = ""
 
 setup(
-    name='podman-compose',
+    name="podman-compose",
     description="A script to run docker-compose.yml using podman",
     long_description=readme,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
-    keywords='podman, podman-compose',
-    author='Muayyad Alsadi',
-    author_email='alsadi@gmail.com',
-    url='https://github.com/containers/podman-compose',
-    py_modules=['podman_compose'],
-    entry_points={
-        'console_scripts': [
-            'podman-compose = podman_compose:main'
-        ]
-    },
+    keywords="podman, podman-compose",
+    author="Muayyad Alsadi",
+    author_email="alsadi@gmail.com",
+    url="https://github.com/containers/podman-compose",
+    py_modules=["podman_compose"],
+    entry_points={"console_scripts": ["podman-compose = podman_compose:main"]},
     include_package_data=True,
-    license='GPL-2.0-only',
+    license="GPL-2.0-only",
     install_requires=[
-        'pyyaml',
-        'python-dotenv',
+        "pyyaml",
+        "python-dotenv",
     ],
+    extras_require={
+        "devel": [
+            "flake8",
+            "black",
+            "pylint",
+            "pre-commit",
+        ]
+    }
     # test_suite='tests',
     # tests_require=[
     #     'coverage',
     #     'pytest-cov',
     #     'pytest',
     #     'tox',
     # ]
```

