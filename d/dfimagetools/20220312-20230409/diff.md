# Comparing `tmp/dfimagetools-20220312.tar.gz` & `tmp/dfimagetools-20230409.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfimagetools-20220312.tar", last modified: Sat Mar 12 08:23:50 2022, max compression
+gzip compressed data, was "dfimagetools-20230409.tar", last modified: Sun Apr  9 20:55:44 2023, max compression
```

## Comparing `dfimagetools-20220312.tar` & `dfimagetools-20230409.tar`

### file list

```diff
@@ -1,89 +1,96 @@
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.850754 dfimagetools-20220312/
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.761753 dfimagetools-20220312/.github/
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.813753 dfimagetools-20220312/.github/workflows/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3686 2022-02-19 12:29:52.000000 dfimagetools-20220312/.github/workflows/test_docker.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1936 2022-02-19 12:29:52.000000 dfimagetools-20220312/.github/workflows/test_docs.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2236 2022-02-19 12:29:52.000000 dfimagetools-20220312/.github/workflows/test_tox.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19381 2022-02-19 12:29:52.000000 dfimagetools-20220312/.pylintrc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      479 2022-02-02 19:54:32.000000 dfimagetools-20220312/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      292 2022-01-29 19:59:40.000000 dfimagetools-20220312/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2021-10-31 13:10:45.000000 dfimagetools-20220312/LICENSE
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      608 2022-01-29 19:59:40.000000 dfimagetools-20220312/MANIFEST.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-01-29 19:59:40.000000 dfimagetools-20220312/MANIFEST.test_data.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      548 2022-03-12 08:23:50.850754 dfimagetools-20220312/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      153 2021-12-26 07:38:07.000000 dfimagetools-20220312/README
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1490 2022-02-19 12:29:52.000000 dfimagetools-20220312/appveyor.yml
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.762754 dfimagetools-20220312/config/
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.825754 dfimagetools-20220312/config/appveyor/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1053 2022-02-19 12:29:52.000000 dfimagetools-20220312/config/appveyor/install.ps1
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)       91 2022-02-19 12:29:52.000000 dfimagetools-20220312/config/appveyor/install.sh
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      466 2022-02-19 12:29:52.000000 dfimagetools-20220312/config/appveyor/runtests.sh
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.827754 dfimagetools-20220312/config/dpkg/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      175 2022-03-12 08:22:43.000000 dfimagetools-20220312/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       23 2021-12-23 07:30:27.000000 dfimagetools-20220312/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2022-02-19 12:29:52.000000 dfimagetools-20220312/config/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1766 2022-02-20 05:35:33.000000 dfimagetools-20220312/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      976 2021-12-26 07:38:07.000000 dfimagetools-20220312/config/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2021-12-26 07:38:07.000000 dfimagetools-20220312/config/dpkg/dfimagetools-tools.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      105 2021-12-26 07:38:07.000000 dfimagetools-20220312/config/dpkg/python3-dfimagetools.install
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2022-02-19 12:29:52.000000 dfimagetools-20220312/config/dpkg/rules
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.827754 dfimagetools-20220312/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2021-12-23 07:30:27.000000 dfimagetools-20220312/config/dpkg/source/format
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.827754 dfimagetools-20220312/config/pylint/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      229 2021-12-21 12:01:47.000000 dfimagetools-20220312/config/pylint/spelling-private-dict
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5509 2022-02-20 05:35:33.000000 dfimagetools-20220312/dependencies.ini
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.829753 dfimagetools-20220312/dfimagetools/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      110 2022-03-12 08:22:43.000000 dfimagetools-20220312/dfimagetools/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4460 2022-03-11 16:32:34.000000 dfimagetools-20220312/dfimagetools/artifact_filters.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7918 2022-02-02 20:12:18.000000 dfimagetools-20220312/dfimagetools/bodyfile.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3427 2022-01-29 19:59:40.000000 dfimagetools-20220312/dfimagetools/data_stream_writer.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      711 2022-01-29 19:59:40.000000 dfimagetools-20220312/dfimagetools/decorators.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3562 2022-01-29 19:59:40.000000 dfimagetools-20220312/dfimagetools/environment_variables.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7426 2022-01-29 19:59:40.000000 dfimagetools-20220312/dfimagetools/file_entry_lister.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1138 2021-12-26 07:38:07.000000 dfimagetools-20220312/dfimagetools/helpers.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11157 2022-03-11 16:32:34.000000 dfimagetools-20220312/dfimagetools/path_resolver.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2362 2022-01-29 19:59:40.000000 dfimagetools-20220312/dfimagetools/resources.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2022-02-20 08:15:25.000000 dfimagetools-20220312/dfimagetools/windows_registry.py
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.830753 dfimagetools-20220312/dfimagetools.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      548 2022-03-12 08:23:49.000000 dfimagetools-20220312/dfimagetools.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1728 2022-03-12 08:23:50.000000 dfimagetools-20220312/dfimagetools.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2022-03-12 08:23:49.000000 dfimagetools-20220312/dfimagetools.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      775 2022-03-12 08:23:49.000000 dfimagetools-20220312/dfimagetools.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       13 2022-03-12 08:23:49.000000 dfimagetools-20220312/dfimagetools.egg-info/top_level.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      388 2021-12-26 07:38:07.000000 dfimagetools-20220312/dfimagetools.ini
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.831754 dfimagetools-20220312/docs/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5100 2022-02-19 12:29:53.000000 dfimagetools-20220312/docs/conf.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2021-12-26 07:38:07.000000 dfimagetools-20220312/docs/index.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       87 2022-02-19 12:29:53.000000 dfimagetools-20220312/docs/requirements.txt
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.836753 dfimagetools-20220312/docs/sources/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5512 2022-01-29 19:59:40.000000 dfimagetools-20220312/docs/sources/Bodyfile-format.md
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.837754 dfimagetools-20220312/docs/sources/api/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1883 2022-03-12 08:22:43.000000 dfimagetools-20220312/docs/sources/api/dfimagetools.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       73 2021-12-26 07:38:07.000000 dfimagetools-20220312/docs/sources/api/modules.rst
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.837754 dfimagetools-20220312/docs/sources/user/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1693 2022-02-02 19:54:32.000000 dfimagetools-20220312/docs/sources/user/Installation-instructions.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      296 2021-12-26 07:38:07.000000 dfimagetools-20220312/docs/sources/user/index.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      843 2022-02-20 05:35:33.000000 dfimagetools-20220312/requirements.txt
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1027 2021-12-21 09:32:11.000000 dfimagetools-20220312/run_tests.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2022-03-12 08:23:50.851754 dfimagetools-20220312/setup.cfg
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     6800 2022-02-19 12:29:52.000000 dfimagetools-20220312/setup.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      287 2021-12-21 09:32:11.000000 dfimagetools-20220312/test_dependencies.ini
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       40 2022-02-19 12:29:52.000000 dfimagetools-20220312/test_requirements.txt
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.839753 dfimagetools-20220312/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20220312/tests/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7807 2022-03-11 16:32:34.000000 dfimagetools-20220312/tests/artifact_filters.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4034 2022-01-29 19:59:40.000000 dfimagetools-20220312/tests/bodyfile.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2291 2022-01-29 19:59:40.000000 dfimagetools-20220312/tests/environment_variables.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3293 2022-01-29 19:59:40.000000 dfimagetools-20220312/tests/file_entry_lister.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11717 2022-03-11 16:32:34.000000 dfimagetools-20220312/tests/path_resover.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2282 2021-12-21 12:01:47.000000 dfimagetools-20220312/tests/test_lib.py
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.849753 dfimagetools-20220312/tools/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       57 2021-12-21 09:32:11.000000 dfimagetools-20220312/tools/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     8910 2022-02-20 14:51:47.000000 dfimagetools-20220312/tools/extract_data_streams.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     8109 2022-02-20 14:51:47.000000 dfimagetools-20220312/tools/list_file_entries.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1229 2022-02-19 12:29:53.000000 dfimagetools-20220312/tox.ini
-drwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-03-12 08:23:50.850754 dfimagetools-20220312/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20220312/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2022-02-19 12:29:52.000000 dfimagetools-20220312/utils/check_dependencies.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11928 2022-02-19 12:29:53.000000 dfimagetools-20220312/utils/dependencies.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      655 2021-12-26 07:38:07.000000 dfimagetools-20220312/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.132284 dfimagetools-20230409/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:43.984284 dfimagetools-20230409/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.020284 dfimagetools-20230409/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3653 2023-04-09 14:48:22.000000 dfimagetools-20230409/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2023-04-09 14:48:22.000000 dfimagetools-20230409/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2023-04-09 14:48:22.000000 dfimagetools-20230409/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22101 2023-04-09 14:48:22.000000 dfimagetools-20230409/.pylintrc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-04-30 13:22:39.000000 dfimagetools-20230409/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      479 2022-04-30 13:22:39.000000 dfimagetools-20230409/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      292 2022-04-30 13:22:39.000000 dfimagetools-20230409/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2021-10-31 13:10:45.000000 dfimagetools-20230409/LICENSE
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      608 2022-01-29 19:59:40.000000 dfimagetools-20230409/MANIFEST.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-01-29 19:59:40.000000 dfimagetools-20230409/MANIFEST.test_data.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      566 2023-04-09 20:55:44.132284 dfimagetools-20230409/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      153 2021-12-26 07:38:07.000000 dfimagetools-20230409/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-09 20:52:07.000000 dfimagetools-20230409/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:43.984284 dfimagetools-20230409/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.020284 dfimagetools-20230409/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-04-09 20:52:07.000000 dfimagetools-20230409/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-04-09 14:48:22.000000 dfimagetools-20230409/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-04-09 14:48:22.000000 dfimagetools-20230409/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.022284 dfimagetools-20230409/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-04-09 20:52:07.000000 dfimagetools-20230409/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       23 2021-12-23 07:30:27.000000 dfimagetools-20230409/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-04-09 14:48:22.000000 dfimagetools-20230409/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1798 2023-04-09 14:48:22.000000 dfimagetools-20230409/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      976 2021-12-26 07:38:07.000000 dfimagetools-20230409/config/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2021-12-26 07:38:07.000000 dfimagetools-20230409/config/dpkg/dfimagetools-tools.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      105 2021-12-26 07:38:07.000000 dfimagetools-20230409/config/dpkg/python3-dfimagetools.install
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-04-09 14:48:22.000000 dfimagetools-20230409/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.022284 dfimagetools-20230409/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2021-12-23 07:30:27.000000 dfimagetools-20230409/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.022284 dfimagetools-20230409/config/pylint/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      229 2021-12-21 12:01:47.000000 dfimagetools-20230409/config/pylint/spelling-private-dict
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5687 2022-09-03 04:58:03.000000 dfimagetools-20230409/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.024284 dfimagetools-20230409/dfimagetools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      110 2023-04-09 20:52:07.000000 dfimagetools-20230409/dfimagetools/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/artifact_filters.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9053 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/bodyfile.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/data_stream_writer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/decorators.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/environment_variables.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6866 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/file_entry_lister.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2022-09-03 04:58:03.000000 dfimagetools-20230409/dfimagetools/helpers.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11121 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/path_resolver.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4304 2022-12-26 19:18:50.000000 dfimagetools-20230409/dfimagetools/recursive_hasher.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2362 2022-04-30 13:22:39.000000 dfimagetools-20230409/dfimagetools/resources.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2861 2022-12-26 04:50:18.000000 dfimagetools-20230409/dfimagetools/source_analyzer.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2022-04-30 13:22:39.000000 dfimagetools-20230409/dfimagetools/windows_registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.025284 dfimagetools-20230409/dfimagetools.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2023-04-09 20:55:42.000000 dfimagetools-20230409/dfimagetools.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1905 2023-04-09 20:55:43.000000 dfimagetools-20230409/dfimagetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-04-09 20:55:42.000000 dfimagetools-20230409/dfimagetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      801 2023-04-09 20:55:42.000000 dfimagetools-20230409/dfimagetools.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       13 2023-04-09 20:55:42.000000 dfimagetools-20230409/dfimagetools.egg-info/top_level.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      388 2021-12-26 07:38:07.000000 dfimagetools-20230409/dfimagetools.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.036284 dfimagetools-20230409/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2023-04-09 14:48:22.000000 dfimagetools-20230409/docs/conf.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-11-21 19:36:05.000000 dfimagetools-20230409/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-04-09 14:48:38.000000 dfimagetools-20230409/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.053284 dfimagetools-20230409/docs/sources/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2022-12-18 20:43:00.000000 dfimagetools-20230409/docs/sources/Bodyfile-format.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.073284 dfimagetools-20230409/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2236 2023-04-09 20:52:07.000000 dfimagetools-20230409/docs/sources/api/dfimagetools.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       73 2022-11-21 19:36:05.000000 dfimagetools-20230409/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.105284 dfimagetools-20230409/docs/sources/user/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1693 2022-11-21 19:36:05.000000 dfimagetools-20230409/docs/sources/user/Installation-instructions.md
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      296 2022-11-21 19:36:05.000000 dfimagetools-20230409/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      871 2023-04-09 14:48:22.000000 dfimagetools-20230409/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-10-02 12:20:49.000000 dfimagetools-20230409/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2023-04-09 20:55:44.133284 dfimagetools-20230409/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6828 2023-04-09 14:48:22.000000 dfimagetools-20230409/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 18:36:28.000000 dfimagetools-20230409/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 14:48:22.000000 dfimagetools-20230409/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.108284 dfimagetools-20230409/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20230409/tests/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7807 2022-04-30 13:22:39.000000 dfimagetools-20230409/tests/artifact_filters.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4034 2022-01-29 19:59:40.000000 dfimagetools-20230409/tests/bodyfile.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2291 2022-04-30 13:22:39.000000 dfimagetools-20230409/tests/environment_variables.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3293 2022-01-29 19:59:40.000000 dfimagetools-20230409/tests/file_entry_lister.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11717 2022-04-30 13:22:39.000000 dfimagetools-20230409/tests/path_resover.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      655 2022-12-23 10:46:53.000000 dfimagetools-20230409/tests/source_analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2273 2022-10-02 12:20:49.000000 dfimagetools-20230409/tests/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.122284 dfimagetools-20230409/tools/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       57 2021-12-21 09:32:11.000000 dfimagetools-20230409/tools/__init__.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     8865 2022-10-02 12:20:49.000000 dfimagetools-20230409/tools/extract_data_streams.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     8136 2022-12-18 20:43:00.000000 dfimagetools-20230409/tools/list_file_entries.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     5100 2022-10-02 12:20:49.000000 dfimagetools-20230409/tools/map_extents.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4465 2022-12-26 19:18:50.000000 dfimagetools-20230409/tools/recursive_hasher.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3866 2022-12-25 20:20:03.000000 dfimagetools-20230409/tools/source_analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2023-04-09 14:48:22.000000 dfimagetools-20230409/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.123284 dfimagetools-20230409/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20230409/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-04-09 14:48:22.000000 dfimagetools-20230409/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-04-09 14:48:22.000000 dfimagetools-20230409/utils/dependencies.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      655 2022-04-30 13:22:18.000000 dfimagetools-20230409/utils/update_release.sh
```

### Comparing `dfimagetools-20220312/.github/workflows/test_docker.yml` & `dfimagetools-20230409/.github/workflows/test_docker.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # Run tests on Fedora and Ubuntu Docker images using GIFT CORP and GIFT PPA on commit
 name: test_docker
 on: [push]
+permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['34', '35']
+        version: ['37']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
     - uses: actions/checkout@v2
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
-        dnf install -y @development-tools python3 python3-devel libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-dtfabric python3-idna python3-mock python3-pbr python3-pytsk3 python3-pyxattr python3-pyyaml python3-setuptools python3-six
+        dnf install -y @development-tools python3 python3-devel libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-dtfabric python3-idna python3-pytsk3 python3-pyxattr python3-pyyaml python3-setuptools
     - name: Run tests
       env:
         LANG: C.utf8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       run: |
@@ -36,15 +37,15 @@
       run: |
         python3 ./setup.py build
         python3 ./setup.py install
   test_ubuntu:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['18.04', '20.04']
+        version: ['22.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
     - uses: actions/checkout@v2
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
@@ -53,15 +54,15 @@
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
         ln -f -s /usr/share/zoneinfo/UTC /etc/localtime
     - name: Install dependencies
       run: |
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential python3 python3-dev libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi-backend python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-distutils python3-dtfabric python3-idna python3-mock python3-pbr python3-pytsk3 python3-pyxattr python3-setuptools python3-six python3-yaml
+        apt-get install -y build-essential python3 python3-dev libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi-backend python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-distutils python3-dtfabric python3-idna python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       env:
```

### Comparing `dfimagetools-20220312/.github/workflows/test_docs.yml` & `dfimagetools-20230409/.github/workflows/test_docs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 on:
   pull_request:
     branches:
     - main
   push:
     branches:
     - main
+permissions: read-all
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
         - python-version: '3.8'
           toxenv: 'docs'
     container:
-      image: ubuntu:20.04
+      image: ubuntu:22.04
     steps:
     - uses: actions/checkout@v2
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
@@ -31,15 +32,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi-backend python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-distutils python3-dtfabric python3-idna python3-mock python3-pbr python3-pip python3-pytsk3 python3-pyxattr python3-setuptools python3-six python3-yaml
+        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi-backend python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
```

### Comparing `dfimagetools-20220312/.github/workflows/test_tox.yml` & `dfimagetools-20230409/.github/workflows/test_tox.yml`

 * *Files 9% similar despite different names*

```diff
@@ -3,34 +3,35 @@
 on:
   pull_request:
     branches:
     - main
   push:
     branches:
     - main
+permissions: read-all
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
-        - python-version: '3.6'
-          toxenv: 'py36'
         - python-version: '3.7'
           toxenv: 'py37'
         - python-version: '3.8'
           toxenv: 'py38,coverage,codecov'
         - python-version: '3.9'
           toxenv: 'py39'
         - python-version: '3.10'
           toxenv: 'py310'
-        - python-version: '3.8'
-          toxenv: 'pylint'
+        - python-version: '3.11'
+          toxenv: 'py311'
+        - python-version: '3.11'
+          toxenv: 'lint'
     container:
-      image: ubuntu:20.04
+      image: ubuntu:22.04
     steps:
     - uses: actions/checkout@v2
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
@@ -41,15 +42,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi-backend python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-distutils python3-dtfabric python3-idna python3-mock python3-pbr python3-pip python3-pytsk3 python3-pyxattr python3-setuptools python3-six python3-yaml
+        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi-backend python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
```

### Comparing `dfimagetools-20220312/.pylintrc` & `dfimagetools-20230409/.pylintrc`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,30 @@
-# Pylint 2.9.x configuration file
+# Pylint 2.14.x configuration file
 #
 # This file is generated by l2tdevtools update-dependencies.py, any dependency
 # related changes should be made in dependencies.ini.
-[MASTER]
+[MAIN]
+
+# Analyse import fallback blocks. This can be used to support both Python 2 and
+# 3 compatible code, which means that the block might have code that exists
+# only in one or another interpreter, leading to false positives when analysed.
+analyse-fallback-blocks=no
+
+# Load and enable all available extensions. Use --list-extensions to see a list
+# all available extensions.
+#enable-all-extensions=
+
+# In error mode, messages with a category besides ERROR or FATAL are
+# suppressed, and no reports are done by default. Error mode is compatible with
+# disabling specific errors.
+#errors-only=
+
+# Always return a 0 (non-error) status code, even if lint errors are found.
+# This is primarily useful in continuous integration scripts.
+#exit-zero=
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code.
 extension-pkg-allow-list=pybde,pycreg,pyewf,pyfsapfs,pyfsext,pyfshfs,pyfsntfs,pyfsxfs,pyfvde,pyfwnt,pyluksde,pymodi,pyphdi,pyqcow,pyregf,pysigscan,pysmdev,pysmraw,pytsk3,pyvhdi,pyvmdk,pyvsgpt,pyvshadow,pyvslvm,xattr
 
 # A comma-separated list of package or module names from where C extensions may
@@ -17,86 +35,137 @@
 
 # Return non-zero exit code if any of these messages/categories are detected,
 # even if score is above --fail-under value. Syntax same as enable. Messages
 # specified are enabled, while categories only check already-enabled messages.
 fail-on=
 
 # Specify a score threshold to be exceeded before program exits with error.
-fail-under=10.0
+fail-under=10
+
+# Interpret the stdin as a python script, whose filename needs to be passed as
+# the module_or_package argument.
+#from-stdin=
 
 # Files or directories to be skipped. They should be base names, not paths.
 ignore=CVS
 
 # Add files or directories matching the regex patterns to the ignore-list. The
-# regex matches against paths.
+# regex matches against paths and can be in Posix or Windows format.
 ignore-paths=
 
 # Files or directories matching the regex patterns are skipped. The regex
-# matches against base names, not paths.
-ignore-patterns=
+# matches against base names, not paths. The default value ignores Emacs file
+# locks
+ignore-patterns=^\.#
+
+# List of module names for which member attributes should not be checked
+# (useful for modules/projects where namespaces are manipulated during runtime
+# and thus existing member attributes cannot be deduced by static analysis). It
+# supports qualified module names, as well as Unix pattern matching.
+ignored-modules=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
-# number of processors available to use.
+# number of processors available to use, and will cap the count on Windows to
+# avoid hangs.
 jobs=1
 
 # Control the amount of potential inferred values when inferring a single
 # object. This can help the performance when dealing with large functions or
 # complex, nested conditions.
 limit-inference-results=100
 
 # List of plugins (as comma separated values of python module names) to load,
 # usually to register additional checkers.
+# load-plugins=
 load-plugins=pylint.extensions.docparams
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
+# Minimum Python version to use for version dependent checks. Will default to
+# the version used to run pylint.
+py-version=3.11
+
+# Discover python modules and packages in the file system subtree.
+# recursive=no
+recursive=yes
+
 # When enabled, pylint would attempt to guess common misconfiguration and emit
 # user-friendly hints instead of false-positive error messages.
 suggestion-mode=yes
 
 # Allow loading of arbitrary C extensions. Extensions are imported into the
 # active Python interpreter and may run arbitrary code.
 unsafe-load-any-extension=no
 
+# In verbose mode, extra non-checker-related info will be displayed.
+#verbose=
+
+
+[REPORTS]
+
+# Python expression which should return a score less than or equal to 10. You
+# have access to the variables 'fatal', 'error', 'warning', 'refactor',
+# 'convention', and 'info' which contain the number of messages in each
+# category, as well as 'statement' which is the total number of statements
+# analyzed. This score is used by the global evaluation report (RP0004).
+evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
+
+# Template used to display messages. This is a python new-style format string
+# used to format the message information. See doc for all details.
+msg-template=
+
+# Set the output format. Available formats are text, parseable, colorized, json
+# and msvs (visual studio). You can also give a reporter class, e.g.
+# mypackage.mymodule.MyReporterClass.
+#output-format=
+
+# Tells whether to display a full report or only the messages.
+reports=no
+
+# Activate the evaluation score.
+# score=yes
+score=no
+
 
 [MESSAGES CONTROL]
 
 # Only show warnings with the listed confidence levels. Leave empty to show
-# all. Valid levels: HIGH, INFERENCE, INFERENCE_FAILURE, UNDEFINED.
-confidence=
+# all. Valid levels: HIGH, CONTROL_FLOW, INFERENCE, INFERENCE_FAILURE,
+# UNDEFINED.
+confidence=HIGH,
+           CONTROL_FLOW,
+           INFERENCE,
+           INFERENCE_FAILURE,
+           UNDEFINED
 
 # Disable the message, report, category or checker with the given id(s). You
 # can either give multiple identifiers separated by comma (,) or put this
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once). You can also use "--disable=all" to
-# disable everything first and then reenable specific checks. For example, if
+# disable everything first and then re-enable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use "--disable=all --enable=classes
 # --disable=W".
 disable=assignment-from-none,
         bad-inline-option,
+        consider-using-f-string,
         deprecated-pragma,
         duplicate-code,
-        eq-without-hash,
         file-ignored,
         fixme,
         locally-disabled,
-        locally-enabled,
         logging-format-interpolation,
-        metaclass-assignment,
+        logging-fstring-interpolation,
         missing-param-doc,
-        no-absolute-import,
-        no-self-use,
-        parameter-unpacking,
         raise-missing-from,
         raw-checker-failed,
         super-with-arguments,
         suppressed-message,
         too-few-public-methods,
         too-many-ancestors,
         too-many-boolean-expressions,
@@ -115,51 +184,14 @@
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=c-extension-no-member
 
 
-[REPORTS]
-
-# Python expression which should return a score less than or equal to 10. You
-# have access to the variables 'error', 'warning', 'refactor', and 'convention'
-# which contain the number of messages in each category, as well as 'statement'
-# which is the total number of statements analyzed. This score is used by the
-# global evaluation report (RP0004).
-evaluation=10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10)
-
-# Template used to display messages. This is a python new-style format string
-# used to format the message information. See doc for all details.
-#msg-template=
-
-# Set the output format. Available formats are text, parseable, colorized, json
-# and msvs (visual studio). You can also give a reporter class, e.g.
-# mypackage.mymodule.MyReporterClass.
-output-format=text
-
-# Tells whether to display a full report or only the messages.
-reports=no
-
-# Activate the evaluation score.
-score=no
-
-
-[REFACTORING]
-
-# Maximum number of nested blocks for function / method body
-max-nested-blocks=5
-
-# Complete name of functions that never returns. When checking for
-# inconsistent-return-statements if a never returning function is called then
-# it will be considered as an explicit return statement and no message will be
-# printed.
-never-returning-functions=sys.exit,argparse.parse_error
-
-
 [VARIABLES]
 
 # List of additional names supposed to be defined in builtins. Remember that
 # you should avoid defining new builtins when possible.
 additional-builtins=
 
 # Tells whether unused global variables should be treated as a violation.
@@ -197,53 +229,52 @@
 contextmanager-decorators=contextlib.contextmanager
 
 # List of members which are set dynamically and missed by pylint inference
 # system, and so shouldn't trigger E1101 when accessed. Python regular
 # expressions are accepted.
 generated-members=
 
-# Tells whether missing members accessed in mixin class should be ignored. A
-# mixin class is detected if its name ends with "mixin" (case insensitive).
-ignore-mixin-members=yes
-
 # Tells whether to warn about missing members when the owner of the attribute
 # is inferred to be None.
 ignore-none=yes
 
 # This flag controls whether pylint should warn about no-member and similar
 # checks whenever an opaque object is returned when inferring. The inference
 # can return multiple potential results while evaluating a Python object, but
 # some branches might not be evaluated, which results in partial inference. In
 # that case, it might be useful to still emit no-member and other checks for
 # the rest of the inferred objects.
 ignore-on-opaque-inference=yes
 
+# List of symbolic message names to ignore for Mixin members.
+ignored-checks-for-mixins=no-member,
+                          not-async-context-manager,
+                          not-context-manager,
+                          attribute-defined-outside-init
+
 # List of class names for which member attributes should not be checked (useful
 # for classes with dynamically set attributes). This supports the use of
 # qualified names.
-ignored-classes=optparse.Values,thread._local,_thread._local
-
-# List of module names for which member attributes should not be checked
-# (useful for modules/projects where namespaces are manipulated during runtime
-# and thus existing member attributes cannot be deduced by static analysis). It
-# supports qualified module names, as well as Unix pattern matching.
-ignored-modules=
+ignored-classes=optparse.Values,thread._local,_thread._local,argparse.Namespace
 
 # Show a hint with possible names when a member name was not found. The aspect
 # of finding the hint is based on edit distance.
 missing-member-hint=yes
 
 # The minimum edit distance a name should have in order to be considered a
 # similar match for a missing member name.
 missing-member-hint-distance=1
 
 # The total number of similar names that should be taken in consideration when
 # showing a hint for a missing member.
 missing-member-max-choices=1
 
+# Regex pattern to define which classes are considered mixins.
+mixin-class-rgx=.*[Mm]ixin
+
 # List of decorators that change the signature of a decorated function.
 signature-mutators=
 
 
 [LOGGING]
 
 # The type of string formatting that logging methods do. `old` means using %
@@ -251,28 +282,74 @@
 logging-format-style=old
 
 # Logging modules to check that the string format arguments are in logging
 # function parameter format.
 logging-modules=logging
 
 
+[DESIGN]
+
+# List of regular expressions of class ancestor names to ignore when counting
+# public methods (see R0903)
+exclude-too-few-public-methods=
+
+# List of qualified class names to ignore when counting class parents (see
+# R0901)
+ignored-parents=
+
+# Maximum number of arguments for function / method.
+# max-args=5
+max-args=10
+
+# Maximum number of attributes for a class (see R0902).
+max-attributes=7
+
+# Maximum number of boolean expressions in an if statement (see R0916).
+max-bool-expr=5
+
+# Maximum number of branch for function / method body.
+max-branches=12
+
+# Maximum number of locals for function / method body.
+max-locals=15
+
+# Maximum number of parents for a class (see R0901).
+max-parents=7
+
+# Maximum number of public methods for a class (see R0904).
+max-public-methods=20
+
+# Maximum number of return / yield for function / method body.
+max-returns=6
+
+# Maximum number of statements in function / method body.
+max-statements=50
+
+# Minimum number of public methods for a class (see R0903).
+min-public-methods=2
+
+
 [BASIC]
 
 # Naming style matching correct argument names.
 argument-naming-style=snake_case
 
 # Regular expression matching correct argument names. Overrides argument-
-# naming-style.
+# naming-style. If left empty, argument names will be checked with the set
+# naming style.
+#argument-rgx=
 argument-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 # Naming style matching correct attribute names.
 attr-naming-style=snake_case
 
 # Regular expression matching correct attribute names. Overrides attr-naming-
+# style. If left empty, attribute names will be checked with the set naming
 # style.
+#attr-rgx=
 attr-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma.
 bad-names=foo,
           bar,
           baz,
           toto,
@@ -283,47 +360,55 @@
 # they will always be refused
 bad-names-rgxs=
 
 # Naming style matching correct class attribute names.
 class-attribute-naming-style=any
 
 # Regular expression matching correct class attribute names. Overrides class-
-# attribute-naming-style.
+# attribute-naming-style. If left empty, class attribute names will be checked
+# with the set naming style.
+#class-attribute-rgx=
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]*|(__.*__))$
 
 # Naming style matching correct class constant names.
 class-const-naming-style=UPPER_CASE
 
 # Regular expression matching correct class constant names. Overrides class-
-# const-naming-style.
+# const-naming-style. If left empty, class constant names will be checked with
+# the set naming style.
 #class-const-rgx=
 
 # Naming style matching correct class names.
 class-naming-style=PascalCase
 
 # Regular expression matching correct class names. Overrides class-naming-
-# style.
+# style. If left empty, class names will be checked with the set naming style.
+#class-rgx=
 class-rgx=[A-Z_][a-zA-Z0-9]+$
 
 # Naming style matching correct constant names.
 const-naming-style=UPPER_CASE
 
 # Regular expression matching correct constant names. Overrides const-naming-
+# style. If left empty, constant names will be checked with the set naming
 # style.
+#const-rgx=
 const-rgx=(([a-zA-Z_][a-zA-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
 # Naming style matching correct function names.
 function-naming-style=snake_case
 
 # Regular expression matching correct function names. Overrides function-
-# naming-style.
+# naming-style. If left empty, function names will be checked with the set
+# naming style.
+#function-rgx=
 function-rgx=[A-Z_][a-zA-Z0-9_]*$
 
 # Good variable names which should always be accepted, separated by a comma.
 good-names=i,
            j,
            k,
            ex,
@@ -337,29 +422,33 @@
 # Include a hint for the correct naming format with invalid-name.
 include-naming-hint=no
 
 # Naming style matching correct inline iteration names.
 inlinevar-naming-style=any
 
 # Regular expression matching correct inline iteration names. Overrides
-# inlinevar-naming-style.
+# inlinevar-naming-style. If left empty, inline iteration names will be checked
+# with the set naming style.
+#inlinevar-rgx=
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
 # Naming style matching correct method names.
 method-naming-style=snake_case
 
 # Regular expression matching correct method names. Overrides method-naming-
-# style.
+# style. If left empty, method names will be checked with the set naming style.
+#method-rgx=
 method-rgx=(test|[A-Z_])[a-zA-Z0-9_]*$
 
 # Naming style matching correct module names.
 module-naming-style=snake_case
 
 # Regular expression matching correct module names. Overrides module-naming-
-# style.
+# style. If left empty, module names will be checked with the set naming style.
+#module-rgx=
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
 # Regular expression which should only match function or class names that do
@@ -367,31 +456,70 @@
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 # These decorators are taken in consideration only for invalid-name.
 property-classes=abc.abstractproperty
 
+# Regular expression matching correct type variable names. If left empty, type
+# variable names will be checked with the set naming style.
+#typevar-rgx=
+
 # Naming style matching correct variable names.
 variable-naming-style=snake_case
 
 # Regular expression matching correct variable names. Overrides variable-
-# naming-style.
+# naming-style. If left empty, variable names will be checked with the set
+# naming style.
+#variable-rgx=
 variable-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 
+[EXCEPTIONS]
+
+# Exceptions that will emit a warning when caught.
+overgeneral-exceptions=BaseException,
+                       Exception
+
+
+[CLASSES]
+
+# Warn about protected attribute access inside special methods
+check-protected-access-in-special-methods=no
+
+# List of method names used to declare (i.e. assign) instance attributes.
+defining-attr-methods=__init__,
+                      __new__,
+                      setUp,
+                      __post_init__
+
+# List of member names, which should be excluded from the protected access
+# warning.
+exclude-protected=_asdict,
+                  _fields,
+                  _replace,
+                  _source,
+                  _make
+
+# List of valid names for the first argument in a class method.
+valid-classmethod-first-arg=cls
+
+# List of valid names for the first argument in a metaclass class method.
+valid-metaclass-classmethod-first-arg=cls
+
+
 [MISCELLANEOUS]
 
 # List of note tags to take in consideration, separated by a comma.
 notes=FIXME,
       XXX,
       TODO
 
 # Regular expression of note tags to take in consideration.
-#notes-rgx=
+notes-rgx=
 
 
 [FORMAT]
 
 # Expected format of line ending, e.g. empty (any line ending), LF or CRLF.
 expected-line-ending-format=
 
@@ -399,17 +527,19 @@
 ignore-long-lines=^\s*(# )?<?https?://\S+>?$
 
 # Number of spaces of indent required inside a hanging or continued line.
 indent-after-paren=4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
+# indent-string='    '
 indent-string='  '
 
 # Maximum number of characters on a single line.
+# max-line-length=100
 max-line-length=80
 
 # Maximum number of lines in a module.
 max-module-lines=1000
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
@@ -431,15 +561,15 @@
 # (hunspell), en_IE (hunspell), en_IN (hunspell), en_JM (hunspell), en_MW
 # (hunspell), en_NA (hunspell), en_NG (hunspell), en_NZ (hunspell), en_PH
 # (hunspell), en_SG (hunspell), en_TT (hunspell), en_US (hunspell), en_ZA
 # (hunspell), en_ZM (hunspell), en_ZW (hunspell).
 spelling-dict=
 
 # List of comma separated words that should be considered directives if they
-# appear and the beginning of a comment and should not be checked.
+# appear at the beginning of a comment and should not be checked.
 spelling-ignore-comment-directives=fmt: on,fmt: off,noqa:,noqa,nosec,isort:skip,mypy:
 
 # List of comma separated words that should not be checked.
 spelling-ignore-words=
 
 # A path to a file that contains the private dictionary; one word per line.
 spelling-private-dict-file=
@@ -447,25 +577,25 @@
 # Tells whether to store unknown words to the private dictionary (see the
 # --spelling-private-dict-file option) instead of raising a message.
 spelling-store-unknown-words=no
 
 
 [SIMILARITIES]
 
-# Ignore comments when computing similarities.
+# Comments are removed from the similarity computation
 ignore-comments=yes
 
-# Ignore docstrings when computing similarities.
+# Docstrings are removed from the similarity computation
 ignore-docstrings=yes
 
-# Ignore imports when computing similarities.
-ignore-imports=no
+# Imports are removed from the similarity computation
+ignore-imports=yes
 
-# Ignore function signatures when computing similarities.
-ignore-signatures=no
+# Signatures are removed from the similarity computation
+ignore-signatures=yes
 
 # Minimum lines number of a similarity.
 min-similarity-lines=4
 
 
 [STRING]
 
@@ -474,89 +604,25 @@
 check-quote-consistency=no
 
 # This flag controls whether the implicit-str-concat should generate a warning
 # on implicit string concatenation in sequences defined over several lines.
 check-str-concat-over-line-jumps=no
 
 
-[DESIGN]
-
-# Maximum number of arguments for function / method.
-max-args=10
-
-# Maximum number of attributes for a class (see R0902).
-max-attributes=7
-
-# Maximum number of boolean expressions in an if statement (see R0916).
-max-bool-expr=5
-
-# Maximum number of branch for function / method body.
-max-branches=12
-
-# Maximum number of locals for function / method body.
-max-locals=15
-
-# Maximum number of parents for a class (see R0901).
-max-parents=7
-
-# Maximum number of public methods for a class (see R0904).
-max-public-methods=20
-
-# Maximum number of return / yield for function / method body.
-max-returns=6
-
-# Maximum number of statements in function / method body.
-max-statements=50
-
-# Minimum number of public methods for a class (see R0903).
-min-public-methods=2
-
-
-[CLASSES]
-
-# Warn about protected attribute access inside special methods
-check-protected-access-in-special-methods=no
-
-# List of method names used to declare (i.e. assign) instance attributes.
-defining-attr-methods=__init__,
-                      __new__,
-                      setUp,
-                      __post_init__
-
-# List of member names, which should be excluded from the protected access
-# warning.
-exclude-protected=_asdict,
-                  _fields,
-                  _replace,
-                  _source,
-                  _make
-
-# List of valid names for the first argument in a class method.
-valid-classmethod-first-arg=cls
-
-# List of valid names for the first argument in a metaclass class method.
-valid-metaclass-classmethod-first-arg=cls
-
-
 [IMPORTS]
 
 # List of modules that can be imported at any level, not just the top level
 # one.
 allow-any-import-level=
 
 # Allow wildcard imports from modules that define __all__.
 allow-wildcard-with-all=no
 
-# Analyse import fallback blocks. This can be used to support both Python 2 and
-# 3 compatible code, which means that the block might have code that exists
-# only in one or another interpreter, leading to false positives when analysed.
-analyse-fallback-blocks=no
-
 # Deprecated modules which should not be used, separated by a comma.
-deprecated-modules=optparse,tkinter.tix
+deprecated-modules=
 
 # Output a graph (.gv or any supported image format) of external dependencies
 # to the given file (report RP0402 must not be disabled).
 ext-import-graph=
 
 # Output a graph (.gv or any supported image format) of all (i.e. internal and
 # external) dependencies to the given file (report RP0402 must not be
@@ -574,13 +640,17 @@
 # Force import order to recognize a module as part of a third party library.
 known-third-party=enchant
 
 # Couples of modules and preferred modules, separated by a comma.
 preferred-modules=
 
 
-[EXCEPTIONS]
+[REFACTORING]
 
-# Exceptions that will emit a warning when being caught. Defaults to
-# "BaseException, Exception".
-overgeneral-exceptions=BaseException,
-                       Exception
+# Maximum number of nested blocks for function / method body
+max-nested-blocks=5
+
+# Complete name of functions that never returns. When checking for
+# inconsistent-return-statements if a never returning function is called then
+# it will be considered as an explicit return statement and no message will be
+# printed.
+never-returning-functions=sys.exit,argparse.parse_error
```

### Comparing `dfimagetools-20220312/LICENSE` & `dfimagetools-20230409/LICENSE`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/MANIFEST.in` & `dfimagetools-20230409/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/MANIFEST.test_data.in` & `dfimagetools-20230409/MANIFEST.test_data.in`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/PKG-INFO` & `dfimagetools-20230409/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dfimagetools
-Version: 20220312
+Version: 20230409
 Summary: Storage media image tools
 Home-page: https://github.com/log2timeline/dfimagetools
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Description-Content-Type: text/plain
 License-File: LICENSE
 
 Collection of tools to process storage media images.
-
```

### Comparing `dfimagetools-20220312/appveyor.yml` & `dfimagetools-20230409/appveyor.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 environment:
   matrix:
-  - DESCRIPTION: "Windows with 32-bit Python 3.10"
+  - DESCRIPTION: "Windows with 32-bit Python 3.11"
     MACHINE_TYPE: "x86"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
-  - DESCRIPTION: "Windows with 64-bit Python 3.10"
+  - DESCRIPTION: "Windows with 64-bit Python 3.11"
     MACHINE_TYPE: "amd64"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310-x64"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311-x64"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
-  - DESCRIPTION: "Mac OS with Python 3.10"
-    APPVEYOR_BUILD_WORKER_IMAGE: macos
+  - DESCRIPTION: "Mac OS with Python 3.11"
+    APPVEYOR_BUILD_WORKER_IMAGE: macos-monterey
     HOMEBREW_NO_INSTALL_CLEANUP: 1
 
 install:
 - cmd: "%PYTHON%\\python.exe -m pip install -U pip setuptools twine wheel"
 - cmd: "%PYTHON%\\python.exe -m pip install pywin32 WMI"
 - cmd: "%PYTHON%\\python.exe %PYTHON%\\Scripts\\pywin32_postinstall.py -install"
 - ps: If ($isWindows) { .\config\appveyor\install.ps1 }
 - sh: config/appveyor/install.sh
 
 build_script:
-# Note that bdist_msi will change the version number to work-around limitations
-# of the MSI version version numbering. Hence a MSI build is done separately
-# from building the wheel to not influence its version number.
-- cmd: "%PYTHON%\\python.exe setup.py bdist_msi"
 - cmd: "%PYTHON%\\python.exe setup.py bdist_wheel"
 
 test_script:
 - cmd: "%PYTHON%\\python.exe run_tests.py"
 - cmd: IF EXIST "tests\\end-to-end.py" (
     set PYTHONPATH=. &&
     "%PYTHON%\\python.exe" "tests\\end-to-end.py" --debug -c "config\\end-to-end.ini" )
```

### Comparing `dfimagetools-20220312/config/appveyor/install.ps1` & `dfimagetools-20230409/config/appveyor/install.ps1`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Script to set up tests on AppVeyor Windows.
 
-$Dependencies = "PyYAML artifacts cffi cryptography dfdatetime dfvfs dfwinreg dtfabric idna libbde libcreg libewf libfsapfs libfsext libfshfs libfsntfs libfsxfs libfvde libfwnt libluksde libmodi libphdi libqcow libregf libsigscan libsmdev libsmraw libvhdi libvmdk libvsgpt libvshadow libvslvm mock pbr pytsk3 six xattr"
-$Dependencies = ${Dependencies} -split " "
+$Dependencies = "PyYAML artifacts cffi cryptography dfdatetime dfvfs dfwinreg dtfabric idna libbde libcreg libewf libfsapfs libfsext libfsfat libfshfs libfsntfs libfsxfs libfvde libfwnt libluksde libmodi libphdi libqcow libregf libsigscan libsmdev libsmraw libvhdi libvmdk libvsgpt libvshadow libvslvm pytsk3 xattr"
 
-$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1"
-Write-Host (${Output} | Out-String)
-
-If ($env:APPVEYOR_REPO_BRANCH -eq "main")
-{
-	$Track = "stable"
-}
-Else
+If ($Dependencies.Length -gt 0)
 {
-	$Track = $env:APPVEYOR_REPO_BRANCH
-}
-New-Item -ItemType "directory" -Name "dependencies"
+	$Dependencies = ${Dependencies} -split " "
 
-$env:PYTHONPATH = "..\l2tdevtools"
+	$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1 | %{ '$_' }"
+	Write-Host (${Output} | Out-String)
 
-$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1"
-Write-Host (${Output} | Out-String)
+	If ($env:APPVEYOR_REPO_BRANCH -eq "main")
+	{
+		$Track = "stable"
+	}
+	Else
+	{
+		$Track = $env:APPVEYOR_REPO_BRANCH
+	}
+	New-Item -ItemType "directory" -Name "dependencies"
+
+	$env:PYTHONPATH = "..\l2tdevtools"
+
+	$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1"
+	Write-Host (${Output} | Out-String)
+}
```

### Comparing `dfimagetools-20220312/config/dpkg/control` & `dfimagetools-20230409/config/dpkg/control`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Build-Depends: debhelper (>= 9), dh-python, python3-all (>= 3.6~), python3-setuptools
 Standards-Version: 4.1.4
 X-Python3-Version: >= 3.6
 Homepage: https://github.com/log2timeline/dfimagetools
 
 Package: python3-dfimagetools
 Architecture: all
-Depends: libbde-python3 (>= 20220121), libcreg-python3 (>= 20200725), libewf-python3 (>= 20131210), libfsapfs-python3 (>= 20201107), libfsext-python3 (>= 20220112), libfshfs-python3 (>= 20220115), libfsntfs-python3 (>= 20211229), libfsxfs-python3 (>= 20220113), libfvde-python3 (>= 20220121), libfwnt-python3 (>= 20210717), libluksde-python3 (>= 20220121), libmodi-python3 (>= 20210405), libphdi-python3 (>= 20220110), libqcow-python3 (>= 20201213), libregf-python3 (>= 20180303), libsigscan-python3 (>= 20191221), libsmdev-python3 (>= 20140529), libsmraw-python3 (>= 20140612), libvhdi-python3 (>= 20201014), libvmdk-python3 (>= 20140421), libvsgpt-python3 (>= 20211115), libvshadow-python3 (>= 20160109), libvslvm-python3 (>= 20160109), python3-artifacts (>= 20220219), python3-cffi-backend (>= 1.9.1), python3-cryptography (>= 2.0.2), python3-dfdatetime (>= 20211113), python3-dfvfs (>= 20220121), python3-dfwinreg (>= 20201002), python3-dtfabric (>= 20170524), python3-idna (>= 2.5), python3-pytsk3 (>= 20210419), python3-pyxattr (>= 0.7.2), python3-yaml (>= 3.10), ${misc:Depends}
+Depends: libbde-python3 (>= 20220121), libcreg-python3 (>= 20200725), libewf-python3 (>= 20131210), libfsapfs-python3 (>= 20220709), libfsext-python3 (>= 20220829), libfsfat-python3 (>= 20220816), libfshfs-python3 (>= 20220831), libfsntfs-python3 (>= 20211229), libfsxfs-python3 (>= 20220829), libfvde-python3 (>= 20220121), libfwnt-python3 (>= 20210717), libluksde-python3 (>= 20220121), libmodi-python3 (>= 20210405), libphdi-python3 (>= 20220228), libqcow-python3 (>= 20201213), libregf-python3 (>= 20201002), libsigscan-python3 (>= 20191221), libsmdev-python3 (>= 20140529), libsmraw-python3 (>= 20140612), libvhdi-python3 (>= 20201014), libvmdk-python3 (>= 20140421), libvsgpt-python3 (>= 20211115), libvshadow-python3 (>= 20160109), libvslvm-python3 (>= 20160109), python3-artifacts (>= 20220219), python3-cffi-backend (>= 1.9.1), python3-cryptography (>= 2.0.2), python3-dfdatetime (>= 20220816), python3-dfvfs (>= 20220831), python3-dfwinreg (>= 20211207), python3-dtfabric (>= 20220219), python3-idna (>= 2.5), python3-pytsk3 (>= 20210419), python3-pyxattr (>= 0.7.2), python3-yaml (>= 3.10), ${misc:Depends}
 Description: Python 3 module of dfImageTools
  Collection of tools to process storage media images.
 
 Package: dfimagetools-tools
 Architecture: all
 Depends: python3-dfimagetools (>= ${binary:Version}), ${misc:Depends}
 Description: Tools of dfImageTools
```

### Comparing `dfimagetools-20220312/config/dpkg/copyright` & `dfimagetools-20230409/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/dependencies.ini` & `dfimagetools-20230409/dependencies.ini`

 * *Files 2% similar despite different names*

```diff
@@ -15,33 +15,33 @@
 dpkg_name: python3-cryptography
 minimum_version: 2.0.2
 rpm_name: python3-cryptography
 version_property: __version__
 
 [dfdatetime]
 dpkg_name: python3-dfdatetime
-minimum_version: 20211113
+minimum_version: 20220816
 rpm_name: python3-dfdatetime
 version_property: __version__
 
 [dfvfs]
 dpkg_name: python3-dfvfs
-minimum_version: 20220121
+minimum_version: 20220831
 rpm_name: python3-dfvfs
 version_property: __version__
 
 [dfwinreg]
 dpkg_name: python3-dfwinreg
-minimum_version: 20201002
+minimum_version: 20211207
 rpm_name: python3-dfwinreg
 version_property: __version__
 
 [dtfabric]
 dpkg_name: python3-dtfabric
-minimum_version: 20170524
+minimum_version: 20220219
 rpm_name: python3-dtfabric
 version_property: __version__
 
 [idna]
 skip_check: true
 skip_requires: true
 dpkg_name: python3-idna
@@ -72,31 +72,39 @@
 pypi_name: libewf-python
 rpm_name: libewf-python3
 version_property: get_version()
 
 [pyfsapfs]
 dpkg_name: libfsapfs-python3
 l2tbinaries_name: libfsapfs
-minimum_version: 20201107
+minimum_version: 20220709
 pypi_name: libfsapfs-python
 rpm_name: libfsapfs-python3
 version_property: get_version()
 
 [pyfsext]
 dpkg_name: libfsext-python3
 l2tbinaries_name: libfsext
-minimum_version: 20220112
+minimum_version: 20220829
 pypi_name: libfsext-python
 rpm_name: libfsext-python3
 version_property: get_version()
 
+[pyfsfat]
+dpkg_name: libfsfat-python3
+l2tbinaries_name: libfsfat
+minimum_version: 20220816
+pypi_name: libfsfat-python
+rpm_name: libfsfat-python3
+version_property: get_version()
+
 [pyfshfs]
 dpkg_name: libfshfs-python3
 l2tbinaries_name: libfshfs
-minimum_version: 20220115
+minimum_version: 20220831
 pypi_name: libfshfs-python
 rpm_name: libfshfs-python3
 version_property: get_version()
 
 [pyfsntfs]
 dpkg_name: libfsntfs-python3
 l2tbinaries_name: libfsntfs
@@ -104,15 +112,15 @@
 pypi_name: libfsntfs-python
 rpm_name: libfsntfs-python3
 version_property: get_version()
 
 [pyfsxfs]
 dpkg_name: libfsxfs-python3
 l2tbinaries_name: libfsxfs
-minimum_version: 20220113
+minimum_version: 20220829
 pypi_name: libfsxfs-python
 rpm_name: libfsxfs-python3
 version_property: get_version()
 
 [pyfvde]
 dpkg_name: libfvde-python3
 l2tbinaries_name: libfvde
@@ -144,15 +152,15 @@
 pypi_name: libmodi-python
 rpm_name: libmodi-python3
 version_property: get_version()
 
 [pyphdi]
 dpkg_name: libphdi-python3
 l2tbinaries_name: libphdi
-minimum_version: 20220110
+minimum_version: 20220228
 pypi_name: libphdi-python
 rpm_name: libphdi-python3
 version_property: get_version()
 
 [pyqcow]
 dpkg_name: libqcow-python3
 l2tbinaries_name: libqcow
@@ -160,15 +168,15 @@
 pypi_name: libqcow-python
 rpm_name: libqcow-python3
 version_property: get_version()
 
 [pyregf]
 dpkg_name: libregf-python3
 l2tbinaries_name: libregf
-minimum_version: 20180303
+minimum_version: 20201002
 pypi_name: libregf-python
 rpm_name: libregf-python3
 version_property: get_version()
 
 [pysigscan]
 dpkg_name: libsigscan-python3
 l2tbinaries_name: libsigscan
```

### Comparing `dfimagetools-20220312/dfimagetools/artifact_filters.py` & `dfimagetools-20230409/dfimagetools/artifact_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,29 +38,29 @@
       dfvfs.FindSpec: file system (dfVFS) find specification.
     """
     definition = self._artifacts_registry.GetDefinitionByName(name)
     if not definition:
       definition = self._artifacts_registry.GetDefinitionByAlias(name)
 
     if not definition:
-      logging.warning('Undefined artifact definition: {0:s}'.format(name))
+      logging.warning(f'Undefined artifact definition: {name:s}')
     else:
       for source in definition.sources:
         source_type = source.type_indicator
         if source_type not in (
             artifacts_definitions.TYPE_INDICATOR_ARTIFACT_GROUP,
             artifacts_definitions.TYPE_INDICATOR_DIRECTORY,
             artifacts_definitions.TYPE_INDICATOR_FILE,
             artifacts_definitions.TYPE_INDICATOR_PATH):
           continue
 
         if source_type == artifacts_definitions.TYPE_INDICATOR_DIRECTORY:
           logging.warning((
-              'Use of deprecated source type: directory in artifact '
-              'definition: {0:s}').format(name))
+              f'Use of deprecated source type: directory in artifact '
+              f'definition: {name:s}'))
 
         if source_type == artifacts_definitions.TYPE_INDICATOR_ARTIFACT_GROUP:
           for source_name in set(source.names):
             for find_spec in self._BuildFindSpecsFromArtifactDefinition(
                 source_name):
               yield find_spec
 
@@ -98,16 +98,16 @@
 
         try:
           find_spec = dfvfs_file_system_searcher.FindSpec(
               case_sensitive=False, location_glob=path,
               location_separator=path_separator)
         except ValueError as exception:
           logging.error((
-              'Unable to build find specification for path: "{0:s}" with '
-              'error: {1!s}').format(path, exception))
+              f'Unable to build find specification for path: "{path:s}" with '
+              f'error: {exception!s}'))
           continue
 
         yield find_spec
 
   def GetFindSpecs(self, names):
     """Retrieves find specifications for one or more artifact definitions.
```

### Comparing `dfimagetools-20220312/dfimagetools/bodyfile.py` & `dfimagetools-20230409/dfimagetools/bodyfile.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,56 +14,62 @@
 
   _ESCAPE_CHARACTERS = {
       '/': '\\/',
       ':': '\\:',
       '\\': '\\\\',
       '|': '\\|'}
   _ESCAPE_CHARACTERS.update({
-      value: '\\x{0:02x}'.format(value)
-      for value in _NON_PRINTABLE_CHARACTERS})
+      value: f'\\x{value:02x}' for value in _NON_PRINTABLE_CHARACTERS})
 
   _FILE_TYPES = {
       0x1000: 'p',
       0x2000: 'c',
       0x4000: 'd',
       0x6000: 'b',
       0xa000: 'l',
       0xc000: 's'}
 
   _FILE_ATTRIBUTE_READONLY = 1
+  _FILE_ATTRIBUTE_HIDDEN = 2
   _FILE_ATTRIBUTE_SYSTEM = 4
 
   _TIMESTAMP_FORMAT_STRINGS = {
       dfdatetime_definitions.PRECISION_1_NANOSECOND: '{0:d}.{1:09d}',
+      dfdatetime_definitions.PRECISION_10_NANOSECONDS: '{0:d}.{1:08d}',
       dfdatetime_definitions.PRECISION_100_NANOSECONDS: '{0:d}.{1:07d}',
       dfdatetime_definitions.PRECISION_1_MICROSECOND: '{0:d}.{1:06d}',
-      dfdatetime_definitions.PRECISION_1_MILLISECOND: '{0:d}.{1:03d}'}
+      dfdatetime_definitions.PRECISION_10_MICROSECONDS: '{0:d}.{1:05d}',
+      dfdatetime_definitions.PRECISION_100_MICROSECONDS: '{0:d}.{1:04d}',
+      dfdatetime_definitions.PRECISION_1_MILLISECOND: '{0:d}.{1:03d}',
+      dfdatetime_definitions.PRECISION_10_MILLISECONDS: '{0:d}.{1:02d}',
+      dfdatetime_definitions.PRECISION_100_MILLISECONDS: '{0:d}.{1:01d}'}
 
   def __init__(self):
     """Initializes a bodyfile generator."""
     super(BodyfileGenerator, self).__init__()
     self._bodyfile_escape_characters = str.maketrans(self._ESCAPE_CHARACTERS)
+    self._root_file_entry_identifier = None
 
   def _GetFileAttributeFlagsString(self, file_type, file_attribute_flags):
     """Retrieves a bodyfile string representation of file attributes flags.
 
     Args:
       file_type (str): bodyfile file type identifier.
       file_attribute_flags (int): file attribute flags.
 
     Returns:
       str: bodyfile representation of the file attributes flags.
     """
-    string_parts = [file_type, 'r', '-', 'x', 'r', '-', 'x', 'r', '-', 'x']
+    string_parts = [file_type, 'r', 'w', 'x', 'r', 'w', 'x', 'r', 'w', 'x']
 
-    if (not file_attribute_flags & self._FILE_ATTRIBUTE_READONLY and
-        not file_attribute_flags & self._FILE_ATTRIBUTE_SYSTEM):
-      string_parts[2] = 'w'
-      string_parts[5] = 'w'
-      string_parts[8] = 'w'
+    if (file_attribute_flags & self._FILE_ATTRIBUTE_READONLY or
+        file_attribute_flags & self._FILE_ATTRIBUTE_SYSTEM):
+      string_parts[2] = '-'
+      string_parts[5] = '-'
+      string_parts[8] = '-'
 
     return ''.join(string_parts)
 
   def _GetModeString(self, mode):
     """Retrieves a bodyfile string representation of a mode.
 
     Args:
@@ -125,35 +131,43 @@
       path_segments (str): path segments of the full path of the file entry.
 
     Yields:
       str: bodyfile entry.
     """
     file_attribute_flags = None
     parent_file_reference = None
-    if file_entry.type_indicator == dfvfs_definitions.TYPE_INDICATOR_NTFS:
+    if file_entry.type_indicator == dfvfs_definitions.TYPE_INDICATOR_FAT:
+      fsfat_file_entry = file_entry.GetFATFileEntry()
+      file_attribute_flags = fsfat_file_entry.file_attribute_flags
+
+    elif file_entry.type_indicator == dfvfs_definitions.TYPE_INDICATOR_NTFS:
       mft_attribute_index = getattr(file_entry.path_spec, 'mft_attribute', None)
       if mft_attribute_index is not None:
         fsntfs_file_entry = file_entry.GetNTFSFileEntry()
         file_attribute_flags = fsntfs_file_entry.file_attribute_flags
         parent_file_reference = (
             fsntfs_file_entry.get_parent_file_reference_by_attribute_index(
                 mft_attribute_index))
 
     stat_attribute = file_entry.GetStatAttribute()
 
     if stat_attribute.inode_number is None:
       inode_string = ''
+    elif file_entry.type_indicator == dfvfs_definitions.TYPE_INDICATOR_FAT:
+      inode_string = f'0x{stat_attribute.inode_number:x}'
     elif file_entry.type_indicator == dfvfs_definitions.TYPE_INDICATOR_NTFS:
-      inode_string = '{0:d}-{1:d}'.format(
-          stat_attribute.inode_number & 0xffffffffffff,
-          stat_attribute.inode_number >> 48)
+      mft_entry_number = stat_attribute.inode_number & 0xffffffffffff
+      mft_sequence_number = stat_attribute.inode_number >> 48
+      inode_string = f'{mft_entry_number:d}-{mft_sequence_number:d}'
     else:
-      inode_string = '{0:d}'.format(stat_attribute.inode_number)
+      inode_string = f'{stat_attribute.inode_number:d}'
 
-    if file_entry.type_indicator != dfvfs_definitions.TYPE_INDICATOR_NTFS:
+    if file_entry.type_indicator not in (
+        dfvfs_definitions.TYPE_INDICATOR_FAT,
+        dfvfs_definitions.TYPE_INDICATOR_NTFS):
       mode = getattr(stat_attribute, 'mode', None) or 0
       mode_string = self._GetModeString(mode)
 
     else:
       if file_entry.entry_type == dfvfs_definitions.FILE_ENTRY_TYPE_DIRECTORY:
         file_type = 'd'
       elif file_entry.entry_type == dfvfs_definitions.FILE_ENTRY_TYPE_LINK:
@@ -186,21 +200,28 @@
     md5_string = '0'
 
     path_segments = [
         segment.translate(self._bodyfile_escape_characters)
         for segment in path_segments]
     file_entry_name_value = '/'.join(path_segments) or '/'
 
-    if file_entry.link:
-      file_entry_link = file_entry.link.translate(
-          self._bodyfile_escape_characters)
-      name_value = '{0:s} -> {1:s}'.format(
-          file_entry_name_value, file_entry_link)
-    else:
+    if not file_entry.link:
       name_value = file_entry_name_value
+    else:
+      if file_entry.type_indicator in (
+          dfvfs_definitions.TYPE_INDICATOR_FAT,
+          dfvfs_definitions.TYPE_INDICATOR_NTFS):
+        path_segments = file_entry.link.split('\\')
+      else:
+        path_segments = file_entry.link.split('/')
+
+      file_entry_link = '/'.join([
+          segment.translate(self._bodyfile_escape_characters)
+          for segment in path_segments])
+      name_value = ' -> '.join([file_entry_name_value, file_entry_link])
 
     yield '|'.join([
         md5_string, name_value, inode_string, mode_string, owner_identifier,
         group_identifier, size, access_time, modification_time, change_time,
         creation_time])
 
     for data_stream in file_entry.data_streams:
@@ -215,16 +236,16 @@
             owner_identifier, group_identifier, size, access_time,
             modification_time, change_time, creation_time])
 
     for attribute in file_entry.attributes:
       if isinstance(attribute, dfvfs_ntfs_attribute.FileNameNTFSAttribute):
         if (attribute.name == file_entry.name and
             attribute.parent_file_reference == parent_file_reference):
-          attribute_name_value = '{0:s} ($FILE_NAME)'.format(
-              file_entry_name_value)
+          attribute_name_value = ' '.join([
+              file_entry_name_value, '($FILE_NAME)'])
 
           access_time = self._GetTimestamp(attribute.access_time)
           creation_time = self._GetTimestamp(attribute.creation_time)
           change_time = self._GetTimestamp(attribute.entry_modification_time)
           modification_time = self._GetTimestamp(attribute.modification_time)
 
           yield '|'.join([
```

### Comparing `dfimagetools-20220312/dfimagetools/data_stream_writer.py` & `dfimagetools-20230409/dfimagetools/data_stream_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
   _ESCAPE_CHARACTERS = {
       '/': '\\/',
       ':': '\\:',
       '\\': '\\\\',
       '|': '\\|'}
   _ESCAPE_CHARACTERS.update({
-      value: '\\x{0:02x}'.format(value)
-      for value in _NON_PRINTABLE_CHARACTERS})
+      value: f'\\x{value:02x}' for value in _NON_PRINTABLE_CHARACTERS})
 
   _INVALID_PATH_CHARACTERS = [
       os.path.sep, '!', '$', '%', '&', '*', '+', ':', ';', '<', '>', '?', '@',
       '|', '~']
   _INVALID_PATH_CHARACTERS.extend(_NON_PRINTABLE_CHARACTERS)
 
   def __init__(self):
```

### Comparing `dfimagetools-20220312/dfimagetools/decorators.py` & `dfimagetools-20230409/dfimagetools/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 
 def deprecated(function):  # pylint: disable=invalid-name
   """Decorator to mark functions or methods as deprecated."""
 
   def IssueDeprecationWarning(*args, **kwargs):
     """Issue a deprecation warning."""
     warnings.simplefilter('default', DeprecationWarning)
-    warnings.warn('Call to deprecated function: {0:s}.'.format(
-        function.__name__), category=DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        f'Call to deprecated function: {function.__name__:s}.',
+        category=DeprecationWarning, stacklevel=2)
 
     return function(*args, **kwargs)
 
   IssueDeprecationWarning.__name__ = function.__name__
   IssueDeprecationWarning.__doc__ = function.__doc__
   IssueDeprecationWarning.__dict__.update(function.__dict__)
   return IssueDeprecationWarning
```

### Comparing `dfimagetools-20220312/dfimagetools/environment_variables.py` & `dfimagetools-20230409/dfimagetools/environment_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,17 @@
       registry_key (dfwinreg.WinRegistryKey): environment Windows Registry
           key.
 
     Yields:
       EnvironmentVariable: an environment variable.
     """
     for registry_value in registry_key.GetValues():
-      environment_variable_name = '%{0:s}%'.format(registry_value.name)
       value_string = registry_value.GetDataAsObject()
       yield resources.EnvironmentVariable(
-          case_sensitive=False, name=environment_variable_name,
+          case_sensitive=False, name=f'%{registry_value.name:s}%',
           value=value_string)
 
   def _CollectEnvironmentVariablesWithMappings(self, registry_key, mappings):
     """Collects environment variables.
 
     Args:
       registry_key (dfwinreg.WinRegistryKey): Windows Registry key.
```

### Comparing `dfimagetools-20220312/dfimagetools/file_entry_lister.py` & `dfimagetools-20230409/dfimagetools/file_entry_lister.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 from dfvfs.helpers import volume_scanner
 from dfvfs.helpers import windows_path_resolver
 from dfvfs.lib import definitions as dfvfs_definitions
 from dfvfs.path import factory as dfvfs_path_spec_factory
 from dfvfs.resolver import resolver as dfvfs_resolver
 from dfvfs.volume import factory as dfvfs_volume_system_factory
 
-from dfimagetools import bodyfile
-from dfimagetools import decorators
-
 
 class FileEntryLister(volume_scanner.VolumeScanner):
   """File entry lister."""
 
   _UNICODE_SURROGATES_RE = re.compile('[\ud800-\udfff]')
 
   _WINDOWS_DIRECTORIES = frozenset([
@@ -31,15 +28,14 @@
   def __init__(self, mediator=None):
     """Initializes a file entry lister.
 
     Args:
       mediator (dfvfs.VolumeScannerMediator): a volume scanner mediator.
     """
     super(FileEntryLister, self).__init__(mediator=mediator)
-    self._bodyfile_generator = bodyfile.BodyfileGenerator()
     self._list_only_files = False
 
   def _GetBasePathSegments(self, base_path_spec):
     """Retrieves the base path segments.
 
     Args:
       base_path_specs (list[dfvfs.PathSpec]): source path specification.
@@ -65,16 +61,16 @@
           dfvfs_definitions.TYPE_INDICATOR_GPT):
         volume_identifier_prefix = 'gpt'
       else:
         volume_identifier_prefix = volume_system.VOLUME_IDENTIFIER_PREFIX
 
       volume_identifier = volume.GetAttribute('identifier')
 
-      volume_path_segment = '{0:s}{{{1:s}}}'.format(
-          volume_identifier_prefix, volume_identifier.value)
+      volume_path_segment = (
+          f'{volume_identifier_prefix:s}{{{volume_identifier.value:s}}}')
       return ['', volume_path_segment]
 
     if base_path_spec.parent.type_indicator == (
         dfvfs_definitions.TYPE_INDICATOR_TSK_PARTITION):
       return base_path_spec.parent.location.split('/')
 
     return ['']
@@ -118,27 +114,14 @@
       yield file_entry, path_segments
 
     for sub_file_entry in file_entry.sub_file_entries:
       for result in self._ListFileEntry(
           file_system, sub_file_entry, path_segments):
         yield result
 
-  @decorators.deprecated
-  def GetBodyfileEntries(self, file_entry, path_segments):
-    """Retrieves bodyfile entry representations of a file entry.
-
-    Args:
-      file_entry (dfvfs.FileEntry): file entry.
-      path_segments (str): path segments of the full path of the file entry.
-
-    Returns:
-      generator[str]: bodyfile entry generator.
-    """
-    return self._bodyfile_generator.GetEntries(file_entry, path_segments)
-
   def GetWindowsDirectory(self, base_path_spec):
     """Retrieves the Windows directory from the base path specification.
 
     Args:
       base_path_spec (dfvfs.PathSpec): source path specification.
 
     Returns:
@@ -171,16 +154,17 @@
     """
     for base_path_spec in base_path_specs:
       file_system = dfvfs_resolver.Resolver.OpenFileSystem(base_path_spec)
       file_entry = dfvfs_resolver.Resolver.OpenFileEntry(base_path_spec)
       if file_entry is None:
         path_specification_string = self._GetPathSpecificationString(
             base_path_spec)
-        logging.warning('Unable to open base path specification:\n{0:s}'.format(
-            path_specification_string))
+        logging.warning(''.join([
+            'Unable to open base path specification:\n',
+            path_specification_string]))
         return
 
       base_path_segments = self._GetBasePathSegments(base_path_spec)
       for result in self._ListFileEntry(
           file_system, file_entry, base_path_segments):
         yield result
```

### Comparing `dfimagetools-20220312/dfimagetools/helpers.py` & `dfimagetools-20230409/dfimagetools/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,18 @@
   Args:
     back_end (str): dfVFS back-end.
   """
   if back_end == 'EXT':
     dfvfs_definitions.PREFERRED_EXT_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_EXT)
 
+  elif back_end == 'FAT':
+    dfvfs_definitions.PREFERRED_FAT_BACK_END = (
+        dfvfs_definitions.TYPE_INDICATOR_FAT)
+
   elif back_end == 'GPT':
     dfvfs_definitions.PREFERRED_GPT_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_GPT)
 
   elif back_end == 'HFS':
     dfvfs_definitions.PREFERRED_HFS_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_HFS)
@@ -25,13 +29,15 @@
   elif back_end == 'NTFS':
     dfvfs_definitions.PREFERRED_NTFS_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_NTFS)
 
   elif back_end == 'TSK':
     dfvfs_definitions.PREFERRED_EXT_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_TSK)
+    dfvfs_definitions.PREFERRED_FAT_BACK_END = (
+        dfvfs_definitions.TYPE_INDICATOR_TSK)
     dfvfs_definitions.PREFERRED_GPT_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_TSK_PARTITION)
     dfvfs_definitions.PREFERRED_HFS_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_TSK)
     dfvfs_definitions.PREFERRED_NTFS_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_TSK)
```

### Comparing `dfimagetools-20220312/dfimagetools/path_resolver.py` & `dfimagetools-20230409/dfimagetools/path_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,29 +273,29 @@
         if len(path_segment) == 2:
           recursion_depth = 10
         else:
           try:
             recursion_depth = int(path_segment[2:], 10)
           except (TypeError, ValueError):
             logging.warning((
-                'Globstar with suffix "{0:s}" in path "{1:s}" not '
-                'supported.').format(path_segment, path))
+                f'Globstar with suffix "{path_segment:s}" in path "{path:s}" '
+                f'not supported.'))
 
       elif '**' in path_segment:
         logging.warning((
-            'Globstar with prefix "{0:s}" in path "{1:s}" not '
-            'supported.').format(path_segment, path))
+            f'Globstar with prefix "{path_segment:s}" in path "{path:s}" not '
+            f'supported.'))
 
       if recursion_depth is not None:
         if (recursion_depth <= 1 or
             recursion_depth > self._GLOBSTAR_RECURSION_LIMIT):
           logging.warning((
-              'Globstar "{0:s}" in path "{1:s}" exceed recursion maximum '
-              'recursion depth, limiting to: {2:d}.').format(
-                  path_segment, path, self._GLOBSTAR_RECURSION_LIMIT))
+              f'Globstar "{path_segment:s}" in path "{path:s}" exceeds '
+              f'recursion maximum recursion depth, limiting to: '
+              f'{self._GLOBSTAR_RECURSION_LIMIT:d}.'))
           recursion_depth = self._GLOBSTAR_RECURSION_LIMIT
 
         next_segment_index = segment_index + 1
         for expanded_path_segment in [
             ['*'] * depth for depth in range(1, recursion_depth + 1)]:
           expanded_path_segments = list(path_segments[:segment_index])
           expanded_path_segments.extend(expanded_path_segment)
```

### Comparing `dfimagetools-20220312/dfimagetools/resources.py` & `dfimagetools-20230409/dfimagetools/resources.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/dfimagetools/windows_registry.py` & `dfimagetools-20230409/dfimagetools/windows_registry.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/dfimagetools.egg-info/PKG-INFO` & `dfimagetools-20230409/dfimagetools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dfimagetools
-Version: 20220312
+Version: 20230409
 Summary: Storage media image tools
 Home-page: https://github.com/log2timeline/dfimagetools
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Description-Content-Type: text/plain
 License-File: LICENSE
 
 Collection of tools to process storage media images.
-
```

### Comparing `dfimagetools-20220312/dfimagetools.egg-info/SOURCES.txt` & `dfimagetools-20230409/dfimagetools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .pylintrc
+.yamllint.yaml
 ACKNOWLEDGEMENTS
 AUTHORS
 LICENSE
 MANIFEST.in
 MANIFEST.test_data.in
 README
 appveyor.yml
@@ -36,15 +37,17 @@
 dfimagetools/bodyfile.py
 dfimagetools/data_stream_writer.py
 dfimagetools/decorators.py
 dfimagetools/environment_variables.py
 dfimagetools/file_entry_lister.py
 dfimagetools/helpers.py
 dfimagetools/path_resolver.py
+dfimagetools/recursive_hasher.py
 dfimagetools/resources.py
+dfimagetools/source_analyzer.py
 dfimagetools/windows_registry.py
 dfimagetools.egg-info/PKG-INFO
 dfimagetools.egg-info/SOURCES.txt
 dfimagetools.egg-info/dependency_links.txt
 dfimagetools.egg-info/requires.txt
 dfimagetools.egg-info/top_level.txt
 docs/conf.py
@@ -57,15 +60,19 @@
 docs/sources/user/index.rst
 tests/__init__.py
 tests/artifact_filters.py
 tests/bodyfile.py
 tests/environment_variables.py
 tests/file_entry_lister.py
 tests/path_resover.py
+tests/source_analyzer.py
 tests/test_lib.py
 tools/__init__.py
 tools/extract_data_streams.py
 tools/list_file_entries.py
+tools/map_extents.py
+tools/recursive_hasher.py
+tools/source_analyzer.py
 utils/__init__.py
 utils/check_dependencies.py
 utils/dependencies.py
 utils/update_release.sh
```

### Comparing `dfimagetools-20220312/dfimagetools.egg-info/requires.txt` & `dfimagetools-20230409/dfimagetools.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 pip>=7.0.0
 PyYAML>=3.10
 artifacts>=20220219
 cffi>=1.9.1
 cryptography>=2.0.2
-dfdatetime>=20211113
-dfvfs>=20220121
-dfwinreg>=20201002
-dtfabric>=20170524
+dfdatetime>=20220816
+dfvfs>=20220831
+dfwinreg>=20211207
+dtfabric>=20220219
 libbde-python>=20220121
 libcreg-python>=20200725
 libewf-python>=20131210
-libfsapfs-python>=20201107
-libfsext-python>=20220112
-libfshfs-python>=20220115
+libfsapfs-python>=20220709
+libfsext-python>=20220829
+libfsfat-python>=20220816
+libfshfs-python>=20220831
 libfsntfs-python>=20211229
-libfsxfs-python>=20220113
+libfsxfs-python>=20220829
 libfvde-python>=20220121
 libfwnt-python>=20210717
 libluksde-python>=20220121
 libmodi-python>=20210405
-libphdi-python>=20220110
+libphdi-python>=20220228
 libqcow-python>=20201213
-libregf-python>=20180303
+libregf-python>=20201002
 libsigscan-python>=20191221
 libsmdev-python>=20140529
 libsmraw-python>=20140612
 libvhdi-python>=20201014
 libvmdk-python>=20140421
 libvsgpt-python>=20211115
 libvshadow-python>=20160109
```

### Comparing `dfimagetools-20220312/docs/conf.py` & `dfimagetools-20230409/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     'sphinx.ext.viewcode',
     'sphinx_markdown_tables',
     'sphinx_rtd_theme',
 ]
 
 # We cannot install architecture dependent Python modules on readthedocs,
 # therefore we mock most imports.
-pip_installed_modules = set(['six'])
+pip_installed_modules = set()
 
 dependency_helper = utils.dependencies.DependencyHelper(
     dependencies_file=os.path.join('..', 'dependencies.ini'),
     test_dependencies_file=os.path.join('..', 'test_dependencies.ini'))
 modules_to_mock = set(dependency_helper.dependencies.keys())
 modules_to_mock = modules_to_mock.difference(pip_installed_modules)
```

### Comparing `dfimagetools-20220312/docs/index.rst` & `dfimagetools-20230409/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/docs/sources/Bodyfile-format.md` & `dfimagetools-20230409/docs/sources/Bodyfile-format.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,44 @@
 The bodyfile (or body file) format is an output format, as far as known,
 introduced by the SleuthKit. SleuthKit tools such as fls or ils, use a
 bodyfile for intermediate storage. These bodyfiles are then provided as
 input to the mactime tool.
 
 The bodyfile format has been adopted by many other, non-SleuthKit tools, and
 does not appear to have a strict definition. This document explains
-the implementation used by the dfImageTools project.
+the implementation used by the dfImageTools and libyal projects.
 
 The dfImageTools project uses a bodyfile format that has been derived from
 the format used by SleuthKit 3.0 and later. Changes have been made to overcome
-several shortcomings of the original format.
+several shortcomings of the original format, therefore this format is also
+referred to as the extended bodyfile version 3 format.
 
-A bodyfile consists of one or more lines with 11 pipe-character ('|') delimited
-values. The [SleuthKit documentation](https://wiki.sleuthkit.org/index.php?title=Body_file)
-defines these values as:
+An extended bodyfile version 3 consists of:
+
+* one or more header comments lines
+* one or more values lines
+
+## Comment lines
+
+The [SleuthKit](https://wiki.sleuthkit.org/index.php?title=Body_file) defines
+a line that start with `#` as comment. The extended bodyfile version 3 format
+uses comment lines to identify the format and store metadata.
+
+Therefore the first line of an extended bodyfile version 3 is used to uniquely
+identify the format and must contain:
+
+```
+# extended bodyfile 3 format
+```
+
+## Values lines
+
+A values line consists of with 11 pipe-character ('|') delimited values. The
+[SleuthKit](https://wiki.sleuthkit.org/index.php?title=Body_file) defines these
+values as:
 
 ```
 MD5|name|inode|mode_as_string|UID|GID|size|atime|mtime|ctime|crtime
 ```
 
 Value | Description
 --- | ---
@@ -31,24 +52,24 @@
 GID | POSIX group identifier (GID) of the group owning the file entry. <br> Note that this value will be empty if the file system has no group identifier equivalent.
 size | Size of the data of the file entry. <br> Note that the `list_file_entries.py` script only reports the size of "regular" file entries.
 atime | File entry last access time.
 mtime | File entry last modification time.
 ctime | File entry last change (or entry modification) time.
 crtime | File entry creation time.
 
-## MD5 value
+### MD5 value
 
 The SleuthKit documentation does not define the MD5 values. From observations
 the following convention is used:
 
 * '0' if "hashing" is disabled;
 * '00000000000000000000000000000000' if "hashing" is enabled but no MD5 was calculated;
 * '[0-9a-f]{32}' if a MD5 was calculated.
 
-## Name value
+### Name value
 
 The name value typically contains a full path of the file entry, but it can also
 contain a symobolic link target using the convention:
 
 ```
 ${PATH} -> ${SYMBOLIC_LINK_TARGET}
 ```
@@ -75,24 +96,27 @@
 * U+007f (delete, non-printable)
 * U+0080 - U+009f (C1 control codes, non-printable)
 
 Paths are prefixed with a partition or volume indicator if
 the `list_file_entries.py` script is used to list multiple partitions and/or
 volumes at once.
 
-## Inode value
+### Inode value
 
 The inode value contains an unique identifier of the file entry within the file
 system, which for some file systems is the inode number.
 
-For NTFS the convention `${MFT_ENTRY}-${SEQUENCE_NUMBER}` is used instead of
-the non-portable [metadata address](https://wiki.sleuthkit.org/index.php?title=Metadata_Address)
+For the dfVFS FAT back-end the offset, relative to the start of the volume, to
+the directory entry is used.
+
+For the dfVFS NTFS back-end the convention `${MFT_ENTRY}-${SEQUENCE_NUMBER}` is
+used instead of the non-portable [metadata address](https://wiki.sleuthkit.org/index.php?title=Metadata_Address)
 used by the SleuthKit tools.
 
-## Mode_as_string value
+### Mode_as_string value
 
 The mode_as_string value contains a POSIX file mode represented as a string, for
 example 'drwxr-xr-x'.
 
 The first character represents the file entry type:
 
 * '-' to indicate a "regular" file (S_IFREG) or unknown type
@@ -107,33 +131,36 @@
 project.
 
 The remaining characters are the read, write and execute permissions for owner,
 group and other.
 
 The SleuthKit specific `[-dlr]/` prefix is not used by the dfImageTools project.
 
-### NTFS
+#### FAT and NTFS
 
-For NTFS dfImageTools uses the following approximation to generate
-a mode_as_string value.
+For the FAT and NTFS dfVFS back-end, dfImageTools uses the following approach
+to generate a mode_as_string value.
 
 The first character represents the file entry type:
 
 * '-' to indicate a "regular" file or unknown type
-* 'd' to indicate a directory, if the file entry has an \$I30 index and is not a symbolic link
-* 'l' to indicate a symbolic link, if the file entry has a \$REPARSE_POINT attribute with tag 0xa000000c
+* 'd' to indicate a directory, e.g. for NTFS if the file entry has an \$I30 index and is not a symbolic link
+* 'l' to indicate a symbolic link, e.g. for NTFS if the file entry has a \$REPARSE_POINT attribute with tag 0xa000000c
 
 The remaining characters are based on the file attribute flags and will be
 'r-xr-xr-x' if FILE_ATTRIBUTE_READONLY or FILE_ATTRIBUTE_SYSTEM is set or
 'rwxrwxrwx' otherwise.
 
-## Time values
+### Time values
 
 Time values are provided as a number of seconds since January 1, 1970 00:00:00
 (epoch) without a time zone, where negative time values predate the epoch.
 A fraction of second is provided if the original time value has a higher
 [datetime value granularity](https://dfdatetime.readthedocs.io/en/latest/sources/Date-and-time-values.html#terminology).
 
+Note that a time value of 0 represent not-set or that the original time value,
+before conversion to POSIX time, was 0.
+
 ## Also see
 
-* [Forensics wiki: Bodyfile](https://forensicswiki.xyz/wiki/index.php?title=Bodyfile)
+* [Forensics Wiki: Body file](https://forensics.wiki/body_file)
 * [SleuthKit: Body file](https://wiki.sleuthkit.org/index.php?title=Body_file)
```

### Comparing `dfimagetools-20220312/docs/sources/api/dfimagetools.rst` & `dfimagetools-20230409/docs/sources/api/dfimagetools.rst`

 * *Files 5% similar despite different names*

```diff
@@ -64,22 +64,38 @@
 ----------------------------------
 
 .. automodule:: dfimagetools.path_resolver
    :members:
    :undoc-members:
    :show-inheritance:
 
+dfimagetools.recursive\_hasher module
+-------------------------------------
+
+.. automodule:: dfimagetools.recursive_hasher
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 dfimagetools.resources module
 -----------------------------
 
 .. automodule:: dfimagetools.resources
    :members:
    :undoc-members:
    :show-inheritance:
 
+dfimagetools.source\_analyzer module
+------------------------------------
+
+.. automodule:: dfimagetools.source_analyzer
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 dfimagetools.windows\_registry module
 -------------------------------------
 
 .. automodule:: dfimagetools.windows_registry
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `dfimagetools-20220312/docs/sources/user/Installation-instructions.md` & `dfimagetools-20230409/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/requirements.txt` & `dfimagetools-20230409/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 pip >= 7.0.0
 PyYAML >= 3.10
 artifacts >= 20220219
 cffi >= 1.9.1
 cryptography >= 2.0.2
-dfdatetime >= 20211113
-dfvfs >= 20220121
-dfwinreg >= 20201002
-dtfabric >= 20170524
+dfdatetime >= 20220816
+dfvfs >= 20220831
+dfwinreg >= 20211207
+dtfabric >= 20220219
 libbde-python >= 20220121
 libcreg-python >= 20200725
 libewf-python >= 20131210
-libfsapfs-python >= 20201107
-libfsext-python >= 20220112
-libfshfs-python >= 20220115
+libfsapfs-python >= 20220709
+libfsext-python >= 20220829
+libfsfat-python >= 20220816
+libfshfs-python >= 20220831
 libfsntfs-python >= 20211229
-libfsxfs-python >= 20220113
+libfsxfs-python >= 20220829
 libfvde-python >= 20220121
 libfwnt-python >= 20210717
 libluksde-python >= 20220121
 libmodi-python >= 20210405
-libphdi-python >= 20220110
+libphdi-python >= 20220228
 libqcow-python >= 20201213
-libregf-python >= 20180303
+libregf-python >= 20201002
 libsigscan-python >= 20191221
 libsmdev-python >= 20140529
 libsmraw-python >= 20140612
 libvhdi-python >= 20201014
 libvmdk-python >= 20140421
 libvsgpt-python >= 20211115
 libvshadow-python >= 20160109
```

### Comparing `dfimagetools-20220312/run_tests.py` & `dfimagetools-20230409/run_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Change PYTHONPATH to include dependencies.
 sys.path.insert(0, '.')
 
 import utils.dependencies  # pylint: disable=wrong-import-position
 
 
 if __name__ == '__main__':
-  print('Using Python version {0!s}'.format(sys.version))
+  print(f'Using Python version {sys.version!s}')
 
   fail_unless_has_test_file = '--fail-unless-has-test-file' in sys.argv
   setattr(unittest, 'fail_unless_has_test_file', fail_unless_has_test_file)
   if fail_unless_has_test_file:
     # Remove --fail-unless-has-test-file otherwise it will conflict with
     # the argparse tests.
     sys.argv.remove('--fail-unless-has-test-file')
```

### Comparing `dfimagetools-20220312/setup.cfg` & `dfimagetools-20230409/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-license_file = LICENSE
+license_files = LICENSE
 
 [sdist]
 template = MANIFEST.in
 manifest = MANIFEST
 
 [sdist_test_data]
 template = MANIFEST.test_data.in
@@ -16,41 +16,42 @@
 	AUTHORS
 	LICENSE
 	README
 build_requires = python3-setuptools
 requires = libbde-python3 >= 20220121
 	libcreg-python3 >= 20200725
 	libewf-python3 >= 20131210
-	libfsapfs-python3 >= 20201107
-	libfsext-python3 >= 20220112
-	libfshfs-python3 >= 20220115
+	libfsapfs-python3 >= 20220709
+	libfsext-python3 >= 20220829
+	libfsfat-python3 >= 20220816
+	libfshfs-python3 >= 20220831
 	libfsntfs-python3 >= 20211229
-	libfsxfs-python3 >= 20220113
+	libfsxfs-python3 >= 20220829
 	libfvde-python3 >= 20220121
 	libfwnt-python3 >= 20210717
 	libluksde-python3 >= 20220121
 	libmodi-python3 >= 20210405
-	libphdi-python3 >= 20220110
+	libphdi-python3 >= 20220228
 	libqcow-python3 >= 20201213
-	libregf-python3 >= 20180303
+	libregf-python3 >= 20201002
 	libsigscan-python3 >= 20191221
 	libsmdev-python3 >= 20140529
 	libsmraw-python3 >= 20140612
 	libvhdi-python3 >= 20201014
 	libvmdk-python3 >= 20140421
 	libvsgpt-python3 >= 20211115
 	libvshadow-python3 >= 20160109
 	libvslvm-python3 >= 20160109
 	python3-artifacts >= 20220219
 	python3-cffi >= 1.9.1
 	python3-cryptography >= 2.0.2
-	python3-dfdatetime >= 20211113
-	python3-dfvfs >= 20220121
-	python3-dfwinreg >= 20201002
-	python3-dtfabric >= 20170524
+	python3-dfdatetime >= 20220816
+	python3-dfvfs >= 20220831
+	python3-dfwinreg >= 20211207
+	python3-dtfabric >= 20220219
 	python3-idna >= 2.5
 	python3-pytsk3 >= 20210419
 	python3-pyxattr >= 0.7.2
 	python3-pyyaml >= 3.10
 
 [bdist_wheel]
 universal = 1
```

### Comparing `dfimagetools-20220312/setup.py` & `dfimagetools-20230409/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,17 @@
 
 try:
   from setuptools.commands.sdist import sdist
 except ImportError:
   from distutils.command.sdist import sdist
 
 version_tuple = (sys.version_info[0], sys.version_info[1])
-if version_tuple < (3, 6):
-  print((
-      'Unsupported Python version: {0:s}, version 3.6 or higher '
-      'required.').format(sys.version))
+if version_tuple < (3, 7):
+  print(f'Unsupported Python version: {sys.version:s}, version 3.7 or higher '
+        f'required.')
   sys.exit(1)
 
 # Change PYTHONPATH to include dfimagetools so that we can get the version.
 sys.path.insert(0, '.')
 
 import dfimagetools  # pylint: disable=wrong-import-position
 
@@ -84,16 +83,16 @@
 
       python_spec_file = []
       for line in iter(spec_file):
         if line.startswith('Summary: '):
           summary = line[9:]
 
         elif line.startswith('BuildRequires: '):
-          line = 'BuildRequires: {0:s}-setuptools, {0:s}-devel'.format(
-              python_package)
+          line = (f'BuildRequires: {python_package:s}-setuptools, '
+                  f'{python_package:s}-devel')
 
         elif line.startswith('Requires: '):
           requires = line[10:]
           continue
 
         elif line.startswith('%description'):
           in_description = True
@@ -108,15 +107,15 @@
           if python_package == 'python3':
             line = '%py3_install'
           else:
             line = '%py2_install'
 
         elif line.startswith('%files'):
           lines = [
-              '%files -n {0:s}-%{{name}}'.format(python_package),
+              f'%files -n {python_package:s}-%{{name}}',
               '%defattr(644,root,root,755)',
               '%license LICENSE',
               '%doc ACKNOWLEDGEMENTS AUTHORS README']
 
           lines.extend([
               '%{python3_sitelib}/dfimagetools/*.py',
               '%{python3_sitelib}/dfimagetools*.egg-info/*',
@@ -127,31 +126,29 @@
 
           python_spec_file.extend(lines)
           break
 
         elif line.startswith('%prep'):
           in_description = False
 
-          python_spec_file.append(
-              '%package -n {0:s}-%{{name}}'.format(python_package))
-          python_summary = 'Python 3 module of {0:s}'.format(summary)
+          python_spec_file.append(f'%package -n {python_package:s}-%{{name}}')
+          python_summary = f'Python 3 module of {summary:s}'
 
           python_spec_file.extend([
-              'Requires: {0:s}'.format(requires),
-              'Summary: {0:s}'.format(python_summary),
+              f'Requires: {requires:s}',
+              f'Summary: {python_summary:s}',
               '',
-              '%description -n {0:s}-%{{name}}'.format(python_package)])
+              f'%description -n {python_package:s}-%{{name}}'])
 
           python_spec_file.extend(description)
 
           python_spec_file.extend([
               '%package -n %{name}-tools',
-              'Requires: {0:s}-dfimagetools >= %{{version}}'.format(
-                  python_package),
-              'Summary: Tools for {0:s}'.format(summary),
+              f'Requires: {python_package:s}-dfimagetools >= %{{version}}',
+              f'Summary: Tools for {summary:s}',
               '',
               '%description -n %{name}-tools'])
 
           python_spec_file.extend(description)
 
         elif in_description:
           # Ignore leading white lines in the description.
@@ -198,27 +195,31 @@
 
 dfimagetools_description = (
     'Storage media image tools')
 
 dfimagetools_long_description = (
     'Collection of tools to process storage media images.')
 
+command_classes = {'sdist_test_data': sdist}
+if BdistMSICommand:
+  command_classes['bdist_msi'] = BdistMSICommand
+if BdistRPMCommand:
+  command_classes['bdist_rpm'] = BdistRPMCommand
+
 setup(
     name='dfimagetools',
     version=dfimagetools.__version__,
     description=dfimagetools_description,
     long_description=dfimagetools_long_description,
+    long_description_content_type='text/plain',
     license='Apache License, Version 2.0',
     url='https://github.com/log2timeline/dfimagetools',
     maintainer='Log2Timeline maintainers',
     maintainer_email='log2timeline-maintainers@googlegroups.com',
-    cmdclass={
-        'bdist_msi': BdistMSICommand,
-        'bdist_rpm': BdistRPMCommand,
-        'sdist_test_data': sdist},
+    cmdclass=command_classes,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
     ],
     packages=find_packages('.', exclude=[
```

### Comparing `dfimagetools-20220312/tests/artifact_filters.py` & `dfimagetools-20230409/tests/artifact_filters.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/tests/bodyfile.py` & `dfimagetools-20230409/tests/bodyfile.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/tests/environment_variables.py` & `dfimagetools-20230409/tests/environment_variables.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/tests/file_entry_lister.py` & `dfimagetools-20230409/tests/file_entry_lister.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/tests/path_resover.py` & `dfimagetools-20230409/tests/path_resover.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20220312/tests/test_lib.py` & `dfimagetools-20230409/tests/test_lib.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,15 +54,15 @@
       path (str): path of a test file.
 
     Raises:
       SkipTest: if the path does not exist and the test should be skipped.
     """
     if not os.path.exists(path):
       filename = os.path.basename(path)
-      raise unittest.SkipTest('missing test file: {0:s}'.format(filename))
+      raise unittest.SkipTest(f'missing test file: {filename:s}')
 
 
 class TempDirectory(object):
   """Class that implements a temporary directory."""
 
   def __init__(self):
     """Initializes a temporary directory."""
```

### Comparing `dfimagetools-20220312/tools/extract_data_streams.py` & `dfimagetools-20230409/tools/extract_data_streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,16 +113,16 @@
   if not options.artifact_filters:
     print('[ERROR] no artifact filters were specified.')
     print('')
     return False
 
   target_path = options.target
   if not target_path:
-    target_path = '{0:s}.extracted'.format(os.path.basename(options.source))
-    target_path = os.path.join(os.getcwd(), target_path)
+    source_name = os.path.basename(options.source)
+    target_path = os.path.join(os.getcwd(), f'{source_name:s}.extracted')
 
   if not os.path.exists(target_path):
     os.makedirs(target_path)
 
   elif not os.path.isdir(target_path):
     print('[ERROR] target path is not a directory.')
     print('')
@@ -206,25 +206,24 @@
       stream_writer = data_stream_writer.DataStreamWriter()
       for file_entry, path_segments in file_entries_generator:
         for data_stream in file_entry.data_streams:
           display_path = stream_writer.GetDisplayPath(
               path_segments, data_stream.name)
           destination_path = stream_writer.GetSanitizedPath(
               path_segments, data_stream.name, target_path)
-          logging.info('Extracting: {0:s} to: {1:s}'.format(
-              display_path, destination_path))
+          logging.info(f'Extracting: {display_path:s} to: {destination_path:s}')
 
           destination_directory = os.path.dirname(destination_path)
           os.makedirs(destination_directory, exist_ok=True)
 
           stream_writer.WriteDataStream(
               file_entry, data_stream.name, destination_path)
 
   except dfvfs_errors.ScannerError as exception:
-    print('[ERROR] {0!s}'.format(exception), file=sys.stderr)
+    print(f'[ERROR] {exception!s}', file=sys.stderr)
     print('')
     return False
 
   except KeyboardInterrupt:
     print('Aborted by user.', file=sys.stderr)
     print('')
     return False
```

### Comparing `dfimagetools-20220312/tools/list_file_entries.py` & `dfimagetools-20230409/tools/list_file_entries.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     print('Source value is missing.')
     print('')
     argument_parser.print_help()
     print('')
     return False
 
   if options.output_format != 'bodyfile':
-    print('Unsupported output format: {0:s}.'.format(options.output_format))
+    print(f'Unsupported output format: {options.output_format:s}.')
     print('')
     argument_parser.print_help()
     print('')
     return False
 
   if options.artifact_filters:
     if (not options.artifact_definitions and
@@ -188,22 +188,24 @@
 
       if find_specs:
         file_entries_generator = entry_lister.ListFileEntriesWithFindSpecs(
             [base_path_spec], find_specs)
       else:
         file_entries_generator = entry_lister.ListFileEntries([base_path_spec])
 
+      print('# extended bodyfile 3 format')
+
       bodyfile_generator = bodyfile.BodyfileGenerator()
       for file_entry, path_segments in file_entries_generator:
         for bodyfile_entry in bodyfile_generator.GetEntries(
             file_entry, path_segments):
           print(bodyfile_entry)
 
   except dfvfs_errors.ScannerError as exception:
-    print('[ERROR] {0!s}'.format(exception), file=sys.stderr)
+    print(f'[ERROR] {exception!s}', file=sys.stderr)
     print('')
     return False
 
   except KeyboardInterrupt:
     print('Aborted by user.', file=sys.stderr)
     print('')
     return False
```

### Comparing `dfimagetools-20220312/tox.ini` & `dfimagetools-20230409/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 [tox]
-envlist = py3{6,7,8,9,10},coverage,docs,pylint
+envlist = py3{7,8,9,10,11},coverage,docs,lint
 
 [testenv]
+allowlist_externals = ./run_tests.py
 pip_pre = True
+passenv =
+    CFLAGS
+    CPPFLAGS
+    LDFLAGS
 setenv =
     PYTHONPATH = {toxinidir}
 deps =
     -rrequirements.txt
     -rtest_requirements.txt
     coverage: coverage
 commands =
-    py3{6,7,8,9,10}: ./run_tests.py
+    py3{7,8,9,10,11}: ./run_tests.py
     coverage: coverage erase
     coverage: coverage run --source=dfimagetools --omit="*_test*,*__init__*,*test_lib*" run_tests.py
 
 [testenv:codecov]
-skip_install = true
+skip_install = True
 passenv =
+    CFLAGS
+    CPPFLAGS
     GITHUB_ACTION
     GITHUB_HEAD_REF
     GITHUB_REF
     GITHUB_REPOSITORY
     GITHUB_RUN_ID
     GITHUB_SHA
+    LDFLAGS
 deps =
     codecov < 2.1.10
 commands =
     codecov
 
 [testenv:docs]
-usedevelop = true
+usedevelop = True
 deps =
     -rdocs/requirements.txt
 commands =
     sphinx-build -b html -d build/doctrees docs dist/docs
     sphinx-build -b linkcheck docs dist/docs
 
-[testenv:pylint]
-skipsdist=True
+[testenv:lint]
+skipsdist = True
 pip_pre = True
+passenv =
+    CFLAGS
+    CPPFLAGS
+    LDFLAGS
 setenv =
     PYTHONPATH = {toxinidir}
 deps =
     -rrequirements.txt
     -rtest_requirements.txt
-    pylint >= 2.9.0, < 2.10.0
+    pylint >= 2.14.0, < 2.15.0
+    yamllint >= 1.26.0
 commands =
     pylint --version
+    yamllint -v
     # Ignore setup.py for now due to:
     # setup.py:15:0: E0001: Cannot import 'distutils.command.bdist_msi' due to
     # syntax error 'expected an indented block (<unknown>, line 347)' (syntax-error)
     pylint --rcfile=.pylintrc dfimagetools tests tools
+    yamllint -c .yamllint.yaml test_data
```

### Comparing `dfimagetools-20220312/utils/dependencies.py` & `dfimagetools-20230409/utils/dependencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -129,20 +129,20 @@
     """
     super(DependencyHelper, self).__init__()
     self._test_dependencies = {}
     self.dependencies = {}
 
     dependency_reader = DependencyDefinitionReader()
 
-    with open(dependencies_file, 'r') as file_object:
+    with open(dependencies_file, 'r', encoding='utf-8') as file_object:
       for dependency in dependency_reader.Read(file_object):
         self.dependencies[dependency.name] = dependency
 
     if os.path.exists(test_dependencies_file):
-      with open(test_dependencies_file, 'r') as file_object:
+      with open(test_dependencies_file, 'r', encoding='utf-8') as file_object:
         for dependency in dependency_reader.Read(file_object):
           self._test_dependencies[dependency.name] = dependency
 
   def _CheckPythonModule(self, dependency):
     """Checks the availability of a Python module.
 
     Args:
@@ -153,16 +153,15 @@
 
         bool: True if the Python module is available and conforms to
             the minimum required version, False otherwise.
         str: status message.
     """
     module_object = self._ImportPythonModule(dependency.name)
     if not module_object:
-      status_message = 'missing: {0:s}'.format(dependency.name)
-      return False, status_message
+      return False, f'missing: {dependency.name:s}'
 
     if not dependency.version_property:
       return True, dependency.name
 
     return self._CheckPythonModuleVersion(
         dependency.name, module_object, dependency.version_property,
         dependency.minimum_version, dependency.maximum_version)
@@ -192,71 +191,65 @@
     else:
       version_method = getattr(
           module_object, version_property[:-2], None)
       if version_method:
         module_version = version_method()
 
     if not module_version:
-      status_message = (
-          'unable to determine version information for: {0:s}').format(
-              module_name)
-      return False, status_message
+      return False, (
+          f'unable to determine version information for: {module_name:s}')
 
     # Make sure the module version is a string.
-    module_version = '{0!s}'.format(module_version)
+    module_version = f'{module_version!s}'
 
     # Split the version string and convert every digit into an integer.
     # A string compare of both version strings will yield an incorrect result.
 
     # Strip any semantic suffixes such as a1, b1, pre, post, rc, dev.
     module_version = self._VERSION_NUMBERS_REGEX.findall(module_version)[0]
 
     if module_version[-1] == '.':
       module_version = module_version[:-1]
 
     try:
       module_version_map = list(
           map(int, self._VERSION_SPLIT_REGEX.split(module_version)))
     except ValueError:
-      status_message = 'unable to parse module version: {0:s} {1:s}'.format(
-          module_name, module_version)
-      return False, status_message
+      return False, (
+          f'unable to parse module version: {module_name:s} {module_version:s}')
 
     if minimum_version:
       try:
         minimum_version_map = list(
             map(int, self._VERSION_SPLIT_REGEX.split(minimum_version)))
       except ValueError:
-        status_message = 'unable to parse minimum version: {0:s} {1:s}'.format(
-            module_name, minimum_version)
-        return False, status_message
+        return False, (
+            f'unable to parse minimum version: {module_name:s} '
+            f'{minimum_version:s}')
 
       if module_version_map < minimum_version_map:
-        status_message = (
-            '{0:s} version: {1!s} is too old, {2!s} or later required').format(
-                module_name, module_version, minimum_version)
-        return False, status_message
+        return False, (
+            f'{module_name:s} version: {module_version!s} is too old, '
+            f'{minimum_version!s} or later required')
 
     if maximum_version:
       try:
         maximum_version_map = list(
             map(int, self._VERSION_SPLIT_REGEX.split(maximum_version)))
       except ValueError:
-        status_message = 'unable to parse maximum version: {0:s} {1:s}'.format(
-            module_name, maximum_version)
-        return False, status_message
+        return False, (
+            f'unable to parse maximum version: {module_name:s} '
+            f'{maximum_version:s}')
 
       if module_version_map > maximum_version_map:
-        status_message = (
-            '{0:s} version: {1!s} is too recent, {2!s} or earlier '
-            'required').format(module_name, module_version, maximum_version)
-        return False, status_message
+        return False, (
+            f'{module_name:s} version: {module_version!s} is too recent, '
+            f'{maximum_version!s} or earlier required')
 
-    status_message = '{0:s} version: {1!s}'.format(module_name, module_version)
-    return True, status_message
+    return True, f'{module_name:s} version: {module_version!s}'
 
   def _ImportPythonModule(self, module_name):
     """Imports a Python module.
 
     Args:
       module_name (str): name of the module.
 
@@ -288,18 +281,18 @@
     """
     if not result or dependency.is_optional:
       if dependency.is_optional:
         status_indicator = '[OPTIONAL]'
       else:
         status_indicator = '[FAILURE]'
 
-      print('{0:s}\t{1:s}'.format(status_indicator, status_message))
+      print(f'{status_indicator:s}\t{status_message:s}')
 
     elif verbose_output:
-      print('[OK]\t\t{0:s}'.format(status_message))
+      print(f'[OK]\t\t{status_message:s}')
 
   def CheckDependencies(self, verbose_output=True):
     """Checks the availability of the dependencies.
 
     Args:
       verbose_output (Optional[bool]): True if output should be verbose.
 
@@ -345,15 +338,16 @@
     for dependency in sorted(
         self._test_dependencies.values(),
         key=lambda dependency: dependency.name):
       if dependency.skip_check:
         continue
 
       result, status_message = self._CheckPythonModule(dependency)
-      if not result:
+
+      if not result and not dependency.is_optional:
         check_result = False
 
       self._PrintCheckDependencyStatus(
           dependency, result, status_message, verbose_output=verbose_output)
 
     if check_result and not verbose_output:
       print('[OK]')
```

### Comparing `dfimagetools-20220312/utils/update_release.sh` & `dfimagetools-20230409/utils/update_release.sh`

 * *Files identical despite different names*

