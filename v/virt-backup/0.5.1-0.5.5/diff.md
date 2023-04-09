# Comparing `tmp/virt-backup-0.5.1.tar.gz` & `tmp/virt-backup-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virt-backup-0.5.1.tar", last modified: Wed Jan  6 11:31:01 2021, max compression
+gzip compressed data, was "virt-backup-0.5.5.tar", last modified: Sun Apr  9 15:05:52 2023, max compression
```

## Comparing `virt-backup-0.5.1.tar` & `virt-backup-0.5.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.353861 virt-backup-0.5.1/
--rw-r--r--   0 anthony   (1000) users      (100)       33 2017-03-21 00:08:25.000000 virt-backup-0.5.1/.coveragerc
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.349861 virt-backup-0.5.1/.github/
--rw-r--r--   0 anthony   (1000) users      (100)      433 2020-03-20 19:03:02.000000 virt-backup-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 anthony   (1000) users      (100)     1102 2017-03-21 00:08:25.000000 virt-backup-0.5.1/.gitignore
--rw-r--r--   0 anthony   (1000) users      (100)      761 2021-01-06 11:17:06.000000 virt-backup-0.5.1/.travis.yml
--rw-r--r--   0 anthony   (1000) users      (100)     1507 2017-03-21 00:08:25.000000 virt-backup-0.5.1/LICENSE.mkd
--rw-r--r--   0 anthony   (1000) users      (100)      476 2021-01-06 11:31:01.353861 virt-backup-0.5.1/PKG-INFO
--rw-r--r--   0 anthony   (1000) users      (100)     5359 2021-01-06 00:00:53.000000 virt-backup-0.5.1/README.mkd
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.349861 virt-backup-0.5.1/docs/
--rw-r--r--   0 anthony   (1000) users      (100)        0 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/.gitignore
--rw-r--r--   0 anthony   (1000) users      (100)      612 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/Makefile
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.349861 virt-backup-0.5.1/docs/_static/
--rw-r--r--   0 anthony   (1000) users      (100)       40 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/_static/theme_override.css
--rw-r--r--   0 anthony   (1000) users      (100)     8184 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/backup.rst
--rw-r--r--   0 anthony   (1000) users      (100)      571 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/clean.rst
--rwxr-xr-x   0 anthony   (1000) users      (100)     2141 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/conf.py
--rw-r--r--   0 anthony   (1000) users      (100)    10590 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/config.rst
--rw-r--r--   0 anthony   (1000) users      (100)     6471 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/data_map.rst
--rw-r--r--   0 anthony   (1000) users      (100)     1890 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/index.rst
--rw-r--r--   0 anthony   (1000) users      (100)      775 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/make.bat
--rw-r--r--   0 anthony   (1000) users      (100)     7344 2021-01-06 00:00:53.000000 virt-backup-0.5.1/docs/quickstart.rst
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.349861 virt-backup-0.5.1/example/
--rw-r--r--   0 anthony   (1000) users      (100)     4092 2021-01-06 00:00:53.000000 virt-backup-0.5.1/example/config.yml
--rw-r--r--   0 anthony   (1000) users      (100)      229 2017-05-16 21:39:04.000000 virt-backup-0.5.1/example/virt-backup-clean.service
--rw-r--r--   0 anthony   (1000) users      (100)      223 2020-03-20 19:03:02.000000 virt-backup-0.5.1/pytest.ini
--rw-r--r--   0 anthony   (1000) users      (100)      720 2021-01-06 11:31:01.353861 virt-backup-0.5.1/setup.cfg
--rwxr-xr-x   0 anthony   (1000) users      (100)     1221 2021-01-06 11:26:32.000000 virt-backup-0.5.1/setup.py
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.351861 virt-backup-0.5.1/tests/
--rw-r--r--   0 anthony   (1000) users      (100)     2384 2021-01-06 00:05:28.000000 virt-backup-0.5.1/tests/conftest.py
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.351861 virt-backup-0.5.1/tests/helper/
--rw-r--r--   0 anthony   (1000) users      (100)        0 2017-03-21 00:08:25.000000 virt-backup-0.5.1/tests/helper/__init__.py
--rw-r--r--   0 anthony   (1000) users      (100)      145 2020-03-20 19:03:02.000000 virt-backup-0.5.1/tests/helper/datetime.py
--rw-r--r--   0 anthony   (1000) users      (100)     1342 2020-04-18 14:42:13.000000 virt-backup-0.5.1/tests/helper/testdomain.xml
--rw-r--r--   0 anthony   (1000) users      (100)     7511 2021-01-06 11:17:06.000000 virt-backup-0.5.1/tests/helper/virt_backup.py
--rw-r--r--   0 anthony   (1000) users      (100)     1438 2020-03-20 19:03:02.000000 virt-backup-0.5.1/tests/test_compat_layers_config.py
--rw-r--r--   0 anthony   (1000) users      (100)     5990 2021-01-06 00:00:53.000000 virt-backup-0.5.1/tests/test_compat_layers_definition.py
--rw-r--r--   0 anthony   (1000) users      (100)     6384 2021-01-06 00:00:53.000000 virt-backup-0.5.1/tests/test_compat_layers_pending_info.py
--rw-r--r--   0 anthony   (1000) users      (100)     7237 2021-01-06 00:41:04.000000 virt-backup-0.5.1/tests/test_complete_backup.py
--rw-r--r--   0 anthony   (1000) users      (100)     9791 2021-01-06 00:00:53.000000 virt-backup-0.5.1/tests/test_complete_group.py
--rw-r--r--   0 anthony   (1000) users      (100)     2229 2021-01-06 00:00:53.000000 virt-backup-0.5.1/tests/test_config.py
--rw-r--r--   0 anthony   (1000) users      (100)     1486 2021-01-06 11:17:06.000000 virt-backup-0.5.1/tests/test_domain.py
--rw-r--r--   0 anthony   (1000) users      (100)    14861 2021-01-06 00:05:28.000000 virt-backup-0.5.1/tests/test_group.py
--rw-r--r--   0 anthony   (1000) users      (100)    11788 2021-01-06 00:05:28.000000 virt-backup-0.5.1/tests/test_main.py
--rw-r--r--   0 anthony   (1000) users      (100)     6364 2020-04-16 23:11:07.000000 virt-backup-0.5.1/tests/test_packagers.py
--rw-r--r--   0 anthony   (1000) users      (100)    11455 2020-04-16 23:11:07.000000 virt-backup-0.5.1/tests/test_pending_backup.py
--rw-r--r--   0 anthony   (1000) users      (100)     7599 2021-01-06 00:00:53.000000 virt-backup-0.5.1/tests/test_snapshot.py
--rw-r--r--   0 anthony   (1000) users      (100)      818 2020-03-20 19:03:02.000000 virt-backup-0.5.1/tests/test_unsupported.py
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.351861 virt-backup-0.5.1/tests/testconfig/
--rw-r--r--   0 anthony   (1000) users      (100)      496 2020-03-20 19:03:02.000000 virt-backup-0.5.1/tests/testconfig/config.yml
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.349861 virt-backup-0.5.1/tests/testconfig/versions/
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.351861 virt-backup-0.5.1/tests/testconfig/versions/0.4/
--rw-r--r--   0 anthony   (1000) users      (100)      587 2020-03-20 19:03:02.000000 virt-backup-0.5.1/tests/testconfig/versions/0.4/post.yml
--rw-r--r--   0 anthony   (1000) users      (100)      539 2020-03-20 19:03:02.000000 virt-backup-0.5.1/tests/testconfig/versions/0.4/pre.yml
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.351861 virt-backup-0.5.1/tests/testconfig/versions/full/
--rw-r--r--   0 anthony   (1000) users      (100)      539 2020-03-20 19:03:02.000000 virt-backup-0.5.1/tests/testconfig/versions/full/0.1.yml
--rw-r--r--   0 anthony   (1000) users      (100)      587 2020-03-20 19:03:02.000000 virt-backup-0.5.1/tests/testconfig/versions/full/0.4.yml
--rw-r--r--   0 anthony   (1000) users      (100)      965 2021-01-06 11:17:06.000000 virt-backup-0.5.1/tox.ini
--rwxr-xr-x   0 anthony   (1000) users      (100)      166 2018-01-15 11:22:17.000000 virt-backup-0.5.1/virt-backup
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.351861 virt-backup-0.5.1/virt_backup/
--rw-r--r--   0 anthony   (1000) users      (100)       43 2021-01-06 11:26:32.000000 virt-backup-0.5.1/virt_backup/__init__.py
--rw-r--r--   0 anthony   (1000) users      (100)    13888 2021-01-06 00:05:28.000000 virt-backup-0.5.1/virt_backup/__main__.py
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.351861 virt-backup-0.5.1/virt_backup/backups/
--rw-r--r--   0 anthony   (1000) users      (100)     3288 2020-11-18 23:09:40.000000 virt-backup-0.5.1/virt_backup/backups/__init__.py
--rw-r--r--   0 anthony   (1000) users      (100)     5950 2021-01-06 11:17:06.000000 virt-backup-0.5.1/virt_backup/backups/complete.py
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.351861 virt-backup-0.5.1/virt_backup/backups/packagers/
--rw-r--r--   0 anthony   (1000) users      (100)     2937 2020-04-16 23:11:07.000000 virt-backup-0.5.1/virt_backup/backups/packagers/__init__.py
--rw-r--r--   0 anthony   (1000) users      (100)     2866 2020-04-16 23:11:07.000000 virt-backup-0.5.1/virt_backup/backups/packagers/directory.py
--rw-r--r--   0 anthony   (1000) users      (100)     5829 2020-04-16 23:11:07.000000 virt-backup-0.5.1/virt_backup/backups/packagers/tar.py
--rw-r--r--   0 anthony   (1000) users      (100)     1028 2020-03-20 19:03:02.000000 virt-backup-0.5.1/virt_backup/backups/packagers/unsupported.py
--rw-r--r--   0 anthony   (1000) users      (100)     4923 2020-04-16 23:11:07.000000 virt-backup-0.5.1/virt_backup/backups/packagers/zstd.py
--rw-r--r--   0 anthony   (1000) users      (100)    15319 2021-01-06 11:17:06.000000 virt-backup-0.5.1/virt_backup/backups/pending.py
--rw-r--r--   0 anthony   (1000) users      (100)    11315 2021-01-06 11:17:06.000000 virt-backup-0.5.1/virt_backup/backups/snapshot.py
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.351861 virt-backup-0.5.1/virt_backup/compat_layers/
--rw-r--r--   0 anthony   (1000) users      (100)       82 2020-03-20 19:03:02.000000 virt-backup-0.5.1/virt_backup/compat_layers/__init__.py
--rw-r--r--   0 anthony   (1000) users      (100)     2445 2020-03-20 19:03:02.000000 virt-backup-0.5.1/virt_backup/compat_layers/config.py
--rw-r--r--   0 anthony   (1000) users      (100)     2825 2020-03-20 19:03:02.000000 virt-backup-0.5.1/virt_backup/compat_layers/definition.py
--rw-r--r--   0 anthony   (1000) users      (100)      714 2020-03-20 19:03:02.000000 virt-backup-0.5.1/virt_backup/compat_layers/pending_info.py
--rw-r--r--   0 anthony   (1000) users      (100)     3100 2020-11-18 23:23:09.000000 virt-backup-0.5.1/virt_backup/config.py
--rw-r--r--   0 anthony   (1000) users      (100)     3325 2021-01-06 11:17:06.000000 virt-backup-0.5.1/virt_backup/domains.py
--rw-r--r--   0 anthony   (1000) users      (100)     2424 2020-04-16 23:11:07.000000 virt-backup-0.5.1/virt_backup/exceptions.py
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.353861 virt-backup-0.5.1/virt_backup/groups/
--rw-r--r--   0 anthony   (1000) users      (100)      239 2020-03-20 19:03:02.000000 virt-backup-0.5.1/virt_backup/groups/__init__.py
--rw-r--r--   0 anthony   (1000) users      (100)     9186 2020-12-22 23:44:25.000000 virt-backup-0.5.1/virt_backup/groups/complete.py
--rw-r--r--   0 anthony   (1000) users      (100)     4125 2021-01-06 00:00:53.000000 virt-backup-0.5.1/virt_backup/groups/pattern.py
--rw-r--r--   0 anthony   (1000) users      (100)    11018 2021-01-06 00:05:28.000000 virt-backup-0.5.1/virt_backup/groups/pending.py
--rw-r--r--   0 anthony   (1000) users      (100)      535 2020-03-20 19:03:02.000000 virt-backup-0.5.1/virt_backup/tools.py
-drwxr-xr-x   0 anthony   (1000) users      (100)        0 2021-01-06 11:31:01.351861 virt-backup-0.5.1/virt_backup.egg-info/
--rw-r--r--   0 anthony   (1000) users      (100)      476 2021-01-06 11:31:01.000000 virt-backup-0.5.1/virt_backup.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) users      (100)     2008 2021-01-06 11:31:01.000000 virt-backup-0.5.1/virt_backup.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) users      (100)        1 2021-01-06 11:31:01.000000 virt-backup-0.5.1/virt_backup.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) users      (100)       62 2021-01-06 11:31:01.000000 virt-backup-0.5.1/virt_backup.egg-info/entry_points.txt
--rw-r--r--   0 anthony   (1000) users      (100)       78 2021-01-06 11:31:01.000000 virt-backup-0.5.1/virt_backup.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) users      (100)       12 2021-01-06 11:31:01.000000 virt-backup-0.5.1/virt_backup.egg-info/top_level.txt
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.276276 virt-backup-0.5.5/
+-rw-r--r--   0 anthony   (1000) users      (100)       33 2017-03-21 00:08:25.000000 virt-backup-0.5.5/.coveragerc
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.272276 virt-backup-0.5.5/.github/
+-rw-r--r--   0 anthony   (1000) users      (100)      433 2020-03-20 19:03:02.000000 virt-backup-0.5.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 anthony   (1000) users      (100)     1102 2017-03-21 00:08:25.000000 virt-backup-0.5.5/.gitignore
+-rw-r--r--   0 anthony   (1000) users      (100)      761 2021-01-06 11:17:06.000000 virt-backup-0.5.5/.travis.yml
+-rw-r--r--   0 anthony   (1000) users      (100)     1507 2017-03-21 00:08:25.000000 virt-backup-0.5.5/LICENSE.mkd
+-rw-r--r--   0 anthony   (1000) users      (100)      463 2023-04-09 15:05:52.276276 virt-backup-0.5.5/PKG-INFO
+-rw-r--r--   0 anthony   (1000) users      (100)     5363 2023-04-09 15:02:50.000000 virt-backup-0.5.5/README.mkd
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.274276 virt-backup-0.5.5/docs/
+-rw-r--r--   0 anthony   (1000) users      (100)        0 2021-01-06 00:00:53.000000 virt-backup-0.5.5/docs/.gitignore
+-rw-r--r--   0 anthony   (1000) users      (100)      612 2021-01-06 00:00:53.000000 virt-backup-0.5.5/docs/Makefile
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.274276 virt-backup-0.5.5/docs/_static/
+-rw-r--r--   0 anthony   (1000) users      (100)       40 2021-01-06 00:00:53.000000 virt-backup-0.5.5/docs/_static/theme_override.css
+-rw-r--r--   0 anthony   (1000) users      (100)     8184 2021-01-06 00:00:53.000000 virt-backup-0.5.5/docs/backup.rst
+-rw-r--r--   0 anthony   (1000) users      (100)      571 2021-01-06 00:00:53.000000 virt-backup-0.5.5/docs/clean.rst
+-rwxr-xr-x   0 anthony   (1000) users      (100)     2141 2021-07-14 15:22:59.000000 virt-backup-0.5.5/docs/conf.py
+-rw-r--r--   0 anthony   (1000) users      (100)    10590 2021-01-06 00:00:53.000000 virt-backup-0.5.5/docs/config.rst
+-rw-r--r--   0 anthony   (1000) users      (100)     6471 2021-01-06 00:00:53.000000 virt-backup-0.5.5/docs/data_map.rst
+-rw-r--r--   0 anthony   (1000) users      (100)     1890 2021-01-06 00:00:53.000000 virt-backup-0.5.5/docs/index.rst
+-rw-r--r--   0 anthony   (1000) users      (100)      775 2021-01-06 00:00:53.000000 virt-backup-0.5.5/docs/make.bat
+-rw-r--r--   0 anthony   (1000) users      (100)     7344 2021-01-06 00:00:53.000000 virt-backup-0.5.5/docs/quickstart.rst
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.274276 virt-backup-0.5.5/example/
+-rw-r--r--   0 anthony   (1000) users      (100)     4092 2021-01-06 00:00:53.000000 virt-backup-0.5.5/example/config.yml
+-rw-r--r--   0 anthony   (1000) users      (100)      229 2017-05-16 21:39:04.000000 virt-backup-0.5.5/example/virt-backup-clean.service
+-rw-r--r--   0 anthony   (1000) users      (100)      223 2020-03-20 19:03:02.000000 virt-backup-0.5.5/pytest.ini
+-rw-r--r--   0 anthony   (1000) users      (100)      720 2023-04-09 15:05:52.278276 virt-backup-0.5.5/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) users      (100)     1209 2023-04-09 15:04:44.000000 virt-backup-0.5.5/setup.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.274276 virt-backup-0.5.5/tests/
+-rw-r--r--   0 anthony   (1000) users      (100)     2384 2021-01-06 00:05:28.000000 virt-backup-0.5.5/tests/conftest.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.274276 virt-backup-0.5.5/tests/helper/
+-rw-r--r--   0 anthony   (1000) users      (100)        0 2017-03-21 00:08:25.000000 virt-backup-0.5.5/tests/helper/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)      145 2020-03-20 19:03:02.000000 virt-backup-0.5.5/tests/helper/datetime.py
+-rw-r--r--   0 anthony   (1000) users      (100)     1342 2020-04-18 14:42:13.000000 virt-backup-0.5.5/tests/helper/testdomain.xml
+-rw-r--r--   0 anthony   (1000) users      (100)     7715 2021-07-14 15:25:12.000000 virt-backup-0.5.5/tests/helper/virt_backup.py
+-rw-r--r--   0 anthony   (1000) users      (100)     1438 2020-03-20 19:03:02.000000 virt-backup-0.5.5/tests/test_compat_layers_config.py
+-rw-r--r--   0 anthony   (1000) users      (100)     5990 2021-01-06 00:00:53.000000 virt-backup-0.5.5/tests/test_compat_layers_definition.py
+-rw-r--r--   0 anthony   (1000) users      (100)    15267 2021-07-17 12:56:04.000000 virt-backup-0.5.5/tests/test_compat_layers_pending_info.py
+-rw-r--r--   0 anthony   (1000) users      (100)     7237 2021-01-06 00:41:04.000000 virt-backup-0.5.5/tests/test_complete_backup.py
+-rw-r--r--   0 anthony   (1000) users      (100)     9791 2021-01-06 00:00:53.000000 virt-backup-0.5.5/tests/test_complete_group.py
+-rw-r--r--   0 anthony   (1000) users      (100)     2229 2021-01-06 00:00:53.000000 virt-backup-0.5.5/tests/test_config.py
+-rw-r--r--   0 anthony   (1000) users      (100)     1486 2021-01-06 11:17:06.000000 virt-backup-0.5.5/tests/test_domain.py
+-rw-r--r--   0 anthony   (1000) users      (100)    14861 2021-01-06 00:05:28.000000 virt-backup-0.5.5/tests/test_group.py
+-rw-r--r--   0 anthony   (1000) users      (100)    11790 2023-04-09 15:02:55.000000 virt-backup-0.5.5/tests/test_main.py
+-rw-r--r--   0 anthony   (1000) users      (100)     6364 2020-04-16 23:11:07.000000 virt-backup-0.5.5/tests/test_packagers.py
+-rw-r--r--   0 anthony   (1000) users      (100)    11847 2021-07-17 12:56:04.000000 virt-backup-0.5.5/tests/test_pending_backup.py
+-rw-r--r--   0 anthony   (1000) users      (100)     7642 2021-07-14 15:25:12.000000 virt-backup-0.5.5/tests/test_snapshot.py
+-rw-r--r--   0 anthony   (1000) users      (100)      818 2020-03-20 19:03:02.000000 virt-backup-0.5.5/tests/test_unsupported.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.274276 virt-backup-0.5.5/tests/testconfig/
+-rw-r--r--   0 anthony   (1000) users      (100)      496 2020-03-20 19:03:02.000000 virt-backup-0.5.5/tests/testconfig/config.yml
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.272276 virt-backup-0.5.5/tests/testconfig/versions/
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.274276 virt-backup-0.5.5/tests/testconfig/versions/0.4/
+-rw-r--r--   0 anthony   (1000) users      (100)      587 2020-03-20 19:03:02.000000 virt-backup-0.5.5/tests/testconfig/versions/0.4/post.yml
+-rw-r--r--   0 anthony   (1000) users      (100)      539 2020-03-20 19:03:02.000000 virt-backup-0.5.5/tests/testconfig/versions/0.4/pre.yml
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.274276 virt-backup-0.5.5/tests/testconfig/versions/full/
+-rw-r--r--   0 anthony   (1000) users      (100)      539 2020-03-20 19:03:02.000000 virt-backup-0.5.5/tests/testconfig/versions/full/0.1.yml
+-rw-r--r--   0 anthony   (1000) users      (100)      587 2020-03-20 19:03:02.000000 virt-backup-0.5.5/tests/testconfig/versions/full/0.4.yml
+-rw-r--r--   0 anthony   (1000) users      (100)      965 2021-01-06 11:17:06.000000 virt-backup-0.5.5/tox.ini
+-rwxr-xr-x   0 anthony   (1000) users      (100)      166 2018-01-15 11:22:17.000000 virt-backup-0.5.5/virt-backup
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.276276 virt-backup-0.5.5/virt_backup/
+-rw-r--r--   0 anthony   (1000) users      (100)       43 2023-04-09 15:04:44.000000 virt-backup-0.5.5/virt_backup/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)    14172 2023-04-09 15:02:55.000000 virt-backup-0.5.5/virt_backup/__main__.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.276276 virt-backup-0.5.5/virt_backup/backups/
+-rw-r--r--   0 anthony   (1000) users      (100)     3288 2020-11-18 23:09:40.000000 virt-backup-0.5.5/virt_backup/backups/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)     5950 2021-01-06 11:17:06.000000 virt-backup-0.5.5/virt_backup/backups/complete.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.276276 virt-backup-0.5.5/virt_backup/backups/packagers/
+-rw-r--r--   0 anthony   (1000) users      (100)     2937 2020-04-16 23:11:07.000000 virt-backup-0.5.5/virt_backup/backups/packagers/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)     2866 2020-04-16 23:11:07.000000 virt-backup-0.5.5/virt_backup/backups/packagers/directory.py
+-rw-r--r--   0 anthony   (1000) users      (100)     5923 2023-04-09 15:02:50.000000 virt-backup-0.5.5/virt_backup/backups/packagers/tar.py
+-rw-r--r--   0 anthony   (1000) users      (100)     1028 2020-03-20 19:03:02.000000 virt-backup-0.5.5/virt_backup/backups/packagers/unsupported.py
+-rw-r--r--   0 anthony   (1000) users      (100)     5017 2023-04-09 15:02:50.000000 virt-backup-0.5.5/virt_backup/backups/packagers/zstd.py
+-rw-r--r--   0 anthony   (1000) users      (100)    15506 2021-07-17 12:56:04.000000 virt-backup-0.5.5/virt_backup/backups/pending.py
+-rw-r--r--   0 anthony   (1000) users      (100)    11796 2021-07-17 12:56:04.000000 virt-backup-0.5.5/virt_backup/backups/snapshot.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.276276 virt-backup-0.5.5/virt_backup/compat_layers/
+-rw-r--r--   0 anthony   (1000) users      (100)       82 2020-03-20 19:03:02.000000 virt-backup-0.5.5/virt_backup/compat_layers/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)     2445 2020-03-20 19:03:02.000000 virt-backup-0.5.5/virt_backup/compat_layers/config.py
+-rw-r--r--   0 anthony   (1000) users      (100)     2829 2021-07-17 12:56:04.000000 virt-backup-0.5.5/virt_backup/compat_layers/definition.py
+-rw-r--r--   0 anthony   (1000) users      (100)     1672 2021-07-17 12:56:04.000000 virt-backup-0.5.5/virt_backup/compat_layers/pending_info.py
+-rw-r--r--   0 anthony   (1000) users      (100)     3121 2023-04-09 15:02:55.000000 virt-backup-0.5.5/virt_backup/config.py
+-rw-r--r--   0 anthony   (1000) users      (100)     3325 2021-12-11 17:09:14.000000 virt-backup-0.5.5/virt_backup/domains.py
+-rw-r--r--   0 anthony   (1000) users      (100)     2548 2023-04-09 15:02:50.000000 virt-backup-0.5.5/virt_backup/exceptions.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.276276 virt-backup-0.5.5/virt_backup/groups/
+-rw-r--r--   0 anthony   (1000) users      (100)      239 2020-03-20 19:03:02.000000 virt-backup-0.5.5/virt_backup/groups/__init__.py
+-rw-r--r--   0 anthony   (1000) users      (100)     9353 2023-04-09 15:02:50.000000 virt-backup-0.5.5/virt_backup/groups/complete.py
+-rw-r--r--   0 anthony   (1000) users      (100)     4125 2021-01-06 00:00:53.000000 virt-backup-0.5.5/virt_backup/groups/pattern.py
+-rw-r--r--   0 anthony   (1000) users      (100)    11022 2021-07-14 14:13:22.000000 virt-backup-0.5.5/virt_backup/groups/pending.py
+-rw-r--r--   0 anthony   (1000) users      (100)      499 2023-04-09 15:02:43.000000 virt-backup-0.5.5/virt_backup/tools.py
+drwxr-xr-x   0 anthony   (1000) users      (100)        0 2023-04-09 15:05:52.276276 virt-backup-0.5.5/virt_backup.egg-info/
+-rw-r--r--   0 anthony   (1000) users      (100)      463 2023-04-09 15:05:52.000000 virt-backup-0.5.5/virt_backup.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) users      (100)     2008 2023-04-09 15:05:52.000000 virt-backup-0.5.5/virt_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) users      (100)        1 2023-04-09 15:05:52.000000 virt-backup-0.5.5/virt_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) users      (100)       61 2023-04-09 15:05:52.000000 virt-backup-0.5.5/virt_backup.egg-info/entry_points.txt
+-rw-r--r--   0 anthony   (1000) users      (100)       69 2023-04-09 15:05:52.000000 virt-backup-0.5.5/virt_backup.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) users      (100)       12 2023-04-09 15:05:52.000000 virt-backup-0.5.5/virt_backup.egg-info/top_level.txt
```

### Comparing `virt-backup-0.5.1/.gitignore` & `virt-backup-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/.travis.yml` & `virt-backup-0.5.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/LICENSE.mkd` & `virt-backup-0.5.5/LICENSE.mkd`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/README.mkd` & `virt-backup-0.5.5/README.mkd`

 * *Files 4% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 it will list all its backups, sorted by date.
 
 ```
 $ virt-backup list -h
 usage: virt-backup list [-h] [-D domain_name] [-s] [group [group ...]]
 
 positional arguments:
-  group                 domain group to clean
+  group                 domain group to list
 
 optional arguments:
   -D domain_name, --domain domain_name
                         show list of backups for specific domain
   -a, --all             show all domains matching, even without backup
   -s, --short           short version, do not print details
 ```
@@ -129,15 +129,15 @@
 ```
 $ virt-backup restore -h
 usage: virt-backup restore [-h] [--date date] group domain target_dir
 
 positional arguments:
   group        domain group
   domain       domain name
-  target_dir   backup date
+  target_dir   destination path
 
 optional arguments:
   --date date  backup date (default: last backup)
 ```
 
 ### Clean
```

### Comparing `virt-backup-0.5.1/docs/Makefile` & `virt-backup-0.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/docs/backup.rst` & `virt-backup-0.5.5/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/docs/clean.rst` & `virt-backup-0.5.5/docs/clean.rst`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/docs/conf.py` & `virt-backup-0.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/docs/config.rst` & `virt-backup-0.5.5/docs/config.rst`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/docs/data_map.rst` & `virt-backup-0.5.5/docs/data_map.rst`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/docs/index.rst` & `virt-backup-0.5.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/docs/make.bat` & `virt-backup-0.5.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/docs/quickstart.rst` & `virt-backup-0.5.5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/example/config.yml` & `virt-backup-0.5.5/example/config.yml`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/setup.cfg` & `virt-backup-0.5.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.5.1
+current_version = 0.5.5
 commit = True
 tag = True
 
 [aliases]
 test = pytest --extras --addopts "-m 'not no_extra'"
 testmin = pytest --addopts "-m 'not extra'"
 testv = pytest --addopts "-v --durations=10 -m 'not no_extra'" --extras
```

### Comparing `virt-backup-0.5.1/setup.py` & `virt-backup-0.5.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from os import path
 from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
 setup(
     name="virt-backup",
-    version="0.5.1",
+    version="0.5.5",
 
     description="Automatic backups for libvirt",
 
     url="https://github.com/Anthony25/virt-backup",
     author="Anthony25 <Anthony Ruhier>",
     author_email="anthony.ruhier@gmail.com",
 
@@ -28,15 +28,15 @@
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: BSD License",
     ],
 
     keywords="libvirt",
     packages=find_packages(exclude=["example", "tests"]),
     install_requires=[
-        "appdirs", "argparse", "arrow", "libvirt-python", "lxml", "packaging", "PyYAML"
+        "appdirs", "arrow", "libvirt-python", "lxml", "packaging", "PyYAML"
     ],
     setup_requires=['pytest-runner', ],
     # Deepdiff: 5.0.2 forced for Python 3.5 compatibility.
     tests_require=['pytest', 'pytest-cov', "pytest-mock", "deepdiff==5.0.2"],
     extras_require={"zstd": ["zstandard"], },
     entry_points={
         'console_scripts': [
```

### Comparing `virt-backup-0.5.1/tests/conftest.py` & `virt-backup-0.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/helper/testdomain.xml` & `virt-backup-0.5.5/tests/helper/testdomain.xml`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/helper/virt_backup.py` & `virt-backup-0.5.5/tests/helper/virt_backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import uuid
 import arrow
 import libvirt
 import lxml
 import lxml.etree
 
 from virt_backup.backups import (
     DomBackup,
@@ -26,14 +27,17 @@
         Return the definition of a testing domain
         """
         return lxml.etree.tostring(self.dom_xml, pretty_print=True).decode()
 
     def ID(self):
         return self.dom_xml.get("id")
 
+    def UUID(self):
+        return self.dom_xml.get("uuid")
+
     def name(self):
         return self.dom_xml.xpath("name")[0].text
 
     def state(self):
         return self._state
 
     def isActive(self):
@@ -46,14 +50,17 @@
             elem_name = self.dom_xml.makeelement("name")
             self.dom_xml.insert(0, elem_name)
         elem_name.text = name
 
     def set_id(self, id):
         self.dom_xml.set("id", str(id))
 
+    def set_uuid(self, uuid):
+        self.dom_xml.set("uuid", uuid)
+
     def set_state(self, state_id, reason_id):
         self._state = [state_id, reason_id]
 
     def set_storage_basedir(self, basedir):
         """
         Change the basedir of all attached disks
 
@@ -104,14 +111,15 @@
 
         with open(os.path.join(CUR_PATH, "testdomain.xml")) as dom_xmlfile:
             self.dom_xml = lxml.etree.fromstring(
                 dom_xmlfile.read(), lxml.etree.XMLParser(resolve_entities=False)
             )
         self.set_id(id)
         self.set_name(name)
+        self.set_uuid(kwargs.get("uuid", str(uuid.uuid4())))
 
 
 class MockSnapshot:
     def getName(self):
         return self._name
 
     def __init__(self, name):
```

### Comparing `virt-backup-0.5.1/tests/test_compat_layers_config.py` & `virt-backup-0.5.5/tests/test_compat_layers_config.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/test_compat_layers_definition.py` & `virt-backup-0.5.5/tests/test_compat_layers_definition.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/test_complete_backup.py` & `virt-backup-0.5.5/tests/test_complete_backup.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/test_complete_group.py` & `virt-backup-0.5.5/tests/test_complete_group.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/test_config.py` & `virt-backup-0.5.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/test_domain.py` & `virt-backup-0.5.5/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/test_group.py` & `virt-backup-0.5.5/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/test_main.py` & `virt-backup-0.5.5/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     config = Config(
         defaults={
             "debug": False,
         }
     )
     config.from_dict(get_config(TESTCONF_PATH))
 
-    monkeypatch.setattr(virt_backup.__main__, "get_setup_config", lambda: config)
+    monkeypatch.setattr(virt_backup.__main__, "get_setup_config", lambda _: config)
 
     return config
 
 
 def mock_get_conn(monkeypatch, conn):
     monkeypatch.setattr(virt_backup.__main__, "get_setup_conn", lambda x: conn)
```

### Comparing `virt-backup-0.5.1/tests/test_packagers.py` & `virt-backup-0.5.5/tests/test_packagers.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/test_pending_backup.py` & `virt-backup-0.5.5/tests/test_pending_backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 
         pending_info_path = backup_dir.listdir()[0]
         pending_info = json.loads(pending_info_path.read())
 
         assert definition.items() <= pending_info.items()
         assert "snapshot" in pending_info["disks"]["vda"]
         assert "src" in pending_info["disks"]["vda"]
+        assert "type" in pending_info["disks"]["vda"]
 
     def take_snapshot_and_return_date(self, mock_domain, backup_dir, monkeypatch):
         dombkup = build_dombackup(
             dom=mock_domain, dev_disks=("vda",), backup_dir=backup_dir
         )
 
         snapshot_helper = DomExtSnapshot(
@@ -217,15 +218,20 @@
         backup_dir = tmpdir.mkdir("clean_aborted")
         dombkup = self.prepare_clean_aborted_dombkup(
             build_mock_domain, backup_dir, mocker
         )
 
         backup_dir.join("vda.qcow2").write("")
         dombkup.pending_info["disks"] = {
-            "vda": {"src": "vda.qcow2", "target": "vda.qcow2", "snapshot": "vda.snap"},
+            "vda": {
+                "src": "vda.qcow2",
+                "target": "vda.qcow2",
+                "snapshot": "vda.snap",
+                "type": "qcow2",
+            },
         }
         dombkup.pending_info["packager"] = {"type": "directory", "opts": {}}
         dombkup._dump_pending_info()
         dombkup._dump_json_definition(dombkup.definition)
         assert len(backup_dir.listdir()) == 3
 
         dombkup.clean_aborted()
@@ -240,16 +246,21 @@
         backup_dir = tmpdir.mkdir("clean_aborted")
         dombkup = self.prepare_clean_aborted_dombkup(
             build_mock_domain, backup_dir, mocker
         )
 
         backup_dir.join("vda.qcow2").write("")
         dombkup.pending_info["disks"] = {
-            "vda": {"src": "vda.qcow2", "target": "vda.qcow2", "snapshot": "vda.snap"},
-            "vdb": {"src": "vdb.qcow2", "snapshot": "vda.snap"},
+            "vda": {
+                "src": "vda.qcow2",
+                "target": "vda.qcow2",
+                "snapshot": "vda.snap",
+                "type": "qcow2",
+            },
+            "vdb": {"src": "vdb.qcow2", "snapshot": "vda.snap", "type": "qcow2"},
         }
         dombkup.pending_info["packager"] = {"type": "directory", "opts": {}}
         dombkup._dump_pending_info()
         dombkup._dump_json_definition(dombkup.definition)
         assert len(backup_dir.listdir()) == 3
 
         dombkup.clean_aborted()
@@ -264,26 +275,32 @@
         backup_dir = tmpdir.mkdir("clean_aborted")
         dombkup = self.prepare_clean_aborted_dombkup(
             build_mock_domain, backup_dir, mocker
         )
 
         backup_dir.join("vda.qcow2").write("")
         disk_infos = {
-            "vda": {"src": "vda.qcow2", "target": "vda.qcow2", "snapshot": "vda.snap"},
+            "vda": {
+                "src": "vda.qcow2",
+                "target": "vda.qcow2",
+                "snapshot": "vda.snap",
+                "type": "qcow2",
+            },
         }
         dombkup.pending_info["disks"] = disk_infos.copy()
         dombkup._dump_pending_info()
         dombkup._dump_json_definition(dombkup.definition)
 
         dombkup.clean_aborted()
         DomExtSnapshot.clean.assert_called_once_with()
         assert dombkup._ext_snapshot_helper.metadatas["disks"] == {
             "vda": {
                 "src": disk_infos["vda"]["src"],
                 "snapshot": disk_infos["vda"]["snapshot"],
+                "type": "qcow2",
             }
         }
 
     def prepare_clean_aborted_dombkup(self, mock_domain, backup_dir, mocker):
         dombkup = build_dombackup(
             dom=mock_domain, backup_dir=str(backup_dir), packager="directory"
         )
```

### Comparing `virt-backup-0.5.1/tests/test_snapshot.py` & `virt-backup-0.5.5/tests/test_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         """
         Check if metadatas contains the necessary infos
         """
         metadatas = self.start_snapshot(monkeypatch)
 
         assert len(self.snapshot_helper.disks) == len(metadatas["disks"])
         for disk in self.snapshot_helper.disks:
-            assert sorted(("snapshot", "src")) == sorted(
+            assert sorted(("snapshot", "src", "type")) == sorted(
                 metadatas["disks"][disk].keys()
             )
 
     def test_snapshot_correct_snapshot_path(self, monkeypatch):
         """
         Check if the snapshot is done is the same path as its source disk
         """
@@ -126,15 +126,15 @@
             "  </disks>\n"
             "</domainsnapshot>\n"
         )
         assert self.snapshot_helper.gen_libvirt_snapshot_xml() == expected_xml
 
     def test_manually_pivot_disk(self, build_mock_libvirtconn):
         self.snapshot_helper.conn = build_mock_libvirtconn
-        self.snapshot_helper._manually_pivot_disk("vda", "/testvda")
+        self.snapshot_helper._manually_pivot_disk("vda", "/testvda", "qcow2")
         dom_xml = self.snapshot_helper.dom.XMLDesc()
         assert self.get_src_for_disk(dom_xml, "vda") == "/testvda"
 
     def get_src_for_disk(self, dom_xml, disk):
         elem = get_xml_block_of_disk(dom_xml, disk)
         return elem.xpath("source")[0].get("file")
 
@@ -146,15 +146,15 @@
         conn._libvirt_version = 2000000
         conn._domains.append(self.snapshot_helper.dom)
 
         return self.test_manually_pivot_disk(conn)
 
     def test_manually_pivot_unexistant_disk(self):
         with pytest.raises(DiskNotFoundError):
-            self.snapshot_helper._manually_pivot_disk("sda", "/testvda")
+            self.snapshot_helper._manually_pivot_disk("sda", "/testvda", "qcow2")
 
     def test_clean_no_metadata(self):
         with pytest.raises(SnapshotNotStarted):
             self.snapshot_helper.clean()
 
     def test_clean(self, monkeypatch, tmpdir):
         snapdir = self.prepare_test_clean(monkeypatch, tmpdir)
@@ -168,15 +168,15 @@
         self.mock_pivot_mechanism(monkeypatch)
         # set the domain unactive to avoid the blockcommit
         self.snapshot_helper.dom.set_state(0, 0)
 
         self.snapshot_helper.metadatas = {
             "date": arrow.now(),
             "disks": {
-                disk: {"src": prop["src"], "snapshot": snapshots[disk]}
+                disk: {"src": prop["src"], "snapshot": snapshots[disk], "type": "qcow2"}
                 for disk, prop in self.snapshot_helper.disks.items()
             },
         }
         return tmpdir.join("snaps")
 
     def create_temp_snapshot_files(self, tmpdir):
         tmpdir = tmpdir.mkdir("snaps")
```

### Comparing `virt-backup-0.5.1/tests/test_unsupported.py` & `virt-backup-0.5.5/tests/test_unsupported.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/testconfig/versions/0.4/post.yml` & `virt-backup-0.5.5/tests/testconfig/versions/0.4/post.yml`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/testconfig/versions/0.4/pre.yml` & `virt-backup-0.5.5/tests/testconfig/versions/0.4/pre.yml`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/testconfig/versions/full/0.1.yml` & `virt-backup-0.5.5/tests/testconfig/versions/full/0.1.yml`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tests/testconfig/versions/full/0.4.yml` & `virt-backup-0.5.5/tests/testconfig/versions/full/0.4.yml`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/tox.ini` & `virt-backup-0.5.5/tox.ini`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/virt_backup/__main__.py` & `virt-backup-0.5.5/virt_backup/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     sp_restore = sp_action.add_parser("restore", help=("restore backup"))
     sp_restore.add_argument("group", metavar="group", help="domain group")
     sp_restore.add_argument("domain_name", metavar="domain", help="domain name")
     sp_restore.add_argument(
         "--date", metavar="date", help="backup date (default: last backup)"
     )
-    sp_restore.add_argument("target_dir", metavar="target_dir", help="backup date")
+    sp_restore.add_argument("target_dir", metavar="target_dir", help="destination path")
     sp_restore.set_defaults(func=restore_backup)
 
     sp_clean = sp_action.add_parser("clean", aliases=["cl"], help=("clean groups"))
     sp_clean.add_argument(
         "groups", metavar="group", type=str, nargs="*", help="domain group to clean"
     )
     sp_clean_broken_opts = sp_clean.add_mutually_exclusive_group()
@@ -69,15 +69,15 @@
         dest="no_broken",
         action="store_true",
     )
     sp_clean.set_defaults(func=clean_backups)
 
     sp_list = sp_action.add_parser("list", aliases=["ls"], help=("list groups"))
     sp_list.add_argument(
-        "groups", metavar="group", type=str, nargs="*", help="domain group to clean"
+        "groups", metavar="group", type=str, nargs="*", help="domain group to list"
     )
     sp_list.add_argument(
         "-D",
         "--domain",
         metavar="domain_name",
         dest="domains_names",
         action="append",
@@ -105,14 +105,22 @@
         "-d",
         "--debug",
         help="enable debug, verbose output",
         dest="debug",
         action="store_true",
     )
     parser.add_argument(
+        "-c",
+        "--config",
+        dest="config_path",
+        help="config path",
+        type=str,
+        default=None,
+    )
+    parser.add_argument(
         "--version", action="version", version="{} {}".format(APP_NAME, VERSION)
     )
 
     return parser
 
 
 def parse_args_and_run(parser):
@@ -145,15 +153,15 @@
         parser.print_help()
         sys.exit(1)
 
 
 def start_backups(parsed_args, *args, **kwargs):
     vir_event_loop_native_start()
 
-    config = get_setup_config()
+    config = get_setup_config(parsed_args.config_path)
     conn = get_setup_conn(config)
     callbacks_registrer = DomExtSnapshotCallbackRegistrer(conn)
 
     if config.get("groups", None):
         groups = build_all_or_selected_groups(
             config, conn, callbacks_registrer, parsed_args.groups
         )
@@ -195,15 +203,15 @@
             main_group.add_dombackup(d)
     return main_group
 
 
 def restore_backup(parsed_args, *args, **kwargs):
     vir_event_loop_native_start()
 
-    config = get_setup_config()
+    config = get_setup_config(parsed_args.config_path)
     conn = get_setup_conn(config)
     callbacks_registrer = DomExtSnapshotCallbackRegistrer(conn)
     try:
         group = next(
             get_usable_complete_groups(
                 config, [parsed_args.group], conn, callbacks_registrer
             )
@@ -237,15 +245,15 @@
     with callbacks_registrer:
         backup.restore_to(target_dir)
 
 
 def clean_backups(parsed_args, *args, **kwargs):
     vir_event_loop_native_start()
 
-    config = get_setup_config()
+    config = get_setup_config(parsed_args.config_path)
     conn = get_setup_conn(config)
     callbacks_registrer = DomExtSnapshotCallbackRegistrer(conn)
     groups = get_usable_complete_groups(
         config, parsed_args.groups, conn, callbacks_registrer
     )
 
     with callbacks_registrer:
@@ -275,15 +283,15 @@
                         g.name or "Undefined", len(g.clean_broken_backups())
                     )
                 )
 
 
 def list_groups(parsed_args, *args, **kwargs):
     vir_event_loop_native_start()
-    config = get_setup_config()
+    config = get_setup_config(parsed_args.config_path)
     conn = get_setup_conn(config)
     callbacks_registrer = DomExtSnapshotCallbackRegistrer(conn)
 
     complete_groups = {g.name: g for g in get_usable_complete_groups(config)}
     if parsed_args.groups:
         filtered_groups = {}
         for g in parsed_args.groups:
@@ -364,22 +372,22 @@
                 print(
                     "\t{}: {}".format(
                         b.date, b.get_complete_path_of(b.definition_filename)
                     )
                 )
 
 
-def get_setup_config():
+def get_setup_config(custom_path=None):
     config = Config(
         defaults={
             "debug": False,
         }
     )
     try:
-        loaded_config = get_config()
+        loaded_config = get_config(custom_path)
     except FileNotFoundError:
         sys.exit(1)
 
     compat_layers.config.convert_warn(loaded_config)
     config.from_dict(loaded_config)
     return config
```

### Comparing `virt-backup-0.5.1/virt_backup/backups/__init__.py` & `virt-backup-0.5.5/virt_backup/backups/__init__.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/virt_backup/backups/complete.py` & `virt-backup-0.5.5/virt_backup/backups/complete.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/virt_backup/backups/packagers/__init__.py` & `virt-backup-0.5.5/virt_backup/backups/packagers/__init__.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/virt_backup/backups/packagers/directory.py` & `virt-backup-0.5.5/virt_backup/backups/packagers/directory.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/virt_backup/backups/packagers/tar.py` & `virt-backup-0.5.5/virt_backup/backups/packagers/tar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import logging
 import os
 import re
 import shutil
 import tarfile
 
-from virt_backup.exceptions import CancelledError, ImageNotFoundError
+from virt_backup.exceptions import CancelledError, ImageNotFoundError, ImageFoundError
 from . import (
     _AbstractBackupPackager,
     _AbstractReadBackupPackager,
     _AbstractWriteBackupPackager,
     _opened_only,
     _closed_only,
 )
@@ -100,14 +100,16 @@
         except KeyError:
             raise ImageNotFoundError(name, self.complete_path)
 
         if not os.path.exists(target) and target.endswith("/"):
             os.makedirs(target)
         if os.path.isdir(target):
             target = os.path.join(target, name)
+        if os.path.isfile(target):
+            raise ImageFoundError(target)
 
         buffersize = 2 ** 20
         self._tarfile.fileobj.flush()
         try:
             with self._tarfile.extractfile(disk_tarinfo) as fsrc:
                 with open(target, "xb") as fdst:
                     while True:
```

### Comparing `virt-backup-0.5.1/virt_backup/backups/packagers/unsupported.py` & `virt-backup-0.5.5/virt_backup/backups/packagers/unsupported.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/virt_backup/backups/packagers/zstd.py` & `virt-backup-0.5.5/virt_backup/backups/packagers/zstd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import glob
 import logging
 import os
 import re
 import shutil
 import zstandard as zstd
 
-from virt_backup.exceptions import CancelledError, ImageNotFoundError
+from virt_backup.exceptions import CancelledError, ImageNotFoundError, ImageFoundError
 from . import (
     _AbstractBackupPackager,
     _AbstractReadBackupPackager,
     _AbstractWriteBackupPackager,
     _opened_only,
     _closed_only,
 )
@@ -78,14 +78,16 @@
         if name not in self.list():
             raise ImageNotFoundError(self.archive_path(name), self.complete_path)
 
         if not os.path.exists(target) and target.endswith("/"):
             os.makedirs(target)
         if os.path.isdir(target):
             target = os.path.join(target, name)
+        if os.path.isfile(target):
+            raise ImageFoundError(target)
 
         buffersize = 2 ** 20
         dctx = zstd.ZstdDecompressor()
         try:
             with open(self.archive_path(name), "rb") as ifh, open(target, "xb") as ofh:
                 with dctx.stream_reader(ifh) as reader:
                     while True:
```

### Comparing `virt-backup-0.5.1/virt_backup/backups/pending.py` & `virt-backup-0.5.5/virt_backup/backups/pending.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,15 @@
         definition["date"] = snapshot_metadatas["date"].int_timestamp
 
         self.pending_info = definition.copy()
         self.pending_info["disks"] = {
             disk: {
                 "src": prop["src"],
                 "snapshot": snapshot_metadatas["disks"][disk]["snapshot"],
+                "type": snapshot_metadatas["disks"][disk]["type"],
             }
             for disk, prop in self.disks.items()
         }
         self._dump_pending_info()
 
         return snapshot_metadatas["date"], definition
 
@@ -366,15 +367,19 @@
         is_ext_snap_helper_needed = (
             not self._ext_snapshot_helper and self.pending_info.get("disks", None)
         )
         if is_ext_snap_helper_needed:
             self._ext_snapshot_helper = self._get_ext_snapshot_helper()
             self._ext_snapshot_helper.metadatas = {
                 "disks": {
-                    disk: {"src": val["src"], "snapshot": val["snapshot"]}
+                    disk: {
+                        "src": val["src"],
+                        "snapshot": val["snapshot"],
+                        "type": val["type"],
+                    }
                     for disk, val in self.pending_info["disks"].items()
                 }
             }
 
         if self._ext_snapshot_helper:
             self._ext_snapshot_helper.clean()
 
@@ -405,15 +410,15 @@
         """
         Is compatible with dombackup ?
 
         If the target is the same for both dombackup and self, same thing for
         packager and packager_opts, self and dombackup are considered
         compatibles.
         """
-        same_domain = dombackup.dom.ID() == self.dom.ID()
+        same_domain = dombackup.dom.UUID() == self.dom.UUID()
         if not same_domain:
             return False
 
         attributes_to_compare = ("backup_dir", "packager")
         for a in attributes_to_compare:
             if getattr(self, a) != getattr(dombackup, a):
                 return False
```

### Comparing `virt-backup-0.5.1/virt_backup/backups/snapshot.py` & `virt-backup-0.5.5/virt_backup/backups/snapshot.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         snapshot_date = arrow.now()
 
         self.metadatas = {
             "date": snapshot_date,
             "disks": {
                 disk: {
                     "src": prop["src"],
+                    "type": self._get_disk_type(disk),
                     "snapshot": self._get_snapshot_path(prop["src"], snapshot),
                 }
                 for disk, prop in self.disks.items()
             },
         }
 
         return self.metadatas
@@ -190,14 +191,21 @@
             disks_el.append(disk_el)
 
         return lxml.etree.tostring(xml_tree, pretty_print=True).decode()
 
     def _get_snapshot_path(self, parent_disk_path, snapshot):
         return "{}.{}".format(os.path.splitext(parent_disk_path)[0], snapshot.getName())
 
+    def _get_disk_type(self, disk):
+        dom_xml = lxml.etree.fromstring(
+            self.dom.XMLDesc(), lxml.etree.XMLParser(resolve_entities=False)
+        )
+        disk_xml = get_xml_block_of_disk(dom_xml, disk)
+        return disk_xml.xpath("driver")[0].get("type", "raw")
+
     def clean(self):
         if not self.metadatas:
             raise SnapshotNotStarted()
 
         disks = tuple(self.metadatas["disks"].keys())
         snapshot_paths = tuple(
             os.path.abspath(self.metadatas["disks"][disk]["snapshot"]) for disk in disks
@@ -221,14 +229,15 @@
         if not self.metadatas:
             raise SnapshotNotStarted()
         elif disk not in self.metadatas["disks"]:
             raise DiskNotSnapshot(disk)
 
         snapshot_path = os.path.abspath(self.metadatas["disks"][disk]["snapshot"])
         disk_path = os.path.abspath(self.metadatas["disks"][disk]["src"])
+        disk_type = self.metadatas["disks"][disk]["type"]
 
         # Do not commit and pivot if our snapshot is not the current top disk
         current_disk_path = (
             get_xml_block_of_disk(self.dom.XMLDesc(), disk)
             .xpath("source")[0]
             .get("file")
         )
@@ -245,15 +254,15 @@
             )
             return
 
         if self.dom.isActive():
             self.blockcommit_disk(disk)
         else:
             self._qemu_img_commit(disk_path, snapshot_path)
-            self._manually_pivot_disk(disk, disk_path)
+            self._manually_pivot_disk(disk, disk_path, disk_type)
             os.remove(snapshot_path)
 
         self.metadatas["disks"].pop(disk)
         self._callbacks_registrer.callbacks.pop(snapshot_path, None)
 
     def blockcommit_disk(self, disk):
         """
@@ -286,15 +295,15 @@
     def _pivot_callback(self, conn, dom, snap, event_id, status, *args):
         """
         Pivot the snapshot
 
         If the received domain matches with the one associated to this backup,
         abort the blockjob, pivot it and delete the snapshot.
         """
-        domain_matches = dom.ID() == self.dom.ID()
+        domain_matches = dom.UUID() == self.dom.UUID()
         if status == libvirt.VIR_DOMAIN_BLOCK_JOB_READY and domain_matches:
             dom.blockJobAbort(snap, libvirt.VIR_DOMAIN_BLOCK_JOB_ABORT_PIVOT)
             os.remove(snap)
             self._wait_for_pivot[os.path.abspath(snap)].set()
 
     def _qemu_img_commit(self, parent_disk_path, snapshot_path):
         """
@@ -303,27 +312,28 @@
         Libvirt does not allow to blockcommit a inactive domain, so have to use
         qemu-img instead.
         """
         return subprocess.check_call(
             ("qemu-img", "commit", "-b", parent_disk_path, snapshot_path)
         )
 
-    def _manually_pivot_disk(self, disk, src):
+    def _manually_pivot_disk(self, disk, src, disk_type):
         """
         Replace the disk src
 
         :param disk: disk name
         :param src: new disk path
         """
         dom_xml = lxml.etree.fromstring(
             self.dom.XMLDesc(), lxml.etree.XMLParser(resolve_entities=False)
         )
 
         disk_xml = get_xml_block_of_disk(dom_xml, disk)
         disk_xml.xpath("source")[0].set("file", src)
+        disk_xml.xpath("driver")[0].set("type", disk_type)
 
         if self.conn.getLibVersion() >= 3000000:
             # update a disk is broken in libvirt < 3.0
             return self.dom.updateDeviceFlags(
                 lxml.etree.tostring(disk_xml).decode(),
                 libvirt.VIR_DOMAIN_AFFECT_CONFIG,
             )
```

### Comparing `virt-backup-0.5.1/virt_backup/compat_layers/config.py` & `virt-backup-0.5.5/virt_backup/compat_layers/config.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/virt_backup/compat_layers/definition.py` & `virt-backup-0.5.5/virt_backup/compat_layers/definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import yaml
 
 
 logger = logging.getLogger("virt_backup")
 
 
 def convert(definition):
-    def_version = version_parser(definition["version"])
     converters = (ToV0_4(),)
     for c in converters:
+        def_version = version_parser(definition["version"])
         if c.is_needed(def_version):
             logger.debug(
                 "definition %s needs convertion update to v%s",
                 definition.get("name") or definition["domain_name"],
                 c.from_version_to[1],
             )
             c.convert(definition)
```

### Comparing `virt-backup-0.5.1/virt_backup/config.py` & `virt-backup-0.5.5/virt_backup/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 def get_config(custom_path=None):
     """
     Get config file and load it with yaml
 
     :returns: loaded config in yaml, as a dict object
     """
+    config_path = ""
     if custom_path:
         config_path = custom_path
     else:
         for d in CONFIG_DIRS:
             config_path = os.path.join(d, CONFIG_FILENAME)
             if os.path.isfile(config_path):
                 break
```

### Comparing `virt-backup-0.5.1/virt_backup/domains.py` & `virt-backup-0.5.5/virt_backup/domains.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/virt_backup/exceptions.py` & `virt-backup-0.5.5/virt_backup/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 
 
 class ImageNotFoundError(Exception):
     def __init__(self, image, target):
         super().__init__("Image {} not found in {}".format(image, target))
 
 
+class ImageFoundError(Exception):
+    def __init__(self, image):
+        super().__init__("Image {} found".format(image))
+
+
 class DomainRunningError(Exception):
     """
     Domain is running when a task would need it to be shutdown
     """
 
     def __init__(self, domain):
         message = (
```

### Comparing `virt-backup-0.5.1/virt_backup/groups/complete.py` & `virt-backup-0.5.5/virt_backup/groups/complete.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,24 @@
     return _list_json_following_pattern_by_domain(backup_dir, "*/*.json.pending")
 
 
 def _list_json_following_pattern_by_domain(directory, glob_pattern):
     backups = {}
     for json_file in glob.glob(os.path.join(directory, glob_pattern)):
         logger.debug("{} detected".format(json_file))
-        with open(json_file, "r") as definition_file:
-            try:
-                metadata = json.load(definition_file)
-            except Exception as e:
-                logger.debug("Error for file {}: {}".format(json_file, e))
-                continue
+        try:
+            with open(json_file, "r") as definition_file:
+                try:
+                    metadata = json.load(definition_file)
+                except Exception as e:
+                    logger.debug("Error for file {}: {}".format(json_file, e))
+                    continue
+        except FileNotFoundError as e:
+            logger.warning(f"File not found or already removed: {e}")
+            continue
         domain_name = metadata["domain_name"]
         if domain_name not in backups:
             backups[domain_name] = []
         backups[domain_name].append((json_file, metadata))
     return backups
```

### Comparing `virt-backup-0.5.1/virt_backup/groups/pattern.py` & `virt-backup-0.5.5/virt_backup/groups/pattern.py`

 * *Files identical despite different names*

### Comparing `virt-backup-0.5.1/virt_backup/groups/pending.py` & `virt-backup-0.5.5/virt_backup/groups/pending.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         Search for a domain
 
         :param dom: domain to search the associated DomBackup object.
                     libvirt.virDomain object
         :returns: a generator of DomBackup matching
         """
         for backup in self.backups:
-            if backup.dom.ID() == dom.ID():
+            if backup.dom.UUID() == dom.UUID():
                 yield backup
 
     def propagate_default_backup_attr(self):
         """
         Propagate default backup attributes to all attached backups
         """
         for backup in self.backups:
```

### Comparing `virt-backup-0.5.1/virt_backup.egg-info/SOURCES.txt` & `virt-backup-0.5.5/virt_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

