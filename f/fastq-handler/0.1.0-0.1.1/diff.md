# Comparing `tmp/fastq_handler-0.1.0.tar.gz` & `tmp/fastq_handler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastq_handler-0.1.0.tar", max compression
+gzip compressed data, was "fastq_handler-0.1.1.tar", max compression
```

## Comparing `fastq_handler-0.1.0.tar` & `fastq_handler-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    31904 2023-04-08 10:54:25.406907 fastq_handler-0.1.0/LICENSE
--rw-r--r--   0        0        0      670 2023-04-08 11:11:03.146664 fastq_handler-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      214 2023-04-08 11:18:53.731779 fastq_handler-0.1.0/src/fastq_handler/__init__.py
--rw-r--r--   0        0        0     1411 2023-04-08 11:23:52.682224 fastq_handler-0.1.0/src/fastq_handler/__main__.py
--rw-r--r--   0        0        0    14948 2023-04-06 16:59:47.945976 fastq_handler-0.1.0/src/fastq_handler/fastq_handler.py
--rw-r--r--   0        0        0     7660 2023-04-06 16:59:47.945976 fastq_handler-0.1.0/src/fastq_handler/records.py
--rw-r--r--   0        0        0     3984 2023-04-06 16:59:47.945976 fastq_handler-0.1.0/src/fastq_handler/utilities.py
--rw-r--r--   0        0        0      956 2023-04-08 11:24:08.203563 fastq_handler-0.1.0/setup.py
--rw-r--r--   0        0        0      587 2023-04-08 11:24:08.203809 fastq_handler-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    31904 2023-04-08 10:54:25.406907 fastq_handler-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1735 2023-04-09 21:29:09.259248 fastq_handler-0.1.1/README.md
+-rw-r--r--   0        0        0      708 2023-04-09 21:38:13.624503 fastq_handler-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      214 2023-04-08 11:18:53.731779 fastq_handler-0.1.1/src/fastq_handler/__init__.py
+-rw-r--r--   0        0        0     1411 2023-04-09 21:28:47.254284 fastq_handler-0.1.1/src/fastq_handler/__main__.py
+-rw-r--r--   0        0        0    14948 2023-04-06 16:59:47.945976 fastq_handler-0.1.1/src/fastq_handler/fastq_handler.py
+-rw-r--r--   0        0        0     7660 2023-04-06 16:59:47.945976 fastq_handler-0.1.1/src/fastq_handler/records.py
+-rw-r--r--   0        0        0     3984 2023-04-06 16:59:47.945976 fastq_handler-0.1.1/src/fastq_handler/utilities.py
+-rw-r--r--   0        0        0     2752 2023-04-09 21:38:19.521533 fastq_handler-0.1.1/setup.py
+-rw-r--r--   0        0        0     2428 2023-04-09 21:38:19.522091 fastq_handler-0.1.1/PKG-INFO
```

### Comparing `fastq_handler-0.1.0/LICENSE` & `fastq_handler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastq_handler-0.1.0/pyproject.toml` & `fastq_handler-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "fastq_handler"
-version = "0.1.0"
+version = "0.1.1"
 description = "A python module to process minion fastq files by concatenating reads as they are generated"
 authors = ["SantosJGND <dourado.jns@gmail.com>", "Andre Santos <xiaodre2112@gmail.com>", "insapathogenomics <insapathogenomics@insa.min-saude.pt>"]
+license = "MIT"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dataclasses = "0.6"
 natsort = "8.3.1"
 pandas = "1.5.3"
 pip = "21.2.3"
@@ -17,8 +19,8 @@
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-fastq_handler = "fastq_handler.__main__:main"
+fastq_handler = "fastq_handler.__main__:main"
```

### Comparing `fastq_handler-0.1.0/src/fastq_handler/__main__.py` & `fastq_handler-0.1.1/src/fastq_handler/__main__.py`

 * *Files identical despite different names*

### Comparing `fastq_handler-0.1.0/src/fastq_handler/fastq_handler.py` & `fastq_handler-0.1.1/src/fastq_handler/fastq_handler.py`

 * *Files identical despite different names*

### Comparing `fastq_handler-0.1.0/src/fastq_handler/records.py` & `fastq_handler-0.1.1/src/fastq_handler/records.py`

 * *Files identical despite different names*

### Comparing `fastq_handler-0.1.0/src/fastq_handler/utilities.py` & `fastq_handler-0.1.1/src/fastq_handler/utilities.py`

 * *Files identical despite different names*

