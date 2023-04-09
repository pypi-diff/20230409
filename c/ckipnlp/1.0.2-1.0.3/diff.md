# Comparing `tmp/ckipnlp-1.0.2.tar.gz` & `tmp/ckipnlp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ckipnlp-1.0.2.tar", last modified: Fri May  7 03:16:05 2021, max compression
+gzip compressed data, was "ckipnlp-1.0.3.tar", last modified: Sun Apr  9 05:28:40 2023, max compression
```

## Comparing `ckipnlp-1.0.2.tar` & `ckipnlp-1.0.3.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     5458 2021-05-07 03:09:55.000000 ckipnlp-1.0.2/README.rst
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/ckipnlp.egg-info/
--rw-rw-r--   0 emfomy    (2000) emfomy    (2000)        1 2021-05-07 03:16:04.000000 ckipnlp-1.0.2/ckipnlp.egg-info/dependency_links.txt
--rw-rw-r--   0 emfomy    (2000) emfomy    (2000)     1621 2021-05-07 03:16:04.000000 ckipnlp-1.0.2/ckipnlp.egg-info/SOURCES.txt
--rw-rw-r--   0 emfomy    (2000) emfomy    (2000)        8 2021-05-07 03:16:04.000000 ckipnlp-1.0.2/ckipnlp.egg-info/top_level.txt
--rw-rw-r--   0 emfomy    (2000) emfomy    (2000)     7625 2021-05-07 03:16:04.000000 ckipnlp-1.0.2/ckipnlp.egg-info/PKG-INFO
--rw-rw-r--   0 emfomy    (2000) emfomy    (2000)      144 2021-05-07 03:16:04.000000 ckipnlp-1.0.2/ckipnlp.egg-info/requires.txt
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/ckipnlp/
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/ckipnlp/pipeline/
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     5013 2021-01-20 03:06:54.000000 ckipnlp-1.0.2/ckipnlp/pipeline/coref.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      333 2021-01-20 03:06:55.000000 ckipnlp-1.0.2/ckipnlp/pipeline/__init__.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     8462 2021-01-20 03:06:54.000000 ckipnlp-1.0.2/ckipnlp/pipeline/kernel.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      391 2021-05-07 03:02:34.000000 ckipnlp-1.0.2/ckipnlp/__init__.py
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/ckipnlp/util/
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     3928 2021-01-20 03:06:52.000000 ckipnlp-1.0.2/ckipnlp/util/data.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      212 2021-01-20 03:06:53.000000 ckipnlp-1.0.2/ckipnlp/util/__init__.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      466 2021-01-20 03:06:51.000000 ckipnlp-1.0.2/ckipnlp/util/logger.py
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/ckipnlp/container/
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     6962 2021-01-20 03:07:10.000000 ckipnlp-1.0.2/ckipnlp/container/parse.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     7151 2021-01-20 03:07:12.000000 ckipnlp-1.0.2/ckipnlp/container/coref.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     2180 2021-01-20 03:07:09.000000 ckipnlp-1.0.2/ckipnlp/container/seg.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      923 2021-01-20 03:07:07.000000 ckipnlp-1.0.2/ckipnlp/container/text.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      387 2021-01-20 03:07:14.000000 ckipnlp-1.0.2/ckipnlp/container/__init__.py
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/ckipnlp/container/util/
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      229 2021-01-20 03:07:06.000000 ckipnlp-1.0.2/ckipnlp/container/util/__init__.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)    20153 2021-01-20 03:07:05.000000 ckipnlp-1.0.2/ckipnlp/container/util/parse_tree.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     6569 2021-01-20 03:07:04.000000 ckipnlp-1.0.2/ckipnlp/container/util/wspos.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     6784 2021-01-20 03:07:11.000000 ckipnlp-1.0.2/ckipnlp/container/ner.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     9987 2021-01-20 03:07:13.000000 ckipnlp-1.0.2/ckipnlp/container/base.py
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/ckipnlp/data/
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      634 2021-01-20 03:07:03.000000 ckipnlp-1.0.2/ckipnlp/data/conparse.py
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/ckipnlp/data/coref/
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      459 2020-07-20 04:20:23.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_aristocrat.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)       52 2020-07-20 04:20:23.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_alumnus.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)    25292 2020-07-20 04:20:24.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_professional.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      736 2020-07-20 04:20:25.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_sage.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      181 2020-07-20 04:20:25.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_warrior.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     1045 2020-07-20 04:20:23.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/__init__.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     1761 2020-07-20 04:20:25.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_talent.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     1017 2020-07-20 04:20:25.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_victim.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     2993 2020-07-20 04:20:24.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_humanized.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      107 2020-07-20 04:20:23.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_candidate.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      210 2020-07-20 04:20:25.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_sick_patient.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)       73 2020-07-20 04:20:24.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_recipient.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)    17860 2020-07-20 04:20:24.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_instance.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      558 2020-07-20 04:20:24.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_owner.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     9025 2020-07-20 04:20:24.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_member.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      214 2020-07-20 04:20:23.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_fans.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      937 2020-07-20 04:20:25.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_student.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     1923 2020-07-20 04:20:24.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_human/_religious_follower.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)       67 2020-07-20 04:20:23.000000 ckipnlp-1.0.2/ckipnlp/data/coref/__init__.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     2727 2020-07-20 04:20:26.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_pronoun.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      213 2020-07-20 04:20:26.000000 ckipnlp-1.0.2/ckipnlp/data/coref/_self.py
-drwxrwxr-x   0 emfomy    (2000) emfomy    (2000)        0 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/ckipnlp/driver/
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     8700 2021-05-07 03:02:28.000000 ckipnlp-1.0.2/ckipnlp/driver/classic.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)    14264 2021-01-20 03:07:00.000000 ckipnlp-1.0.2/ckipnlp/driver/coref.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)      513 2021-01-20 03:07:02.000000 ckipnlp-1.0.2/ckipnlp/driver/__init__.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     3566 2021-01-20 03:07:01.000000 ckipnlp-1.0.2/ckipnlp/driver/base.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     2079 2021-01-20 03:06:57.000000 ckipnlp-1.0.2/ckipnlp/driver/ss.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)     6005 2021-05-07 03:02:29.000000 ckipnlp-1.0.2/ckipnlp/driver/tagger.py
--rwxr-xr-x   0 emfomy    (2000) emfomy    (2000)     2039 2021-01-26 07:14:35.000000 ckipnlp-1.0.2/setup.py
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)       26 2020-07-20 04:20:32.000000 ckipnlp-1.0.2/MANIFEST.in
--rw-r--r--   0 emfomy    (2000) emfomy    (2000)       80 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/setup.cfg
--rw-rw-r--   0 emfomy    (2000) emfomy    (2000)     7625 2021-05-07 03:16:05.000000 ckipnlp-1.0.2/PKG-INFO
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.812219 ckipnlp-1.0.3/
+-rw-r--r--   0 emfo       (501) staff       (20)    35149 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/LICENSE
+-rw-r--r--   0 emfo       (501) staff       (20)       26 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/MANIFEST.in
+-rw-r--r--   0 emfo       (501) staff       (20)     6442 2023-04-09 05:28:40.812319 ckipnlp-1.0.3/PKG-INFO
+-rw-r--r--   0 emfo       (501) staff       (20)     5458 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/README.rst
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.803661 ckipnlp-1.0.3/ckipnlp/
+-rw-r--r--   0 emfo       (501) staff       (20)      391 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/__init__.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.806102 ckipnlp-1.0.3/ckipnlp/container/
+-rw-r--r--   0 emfo       (501) staff       (20)      387 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/container/__init__.py
+-rw-r--r--   0 emfo       (501) staff       (20)     9987 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/container/base.py
+-rw-r--r--   0 emfo       (501) staff       (20)     7151 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/container/coref.py
+-rw-r--r--   0 emfo       (501) staff       (20)     6784 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/container/ner.py
+-rw-r--r--   0 emfo       (501) staff       (20)     6962 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/container/parse.py
+-rw-r--r--   0 emfo       (501) staff       (20)     2180 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/container/seg.py
+-rw-r--r--   0 emfo       (501) staff       (20)      923 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/container/text.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.806592 ckipnlp-1.0.3/ckipnlp/container/util/
+-rw-r--r--   0 emfo       (501) staff       (20)      229 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/container/util/__init__.py
+-rw-r--r--   0 emfo       (501) staff       (20)    20153 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/container/util/parse_tree.py
+-rw-r--r--   0 emfo       (501) staff       (20)     6569 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/container/util/wspos.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.806815 ckipnlp-1.0.3/ckipnlp/data/
+-rw-r--r--   0 emfo       (501) staff       (20)      634 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/data/conparse.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.807464 ckipnlp-1.0.3/ckipnlp/data/coref/
+-rw-r--r--   0 emfo       (501) staff       (20)       67 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/__init__.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.810420 ckipnlp-1.0.3/ckipnlp/data/coref/_human/
+-rw-r--r--   0 emfo       (501) staff       (20)     1045 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/__init__.py
+-rw-r--r--   0 emfo       (501) staff       (20)       52 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_alumnus.py
+-rw-r--r--   0 emfo       (501) staff       (20)      459 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_aristocrat.py
+-rw-r--r--   0 emfo       (501) staff       (20)      107 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_candidate.py
+-rw-r--r--   0 emfo       (501) staff       (20)      214 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_fans.py
+-rw-r--r--   0 emfo       (501) staff       (20)     2993 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_humanized.py
+-rw-r--r--   0 emfo       (501) staff       (20)    17860 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_instance.py
+-rw-r--r--   0 emfo       (501) staff       (20)     9025 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_member.py
+-rw-r--r--   0 emfo       (501) staff       (20)      558 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_owner.py
+-rw-r--r--   0 emfo       (501) staff       (20)    25292 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_professional.py
+-rw-r--r--   0 emfo       (501) staff       (20)       73 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_recipient.py
+-rw-r--r--   0 emfo       (501) staff       (20)     1923 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_religious_follower.py
+-rw-r--r--   0 emfo       (501) staff       (20)      736 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_sage.py
+-rw-r--r--   0 emfo       (501) staff       (20)      210 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_sick_patient.py
+-rw-r--r--   0 emfo       (501) staff       (20)      937 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_student.py
+-rw-r--r--   0 emfo       (501) staff       (20)     1761 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_talent.py
+-rw-r--r--   0 emfo       (501) staff       (20)     1017 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_victim.py
+-rw-r--r--   0 emfo       (501) staff       (20)      181 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_human/_warrior.py
+-rw-r--r--   0 emfo       (501) staff       (20)     2727 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_pronoun.py
+-rw-r--r--   0 emfo       (501) staff       (20)      213 2021-04-24 04:27:10.000000 ckipnlp-1.0.3/ckipnlp/data/coref/_self.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.811273 ckipnlp-1.0.3/ckipnlp/driver/
+-rw-r--r--   0 emfo       (501) staff       (20)      513 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/driver/__init__.py
+-rw-r--r--   0 emfo       (501) staff       (20)     3566 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/driver/base.py
+-rw-r--r--   0 emfo       (501) staff       (20)     8700 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/driver/classic.py
+-rw-r--r--   0 emfo       (501) staff       (20)    14264 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/driver/coref.py
+-rw-r--r--   0 emfo       (501) staff       (20)     2079 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/driver/ss.py
+-rw-r--r--   0 emfo       (501) staff       (20)     6005 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/driver/tagger.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.811686 ckipnlp-1.0.3/ckipnlp/pipeline/
+-rw-r--r--   0 emfo       (501) staff       (20)      333 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/pipeline/__init__.py
+-rw-r--r--   0 emfo       (501) staff       (20)     5013 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/pipeline/coref.py
+-rw-r--r--   0 emfo       (501) staff       (20)     8462 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/pipeline/kernel.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.812097 ckipnlp-1.0.3/ckipnlp/util/
+-rw-r--r--   0 emfo       (501) staff       (20)      212 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/util/__init__.py
+-rw-r--r--   0 emfo       (501) staff       (20)     3928 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/util/data.py
+-rw-r--r--   0 emfo       (501) staff       (20)      466 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/ckipnlp/util/logger.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:28:40.804885 ckipnlp-1.0.3/ckipnlp.egg-info/
+-rw-r--r--   0 emfo       (501) staff       (20)     6442 2023-04-09 05:28:40.000000 ckipnlp-1.0.3/ckipnlp.egg-info/PKG-INFO
+-rw-r--r--   0 emfo       (501) staff       (20)     1629 2023-04-09 05:28:40.000000 ckipnlp-1.0.3/ckipnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 emfo       (501) staff       (20)        1 2023-04-09 05:28:40.000000 ckipnlp-1.0.3/ckipnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 emfo       (501) staff       (20)      144 2023-04-09 05:28:40.000000 ckipnlp-1.0.3/ckipnlp.egg-info/requires.txt
+-rw-r--r--   0 emfo       (501) staff       (20)        8 2023-04-09 05:28:40.000000 ckipnlp-1.0.3/ckipnlp.egg-info/top_level.txt
+-rw-r--r--   0 emfo       (501) staff       (20)       80 2023-04-09 05:28:40.812578 ckipnlp-1.0.3/setup.cfg
+-rwxr-xr-x   0 emfo       (501) staff       (20)     2039 2023-04-09 05:27:58.000000 ckipnlp-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ckipnlp-1.0.2/README.rst` & `ckipnlp-1.0.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 - With CkipTagger backend (recommended): ``pip install ckipnlp[tagger]`` or ``pip install ckipnlp[tagger-gpu]``.
 - With CkipClassic Parser Client backend (recommended): ``pip install ckipnlp[classic]``.
 - With CkipClassic offline backend: Please refer https://ckip-classic.readthedocs.io/en/latest/main/readme.html#installation for CkipClassic installation guide.
 
 .. attention::
    To use CkipClassic Parser Client backend, please
 
-   #. Register an account at http://parser.iis.sinica.edu.tw/v1/reg.exe
+   #. Register an account at http://parser.iis.sinica.edu.tw/v1/reg.php
    #. Set the username and password in the pipeline's options:
 
    .. code-block:: python
 
       pipeline = CkipPipeline(opts={'con_parser': {'username': YOUR_USERNAME, 'password': YOUR_PASSWORD})
 
 
@@ -139,11 +139,11 @@
 See https://ckipnlp.readthedocs.io/ for full documentation.
 
 License
 -------
 
 |GPL-3.0|
 
-Copyright (c) 2018-2020 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
+Copyright (c) 2018-2023 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
 
 .. |GPL-3.0| image:: https://www.gnu.org/graphics/gplv3-with-text-136x68.png
    :target: https://www.gnu.org/licenses/gpl-3.0.html
```

### Comparing `ckipnlp-1.0.2/ckipnlp.egg-info/SOURCES.txt` & `ckipnlp-1.0.3/ckipnlp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 ckipnlp/__init__.py
 ckipnlp.egg-info/PKG-INFO
 ckipnlp.egg-info/SOURCES.txt
```

### Comparing `ckipnlp-1.0.2/ckipnlp.egg-info/PKG-INFO` & `ckipnlp-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,16 @@
 Metadata-Version: 2.1
 Name: ckipnlp
-Version: 1.0.2
+Version: 1.0.3
 Summary: CKIP CoreNLP
 Home-page: https://ckipnlp.readthedocs.io
+Download-URL: https://ckipnlp.readthedocs.io/tarball/1.0.3
 Author: Mu Yang
 Author-email: emfomy@gmail.com
 License: GPL-3.0
-Download-URL: https://ckipnlp.readthedocs.io/tarball/1.0.2
-Description: CKIP CoreNLP Toolkit
-        --------------------
-        
-        Features
-        ^^^^^^^^
-        
-        - Sentence Segmentation
-        - Word Segmentation
-        - Part-of-Speech Tagging
-        - Named-Entity Recognition
-        - Constituency Parsing
-        - Coreference Resolution
-        
-        Git
-        ^^^
-        
-        https://github.com/ckiplab/ckipnlp
-        
-        |GitHub Version| |GitHub Release| |GitHub Issues|
-        
-        .. |GitHub Version| image:: https://img.shields.io/github/v/release/ckiplab/ckipnlp.svg?maxAge=3600
-           :target: https://github.com/ckiplab/ckipnlp/releases
-        
-        .. |GitHub License| image:: https://img.shields.io/github/license/ckiplab/ckipnlp.svg?maxAge=3600
-           :target: https://github.com/ckiplab/ckipnlp/blob/master/LICENSE
-        
-        .. |GitHub Release| image:: https://img.shields.io/github/release-date/ckiplab/ckipnlp.svg?maxAge=3600
-        
-        .. |GitHub Downloads| image:: https://img.shields.io/github/downloads/ckiplab/ckipnlp/total.svg?maxAge=3600
-           :target: https://github.com/ckiplab/ckipnlp/releases/latest
-        
-        .. |GitHub Issues| image:: https://img.shields.io/github/issues/ckiplab/ckipnlp.svg?maxAge=3600
-           :target: https://github.com/ckiplab/ckipnlp/issues
-        
-        .. |GitHub Forks| image:: https://img.shields.io/github/forks/ckiplab/ckipnlp.svg?style=social&label=Fork&maxAge=3600
-        
-        .. |GitHub Stars| image:: https://img.shields.io/github/stars/ckiplab/ckipnlp.svg?style=social&label=Star&maxAge=3600
-        
-        .. |GitHub Watchers| image:: https://img.shields.io/github/watchers/ckiplab/ckipnlp.svg?style=social&label=Watch&maxAge=3600
-        
-        PyPI
-        ^^^^
-        
-        https://pypi.org/project/ckipnlp
-        
-        |PyPI Version| |PyPI License| |PyPI Downloads| |PyPI Python| |PyPI Implementation| |PyPI Status|
-        
-        .. |PyPI Version| image:: https://img.shields.io/pypi/v/ckipnlp.svg?maxAge=3600
-           :target: https://pypi.org/project/ckipnlp
-        
-        .. |PyPI License| image:: https://img.shields.io/pypi/l/ckipnlp.svg?maxAge=3600
-           :target: https://github.com/ckiplab/ckipnlp/blob/master/LICENSE
-        
-        .. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/ckipnlp.svg?maxAge=3600
-           :target: https://pypi.org/project/ckipnlp#files
-        
-        .. |PyPI Python| image:: https://img.shields.io/pypi/pyversions/ckipnlp.svg?maxAge=3600
-        
-        .. |PyPI Implementation| image:: https://img.shields.io/pypi/implementation/ckipnlp.svg?maxAge=3600
-        
-        .. |PyPI Format| image:: https://img.shields.io/pypi/format/ckipnlp.svg?maxAge=3600
-        
-        .. |PyPI Status| image:: https://img.shields.io/pypi/status/ckipnlp.svg?maxAge=3600
-        
-        Documentation
-        ^^^^^^^^^^^^^
-        
-        https://ckipnlp.readthedocs.io/
-        
-        |ReadTheDocs Home|
-        
-        .. |ReadTheDocs Home| image:: https://img.shields.io/website/https/ckipnlp.readthedocs.io.svg?maxAge=3600&up_message=online&down_message=offline
-           :target: https://ckipnlp.readthedocs.io
-        
-        Online Demo
-        ^^^^^^^^^^^
-        
-        https://ckip.iis.sinica.edu.tw/service/corenlp
-        
-        Contributers
-        ^^^^^^^^^^^^
-        
-        * `Mu Yang <https://muyang.pro>`__ at `CKIP <https://ckip.iis.sinica.edu.tw>`__ (Author & Maintainer)
-        * `Wei-Yun Ma <https://www.iis.sinica.edu.tw/pages/ma/>`__ at `CKIP <https://ckip.iis.sinica.edu.tw>`__ (Maintainer)
-        * `DouglasWu <dgrey1116@gmail.com>`__
-        
-        Installation
-        ------------
-        
-        Requirements
-        ^^^^^^^^^^^^
-        
-        * `Python <https://www.python.org>`__ 3.6+
-        * `TreeLib <https://treelib.readthedocs.io>`__ 1.5+
-        * `CkipTagger <https://pypi.org/project/ckiptagger>`__ 0.2.1+ [Optional, Recommended]
-        * `CkipClassic <https://ckip-classic.readthedocs.io>`__ 1.0+ [Optional, Recommended]
-        * `TensorFlow / TensorFlow-GPU <https://www.tensorflow.org/>`__ 1.13.1+ [Required by CkipTagger]
-        
-        Driver Requirements
-        ^^^^^^^^^^^^^^^^^^^
-        
-        ================================  ========  ==========  ===========
-        Driver                            Built-in  CkipTagger  CkipClassic
-        ================================  ========  ==========  ===========
-        Sentence Segmentation             ✔
-        Word Segmentation†                          ✔           ✔
-        Part-of-Speech Tagging†                     ✔           ✔
-        Constituency Parsing                                    ✔
-        Named-Entity Recognition                    ✔
-        Coreference Resolution‡           ✔         ✔           ✔
-        ================================  ========  ==========  ===========
-        
-        - † These drivers require only one of either backends.
-        - ‡ Coreference implementation does not require any backend, but requires results from word segmentation, part-of-speech tagging, constituency parsing, and named-entity recognition.
-        
-        Installation via Pip
-        ^^^^^^^^^^^^^^^^^^^^
-        
-        - No backend (not recommended): ``pip install ckipnlp``.
-        - With CkipTagger backend (recommended): ``pip install ckipnlp[tagger]`` or ``pip install ckipnlp[tagger-gpu]``.
-        - With CkipClassic Parser Client backend (recommended): ``pip install ckipnlp[classic]``.
-        - With CkipClassic offline backend: Please refer https://ckip-classic.readthedocs.io/en/latest/main/readme.html#installation for CkipClassic installation guide.
-        
-        .. attention::
-           To use CkipClassic Parser Client backend, please
-        
-           #. Register an account at http://parser.iis.sinica.edu.tw/v1/reg.exe
-           #. Set the username and password in the pipeline's options:
-        
-           .. code-block:: python
-        
-              pipeline = CkipPipeline(opts={'con_parser': {'username': YOUR_USERNAME, 'password': YOUR_PASSWORD})
-        
-        
-        
-        Detail
-        ------
-        
-        See https://ckipnlp.readthedocs.io/ for full documentation.
-        
-        License
-        -------
-        
-        |GPL-3.0|
-        
-        Copyright (c) 2018-2020 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
-        
-        .. |GPL-3.0| image:: https://www.gnu.org/graphics/gplv3-with-text-136x68.png
-           :target: https://www.gnu.org/licenses/gpl-3.0.html
-        
 Platform: linux_x86_64
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -170,7 +20,158 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: Chinese (Traditional)
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: classic
 Provides-Extra: tagger
 Provides-Extra: tagger-gpu
+License-File: LICENSE
+
+CKIP CoreNLP Toolkit
+--------------------
+
+Features
+^^^^^^^^
+
+- Sentence Segmentation
+- Word Segmentation
+- Part-of-Speech Tagging
+- Named-Entity Recognition
+- Constituency Parsing
+- Coreference Resolution
+
+Git
+^^^
+
+https://github.com/ckiplab/ckipnlp
+
+|GitHub Version| |GitHub Release| |GitHub Issues|
+
+.. |GitHub Version| image:: https://img.shields.io/github/v/release/ckiplab/ckipnlp.svg?maxAge=3600
+   :target: https://github.com/ckiplab/ckipnlp/releases
+
+.. |GitHub License| image:: https://img.shields.io/github/license/ckiplab/ckipnlp.svg?maxAge=3600
+   :target: https://github.com/ckiplab/ckipnlp/blob/master/LICENSE
+
+.. |GitHub Release| image:: https://img.shields.io/github/release-date/ckiplab/ckipnlp.svg?maxAge=3600
+
+.. |GitHub Downloads| image:: https://img.shields.io/github/downloads/ckiplab/ckipnlp/total.svg?maxAge=3600
+   :target: https://github.com/ckiplab/ckipnlp/releases/latest
+
+.. |GitHub Issues| image:: https://img.shields.io/github/issues/ckiplab/ckipnlp.svg?maxAge=3600
+   :target: https://github.com/ckiplab/ckipnlp/issues
+
+.. |GitHub Forks| image:: https://img.shields.io/github/forks/ckiplab/ckipnlp.svg?style=social&label=Fork&maxAge=3600
+
+.. |GitHub Stars| image:: https://img.shields.io/github/stars/ckiplab/ckipnlp.svg?style=social&label=Star&maxAge=3600
+
+.. |GitHub Watchers| image:: https://img.shields.io/github/watchers/ckiplab/ckipnlp.svg?style=social&label=Watch&maxAge=3600
+
+PyPI
+^^^^
+
+https://pypi.org/project/ckipnlp
+
+|PyPI Version| |PyPI License| |PyPI Downloads| |PyPI Python| |PyPI Implementation| |PyPI Status|
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/ckipnlp.svg?maxAge=3600
+   :target: https://pypi.org/project/ckipnlp
+
+.. |PyPI License| image:: https://img.shields.io/pypi/l/ckipnlp.svg?maxAge=3600
+   :target: https://github.com/ckiplab/ckipnlp/blob/master/LICENSE
+
+.. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/ckipnlp.svg?maxAge=3600
+   :target: https://pypi.org/project/ckipnlp#files
+
+.. |PyPI Python| image:: https://img.shields.io/pypi/pyversions/ckipnlp.svg?maxAge=3600
+
+.. |PyPI Implementation| image:: https://img.shields.io/pypi/implementation/ckipnlp.svg?maxAge=3600
+
+.. |PyPI Format| image:: https://img.shields.io/pypi/format/ckipnlp.svg?maxAge=3600
+
+.. |PyPI Status| image:: https://img.shields.io/pypi/status/ckipnlp.svg?maxAge=3600
+
+Documentation
+^^^^^^^^^^^^^
+
+https://ckipnlp.readthedocs.io/
+
+|ReadTheDocs Home|
+
+.. |ReadTheDocs Home| image:: https://img.shields.io/website/https/ckipnlp.readthedocs.io.svg?maxAge=3600&up_message=online&down_message=offline
+   :target: https://ckipnlp.readthedocs.io
+
+Online Demo
+^^^^^^^^^^^
+
+https://ckip.iis.sinica.edu.tw/service/corenlp
+
+Contributers
+^^^^^^^^^^^^
+
+* `Mu Yang <https://muyang.pro>`__ at `CKIP <https://ckip.iis.sinica.edu.tw>`__ (Author & Maintainer)
+* `Wei-Yun Ma <https://www.iis.sinica.edu.tw/pages/ma/>`__ at `CKIP <https://ckip.iis.sinica.edu.tw>`__ (Maintainer)
+* `DouglasWu <dgrey1116@gmail.com>`__
+
+Installation
+------------
+
+Requirements
+^^^^^^^^^^^^
+
+* `Python <https://www.python.org>`__ 3.6+
+* `TreeLib <https://treelib.readthedocs.io>`__ 1.5+
+* `CkipTagger <https://pypi.org/project/ckiptagger>`__ 0.2.1+ [Optional, Recommended]
+* `CkipClassic <https://ckip-classic.readthedocs.io>`__ 1.0+ [Optional, Recommended]
+* `TensorFlow / TensorFlow-GPU <https://www.tensorflow.org/>`__ 1.13.1+ [Required by CkipTagger]
+
+Driver Requirements
+^^^^^^^^^^^^^^^^^^^
+
+================================  ========  ==========  ===========
+Driver                            Built-in  CkipTagger  CkipClassic
+================================  ========  ==========  ===========
+Sentence Segmentation             ✔
+Word Segmentation†                          ✔           ✔
+Part-of-Speech Tagging†                     ✔           ✔
+Constituency Parsing                                    ✔
+Named-Entity Recognition                    ✔
+Coreference Resolution‡           ✔         ✔           ✔
+================================  ========  ==========  ===========
+
+- † These drivers require only one of either backends.
+- ‡ Coreference implementation does not require any backend, but requires results from word segmentation, part-of-speech tagging, constituency parsing, and named-entity recognition.
+
+Installation via Pip
+^^^^^^^^^^^^^^^^^^^^
+
+- No backend (not recommended): ``pip install ckipnlp``.
+- With CkipTagger backend (recommended): ``pip install ckipnlp[tagger]`` or ``pip install ckipnlp[tagger-gpu]``.
+- With CkipClassic Parser Client backend (recommended): ``pip install ckipnlp[classic]``.
+- With CkipClassic offline backend: Please refer https://ckip-classic.readthedocs.io/en/latest/main/readme.html#installation for CkipClassic installation guide.
+
+.. attention::
+   To use CkipClassic Parser Client backend, please
+
+   #. Register an account at http://parser.iis.sinica.edu.tw/v1/reg.php
+   #. Set the username and password in the pipeline's options:
+
+   .. code-block:: python
+
+      pipeline = CkipPipeline(opts={'con_parser': {'username': YOUR_USERNAME, 'password': YOUR_PASSWORD})
+
+
+
+Detail
+------
+
+See https://ckipnlp.readthedocs.io/ for full documentation.
+
+License
+-------
+
+|GPL-3.0|
+
+Copyright (c) 2018-2023 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
+
+.. |GPL-3.0| image:: https://www.gnu.org/graphics/gplv3-with-text-136x68.png
+   :target: https://www.gnu.org/licenses/gpl-3.0.html
```

### Comparing `ckipnlp-1.0.2/ckipnlp/pipeline/coref.py` & `ckipnlp-1.0.3/ckipnlp/pipeline/coref.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides coreference resolution pipeline.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from collections.abc import (
     Mapping as _Mapping,
 )
 
 from ckipnlp.driver.base import (
```

### Comparing `ckipnlp-1.0.2/ckipnlp/pipeline/kernel.py` & `ckipnlp-1.0.3/ckipnlp/pipeline/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides kernel CKIPNLP pipeline.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from collections.abc import (
     Mapping as _Mapping,
 )
 
 from ckipnlp.driver.base import (
```

### Comparing `ckipnlp-1.0.2/ckipnlp/util/data.py` & `ckipnlp-1.0.3/ckipnlp/util/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 This module implements data loading utilities for CKIPNLP.
 """
 
 # pylint: disable=missing-docstring
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 import os as _os
 import shutil as _shutil
 
 from abc import (
     ABCMeta as _ABCMeta,
```

### Comparing `ckipnlp-1.0.2/ckipnlp/container/parse.py` & `ckipnlp-1.0.3/ckipnlp/container/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides containers for parsed sentences.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from typing import (
     NamedTuple as _NamedTuple,
 )
 
 from .base import (
```

### Comparing `ckipnlp-1.0.2/ckipnlp/container/coref.py` & `ckipnlp-1.0.3/ckipnlp/container/coref.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides containers for coreference sentences.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from typing import (
     NamedTuple as _NamedTuple,
     Tuple as _Tuple,
 )
```

### Comparing `ckipnlp-1.0.2/ckipnlp/container/seg.py` & `ckipnlp-1.0.3/ckipnlp/container/seg.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides containers for word-segmented sentences.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from .base import (
     BaseList as _BaseList,
     BaseSentence0 as _BaseSentence0,
 )
```

### Comparing `ckipnlp-1.0.2/ckipnlp/container/text.py` & `ckipnlp-1.0.3/ckipnlp/container/text.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides containers for text sentences.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from .base import (
     BaseList0 as _BaseList0
 )
 
 ################################################################################################################################
```

### Comparing `ckipnlp-1.0.2/ckipnlp/container/util/parse_tree.py` & `ckipnlp-1.0.3/ckipnlp/container/util/parse_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides tree containers for parsed sentences.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 
 from collections import (
     deque as _deque,
 )
```

### Comparing `ckipnlp-1.0.2/ckipnlp/container/util/wspos.py` & `ckipnlp-1.0.3/ckipnlp/container/util/wspos.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides containers for word-segmented sentences with part-of-speech-tags.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from abc import (
     ABCMeta as _ABCMeta,
     abstractmethod as _abstractmethod,
 )
```

### Comparing `ckipnlp-1.0.2/ckipnlp/container/ner.py` & `ckipnlp-1.0.3/ckipnlp/container/ner.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides containers for NER sentences.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from typing import (
     NamedTuple as _NamedTuple,
     Tuple as _Tuple,
 )
```

### Comparing `ckipnlp-1.0.2/ckipnlp/container/base.py` & `ckipnlp-1.0.3/ckipnlp/container/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides base containers.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 import json as _json
 
 from abc import (
     ABCMeta as _ABCMeta,
     abstractmethod as _abstractmethod,
```

### Comparing `ckipnlp-1.0.2/ckipnlp/data/conparse.py` & `ckipnlp-1.0.3/ckipnlp/data/conparse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 # pylint: disable=missing-docstring
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 ################################################################################################################################
 
 SUBJECT_ROLES = {'agent', 'causer', 'experiencer'}
 OBJECT_ROLES = {'benefactor', 'companion', 'comparison', 'goal', 'range', 'source', 'target'}
 NEUTRAL_ROLES = {'theme', 'topic'}
```

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/_professional.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/_professional.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/_sage.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/_sage.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/__init__.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/__init__.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/_talent.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/_talent.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/_victim.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/_victim.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/_humanized.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/_humanized.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/_instance.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/_instance.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/_owner.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/_owner.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/_member.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/_member.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/_student.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/_student.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_human/_religious_follower.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_human/_religious_follower.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/data/coref/_pronoun.py` & `ckipnlp-1.0.3/ckipnlp/data/coref/_pronoun.py`

 * *Files identical despite different names*

### Comparing `ckipnlp-1.0.2/ckipnlp/driver/classic.py` & `ckipnlp-1.0.3/ckipnlp/driver/classic.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides drivers with CkipClassic backend.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from abc import (
     abstractmethod as _abstractmethod,
 )
 
 from itertools import (
@@ -248,15 +248,15 @@
             (*optional*) The username of CkipClassicParserClient.
         password : string
             (*optional*) The password of CkipClassicParserClient.
 
     Notes
     -----
 
-        Please register an account at http://parser.iis.sinica.edu.tw/v1/reg.exe and
+        Please register an account at http://parser.iis.sinica.edu.tw/v1/reg.php and
         set the environment variables ``$CKIPPARSER_USERNAME`` and ``$CKIPPARSER_PASSWORD``.
 
     .. method:: __call__(*, ws, pos)
 
         Apply constituency parsing.
 
         Parameters
```

### Comparing `ckipnlp-1.0.2/ckipnlp/driver/coref.py` & `ckipnlp-1.0.3/ckipnlp/driver/coref.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides built-in coreference resolution driver.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 import numpy as _np
 
 from treelib import (
     Tree as _Tree,
 )
```

### Comparing `ckipnlp-1.0.2/ckipnlp/driver/__init__.py` & `ckipnlp-1.0.3/ckipnlp/driver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module implements CKIPNLP drivers.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from .tagger import (
     CkipTaggerWordSegmenter,
     CkipTaggerPosTagger,
     CkipTaggerNerChunker,
 )
```

### Comparing `ckipnlp-1.0.2/ckipnlp/driver/base.py` & `ckipnlp-1.0.3/ckipnlp/driver/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides base drivers.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from abc import (
     ABCMeta as _ABCMeta,
     abstractmethod as _abstractmethod,
 )
```

### Comparing `ckipnlp-1.0.2/ckipnlp/driver/ss.py` & `ckipnlp-1.0.3/ckipnlp/driver/ss.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides built-in sentence segmentation driver.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 import re as _re
 
 from ckipnlp.container import (
     TextParagraph as _TextParagraph,
 )
```

### Comparing `ckipnlp-1.0.2/ckipnlp/driver/tagger.py` & `ckipnlp-1.0.3/ckipnlp/driver/tagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module provides drivers with CkipTagger backend.
 """
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from ckipnlp.container import (
     TextParagraph as _TextParagraph,
     SegParagraph as _SegParagraph,
     NerParagraph as _NerParagraph,
 )
```

### Comparing `ckipnlp-1.0.2/setup.py` & `ckipnlp-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 __author__ = 'Mu Yang <http://muyang.pro>'
-__copyright__ = '2018-2020 CKIP Lab'
+__copyright__ = '2018-2023 CKIP Lab'
 __license__ = 'GPL-3.0'
 
 from setuptools import setup, find_namespace_packages
 import ckipnlp as about
 
 ################################################################################
```

### Comparing `ckipnlp-1.0.2/PKG-INFO` & `ckipnlp-1.0.3/ckipnlp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,16 @@
 Metadata-Version: 2.1
 Name: ckipnlp
-Version: 1.0.2
+Version: 1.0.3
 Summary: CKIP CoreNLP
 Home-page: https://ckipnlp.readthedocs.io
+Download-URL: https://ckipnlp.readthedocs.io/tarball/1.0.3
 Author: Mu Yang
 Author-email: emfomy@gmail.com
 License: GPL-3.0
-Download-URL: https://ckipnlp.readthedocs.io/tarball/1.0.2
-Description: CKIP CoreNLP Toolkit
-        --------------------
-        
-        Features
-        ^^^^^^^^
-        
-        - Sentence Segmentation
-        - Word Segmentation
-        - Part-of-Speech Tagging
-        - Named-Entity Recognition
-        - Constituency Parsing
-        - Coreference Resolution
-        
-        Git
-        ^^^
-        
-        https://github.com/ckiplab/ckipnlp
-        
-        |GitHub Version| |GitHub Release| |GitHub Issues|
-        
-        .. |GitHub Version| image:: https://img.shields.io/github/v/release/ckiplab/ckipnlp.svg?maxAge=3600
-           :target: https://github.com/ckiplab/ckipnlp/releases
-        
-        .. |GitHub License| image:: https://img.shields.io/github/license/ckiplab/ckipnlp.svg?maxAge=3600
-           :target: https://github.com/ckiplab/ckipnlp/blob/master/LICENSE
-        
-        .. |GitHub Release| image:: https://img.shields.io/github/release-date/ckiplab/ckipnlp.svg?maxAge=3600
-        
-        .. |GitHub Downloads| image:: https://img.shields.io/github/downloads/ckiplab/ckipnlp/total.svg?maxAge=3600
-           :target: https://github.com/ckiplab/ckipnlp/releases/latest
-        
-        .. |GitHub Issues| image:: https://img.shields.io/github/issues/ckiplab/ckipnlp.svg?maxAge=3600
-           :target: https://github.com/ckiplab/ckipnlp/issues
-        
-        .. |GitHub Forks| image:: https://img.shields.io/github/forks/ckiplab/ckipnlp.svg?style=social&label=Fork&maxAge=3600
-        
-        .. |GitHub Stars| image:: https://img.shields.io/github/stars/ckiplab/ckipnlp.svg?style=social&label=Star&maxAge=3600
-        
-        .. |GitHub Watchers| image:: https://img.shields.io/github/watchers/ckiplab/ckipnlp.svg?style=social&label=Watch&maxAge=3600
-        
-        PyPI
-        ^^^^
-        
-        https://pypi.org/project/ckipnlp
-        
-        |PyPI Version| |PyPI License| |PyPI Downloads| |PyPI Python| |PyPI Implementation| |PyPI Status|
-        
-        .. |PyPI Version| image:: https://img.shields.io/pypi/v/ckipnlp.svg?maxAge=3600
-           :target: https://pypi.org/project/ckipnlp
-        
-        .. |PyPI License| image:: https://img.shields.io/pypi/l/ckipnlp.svg?maxAge=3600
-           :target: https://github.com/ckiplab/ckipnlp/blob/master/LICENSE
-        
-        .. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/ckipnlp.svg?maxAge=3600
-           :target: https://pypi.org/project/ckipnlp#files
-        
-        .. |PyPI Python| image:: https://img.shields.io/pypi/pyversions/ckipnlp.svg?maxAge=3600
-        
-        .. |PyPI Implementation| image:: https://img.shields.io/pypi/implementation/ckipnlp.svg?maxAge=3600
-        
-        .. |PyPI Format| image:: https://img.shields.io/pypi/format/ckipnlp.svg?maxAge=3600
-        
-        .. |PyPI Status| image:: https://img.shields.io/pypi/status/ckipnlp.svg?maxAge=3600
-        
-        Documentation
-        ^^^^^^^^^^^^^
-        
-        https://ckipnlp.readthedocs.io/
-        
-        |ReadTheDocs Home|
-        
-        .. |ReadTheDocs Home| image:: https://img.shields.io/website/https/ckipnlp.readthedocs.io.svg?maxAge=3600&up_message=online&down_message=offline
-           :target: https://ckipnlp.readthedocs.io
-        
-        Online Demo
-        ^^^^^^^^^^^
-        
-        https://ckip.iis.sinica.edu.tw/service/corenlp
-        
-        Contributers
-        ^^^^^^^^^^^^
-        
-        * `Mu Yang <https://muyang.pro>`__ at `CKIP <https://ckip.iis.sinica.edu.tw>`__ (Author & Maintainer)
-        * `Wei-Yun Ma <https://www.iis.sinica.edu.tw/pages/ma/>`__ at `CKIP <https://ckip.iis.sinica.edu.tw>`__ (Maintainer)
-        * `DouglasWu <dgrey1116@gmail.com>`__
-        
-        Installation
-        ------------
-        
-        Requirements
-        ^^^^^^^^^^^^
-        
-        * `Python <https://www.python.org>`__ 3.6+
-        * `TreeLib <https://treelib.readthedocs.io>`__ 1.5+
-        * `CkipTagger <https://pypi.org/project/ckiptagger>`__ 0.2.1+ [Optional, Recommended]
-        * `CkipClassic <https://ckip-classic.readthedocs.io>`__ 1.0+ [Optional, Recommended]
-        * `TensorFlow / TensorFlow-GPU <https://www.tensorflow.org/>`__ 1.13.1+ [Required by CkipTagger]
-        
-        Driver Requirements
-        ^^^^^^^^^^^^^^^^^^^
-        
-        ================================  ========  ==========  ===========
-        Driver                            Built-in  CkipTagger  CkipClassic
-        ================================  ========  ==========  ===========
-        Sentence Segmentation             ✔
-        Word Segmentation†                          ✔           ✔
-        Part-of-Speech Tagging†                     ✔           ✔
-        Constituency Parsing                                    ✔
-        Named-Entity Recognition                    ✔
-        Coreference Resolution‡           ✔         ✔           ✔
-        ================================  ========  ==========  ===========
-        
-        - † These drivers require only one of either backends.
-        - ‡ Coreference implementation does not require any backend, but requires results from word segmentation, part-of-speech tagging, constituency parsing, and named-entity recognition.
-        
-        Installation via Pip
-        ^^^^^^^^^^^^^^^^^^^^
-        
-        - No backend (not recommended): ``pip install ckipnlp``.
-        - With CkipTagger backend (recommended): ``pip install ckipnlp[tagger]`` or ``pip install ckipnlp[tagger-gpu]``.
-        - With CkipClassic Parser Client backend (recommended): ``pip install ckipnlp[classic]``.
-        - With CkipClassic offline backend: Please refer https://ckip-classic.readthedocs.io/en/latest/main/readme.html#installation for CkipClassic installation guide.
-        
-        .. attention::
-           To use CkipClassic Parser Client backend, please
-        
-           #. Register an account at http://parser.iis.sinica.edu.tw/v1/reg.exe
-           #. Set the username and password in the pipeline's options:
-        
-           .. code-block:: python
-        
-              pipeline = CkipPipeline(opts={'con_parser': {'username': YOUR_USERNAME, 'password': YOUR_PASSWORD})
-        
-        
-        
-        Detail
-        ------
-        
-        See https://ckipnlp.readthedocs.io/ for full documentation.
-        
-        License
-        -------
-        
-        |GPL-3.0|
-        
-        Copyright (c) 2018-2020 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
-        
-        .. |GPL-3.0| image:: https://www.gnu.org/graphics/gplv3-with-text-136x68.png
-           :target: https://www.gnu.org/licenses/gpl-3.0.html
-        
 Platform: linux_x86_64
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -170,7 +20,158 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: Chinese (Traditional)
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: classic
 Provides-Extra: tagger
 Provides-Extra: tagger-gpu
+License-File: LICENSE
+
+CKIP CoreNLP Toolkit
+--------------------
+
+Features
+^^^^^^^^
+
+- Sentence Segmentation
+- Word Segmentation
+- Part-of-Speech Tagging
+- Named-Entity Recognition
+- Constituency Parsing
+- Coreference Resolution
+
+Git
+^^^
+
+https://github.com/ckiplab/ckipnlp
+
+|GitHub Version| |GitHub Release| |GitHub Issues|
+
+.. |GitHub Version| image:: https://img.shields.io/github/v/release/ckiplab/ckipnlp.svg?maxAge=3600
+   :target: https://github.com/ckiplab/ckipnlp/releases
+
+.. |GitHub License| image:: https://img.shields.io/github/license/ckiplab/ckipnlp.svg?maxAge=3600
+   :target: https://github.com/ckiplab/ckipnlp/blob/master/LICENSE
+
+.. |GitHub Release| image:: https://img.shields.io/github/release-date/ckiplab/ckipnlp.svg?maxAge=3600
+
+.. |GitHub Downloads| image:: https://img.shields.io/github/downloads/ckiplab/ckipnlp/total.svg?maxAge=3600
+   :target: https://github.com/ckiplab/ckipnlp/releases/latest
+
+.. |GitHub Issues| image:: https://img.shields.io/github/issues/ckiplab/ckipnlp.svg?maxAge=3600
+   :target: https://github.com/ckiplab/ckipnlp/issues
+
+.. |GitHub Forks| image:: https://img.shields.io/github/forks/ckiplab/ckipnlp.svg?style=social&label=Fork&maxAge=3600
+
+.. |GitHub Stars| image:: https://img.shields.io/github/stars/ckiplab/ckipnlp.svg?style=social&label=Star&maxAge=3600
+
+.. |GitHub Watchers| image:: https://img.shields.io/github/watchers/ckiplab/ckipnlp.svg?style=social&label=Watch&maxAge=3600
+
+PyPI
+^^^^
+
+https://pypi.org/project/ckipnlp
+
+|PyPI Version| |PyPI License| |PyPI Downloads| |PyPI Python| |PyPI Implementation| |PyPI Status|
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/ckipnlp.svg?maxAge=3600
+   :target: https://pypi.org/project/ckipnlp
+
+.. |PyPI License| image:: https://img.shields.io/pypi/l/ckipnlp.svg?maxAge=3600
+   :target: https://github.com/ckiplab/ckipnlp/blob/master/LICENSE
+
+.. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/ckipnlp.svg?maxAge=3600
+   :target: https://pypi.org/project/ckipnlp#files
+
+.. |PyPI Python| image:: https://img.shields.io/pypi/pyversions/ckipnlp.svg?maxAge=3600
+
+.. |PyPI Implementation| image:: https://img.shields.io/pypi/implementation/ckipnlp.svg?maxAge=3600
+
+.. |PyPI Format| image:: https://img.shields.io/pypi/format/ckipnlp.svg?maxAge=3600
+
+.. |PyPI Status| image:: https://img.shields.io/pypi/status/ckipnlp.svg?maxAge=3600
+
+Documentation
+^^^^^^^^^^^^^
+
+https://ckipnlp.readthedocs.io/
+
+|ReadTheDocs Home|
+
+.. |ReadTheDocs Home| image:: https://img.shields.io/website/https/ckipnlp.readthedocs.io.svg?maxAge=3600&up_message=online&down_message=offline
+   :target: https://ckipnlp.readthedocs.io
+
+Online Demo
+^^^^^^^^^^^
+
+https://ckip.iis.sinica.edu.tw/service/corenlp
+
+Contributers
+^^^^^^^^^^^^
+
+* `Mu Yang <https://muyang.pro>`__ at `CKIP <https://ckip.iis.sinica.edu.tw>`__ (Author & Maintainer)
+* `Wei-Yun Ma <https://www.iis.sinica.edu.tw/pages/ma/>`__ at `CKIP <https://ckip.iis.sinica.edu.tw>`__ (Maintainer)
+* `DouglasWu <dgrey1116@gmail.com>`__
+
+Installation
+------------
+
+Requirements
+^^^^^^^^^^^^
+
+* `Python <https://www.python.org>`__ 3.6+
+* `TreeLib <https://treelib.readthedocs.io>`__ 1.5+
+* `CkipTagger <https://pypi.org/project/ckiptagger>`__ 0.2.1+ [Optional, Recommended]
+* `CkipClassic <https://ckip-classic.readthedocs.io>`__ 1.0+ [Optional, Recommended]
+* `TensorFlow / TensorFlow-GPU <https://www.tensorflow.org/>`__ 1.13.1+ [Required by CkipTagger]
+
+Driver Requirements
+^^^^^^^^^^^^^^^^^^^
+
+================================  ========  ==========  ===========
+Driver                            Built-in  CkipTagger  CkipClassic
+================================  ========  ==========  ===========
+Sentence Segmentation             ✔
+Word Segmentation†                          ✔           ✔
+Part-of-Speech Tagging†                     ✔           ✔
+Constituency Parsing                                    ✔
+Named-Entity Recognition                    ✔
+Coreference Resolution‡           ✔         ✔           ✔
+================================  ========  ==========  ===========
+
+- † These drivers require only one of either backends.
+- ‡ Coreference implementation does not require any backend, but requires results from word segmentation, part-of-speech tagging, constituency parsing, and named-entity recognition.
+
+Installation via Pip
+^^^^^^^^^^^^^^^^^^^^
+
+- No backend (not recommended): ``pip install ckipnlp``.
+- With CkipTagger backend (recommended): ``pip install ckipnlp[tagger]`` or ``pip install ckipnlp[tagger-gpu]``.
+- With CkipClassic Parser Client backend (recommended): ``pip install ckipnlp[classic]``.
+- With CkipClassic offline backend: Please refer https://ckip-classic.readthedocs.io/en/latest/main/readme.html#installation for CkipClassic installation guide.
+
+.. attention::
+   To use CkipClassic Parser Client backend, please
+
+   #. Register an account at http://parser.iis.sinica.edu.tw/v1/reg.php
+   #. Set the username and password in the pipeline's options:
+
+   .. code-block:: python
+
+      pipeline = CkipPipeline(opts={'con_parser': {'username': YOUR_USERNAME, 'password': YOUR_PASSWORD})
+
+
+
+Detail
+------
+
+See https://ckipnlp.readthedocs.io/ for full documentation.
+
+License
+-------
+
+|GPL-3.0|
+
+Copyright (c) 2018-2023 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
+
+.. |GPL-3.0| image:: https://www.gnu.org/graphics/gplv3-with-text-136x68.png
+   :target: https://www.gnu.org/licenses/gpl-3.0.html
```

