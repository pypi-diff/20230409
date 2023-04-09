# Comparing `tmp/vidua-0.4.4.tar.gz` & `tmp/vidua-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidua-0.4.4.tar", last modified: Mon Feb 21 17:34:21 2022, max compression
+gzip compressed data, was "vidua-0.4.5.tar", last modified: Sun Apr  9 17:00:01 2023, max compression
```

## Comparing `vidua-0.4.4.tar` & `vidua-0.4.5.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2022-02-21 17:34:21.727537 vidua-0.4.4/
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       63 2022-02-21 06:10:18.000000 vidua-0.4.4/.coveragerc
-drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2022-02-21 17:34:21.723537 vidua-0.4.4/.github/
-drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2022-02-21 17:34:21.723537 vidua-0.4.4/.github/workflows/
--rw-rw-r--   0 tracy     (1000) tracy     (1000)     1469 2022-02-21 08:33:40.000000 vidua-0.4.4/.github/workflows/test.yml
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      157 2022-02-21 17:21:44.000000 vidua-0.4.4/.gitignore
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      127 2022-02-21 06:10:18.000000 vidua-0.4.4/.pyup.yml
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      164 2022-02-21 16:00:37.000000 vidua-0.4.4/.readthedocs.yaml
--rw-rw-r--   0 tracy     (1000) tracy     (1000)    35148 2022-02-21 06:10:18.000000 vidua-0.4.4/COPYING
--rw-rw-r--   0 tracy     (1000) tracy     (1000)     1150 2022-02-21 17:20:48.000000 vidua-0.4.4/Makefile
--rw-rw-r--   0 tracy     (1000) tracy     (1000)     2599 2022-02-21 17:34:21.727537 vidua-0.4.4/PKG-INFO
--rw-r--r--   0 tracy     (1000) tracy     (1000)     1449 2022-02-21 11:41:52.000000 vidua-0.4.4/README.md
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      105 2022-02-21 08:52:54.000000 vidua-0.4.4/bandit.yml
-drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2022-02-21 17:34:21.723537 vidua-0.4.4/docs/
--rw-r--r--   0 tracy     (1000) tracy     (1000)      602 2018-07-13 13:14:02.000000 vidua-0.4.4/docs/Makefile
--rw-r--r--   0 tracy     (1000) tracy     (1000)     1169 2022-02-21 10:44:00.000000 vidua-0.4.4/docs/bps.md
--rw-r--r--   0 tracy     (1000) tracy     (1000)     4637 2022-02-21 17:29:46.000000 vidua-0.4.4/docs/conf.py
--rw-r--r--   0 tracy     (1000) tracy     (1000)     1880 2022-02-21 11:24:58.000000 vidua-0.4.4/docs/index.rst
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       58 2022-02-21 16:00:46.000000 vidua-0.4.4/docs/requirements.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      100 2022-02-21 09:25:05.000000 vidua-0.4.4/pyproject.toml
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      122 2022-02-21 17:34:21.727537 vidua-0.4.4/setup.cfg
--rw-r--r--   0 tracy     (1000) tracy     (1000)     1120 2022-02-21 17:33:44.000000 vidua-0.4.4/setup.py
-drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2022-02-21 17:34:21.723537 vidua-0.4.4/vidua/
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       86 2022-02-21 09:02:21.000000 vidua-0.4.4/vidua/__init__.py
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       73 2022-02-21 07:32:08.000000 vidua-0.4.4/vidua/__main__.py
--rw-rw-r--   0 tracy     (1000) tracy     (1000)     9610 2022-02-21 17:24:59.000000 vidua-0.4.4/vidua/bps.py
--rw-rw-r--   0 tracy     (1000) tracy     (1000)     2730 2022-02-21 09:55:59.000000 vidua-0.4.4/vidua/ips.py
--rw-rw-r--   0 tracy     (1000) tracy     (1000)     2143 2022-02-21 09:19:08.000000 vidua-0.4.4/vidua/scripts.py
-drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2022-02-21 17:34:21.727537 vidua-0.4.4/vidua/test/
--rw-rw-r--   0 tracy     (1000) tracy     (1000)        0 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/__init__.py
-drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2022-02-21 17:34:21.727537 vidua-0.4.4/vidua/test/test_bps/
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_a.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_a_modified.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       37 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_a_original.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      135 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_b.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      148 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_b_modified.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       38 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_b_original.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)     4207 2022-02-21 17:27:09.000000 vidua-0.4.4/vidua/test/test_bps/test_bps.py
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       16 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_c.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_d.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_e.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_f.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_g.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_h.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_i.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      135 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_j.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_bps/test_k.bps
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      620 2022-02-21 07:19:24.000000 vidua-0.4.4/vidua/test/test_identify.py
-drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2022-02-21 17:34:21.727537 vidua-0.4.4/vidua/test/test_ips/
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       31 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_ips/test_a.ips
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_ips/test_a_modified.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       37 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_ips/test_a_original.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      161 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_ips/test_b.ips
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      148 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_ips/test_b_modified.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       38 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_ips/test_b_original.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      951 2022-02-21 06:10:18.000000 vidua-0.4.4/vidua/test/test_ips/test_ips.py
-drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2022-02-21 17:34:21.727537 vidua-0.4.4/vidua/test/test_scripts/
--rw-rw-r--   0 tracy     (1000) tracy     (1000)     2605 2022-02-21 08:35:32.000000 vidua-0.4.4/vidua/test/test_scripts/test_scripts.py
--rw-rw-r--   0 tracy     (1000) tracy     (1000)      822 2022-02-21 10:10:40.000000 vidua-0.4.4/vidua/util.py
-drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2022-02-21 17:34:21.727537 vidua-0.4.4/vidua.egg-info/
--rw-rw-r--   0 tracy     (1000) tracy     (1000)     2599 2022-02-21 17:34:21.000000 vidua-0.4.4/vidua.egg-info/PKG-INFO
--rw-rw-r--   0 tracy     (1000) tracy     (1000)     1368 2022-02-21 17:34:21.000000 vidua-0.4.4/vidua.egg-info/SOURCES.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)        1 2022-02-21 17:34:21.000000 vidua-0.4.4/vidua.egg-info/dependency_links.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)       46 2022-02-21 17:34:21.000000 vidua-0.4.4/vidua.egg-info/entry_points.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)        6 2022-02-21 17:34:21.000000 vidua-0.4.4/vidua.egg-info/top_level.txt
--rw-rw-r--   0 tracy     (1000) tracy     (1000)        1 2022-02-21 17:34:21.000000 vidua-0.4.4/vidua.egg-info/zip-safe
+drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2023-04-09 17:00:01.932537 vidua-0.4.5/
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       63 2022-02-21 06:10:18.000000 vidua-0.4.5/.coveragerc
+drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2023-04-09 17:00:01.928537 vidua-0.4.5/.github/
+drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2023-04-09 17:00:01.928537 vidua-0.4.5/.github/workflows/
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     1471 2023-04-09 16:54:14.000000 vidua-0.4.5/.github/workflows/test.yml
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      157 2022-02-21 17:21:44.000000 vidua-0.4.5/.gitignore
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      127 2022-02-21 06:10:18.000000 vidua-0.4.5/.pyup.yml
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      164 2022-02-21 16:00:37.000000 vidua-0.4.5/.readthedocs.yaml
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)    35148 2022-02-21 06:10:18.000000 vidua-0.4.5/COPYING
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     1150 2022-02-21 17:20:48.000000 vidua-0.4.5/Makefile
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     2085 2023-04-09 17:00:01.932537 vidua-0.4.5/PKG-INFO
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     1449 2022-02-21 11:41:52.000000 vidua-0.4.5/README.md
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      105 2022-02-21 08:52:54.000000 vidua-0.4.5/bandit.yml
+drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2023-04-09 17:00:01.928537 vidua-0.4.5/docs/
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      602 2018-07-13 13:14:02.000000 vidua-0.4.5/docs/Makefile
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     1169 2022-02-21 10:44:00.000000 vidua-0.4.5/docs/bps.md
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     4637 2022-02-21 17:29:46.000000 vidua-0.4.5/docs/conf.py
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     1880 2022-02-21 11:24:58.000000 vidua-0.4.5/docs/index.rst
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       58 2023-04-09 16:54:14.000000 vidua-0.4.5/docs/requirements.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      100 2022-02-21 09:25:05.000000 vidua-0.4.5/pyproject.toml
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      122 2023-04-09 17:00:01.932537 vidua-0.4.5/setup.cfg
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     1181 2023-04-09 16:54:14.000000 vidua-0.4.5/setup.py
+drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2023-04-09 17:00:01.932537 vidua-0.4.5/vidua/
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       86 2022-02-21 09:02:21.000000 vidua-0.4.5/vidua/__init__.py
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       73 2022-02-21 07:32:08.000000 vidua-0.4.5/vidua/__main__.py
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     9610 2022-02-21 17:24:59.000000 vidua-0.4.5/vidua/bps.py
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     2730 2022-02-21 09:55:59.000000 vidua-0.4.5/vidua/ips.py
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)        0 2023-04-09 16:54:14.000000 vidua-0.4.5/vidua/py.typed
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     2143 2022-02-21 09:19:08.000000 vidua-0.4.5/vidua/scripts.py
+drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2023-04-09 17:00:01.932537 vidua-0.4.5/vidua/test/
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)        0 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/__init__.py
+drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2023-04-09 17:00:01.932537 vidua-0.4.5/vidua/test/test_bps/
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_a.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_a_modified.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       37 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_a_original.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      135 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_b.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      148 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_b_modified.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       38 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_b_original.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     4207 2022-02-21 17:27:09.000000 vidua-0.4.5/vidua/test/test_bps/test_bps.py
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       16 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_c.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_d.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_e.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_f.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_g.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_h.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_i.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      135 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_j.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_bps/test_k.bps
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      620 2022-02-21 07:19:24.000000 vidua-0.4.5/vidua/test/test_identify.py
+drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2023-04-09 17:00:01.932537 vidua-0.4.5/vidua/test/test_ips/
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       31 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_ips/test_a.ips
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       24 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_ips/test_a_modified.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       37 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_ips/test_a_original.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      161 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_ips/test_b.ips
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      148 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_ips/test_b_modified.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       38 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_ips/test_b_original.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      951 2022-02-21 06:10:18.000000 vidua-0.4.5/vidua/test/test_ips/test_ips.py
+drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2023-04-09 17:00:01.932537 vidua-0.4.5/vidua/test/test_scripts/
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     2605 2022-02-21 08:35:32.000000 vidua-0.4.5/vidua/test/test_scripts/test_scripts.py
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)      822 2022-02-21 10:10:40.000000 vidua-0.4.5/vidua/util.py
+drwxrwxr-x   0 tracy     (1000) tracy     (1000)        0 2023-04-09 17:00:01.932537 vidua-0.4.5/vidua.egg-info/
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     2085 2023-04-09 17:00:01.000000 vidua-0.4.5/vidua.egg-info/PKG-INFO
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)     1383 2023-04-09 17:00:01.000000 vidua-0.4.5/vidua.egg-info/SOURCES.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)        1 2023-04-09 17:00:01.000000 vidua-0.4.5/vidua.egg-info/dependency_links.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)       45 2023-04-09 17:00:01.000000 vidua-0.4.5/vidua.egg-info/entry_points.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)        6 2023-04-09 17:00:01.000000 vidua-0.4.5/vidua.egg-info/top_level.txt
+-rw-rw-r--   0 tracy     (1000) tracy     (1000)        1 2023-04-09 17:00:01.000000 vidua-0.4.5/vidua.egg-info/zip-safe
```

### Comparing `vidua-0.4.4/.github/workflows/test.yml` & `vidua-0.4.5/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 on: [push]
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.5.x, 3.6.x, 3.7.x, 3.8.x, 3.9.x]
+        python-version: [3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x]
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
```

### Comparing `vidua-0.4.4/COPYING` & `vidua-0.4.5/COPYING`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/Makefile` & `vidua-0.4.5/Makefile`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/PKG-INFO` & `vidua-0.4.5/docs/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,76 @@
-Metadata-Version: 2.1
-Name: vidua
-Version: 0.4.4
-Summary: Apply patches to ROMs and other files
-Home-page: http://github.com/sopoforic/vidua
-Author: Tracy Poff
-Author-email: tracy.poff@gmail.com
-License: UNKNOWN
-Project-URL: Documentation, https://vidua.readthedocs.io/
-Project-URL: Issues, https://github.com/sopoforic/vidua/issues
-Description: # vidua
-        
-        Vidua can be used to apply (BPS or IPS) patches. It is intended particularly for use with ROM
-        hacks.
-        
-        ## Installation
-        
-        ```shell
-        pip install vidua
-        ```
-        
-        ## Usage
-        
-        A simple script is included to validate or apply patches from the command line:
-        
-        ```shell
-        vidua patch.bps original.rom patched_output.rom
-        ```
-        
-        Full usage instructions:
-        
-        ```shell
-        $ vidua --help
-        usage: vidua [-h] [-v] [-q] PATCH [ORIGINAL] [OUTPUT]
-        
-        Apply or validate patches.
-        
-        positional arguments:
-          PATCH           the patch file
-          ORIGINAL        the file to be patched
-          OUTPUT          filename to write patched file
-        
-        optional arguments:
-          -h, --help      show this help message and exit
-          -v, --validate  validate the patch only; do not apply it
-          -q, --quiet     suppress output except errors
-        ```
-        
-        Vidua may also be used as a library, to validate or apply patches from within
-        another program:
-        
-        ```python
-        from vidua import bps
-        
-        patch = open('patch.bps', 'rb')
-        original = open('original.rom', 'rb')
-        
-        with open('patched.rom', 'wb') as patched:
-            patched.write(bps.patch(original, patch).read())
-        ```
-        
-        If the file is very large, you may prefer to use `shutil.copyfileobj` when
-        writing to disk.
-        
-        ## Credits
-        
-        Alcaro's [Floating IPS](https://www.smwcentral.net/?p=section&a=details&id=11474)
-        was very useful in working out how to handle BPS files when byuu's documentation
-        was unclear.
-        
-        ![Test](https://github.com/sopoforic/vidua/actions/workflows/test.yml/badge.svg?event=push)
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
+.. vidua documentation master file, created by
+   sphinx-quickstart on Fri Jul 13 09:14:02 2018.
+   You can adapt this file completely to your liking, but it should at least
+   contain the root `toctree` directive.
+
+Welcome to vidua's documentation!
+=================================
+
+Vidua can be used to apply (IPS or BPS) patches. It is intended particularly for use with ROM
+hacks.
+
+Usage
+-----
+
+A simple script is included to validate or apply patches from the command line:
+
+.. code-block:: console
+
+    vidua patch.bps original.rom patched_output.rom
+
+Full usage instructions:
+
+.. code-block:: console
+
+    $ vidua --help
+    usage: vidua [-h] [-v] [-q] PATCH [ORIGINAL] [OUTPUT]
+    
+    Apply or validate patches.
+    
+    positional arguments:
+      PATCH           the patch file
+      ORIGINAL        the file to be patched
+      OUTPUT          filename to write patched file
+    
+    optional arguments:
+      -h, --help      show this help message and exit
+      -v, --validate  validate the patch only; do not apply it
+      -q, --quiet     suppress output except errors
+
+
+Vidua may also be used as a library, to validate or apply patches from within
+another program::
+
+    from vidua import bps
+    
+    patch = open('patch.bps', 'rb')
+    original = open('original.rom', 'rb')
+    
+    with open('patched.rom', 'wb') as patched:
+        patched.write(bps.patch(original, patch).read())
+
+
+If the file is very large, you may prefer to use :py:func:`copyfileobj <shutil.copyfileobj>` when
+writing to disk.
+
+Credits
+-------
+
+Alcaro's `Floating IPS <https://www.smwcentral.net/?p=section&a=details&id=11474>`_
+was very useful in working out how to handle BPS files when byuu's documentation
+was unclear.
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Contents:
+
+   vidua
+   bps
+
+Indices and tables
+==================
+
+* :ref:`genindex`
+* :ref:`modindex`
+* :ref:`search`
+
```

### Comparing `vidua-0.4.4/README.md` & `vidua-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/docs/Makefile` & `vidua-0.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/docs/bps.md` & `vidua-0.4.5/docs/bps.md`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/docs/conf.py` & `vidua-0.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/setup.py` & `vidua-0.4.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,17 @@
           'Development Status :: 3 - Alpha',
           'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
           'Operating System :: OS Independent',
           'Programming Language :: Python :: 3',
           'Topic :: Utilities',
       ],
       packages=['vidua'],
+      package_data={
+        'vidua': ['py.typed'],
+      },
       entry_points={
         'console_scripts': [
             'vidua = vidua.scripts:main',
         ],
       },
       setup_requires=['setuptools_scm', 'pytest-runner'],
       tests_require=['pytest'],
```

### Comparing `vidua-0.4.4/vidua/bps.py` & `vidua-0.4.5/vidua/bps.py`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/vidua/ips.py` & `vidua-0.4.5/vidua/ips.py`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/vidua/scripts.py` & `vidua-0.4.5/vidua/scripts.py`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/vidua/test/test_bps/test_bps.py` & `vidua-0.4.5/vidua/test/test_bps/test_bps.py`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/vidua/test/test_identify.py` & `vidua-0.4.5/vidua/test/test_identify.py`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/vidua/test/test_ips/test_ips.py` & `vidua-0.4.5/vidua/test/test_ips/test_ips.py`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/vidua/test/test_scripts/test_scripts.py` & `vidua-0.4.5/vidua/test/test_scripts/test_scripts.py`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/vidua/util.py` & `vidua-0.4.5/vidua/util.py`

 * *Files identical despite different names*

### Comparing `vidua-0.4.4/vidua.egg-info/PKG-INFO` & `vidua-0.4.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,78 @@
 Metadata-Version: 2.1
 Name: vidua
-Version: 0.4.4
+Version: 0.4.5
 Summary: Apply patches to ROMs and other files
 Home-page: http://github.com/sopoforic/vidua
 Author: Tracy Poff
 Author-email: tracy.poff@gmail.com
-License: UNKNOWN
 Project-URL: Documentation, https://vidua.readthedocs.io/
 Project-URL: Issues, https://github.com/sopoforic/vidua/issues
-Description: # vidua
-        
-        Vidua can be used to apply (BPS or IPS) patches. It is intended particularly for use with ROM
-        hacks.
-        
-        ## Installation
-        
-        ```shell
-        pip install vidua
-        ```
-        
-        ## Usage
-        
-        A simple script is included to validate or apply patches from the command line:
-        
-        ```shell
-        vidua patch.bps original.rom patched_output.rom
-        ```
-        
-        Full usage instructions:
-        
-        ```shell
-        $ vidua --help
-        usage: vidua [-h] [-v] [-q] PATCH [ORIGINAL] [OUTPUT]
-        
-        Apply or validate patches.
-        
-        positional arguments:
-          PATCH           the patch file
-          ORIGINAL        the file to be patched
-          OUTPUT          filename to write patched file
-        
-        optional arguments:
-          -h, --help      show this help message and exit
-          -v, --validate  validate the patch only; do not apply it
-          -q, --quiet     suppress output except errors
-        ```
-        
-        Vidua may also be used as a library, to validate or apply patches from within
-        another program:
-        
-        ```python
-        from vidua import bps
-        
-        patch = open('patch.bps', 'rb')
-        original = open('original.rom', 'rb')
-        
-        with open('patched.rom', 'wb') as patched:
-            patched.write(bps.patch(original, patch).read())
-        ```
-        
-        If the file is very large, you may prefer to use `shutil.copyfileobj` when
-        writing to disk.
-        
-        ## Credits
-        
-        Alcaro's [Floating IPS](https://www.smwcentral.net/?p=section&a=details&id=11474)
-        was very useful in working out how to handle BPS files when byuu's documentation
-        was unclear.
-        
-        ![Test](https://github.com/sopoforic/vidua/actions/workflows/test.yml/badge.svg?event=push)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: COPYING
+
+# vidua
+
+Vidua can be used to apply (BPS or IPS) patches. It is intended particularly for use with ROM
+hacks.
+
+## Installation
+
+```shell
+pip install vidua
+```
+
+## Usage
+
+A simple script is included to validate or apply patches from the command line:
+
+```shell
+vidua patch.bps original.rom patched_output.rom
+```
+
+Full usage instructions:
+
+```shell
+$ vidua --help
+usage: vidua [-h] [-v] [-q] PATCH [ORIGINAL] [OUTPUT]
+
+Apply or validate patches.
+
+positional arguments:
+  PATCH           the patch file
+  ORIGINAL        the file to be patched
+  OUTPUT          filename to write patched file
+
+optional arguments:
+  -h, --help      show this help message and exit
+  -v, --validate  validate the patch only; do not apply it
+  -q, --quiet     suppress output except errors
+```
+
+Vidua may also be used as a library, to validate or apply patches from within
+another program:
+
+```python
+from vidua import bps
+
+patch = open('patch.bps', 'rb')
+original = open('original.rom', 'rb')
+
+with open('patched.rom', 'wb') as patched:
+    patched.write(bps.patch(original, patch).read())
+```
+
+If the file is very large, you may prefer to use `shutil.copyfileobj` when
+writing to disk.
+
+## Credits
+
+Alcaro's [Floating IPS](https://www.smwcentral.net/?p=section&a=details&id=11474)
+was very useful in working out how to handle BPS files when byuu's documentation
+was unclear.
+
+![Test](https://github.com/sopoforic/vidua/actions/workflows/test.yml/badge.svg?event=push)
```

### Comparing `vidua-0.4.4/vidua.egg-info/SOURCES.txt` & `vidua-0.4.5/vidua.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 vidua/__init__.py
 vidua/__main__.py
 vidua/bps.py
 vidua/ips.py
+vidua/py.typed
 vidua/scripts.py
 vidua/util.py
 vidua.egg-info/PKG-INFO
 vidua.egg-info/SOURCES.txt
 vidua.egg-info/dependency_links.txt
 vidua.egg-info/entry_points.txt
 vidua.egg-info/top_level.txt
```

