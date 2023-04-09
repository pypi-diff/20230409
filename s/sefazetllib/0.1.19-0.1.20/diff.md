# Comparing `tmp/sefazetllib-0.1.19.tar.gz` & `tmp/sefazetllib-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sefazetllib-0.1.19.tar", max compression
+gzip compressed data, was "sefazetllib-0.1.20.tar", max compression
```

## Comparing `sefazetllib-0.1.19.tar` & `sefazetllib-0.1.20.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    10349 2023-03-22 02:02:06.498182 sefazetllib-0.1.19/LICENSE
--rw-r--r--   0        0        0     2407 2023-04-09 16:41:18.304044 sefazetllib-0.1.19/pyproject.toml
--rw-r--r--   0        0        0     3262 2023-04-08 23:34:38.918442 sefazetllib-0.1.19/README.md
--rw-r--r--   0        0        0      137 2023-03-22 11:22:30.166093 sefazetllib-0.1.19/sefazetllib/__init__.py
--rw-r--r--   0        0        0     1716 2023-03-22 11:35:33.508530 sefazetllib-0.1.19/sefazetllib/Builder.py
--rw-r--r--   0        0        0       53 2023-03-22 11:18:45.691953 sefazetllib-0.1.19/sefazetllib/config/__init__.py
--rw-r--r--   0        0        0     2415 2023-03-28 02:16:14.475807 sefazetllib-0.1.19/sefazetllib/config/CustomLogging.py
--rw-r--r--   0        0        0       37 2023-03-22 02:03:33.079166 sefazetllib-0.1.19/sefazetllib/etl/__init__.py
--rw-r--r--   0        0        0     8363 2023-03-28 02:16:14.477806 sefazetllib-0.1.19/sefazetllib/etl/ETL.py
--rw-r--r--   0        0        0      279 2023-03-22 11:23:55.081767 sefazetllib-0.1.19/sefazetllib/extract/__init__.py
--rw-r--r--   0        0        0      729 2023-03-22 11:35:33.511528 sefazetllib-0.1.19/sefazetllib/extract/Extract.py
--rw-r--r--   0        0        0     2047 2023-03-22 11:35:33.512538 sefazetllib-0.1.19/sefazetllib/extract/ExtractLocal.py
--rw-r--r--   0        0        0     2552 2023-03-24 02:29:17.874836 sefazetllib-0.1.19/sefazetllib/extract/ExtractS3.py
--rw-r--r--   0        0        0     2600 2023-03-22 11:24:35.794185 sefazetllib-0.1.19/sefazetllib/extract/ExtractSQL.py
--rw-r--r--   0        0        0     2351 2023-03-22 11:35:33.515528 sefazetllib-0.1.19/sefazetllib/extract/ExtractStorage.py
--rw-r--r--   0        0        0       91 2023-03-22 02:17:48.512311 sefazetllib-0.1.19/sefazetllib/factory/__init__.py
--rw-r--r--   0        0        0      967 2023-03-22 11:35:33.517536 sefazetllib-0.1.19/sefazetllib/factory/Factory.py
--rw-r--r--   0        0        0      272 2023-03-22 11:24:56.091205 sefazetllib-0.1.19/sefazetllib/factory/platform/__init__.py
--rw-r--r--   0        0        0      137 2023-03-22 11:27:14.887522 sefazetllib-0.1.19/sefazetllib/factory/platform/database/__init__.py
--rw-r--r--   0        0        0      749 2023-03-22 11:35:33.520527 sefazetllib-0.1.19/sefazetllib/factory/platform/database/MySQL.py
--rw-r--r--   0        0        0      814 2023-03-22 11:28:00.370816 sefazetllib-0.1.19/sefazetllib/factory/platform/database/PostgresSQL.py
--rw-r--r--   0        0        0      380 2023-03-22 11:25:06.491132 sefazetllib-0.1.19/sefazetllib/factory/platform/DatabasePlatform.py
--rw-r--r--   0        0        0      198 2023-03-22 11:28:08.380181 sefazetllib-0.1.19/sefazetllib/factory/platform/dataframe/__init__.py
--rw-r--r--   0        0        0      272 2023-03-22 11:35:33.522527 sefazetllib-0.1.19/sefazetllib/factory/platform/dataframe/Default.py
--rw-r--r--   0        0        0     1854 2023-03-22 11:35:33.523528 sefazetllib-0.1.19/sefazetllib/factory/platform/dataframe/Pandas.py
--rw-r--r--   0        0        0     4220 2023-04-08 00:24:55.746715 sefazetllib-0.1.19/sefazetllib/factory/platform/dataframe/Spark.py
--rw-r--r--   0        0        0      297 2023-03-22 11:35:33.518538 sefazetllib-0.1.19/sefazetllib/factory/platform/Platform.py
--rw-r--r--   0        0        0     1077 2023-03-22 11:27:04.493215 sefazetllib-0.1.19/sefazetllib/factory/platform/PlatformFactory.py
--rw-r--r--   0        0        0      234 2023-03-22 11:35:33.533527 sefazetllib-0.1.19/sefazetllib/load/__init__.py
--rw-r--r--   0        0        0      711 2023-03-22 11:35:33.526527 sefazetllib-0.1.19/sefazetllib/load/Load.py
--rw-r--r--   0        0        0     2077 2023-03-22 11:35:33.528526 sefazetllib-0.1.19/sefazetllib/load/LoadLocal.py
--rw-r--r--   0        0        0     2372 2023-03-22 11:35:33.529528 sefazetllib-0.1.19/sefazetllib/load/LoadS3.py
--rw-r--r--   0        0        0     2835 2023-03-22 11:35:33.531566 sefazetllib-0.1.19/sefazetllib/load/LoadSQL.py
--rw-r--r--   0        0        0     2261 2023-03-22 11:35:33.532526 sefazetllib-0.1.19/sefazetllib/load/LoadStorage.py
--rw-r--r--   0        0        0      201 2023-03-22 02:12:37.861367 sefazetllib-0.1.19/sefazetllib/transform/__init__.py
--rw-r--r--   0        0        0     1523 2023-03-22 02:15:28.119480 sefazetllib-0.1.19/sefazetllib/transform/MinMaxLineTransform.py
--rw-r--r--   0        0        0     4445 2023-04-08 00:24:55.749710 sefazetllib-0.1.19/sefazetllib/transform/QuartileTransform.py
--rw-r--r--   0        0        0      577 2023-03-22 11:35:33.535526 sefazetllib-0.1.19/sefazetllib/transform/Transform.py
--rw-r--r--   0        0        0       46 2023-03-22 02:08:23.799891 sefazetllib-0.1.19/sefazetllib/utils/__init__.py
--rw-r--r--   0        0        0      161 2023-03-22 02:03:33.166061 sefazetllib-0.1.19/sefazetllib/utils/key/__init__.py
--rw-r--r--   0        0        0      339 2023-03-22 11:35:33.536528 sefazetllib-0.1.19/sefazetllib/utils/key/DefaultKey.py
--rw-r--r--   0        0        0      419 2023-03-22 11:35:33.537527 sefazetllib-0.1.19/sefazetllib/utils/key/Key.py
--rw-r--r--   0        0        0      775 2023-03-22 11:35:33.538526 sefazetllib-0.1.19/sefazetllib/utils/key/SurrogateKey.py
--rw-r--r--   0        0        0      234 2023-03-22 02:03:33.178225 sefazetllib-0.1.19/sefazetllib/utils/partition/__init__.py
--rw-r--r--   0        0        0     2172 2023-03-22 11:21:12.190698 sefazetllib-0.1.19/sefazetllib/utils/partition/DatePartition.py
--rw-r--r--   0        0        0      652 2023-03-22 11:21:29.374214 sefazetllib-0.1.19/sefazetllib/utils/partition/IncrementalRangePartition.py
--rw-r--r--   0        0        0      447 2023-03-22 11:35:33.539526 sefazetllib-0.1.19/sefazetllib/utils/partition/Partition.py
--rw-r--r--   0        0        0      112 2023-03-22 11:35:33.543527 sefazetllib-0.1.19/sefazetllib/validate/__init__.py
--rw-r--r--   0        0        0     7843 2023-03-22 11:35:33.541526 sefazetllib-0.1.19/sefazetllib/validate/DataValidate.py
--rw-r--r--   0        0        0      122 2023-03-22 11:35:33.542530 sefazetllib-0.1.19/sefazetllib/validate/Validate.py
--rw-r--r--   0        0        0     4539 1970-01-01 00:00:00.000000 sefazetllib-0.1.19/setup.py
--rw-r--r--   0        0        0     4859 1970-01-01 00:00:00.000000 sefazetllib-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0    10349 2023-03-22 02:02:06.498182 sefazetllib-0.1.20/LICENSE
+-rw-r--r--   0        0        0     2409 2023-04-09 17:12:29.001631 sefazetllib-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0     3262 2023-04-08 23:34:38.918442 sefazetllib-0.1.20/README.md
+-rw-r--r--   0        0        0      137 2023-03-22 11:22:30.166093 sefazetllib-0.1.20/sefazetllib/__init__.py
+-rw-r--r--   0        0        0     1716 2023-03-22 11:35:33.508530 sefazetllib-0.1.20/sefazetllib/Builder.py
+-rw-r--r--   0        0        0       53 2023-03-22 11:18:45.691953 sefazetllib-0.1.20/sefazetllib/config/__init__.py
+-rw-r--r--   0        0        0     2415 2023-03-28 02:16:14.475807 sefazetllib-0.1.20/sefazetllib/config/CustomLogging.py
+-rw-r--r--   0        0        0       37 2023-03-22 02:03:33.079166 sefazetllib-0.1.20/sefazetllib/etl/__init__.py
+-rw-r--r--   0        0        0     8363 2023-03-28 02:16:14.477806 sefazetllib-0.1.20/sefazetllib/etl/ETL.py
+-rw-r--r--   0        0        0      279 2023-03-22 11:23:55.081767 sefazetllib-0.1.20/sefazetllib/extract/__init__.py
+-rw-r--r--   0        0        0      729 2023-03-22 11:35:33.511528 sefazetllib-0.1.20/sefazetllib/extract/Extract.py
+-rw-r--r--   0        0        0     2047 2023-03-22 11:35:33.512538 sefazetllib-0.1.20/sefazetllib/extract/ExtractLocal.py
+-rw-r--r--   0        0        0     2552 2023-03-24 02:29:17.874836 sefazetllib-0.1.20/sefazetllib/extract/ExtractS3.py
+-rw-r--r--   0        0        0     2600 2023-03-22 11:24:35.794185 sefazetllib-0.1.20/sefazetllib/extract/ExtractSQL.py
+-rw-r--r--   0        0        0     2351 2023-03-22 11:35:33.515528 sefazetllib-0.1.20/sefazetllib/extract/ExtractStorage.py
+-rw-r--r--   0        0        0       91 2023-03-22 02:17:48.512311 sefazetllib-0.1.20/sefazetllib/factory/__init__.py
+-rw-r--r--   0        0        0      967 2023-03-22 11:35:33.517536 sefazetllib-0.1.20/sefazetllib/factory/Factory.py
+-rw-r--r--   0        0        0      272 2023-03-22 11:24:56.091205 sefazetllib-0.1.20/sefazetllib/factory/platform/__init__.py
+-rw-r--r--   0        0        0      137 2023-03-22 11:27:14.887522 sefazetllib-0.1.20/sefazetllib/factory/platform/database/__init__.py
+-rw-r--r--   0        0        0      749 2023-03-22 11:35:33.520527 sefazetllib-0.1.20/sefazetllib/factory/platform/database/MySQL.py
+-rw-r--r--   0        0        0      814 2023-03-22 11:28:00.370816 sefazetllib-0.1.20/sefazetllib/factory/platform/database/PostgresSQL.py
+-rw-r--r--   0        0        0      380 2023-03-22 11:25:06.491132 sefazetllib-0.1.20/sefazetllib/factory/platform/DatabasePlatform.py
+-rw-r--r--   0        0        0      198 2023-03-22 11:28:08.380181 sefazetllib-0.1.20/sefazetllib/factory/platform/dataframe/__init__.py
+-rw-r--r--   0        0        0      272 2023-03-22 11:35:33.522527 sefazetllib-0.1.20/sefazetllib/factory/platform/dataframe/Default.py
+-rw-r--r--   0        0        0     1854 2023-03-22 11:35:33.523528 sefazetllib-0.1.20/sefazetllib/factory/platform/dataframe/Pandas.py
+-rw-r--r--   0        0        0     4220 2023-04-08 00:24:55.746715 sefazetllib-0.1.20/sefazetllib/factory/platform/dataframe/Spark.py
+-rw-r--r--   0        0        0      297 2023-03-22 11:35:33.518538 sefazetllib-0.1.20/sefazetllib/factory/platform/Platform.py
+-rw-r--r--   0        0        0     1077 2023-03-22 11:27:04.493215 sefazetllib-0.1.20/sefazetllib/factory/platform/PlatformFactory.py
+-rw-r--r--   0        0        0      234 2023-03-22 11:35:33.533527 sefazetllib-0.1.20/sefazetllib/load/__init__.py
+-rw-r--r--   0        0        0      711 2023-03-22 11:35:33.526527 sefazetllib-0.1.20/sefazetllib/load/Load.py
+-rw-r--r--   0        0        0     2077 2023-03-22 11:35:33.528526 sefazetllib-0.1.20/sefazetllib/load/LoadLocal.py
+-rw-r--r--   0        0        0     2372 2023-03-22 11:35:33.529528 sefazetllib-0.1.20/sefazetllib/load/LoadS3.py
+-rw-r--r--   0        0        0     2835 2023-03-22 11:35:33.531566 sefazetllib-0.1.20/sefazetllib/load/LoadSQL.py
+-rw-r--r--   0        0        0     2261 2023-03-22 11:35:33.532526 sefazetllib-0.1.20/sefazetllib/load/LoadStorage.py
+-rw-r--r--   0        0        0      201 2023-03-22 02:12:37.861367 sefazetllib-0.1.20/sefazetllib/transform/__init__.py
+-rw-r--r--   0        0        0     1523 2023-03-22 02:15:28.119480 sefazetllib-0.1.20/sefazetllib/transform/MinMaxLineTransform.py
+-rw-r--r--   0        0        0     4445 2023-04-08 00:24:55.749710 sefazetllib-0.1.20/sefazetllib/transform/QuartileTransform.py
+-rw-r--r--   0        0        0      577 2023-03-22 11:35:33.535526 sefazetllib-0.1.20/sefazetllib/transform/Transform.py
+-rw-r--r--   0        0        0       46 2023-03-22 02:08:23.799891 sefazetllib-0.1.20/sefazetllib/utils/__init__.py
+-rw-r--r--   0        0        0      161 2023-03-22 02:03:33.166061 sefazetllib-0.1.20/sefazetllib/utils/key/__init__.py
+-rw-r--r--   0        0        0      339 2023-03-22 11:35:33.536528 sefazetllib-0.1.20/sefazetllib/utils/key/DefaultKey.py
+-rw-r--r--   0        0        0      419 2023-03-22 11:35:33.537527 sefazetllib-0.1.20/sefazetllib/utils/key/Key.py
+-rw-r--r--   0        0        0      775 2023-03-22 11:35:33.538526 sefazetllib-0.1.20/sefazetllib/utils/key/SurrogateKey.py
+-rw-r--r--   0        0        0      234 2023-03-22 02:03:33.178225 sefazetllib-0.1.20/sefazetllib/utils/partition/__init__.py
+-rw-r--r--   0        0        0     2172 2023-03-22 11:21:12.190698 sefazetllib-0.1.20/sefazetllib/utils/partition/DatePartition.py
+-rw-r--r--   0        0        0      652 2023-03-22 11:21:29.374214 sefazetllib-0.1.20/sefazetllib/utils/partition/IncrementalRangePartition.py
+-rw-r--r--   0        0        0      447 2023-03-22 11:35:33.539526 sefazetllib-0.1.20/sefazetllib/utils/partition/Partition.py
+-rw-r--r--   0        0        0      112 2023-03-22 11:35:33.543527 sefazetllib-0.1.20/sefazetllib/validate/__init__.py
+-rw-r--r--   0        0        0     7843 2023-03-22 11:35:33.541526 sefazetllib-0.1.20/sefazetllib/validate/DataValidate.py
+-rw-r--r--   0        0        0      122 2023-03-22 11:35:33.542530 sefazetllib-0.1.20/sefazetllib/validate/Validate.py
+-rw-r--r--   0        0        0     4539 1970-01-01 00:00:00.000000 sefazetllib-0.1.20/setup.py
+-rw-r--r--   0        0        0     4859 1970-01-01 00:00:00.000000 sefazetllib-0.1.20/PKG-INFO
```

### Comparing `sefazetllib-0.1.19/LICENSE` & `sefazetllib-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/pyproject.toml` & `sefazetllib-0.1.20/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sefazetllib"
-version = "0.1.19"
+version = "0.1.20"
 description = "sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines."
 license = "Apache-2.0"
 authors = ["Felipe Gochi <felipe.gochi@elogroup.com.br>"]
 maintainers = [
     "Bruno Santos <bruno.santos@elogroup.com.br>",
     "Felipe Alcantara <felipe.alcantara@elogroup.com.br>",
     "Felipe Gochi <felipe.gochi@elogroup.com.br>",
@@ -36,43 +36,43 @@
 packages = [{ include = "sefazetllib" }]
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 pandas = "^1.3"
 pyarrow = "^6.0"
 pydeequ = "^1.0"
-boto3 = "^1.26"
+boto3 = "^1.24"
 
 [tool.poetry.group.test.dependencies]
 python = "^3.7.1"
 pandas = "^1.3"
 pyarrow = "^6.0"
 pyspark = "^3.0"
 pydeequ = "^1.0"
-boto3 = "^1.26"
+boto3 = "^1.24"
 mypy = "^1.0"
 isort = "^5.11"
-black = "^23.1"
+black = "^22.10"
 
 [tool.poetry.group.docs.dependencies]
 python = "^3.7.1"
 mkdocs = "^1.4"
 mkdocs-material = "^9.0"
 mkdocs-material-extensions = "^1.1"
 
 [tool.poetry.group.dev.dependencies]
 python = "^3.7.1"
 pandas = "^1.3"
 pyarrow = "^6.0"
 pyspark = "^3.0"
 pydeequ = "^1.0"
-boto3 = "^1.26"
+boto3 = "^1.24"
 mypy = "^1.0"
 isort = "^5.11"
-black = "^23.1"
+black = "^22.10"
 mkdocs = "^1.4"
 mkdocs-material = "^9.0"
 mkdocs-material-extensions = "^1.1"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sefazetllib-0.1.19/README.md` & `sefazetllib-0.1.20/README.md`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/Builder.py` & `sefazetllib-0.1.20/sefazetllib/Builder.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/config/CustomLogging.py` & `sefazetllib-0.1.20/sefazetllib/config/CustomLogging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/etl/ETL.py` & `sefazetllib-0.1.20/sefazetllib/etl/ETL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/extract/Extract.py` & `sefazetllib-0.1.20/sefazetllib/extract/Extract.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/extract/ExtractLocal.py` & `sefazetllib-0.1.20/sefazetllib/extract/ExtractLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/extract/ExtractS3.py` & `sefazetllib-0.1.20/sefazetllib/extract/ExtractS3.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/extract/ExtractSQL.py` & `sefazetllib-0.1.20/sefazetllib/extract/ExtractSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/extract/ExtractStorage.py` & `sefazetllib-0.1.20/sefazetllib/extract/ExtractStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/factory/Factory.py` & `sefazetllib-0.1.20/sefazetllib/factory/Factory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/factory/platform/database/MySQL.py` & `sefazetllib-0.1.20/sefazetllib/factory/platform/database/MySQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/factory/platform/database/PostgresSQL.py` & `sefazetllib-0.1.20/sefazetllib/factory/platform/database/PostgresSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/factory/platform/dataframe/Pandas.py` & `sefazetllib-0.1.20/sefazetllib/factory/platform/dataframe/Pandas.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/factory/platform/dataframe/Spark.py` & `sefazetllib-0.1.20/sefazetllib/factory/platform/dataframe/Spark.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/factory/platform/PlatformFactory.py` & `sefazetllib-0.1.20/sefazetllib/factory/platform/PlatformFactory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/load/Load.py` & `sefazetllib-0.1.20/sefazetllib/load/Load.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/load/LoadLocal.py` & `sefazetllib-0.1.20/sefazetllib/load/LoadLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/load/LoadS3.py` & `sefazetllib-0.1.20/sefazetllib/load/LoadS3.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/load/LoadSQL.py` & `sefazetllib-0.1.20/sefazetllib/load/LoadSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/load/LoadStorage.py` & `sefazetllib-0.1.20/sefazetllib/load/LoadStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/transform/MinMaxLineTransform.py` & `sefazetllib-0.1.20/sefazetllib/transform/MinMaxLineTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/transform/QuartileTransform.py` & `sefazetllib-0.1.20/sefazetllib/transform/QuartileTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/transform/Transform.py` & `sefazetllib-0.1.20/sefazetllib/transform/Transform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/utils/key/SurrogateKey.py` & `sefazetllib-0.1.20/sefazetllib/utils/key/SurrogateKey.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/utils/partition/DatePartition.py` & `sefazetllib-0.1.20/sefazetllib/utils/partition/DatePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/utils/partition/IncrementalRangePartition.py` & `sefazetllib-0.1.20/sefazetllib/utils/partition/IncrementalRangePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/sefazetllib/validate/DataValidate.py` & `sefazetllib-0.1.20/sefazetllib/validate/DataValidate.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.19/setup.py` & `sefazetllib-0.1.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,22 @@
  'sefazetllib.utils.partition',
  'sefazetllib.validate']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['boto3>=1.26,<2.0',
+['boto3>=1.24,<2.0',
  'pandas>=1.3,<2.0',
  'pyarrow>=6.0,<7.0',
  'pydeequ>=1.0,<2.0']
 
 setup_kwargs = {
     'name': 'sefazetllib',
-    'version': '0.1.19',
+    'version': '0.1.20',
     'description': 'sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.',
     'long_description': '# sefazetllib\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n---\n\n**Documentation**: [https://main.d32to2oidohzrl.amplifyapp.com/](https://main.d32to2oidohzrl.amplifyapp.com/)\n\n**Source code**: [AWS CodeCommit](https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1)\n\n---\n\n**sefazetllib** is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.\n\n## Features\n\n- Easy to use and understand library for constructing ETL/ELT pipelines.\n- Compatibility with popular data processing frameworks, such as [pandas](https://pandas.pydata.org/) and [PySpark](https://spark.apache.org/).\n- Support for file formats such as CSV and Parquet.\n- Provides the ability to extract, transform and load data with customizable configurations.\n\n## Requirements\n\n**sefazetllib** requires the following to run:\n\n- [Python](https://www.python.org/) 3.8+\n- [pandas](https://pandas.pydata.org/) 1.4+\n- [PyArrow](https://arrow.apache.org/) 6.0+\n- [PySpark](https://spark.apache.org/) 3.2+\n- [PyDeequ](https://pydeequ.readthedocs.io/) 1.0+\n- [Boto3](https://github.com/boto/boto3) 1.26+\n\n## Installation\n\nUse [pip](https://pip.pypa.io/en/stable/) to install **sefazetllib**:\n\n```bash\npip install sefazetllib\n```\n\n## Usage\n\nHere is an example of how to use the **sefazetllib**:\n\n```Python\nfrom typing import Tuple\n\nfrom pandas import DataFrame\n\nfrom sefazetllib import Builder\nfrom sefazetllib.etl import ETL\nfrom sefazetllib.extract import ExtractLocal\nfrom sefazetllib.factory.platform import PlatformFactory\nfrom sefazetllib.load import LoadLocal\nfrom sefazetllib.transform import Transform\nfrom sefazetllib.utils.key import SurrogateKey\n\n\n@Builder\nclass TestingDataFrame(Transform):\n    def execute(self) -> Tuple[str, DataFrame]:\n        return (\n            "dataframe",\n            DataFrame(\n                [["tom", 10], ["nick", 15], ["juli", 14]], columns=["Name", "Age"]\n            ),\n        )\n\n\n(\n    ETL()\n    .setPlatform(PlatformFactory("Pandas").create(name="test_pandas"))\n    .transform(TestingDataFrame)\n    .load(\n        LoadLocal()\n        .setFileFormat("parquet")\n        .setEntity("load_test")\n        .setMode("overwrite")\n        .setReference("dataframe")\n        .setDuplicates(True)\n        .setKey(SurrogateKey().setColumns(["Name", "Age"]).setDistribute(False))\n    )\n    .extract(\n        ExtractLocal()\n        .setFileFormat("parquet")\n        .setUrl("load_test.parquet")\n        .setReference("extract_test")\n    )\n)\n```\n\n## Testing\n\nTo run the unit tests, run the following command:\n\n```bash\npy -m unittest tests/main.py -v\n```\n\n## License\n\n**sefazetllib** is released under the [Apache-2.0](/LICENSE).\n',
     'author': 'Felipe Gochi',
     'author_email': 'felipe.gochi@elogroup.com.br',
     'maintainer': 'Bruno Santos',
     'maintainer_email': 'bruno.santos@elogroup.com.br',
     'url': 'https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1',
```

### Comparing `sefazetllib-0.1.19/PKG-INFO` & `sefazetllib-0.1.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sefazetllib
-Version: 0.1.19
+Version: 0.1.20
 Summary: sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
 Home-page: https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
 License: Apache-2.0
 Author: Felipe Gochi
 Author-email: felipe.gochi@elogroup.com.br
 Maintainer: Bruno Santos
 Maintainer-email: bruno.santos@elogroup.com.br
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: boto3 (>=1.26,<2.0)
+Requires-Dist: boto3 (>=1.24,<2.0)
 Requires-Dist: pandas (>=1.3,<2.0)
 Requires-Dist: pyarrow (>=6.0,<7.0)
 Requires-Dist: pydeequ (>=1.0,<2.0)
 Project-URL: Documentation, https://main.d32to2oidohzrl.amplifyapp.com/
 Project-URL: Repository, https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
 Description-Content-Type: text/markdown
```

