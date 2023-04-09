# Comparing `tmp/goodcrap-0.2.0.tar.gz` & `tmp/goodcrap-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodcrap-0.2.0.tar", last modified: Fri Apr  7 02:12:01 2023, max compression
+gzip compressed data, was "goodcrap-0.2.1.tar", last modified: Sun Apr  9 16:31:20 2023, max compression
```

## Comparing `goodcrap-0.2.0.tar` & `goodcrap-0.2.1.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.778699 goodcrap-0.2.0/
--rw-rw-rw-   0        0        0       66 2023-03-29 13:09:13.000000 goodcrap-0.2.0/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.686940 goodcrap-0.2.0/.github/
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.716943 goodcrap-0.2.0/.github/workflows/
--rw-rw-rw-   0        0        0      576 2023-04-05 03:09:29.000000 goodcrap-0.2.0/.github/workflows/pylint.yml
--rw-rw-rw-   0        0        0       48 2023-04-05 01:29:51.000000 goodcrap-0.2.0/.gitignore
--rw-rw-rw-   0        0        0      332 2023-04-07 02:10:51.000000 goodcrap-0.2.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-04-05 01:05:21.000000 goodcrap-0.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0    35802 2023-03-29 13:09:13.000000 goodcrap-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      193 2023-04-07 02:11:43.000000 goodcrap-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10765 2023-04-07 02:12:01.780197 goodcrap-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10131 2023-04-07 02:02:32.000000 goodcrap-0.2.0/README.md
--rw-rw-rw-   0        0        0        5 2023-04-07 02:10:55.000000 goodcrap-0.2.0/VERSION
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.720120 goodcrap-0.2.0/examples/
--rw-rw-rw-   0        0        0      139 2023-04-04 14:07:32.000000 goodcrap-0.2.0/examples/mysql_config.json
--rw-rw-rw-   0        0        0       59 2023-04-05 01:09:16.000000 goodcrap-0.2.0/examples/sqlite_config.json
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.726120 goodcrap-0.2.0/goodcrap/
--rw-rw-rw-   0        0        0       87 2023-04-07 02:06:54.000000 goodcrap-0.2.0/goodcrap/__init__.py
--rw-rw-rw-   0        0        0       72 2023-04-04 00:49:25.000000 goodcrap-0.2.0/goodcrap/__main__.py
--rw-rw-rw-   0        0        0     5212 2023-04-06 16:34:32.000000 goodcrap-0.2.0/goodcrap/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.752675 goodcrap-0.2.0/goodcrap/crappers/
--rw-rw-rw-   0        0        0     1021 2023-04-06 04:35:52.000000 goodcrap-0.2.0/goodcrap/crappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.754674 goodcrap-0.2.0/goodcrap/data_warehouses/
--rw-rw-rw-   0        0        0        0 2023-04-05 14:10:31.000000 goodcrap-0.2.0/goodcrap/data_warehouses/__init__.py
--rw-rw-rw-   0        0        0       32 2023-04-05 23:18:00.000000 goodcrap-0.2.0/goodcrap/data_warehouses/dimension_fillers.py
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.758982 goodcrap-0.2.0/goodcrap/databases/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:02:02.000000 goodcrap-0.2.0/goodcrap/databases/__init__.py
--rw-rw-rw-   0        0        0     2904 2023-04-06 16:06:51.000000 goodcrap-0.2.0/goodcrap/databases/database.py
--rw-rw-rw-   0        0        0      450 2023-04-05 01:10:52.000000 goodcrap-0.2.0/goodcrap/databases/mysql.py
--rw-rw-rw-   0        0        0      422 2023-04-05 01:11:01.000000 goodcrap-0.2.0/goodcrap/databases/sqlite.py
--rw-rw-rw-   0        0        0    12341 2023-04-07 02:00:54.000000 goodcrap-0.2.0/goodcrap/goodcrap.py
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.760988 goodcrap-0.2.0/goodcrap/pipelines/
--rw-rw-rw-   0        0        0        0 2023-04-05 15:01:30.000000 goodcrap-0.2.0/goodcrap/pipelines/__init__.py
--rw-rw-rw-   0        0        0     3566 2023-04-06 15:52:52.000000 goodcrap-0.2.0/goodcrap/pipelines/mage.py
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.767016 goodcrap-0.2.0/goodcrap/pipelines/templates/
--rw-rw-rw-   0        0        0        0 2023-04-05 15:01:30.000000 goodcrap-0.2.0/goodcrap/pipelines/templates/__init__.py
--rw-rw-rw-   0        0        0     1126 2023-04-06 13:40:38.000000 goodcrap-0.2.0/goodcrap/pipelines/templates/data_exporter_mysql.py
--rw-rw-rw-   0        0        0      683 2023-04-06 15:53:25.000000 goodcrap-0.2.0/goodcrap/pipelines/templates/data_loader.py
--rw-rw-rw-   0        0        0      832 2023-04-06 06:10:32.000000 goodcrap-0.2.0/goodcrap/pipelines/templates/metadata.yaml
--rw-rw-rw-   0        0        0     2519 2023-04-07 01:50:31.000000 goodcrap-0.2.0/goodcrap/random_mapper.py
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.768132 goodcrap-0.2.0/goodcrap/templates/
--rw-rw-rw-   0        0        0        0 2023-03-31 13:15:48.000000 goodcrap-0.2.0/goodcrap/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.769272 goodcrap-0.2.0/goodcrap/templates/__pycache__/
--rw-rw-rw-   0        0        0      143 2023-03-31 13:16:56.000000 goodcrap-0.2.0/goodcrap/templates/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.771278 goodcrap-0.2.0/goodcrap/templates/data_warehouses/
--rw-rw-rw-   0        0        0     7250 2023-04-05 14:08:49.000000 goodcrap-0.2.0/goodcrap/templates/data_warehouses/sales.sql
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.694937 goodcrap-0.2.0/goodcrap/templates/databases/
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.773437 goodcrap-0.2.0/goodcrap/templates/databases/customers_orders/
--rw-rw-rw-   0        0        0      751 2023-04-04 05:53:19.000000 goodcrap-0.2.0/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json
--rw-rw-rw-   0        0        0     1148 2023-04-06 15:06:31.000000 goodcrap-0.2.0/goodcrap/templates/databases/customers_orders/customers_orders.sql
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.696937 goodcrap-0.2.0/goodcrap/templates/tables/
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.776309 goodcrap-0.2.0/goodcrap/templates/tables/customers/
--rw-rw-rw-   0        0        0      562 2023-04-04 23:45:49.000000 goodcrap-0.2.0/goodcrap/templates/tables/customers/customers.crap_labels.json
--rw-rw-rw-   0        0        0      547 2023-04-02 16:03:37.000000 goodcrap-0.2.0/goodcrap/templates/tables/customers/customers.sql
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.778699 goodcrap-0.2.0/goodcrap/templates/tables/orders/
--rw-rw-rw-   0        0        0      244 2023-04-04 04:00:46.000000 goodcrap-0.2.0/goodcrap/templates/tables/orders/orders.crap_labels.json
--rw-rw-rw-   0        0        0      599 2023-04-04 03:59:42.000000 goodcrap-0.2.0/goodcrap/templates/tables/orders/orders.sql
-drwxrwxrwx   0        0        0        0 2023-04-07 02:12:01.750400 goodcrap-0.2.0/goodcrap.egg-info/
--rw-rw-rw-   0        0        0    10765 2023-04-07 02:12:01.000000 goodcrap-0.2.0/goodcrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1458 2023-04-07 02:12:01.000000 goodcrap-0.2.0/goodcrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 02:12:01.000000 goodcrap-0.2.0/goodcrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-07 02:12:01.000000 goodcrap-0.2.0/goodcrap.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-04-07 02:12:01.000000 goodcrap-0.2.0/goodcrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-07 02:12:01.000000 goodcrap-0.2.0/goodcrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      215 2023-04-07 02:12:01.782203 goodcrap-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-04-06 16:31:50.000000 goodcrap-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.443144 goodcrap-0.2.1/
+-rw-rw-rw-   0        0        0       66 2023-03-29 13:09:13.000000 goodcrap-0.2.1/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.371122 goodcrap-0.2.1/.github/
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.392992 goodcrap-0.2.1/.github/workflows/
+-rw-rw-rw-   0        0        0      576 2023-04-05 03:09:29.000000 goodcrap-0.2.1/.github/workflows/pylint.yml
+-rw-rw-rw-   0        0        0       54 2023-04-09 16:29:54.000000 goodcrap-0.2.1/.gitignore
+-rw-rw-rw-   0        0        0      332 2023-04-07 02:10:51.000000 goodcrap-0.2.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-04-05 01:05:21.000000 goodcrap-0.2.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0    35802 2023-03-29 13:09:13.000000 goodcrap-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      193 2023-04-07 02:11:43.000000 goodcrap-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11178 2023-04-09 16:31:20.443144 goodcrap-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10544 2023-04-09 16:30:52.000000 goodcrap-0.2.1/README.md
+-rw-rw-rw-   0        0        0        5 2023-04-08 02:20:55.000000 goodcrap-0.2.1/VERSION
+-rw-rw-rw-   0        0        0    72291 2023-04-07 05:50:59.000000 goodcrap-0.2.1/customers.parquet
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.393124 goodcrap-0.2.1/examples/
+-rw-rw-rw-   0        0        0      139 2023-04-04 14:07:32.000000 goodcrap-0.2.1/examples/mysql_config.json
+-rw-rw-rw-   0        0        0       59 2023-04-05 01:09:16.000000 goodcrap-0.2.1/examples/sqlite_config.json
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.393124 goodcrap-0.2.1/goodcrap/
+-rw-rw-rw-   0        0        0       87 2023-04-08 02:21:05.000000 goodcrap-0.2.1/goodcrap/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-04-04 00:49:25.000000 goodcrap-0.2.1/goodcrap/__main__.py
+-rw-rw-rw-   0        0        0     5755 2023-04-09 15:59:05.000000 goodcrap-0.2.1/goodcrap/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.409045 goodcrap-0.2.1/goodcrap/crappers/
+-rw-rw-rw-   0        0        0     1019 2023-04-08 15:25:53.000000 goodcrap-0.2.1/goodcrap/crappers/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-04-09 16:23:36.000000 goodcrap-0.2.1/goodcrap/crappers/queries.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.409045 goodcrap-0.2.1/goodcrap/data_warehouses/
+-rw-rw-rw-   0        0        0        0 2023-04-05 14:10:31.000000 goodcrap-0.2.1/goodcrap/data_warehouses/__init__.py
+-rw-rw-rw-   0        0        0     2283 2023-04-08 15:13:42.000000 goodcrap-0.2.1/goodcrap/data_warehouses/dimension_featurizer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.426149 goodcrap-0.2.1/goodcrap/databases/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:02:02.000000 goodcrap-0.2.1/goodcrap/databases/__init__.py
+-rw-rw-rw-   0        0        0     3184 2023-04-09 16:30:44.000000 goodcrap-0.2.1/goodcrap/databases/database.py
+-rw-rw-rw-   0        0        0      532 2023-04-07 06:19:36.000000 goodcrap-0.2.1/goodcrap/databases/mysql.py
+-rw-rw-rw-   0        0        0      194 2023-04-07 06:53:45.000000 goodcrap-0.2.1/goodcrap/databases/queries.py
+-rw-rw-rw-   0        0        0      379 2023-04-07 06:19:48.000000 goodcrap-0.2.1/goodcrap/databases/sqlite.py
+-rw-rw-rw-   0        0        0    13362 2023-04-09 15:54:21.000000 goodcrap-0.2.1/goodcrap/goodcrap.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.426149 goodcrap-0.2.1/goodcrap/pipelines/
+-rw-rw-rw-   0        0        0      560 2023-04-05 15:59:55.000000 goodcrap-0.2.1/goodcrap/pipelines/README.md
+-rw-rw-rw-   0        0        0        0 2023-04-05 15:01:30.000000 goodcrap-0.2.1/goodcrap/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     3608 2023-04-07 06:10:04.000000 goodcrap-0.2.1/goodcrap/pipelines/mage.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.426149 goodcrap-0.2.1/goodcrap/pipelines/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-05 15:01:30.000000 goodcrap-0.2.1/goodcrap/pipelines/templates/__init__.py
+-rw-rw-rw-   0        0        0     1122 2023-04-07 06:20:36.000000 goodcrap-0.2.1/goodcrap/pipelines/templates/data_exporter_mysql.py
+-rw-rw-rw-   0        0        0      683 2023-04-07 06:10:42.000000 goodcrap-0.2.1/goodcrap/pipelines/templates/data_loader.py
+-rw-rw-rw-   0        0        0      832 2023-04-06 06:10:32.000000 goodcrap-0.2.1/goodcrap/pipelines/templates/metadata.yaml
+-rw-rw-rw-   0        0        0     2525 2023-04-09 16:25:30.000000 goodcrap-0.2.1/goodcrap/random_mapper.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.426149 goodcrap-0.2.1/goodcrap/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-31 13:15:48.000000 goodcrap-0.2.1/goodcrap/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.426149 goodcrap-0.2.1/goodcrap/templates/__pycache__/
+-rw-rw-rw-   0        0        0      143 2023-03-31 13:16:56.000000 goodcrap-0.2.1/goodcrap/templates/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.438887 goodcrap-0.2.1/goodcrap/templates/data_warehouses/
+-rw-rw-rw-   0        0        0     3459 2023-04-08 14:48:01.000000 goodcrap-0.2.1/goodcrap/templates/data_warehouses/sales.sql
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.376597 goodcrap-0.2.1/goodcrap/templates/databases/
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.441068 goodcrap-0.2.1/goodcrap/templates/databases/customers_orders/
+-rw-rw-rw-   0        0        0      751 2023-04-04 05:53:19.000000 goodcrap-0.2.1/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json
+-rw-rw-rw-   0        0        0     1148 2023-04-06 15:06:31.000000 goodcrap-0.2.1/goodcrap/templates/databases/customers_orders/customers_orders.sql
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.377596 goodcrap-0.2.1/goodcrap/templates/tables/
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.441068 goodcrap-0.2.1/goodcrap/templates/tables/customers/
+-rw-rw-rw-   0        0        0      562 2023-04-04 23:45:49.000000 goodcrap-0.2.1/goodcrap/templates/tables/customers/customers.crap_labels.json
+-rw-rw-rw-   0        0        0      547 2023-04-02 16:03:37.000000 goodcrap-0.2.1/goodcrap/templates/tables/customers/customers.sql
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.443144 goodcrap-0.2.1/goodcrap/templates/tables/orders/
+-rw-rw-rw-   0        0        0      244 2023-04-04 04:00:46.000000 goodcrap-0.2.1/goodcrap/templates/tables/orders/orders.crap_labels.json
+-rw-rw-rw-   0        0        0      599 2023-04-04 03:59:42.000000 goodcrap-0.2.1/goodcrap/templates/tables/orders/orders.sql
+drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.409045 goodcrap-0.2.1/goodcrap.egg-info/
+-rw-rw-rw-   0        0        0    11178 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1567 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      215 2023-04-09 16:31:20.443144 goodcrap-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-04-06 16:31:50.000000 goodcrap-0.2.1/setup.py
```

### Comparing `goodcrap-0.2.0/.github/workflows/pylint.yml` & `goodcrap-0.2.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.0/CONTRIBUTING.rst` & `goodcrap-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.0/LICENSE` & `goodcrap-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.0/PKG-INFO` & `goodcrap-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: goodcrap
-Version: 0.2.0
+Version: 0.2.1
 Summary: goodcrap creates tables, databases and csv files and fill them with random data
 Home-page: https://github.com/goodcrap/goodcrap
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: gpl-3.0
 Keywords: ai,data engineering,fake data,data science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `goodcrap`
 
-`goodcrap` is a python package that generates data structures (tables, databases and `csv` files) and fill them with random data, or generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures.
+`goodcrap` is a python package that generates data structures (tables, databases and `csv` files) and fill them with random data, generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures, and generate random SQL queries.
 
 ## Motivation
 
-This software enables data engineers to replicate the database schemas at their organisations, and then generate fake data that resemble a random sample of the actual data in their organisation.
+This software enables data engineers to replicate the database schemas at their organisations, and then generate fake data that resemble a random sample of the actual data in their organisation. It also enables them to generate any number of random SQL queries that they can use for testing their analytics pipelines, as well as benchmark their data platforms.
 
 While public datasets, such as those hosted at Google or Kaggle, is a common starting point for people interested in learning data analytics and machine learning, many of these datasets require extensive data cleaning so that they can be usable in analytics pipelines. This makes the use of these datasets difficult for AI learners and practitioners.
 
 Public datasets are also utilized by data engineers who are interested in testing their ETL/ELT pipelines. Those folks are particularly interested in data quantity, more than quality. Most public datasets are limited in quantity, which make them not so useful for testing pipelines or for benchmarking query execution times.
 
 Nowadays, generating random data is increasingly a requirement for data teams. [It is a better alternative to using public datasets that require cleaning](https://motherduck.com/blog/python-faker-duckdb-exploration/).
 
@@ -46,15 +46,15 @@
 
 The simplest use-case scenario is generating a `csv` file with random data. `goodcrap` ships with a number of *template* tables that you can use. For example, let's generate 10,000 records in the `customers` table, using the random seed `3`:
 
 `goodcrap --size 10000 --seed 3 --template_table customers --to_csv`
 
 The file `customers.csv` will be generated. 
 
-`goodcrap` populate databases with crap, in addition to filling `csv` files. You can set `goodcrap` to connect to your database via a database configuration file, the name of which is passed to `goodcrap` via the command line argument `--database_config`. This is a json file that looks like this (for a MySQL database):
+`goodcrap` populate databases with random data, in addition to filling `csv` files. You can set `goodcrap` to connect to your database via a database configuration file, the name of which is passed to `goodcrap` via the command line argument `--database_config`. This is a json file that looks like this (for a MySQL database):
 
 ```json
 {
     "db_type": "mysql",
     "host":"localhost",
     "port":"3306",
     "user":"root",
@@ -203,23 +203,23 @@
     assert output is not None, 'The output is undefined'
 
 ```
 *Note:* If you are planning to run a `Mage` pipeline multiple times, then make sure that it does not have columns that are generated using the faker.unique function. The columns should be universally unique.
 
 ## `goodcrap` generates `Mage` pipelines
 
-`Mage` python files are generated using `Jinja` templates. Here is an example command to generate pipelines for each of the tables in the template database `customers_orders`:
+`Mage` python files are generated using `Jinja` templates. Given that Mage will always be backwards compatible (according to communication with its authors), files and folders generated by `goodcrap` will always be valid. Here is an example command to generate pipelines for each of the tables in the template database `customers_orders`:
 
 `goodcrap --size 1000 --seed 3 --database_config examples\mysql_config --template_database customers_orders --mage_pipeline`
 
 Note that `goodcrap` currently will only generate `Mage` projects if the database configurations are defined.
 
 ## Data warehouses
 
-Some dimensions in data warehouses will required to be filled as part of the testing exercise, but should not be filled with random data. These are the *conformed* dimensions with rigid data, such as the Date, Countries, and Cities dimensions. `goodcrap` will be able to fill these dimensions using the `DimensionFiller` class. Filling these tables will be performed before any other table is populated.
+Some dimensions in data warehouses will required to be filled as part of the testing exercise, but should not be filled with random data. These are the *conformed* dimensions with rigid data, such as the Date, Countries, and Cities dimensions. `goodcrap` will be able to fill these dimensions using the `DimensionFiller` class by providing several options for featurization. Filling these tables will be performed before any other table is populated.
 
 ## Guessing the `crap_labels.json` settings
 
 *in progress*
 
 ## Learning the values from a data sample
```

### Comparing `goodcrap-0.2.0/README.md` & `goodcrap-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # `goodcrap`
 
-`goodcrap` is a python package that generates data structures (tables, databases and `csv` files) and fill them with random data, or generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures.
+`goodcrap` is a python package that generates data structures (tables, databases and `csv` files) and fill them with random data, generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures, and generate random SQL queries.
 
 ## Motivation
 
-This software enables data engineers to replicate the database schemas at their organisations, and then generate fake data that resemble a random sample of the actual data in their organisation.
+This software enables data engineers to replicate the database schemas at their organisations, and then generate fake data that resemble a random sample of the actual data in their organisation. It also enables them to generate any number of random SQL queries that they can use for testing their analytics pipelines, as well as benchmark their data platforms.
 
 While public datasets, such as those hosted at Google or Kaggle, is a common starting point for people interested in learning data analytics and machine learning, many of these datasets require extensive data cleaning so that they can be usable in analytics pipelines. This makes the use of these datasets difficult for AI learners and practitioners.
 
 Public datasets are also utilized by data engineers who are interested in testing their ETL/ELT pipelines. Those folks are particularly interested in data quantity, more than quality. Most public datasets are limited in quantity, which make them not so useful for testing pipelines or for benchmarking query execution times.
 
 Nowadays, generating random data is increasingly a requirement for data teams. [It is a better alternative to using public datasets that require cleaning](https://motherduck.com/blog/python-faker-duckdb-exploration/).
 
@@ -34,15 +34,15 @@
 
 The simplest use-case scenario is generating a `csv` file with random data. `goodcrap` ships with a number of *template* tables that you can use. For example, let's generate 10,000 records in the `customers` table, using the random seed `3`:
 
 `goodcrap --size 10000 --seed 3 --template_table customers --to_csv`
 
 The file `customers.csv` will be generated. 
 
-`goodcrap` populate databases with crap, in addition to filling `csv` files. You can set `goodcrap` to connect to your database via a database configuration file, the name of which is passed to `goodcrap` via the command line argument `--database_config`. This is a json file that looks like this (for a MySQL database):
+`goodcrap` populate databases with random data, in addition to filling `csv` files. You can set `goodcrap` to connect to your database via a database configuration file, the name of which is passed to `goodcrap` via the command line argument `--database_config`. This is a json file that looks like this (for a MySQL database):
 
 ```json
 {
     "db_type": "mysql",
     "host":"localhost",
     "port":"3306",
     "user":"root",
@@ -191,23 +191,23 @@
     assert output is not None, 'The output is undefined'
 
 ```
 *Note:* If you are planning to run a `Mage` pipeline multiple times, then make sure that it does not have columns that are generated using the faker.unique function. The columns should be universally unique.
 
 ## `goodcrap` generates `Mage` pipelines
 
-`Mage` python files are generated using `Jinja` templates. Here is an example command to generate pipelines for each of the tables in the template database `customers_orders`:
+`Mage` python files are generated using `Jinja` templates. Given that Mage will always be backwards compatible (according to communication with its authors), files and folders generated by `goodcrap` will always be valid. Here is an example command to generate pipelines for each of the tables in the template database `customers_orders`:
 
 `goodcrap --size 1000 --seed 3 --database_config examples\mysql_config --template_database customers_orders --mage_pipeline`
 
 Note that `goodcrap` currently will only generate `Mage` projects if the database configurations are defined.
 
 ## Data warehouses
 
-Some dimensions in data warehouses will required to be filled as part of the testing exercise, but should not be filled with random data. These are the *conformed* dimensions with rigid data, such as the Date, Countries, and Cities dimensions. `goodcrap` will be able to fill these dimensions using the `DimensionFiller` class. Filling these tables will be performed before any other table is populated.
+Some dimensions in data warehouses will required to be filled as part of the testing exercise, but should not be filled with random data. These are the *conformed* dimensions with rigid data, such as the Date, Countries, and Cities dimensions. `goodcrap` will be able to fill these dimensions using the `DimensionFiller` class by providing several options for featurization. Filling these tables will be performed before any other table is populated.
 
 ## Guessing the `crap_labels.json` settings
 
 *in progress*
 
 ## Learning the values from a data sample
```

### Comparing `goodcrap-0.2.0/goodcrap/cli.py` & `goodcrap-0.2.1/goodcrap/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import random
 import sys
 import textwrap
 from pathlib import Path
 from typing import Dict, List, Optional, TextIO, TypeVar, Union
 from . import VERSION
 
+
 class CLI:
     def __init__(self, argv: Optional[str] = None) -> None:
         self.argv = argv or sys.argv[:]
         self.prog_name = Path(self.argv[0]).name
         self.formatter_class = argparse.RawDescriptionHelpFormatter
         self.epilog = 'Epilogue'
         self.version = VERSION
@@ -69,23 +70,33 @@
             type=str,
             help="specify one of the databases in the template library",
         )
 
         parser.add_argument(
             "--to_csv",
             action="store_const",
-            const='to_csv',
-            help="stores data to a csv file",
+            default=False,
+            const=True,
+            help="write data to a csv file",
         )
 
         parser.add_argument(
             "--to_json",
             action="store_const",
-            const='to_json',
-            help="stores data to a csv file",
+            default=False,
+            const=True,
+            help="write data to a json file",
+        )
+
+        parser.add_argument(
+            "--to_parquet",
+            action="store_const",
+            default=False,
+            const=True,
+            help="write data to a parquet file",
         )
 
         parser.add_argument(
             "--database_config",
             "-j",
             type=str,
             help="name of json file that includes the database configuration",
@@ -137,31 +148,40 @@
             "-P",
             "--mage_pipeline",
             action="store_const",
             const='mage_pipeline',
             help="generate a new mage pipeline in the current mage project",
         )
 
+        parser.add_argument(
+            "--queries",
+            default=0,
+            type=int,
+            help="generate random SQL queries",
+        )
+
         arguments = parser.parse_args(self.argv[1:])
         random.seed(arguments.seed)
 
         from .goodcrap import GoodCrap
         good_crap = GoodCrap(size=arguments.size,
                              seed=arguments.seed,
                              to_csv=arguments.to_csv,
                              to_json=arguments.to_json,
+                             to_parquet=arguments.to_parquet,
                              template_database=arguments.template_database,
                              template_table=arguments.template_table,
                              database_config=arguments.database_config,
                              table_sql=arguments.table_sql,
                              table_crap_labels=arguments.table_crap_labels,
                              database_sql=arguments.database_sql,
                              database_crap_labels=arguments.database_crap_labels,
                              mage_project_name=arguments.mage_project,
-                             mage_pipeline=arguments.mage_pipeline
+                             mage_pipeline=arguments.mage_pipeline,
+                             queries=arguments.queries
                              )
 
         good_crap.run()
 
 
 def execute_cli(argv: Optional[str] = None) -> None:
     cli = CLI()
```

### Comparing `goodcrap-0.2.0/goodcrap/crappers/__init__.py` & `goodcrap-0.2.1/goodcrap/crappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 import uuid
 
 def crapper_unique(props: dict):
     if props['type'] == 'serial':
         return uuid.uuid4()
     
-
 def crapper(props: dict):
     decimals = 2
     multiplier = 1
     if props['type'] == 'random_int':
         if 'multiplier' in props.keys():
             multiplier = props['multiplier']
         return int(np.random.random()*(props['max'] - props['min'] + 1) + props['min'])*multiplier
```

### Comparing `goodcrap-0.2.0/goodcrap/databases/database.py` & `goodcrap-0.2.1/goodcrap/databases/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import json
+import os
+import pandas as pd
 import sqlalchemy
 from sqlalchemy import MetaData, Table, Column, Integer, String
 from sqlalchemy.sql import text
 
 from ..random_mapper import RandomMapper
-import json
-import os
-import pandas as pd
-
+from ..crappers import queries
 
 class DataBase:
     def __init__(self,
                  database_config) -> None:
         self.database_config = database_config
         self.size = 1000
         self.connection = None
@@ -18,15 +18,16 @@
 
     def set_size(self, size):
         self.size = size
 
     def set_seed(self, seed):
         self.seed = seed
 
-    def run(self, table_sql=None, table_crap_labels=None, database_sql=None, database_crap_labels=None):
+    def run(self, table_sql=None, table_crap_labels=None,
+            database_sql=None, database_crap_labels=None):
         if table_sql is not None and table_crap_labels is not None:
             table_name = os.path.basename(table_sql).split('.')[0]
             with open(table_sql, 'r') as f:
                 self.table_sql = f.read()
                 f.close()
             self.connection.execute(self.table_sql)
             metadata = MetaData(bind=self.engine)
@@ -67,10 +68,14 @@
                         ins = table.insert().values(row)
                         self.engine.execute(ins)
                         if self.database_config['to_csv']:
                             data_csv += [row]
                     if self.database_config['to_csv']:
                         df = pd.DataFrame(data_csv, columns=table.columns)
                         df.to_csv(table_name+'.csv')
+        if 'queries' in self.database_config.keys():
+            with open('queries.sql','a') as f:
+                for i in range(self.database_config['queries']):
+                    f.write(str(queries.crapper(self.engine))+'\n')
 
     def execute(self, sql):
         return self.engine.execute(sql)
```

### Comparing `goodcrap-0.2.0/goodcrap/goodcrap.py` & `goodcrap-0.2.1/goodcrap/goodcrap.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,46 +2,49 @@
 import os
 from .databases.sqlite import SQLite
 from .databases.mysql import MySQL
 from .random_mapper import RandomMapper
 from .pipelines.mage import MageProject
 from . import templates
 
-
 class GoodCrap:
     seed = None
 
     def __init__(
         self,
         size,
         seed,
         template_table=None,
-        to_csv=None,
-        to_json=None,
+        to_csv=False,
+        to_json=False,
+        to_parquet=False,
         database_config=None,
         template_database=None,
         table_sql=None,
         table_crap_labels=None,
         database_sql=None,
         database_crap_labels=None,
         mage_project_name=None,
-        mage_pipeline=None
+        mage_pipeline=None,
+        queries=False
     ) -> None:
         GoodCrap.seed = seed
         self.size = size
         self.to_csv = to_csv
         self.to_json = to_json
+        self.to_parquet = to_parquet
         self.template_table = template_table
         self.template_database = template_database
         self.table_sql = table_sql
         self.table_crap_labels = table_crap_labels
         self.database_sql = database_sql
         self.database_crap_labels = database_crap_labels
         self.mage_project_name = mage_project_name
         self.mage_pipeline = mage_pipeline
+        self.queries = queries
 
         self.templates_path = os.path.dirname(templates.__file__)
 
         if self.table_crap_labels:
             with open(self.table_crap_labels, 'r') as f:
                 self.table_crap_labels = json.load(f)
                 f.close()
@@ -52,49 +55,55 @@
         out_str = 'Starting goodcrap with table size ' + \
             str(size) + ' and random seed ' + str(seed)
         print(out_str)
 
         self.database_instance = None
 
         if database_config is not None:
-            if type(database_config) is str:
+            if isinstance(database_config, str):
                 fdatabase_config = open(database_config+'.json', 'r')
                 database_config = json.load(fdatabase_config)
                 fdatabase_config.close()
             database_config['to_csv'] = self.to_csv
             database_config['to_json'] = self.to_json
+            database_config['to_parquet'] = self.to_parquet
+            database_config['queries'] = self.queries
             self.database_config = database_config
             if database_config['db_type'] == 'sqlite':
                 self.database_instance = SQLite(database_config)
             elif database_config['db_type'] == 'mysql':
                 self.database_instance = MySQL(database_config)
 
             if self.database_instance is not None:
                 self.database_instance.set_size(self.size)
                 self.database_instance.set_seed(self.seed)
 
-    # The function will generate random data given that only one of the following is supplied:
-    # - table_sql and table_crap_labels, or
-    # - database_sql and database_crap_labels, or
-    # - template_table, or
-    # - template_database
     def run(self):
+        '''
+        The function will generate random data given that 
+        only one of the following is supplied:
+        - table_sql and table_crap_labels, or
+        - database_sql and database_crap_labels, or
+        - template_table, or
+        - template_database
+        '''
         if self.template_table is not None:
             self.run_template_table()
         elif self.template_database is not None:
             self.run_template_database()
         elif self.table_crap_labels is not None:
             self.run_table()
         elif self.database_sql is not None and self.database_crap_labels is not None:
             self.run_database()
-        elif self.table_sql is None and self.table_crap_labels is not None and self.database_instance is None:
+        elif self.table_sql is None and self.table_crap_labels is not None\
+                and self.database_instance is None:
             table_name = os.path.basename(
                 self.table_crap_labels).replace('.json', '')
-            self.write_csv(table_name=table_name,
-                           table_crap_labels=self.table_crap_labels)
+            self.write_file(table_name=table_name,
+                            table_crap_labels=self.table_crap_labels)
 
     def run_template_table(self):
         if self.database_instance is not None:
             self._set_template_table_variables()
             with open(self.table_crap_labels, 'r') as f:
                 self.table_crap_labels = json.load(f)
                 f.close()
@@ -102,21 +111,21 @@
                 self.run_mage(table_sql=self.table_sql,
                               table_crap_labels=self.table_crap_labels)
             else:
                 self.database_instance.run(
                     table_sql=self.table_sql, table_crap_labels=self.table_crap_labels)
         else:
             # Generate csv files only
-            self.table_crap_labels = self.template_path + '/tables/' + \
+            self.table_crap_labels = self.templates_path + '/tables/' + \
                 self.template_table+'/'+self.template_table+'.crap_labels.json'
             with open(self.table_crap_labels, 'r') as f:
                 self.table_crap_labels = json.load(f)
                 f.close()
-            self.write_csv(table_name=self.template_table,
-                           table_crap_labels=self.table_crap_labels)
+            self.write_file(table_name=self.template_table,
+                            table_crap_labels=self.table_crap_labels)
 
     def _set_template_table_variables(self):
         self.table_sql = self.templates_path + '/tables/' + \
             self.template_table+'/'+self.template_table+'.sql'
         self.table_crap_labels = self.templates_path + '/tables/' + \
             self.template_table+'/'+self.template_table+'.crap_labels.json'
 
@@ -133,52 +142,61 @@
                 self.database_crap_labels = json.load(f)
                 f.close()
             if self._is_run_with_mage():
                 self.run_mage(database_sql=self.database_sql,
                               database_crap_labels=self.database_crap_labels)
             else:
                 self.database_instance.run(
-                    database_sql=self.database_sql, database_crap_labels=self.database_crap_labels)
+                    database_sql=self.database_sql,
+                    database_crap_labels=self.database_crap_labels)
         else:
             print("WOOPS: You should provide a database configuration file.")
 
     def run_table(self):
         if self.database_instance is not None:
             if self._is_run_with_mage():
-                # Mage can create the table on the fly if the table doesn't exist,
-                # so no need for the sql create statement.
                 self.run_mage(table_sql=self.table_sql,
                               table_crap_labels=self.table_crap_labels)
             elif self.table_sql is not None:
                 self.database_instance.run(
-                    table_sql=self.table_sql, table_crap_labels=self.table_crap_labels)
+                    table_sql=self.table_sql,
+                    table_crap_labels=self.table_crap_labels)
             else:
                 print(
                     "WOOPS: You should provide the table CREATE statement sql file (--table_sql).")
         else:
             print(
                 "WOOPS: You should provide a database configuration file (--database_config).")
 
     def run_database(self):
         if self.database_instance is not None:
             if self._is_run_with_mage():
                 self.run_mage(database_sql=self.database_sql,
                               database_crap_labels=self.database_crap_labels)
             else:
                 self.database_instance.run(
-                    database_sql=self.database_sql, database_crap_labels=self.database_crap_labels)
+                    database_sql=self.database_sql,
+                    database_crap_labels=self.database_crap_labels)
         else:
             print("WOOPS: You should provide a database configuration file.")
 
-    def run_mage(self, table_sql=None, table_crap_labels=None, database_sql=None, database_crap_labels=None):
-        # Choosing Mage means that the data will not be generated using goodcrap,
-        # but will be generated in Mage pipelines by the user.
-        # However, the tables will be created in the target database.
+    def run_mage(self, table_sql=None, table_crap_labels=None, database_sql=None,
+                 database_crap_labels=None):
+        '''
+        Choosing Mage means that the data will not be generated using goodcrap,
+        but will be generated in Mage pipelines by the user.
+        However, the tables will be created in the target database.
+
+        Mage can create the table on the fly if the table doesn't exist,
+        so no need for the sql create statement.
+        '''
         if self.mage_project_name is not None:
-            # If the mage project doesn't exist, create it then add the pipeline to it. Otherwise, just add the pipeline to the existing mage project.
+            # If the mage project doesn't exist, create it then add the
+            # pipeline to it. Otherwise, just add the pipeline
+            # to the existing mage project.
             if self.mage_project is None:
                 self.create_mage_project()
             if table_sql is not None and table_crap_labels is not None:
                 table_name = os.path.basename(
                     table_sql).replace('.sql', '')
                 with open(table_sql, 'r') as f:
                     table_sql = f.read()
@@ -216,34 +234,47 @@
                 for table_name in database_crap_labels.keys():
                     self.create_mage_pipeline(
                         table_name, database_crap_labels[table_name])
 
     def _is_run_with_mage(self):
         return self.mage_pipeline is not None
 
-    def write_csv(self, table_name=None, table_crap_labels=None, database_crap_labels=None):
+    def write_file(self, table_name=None,
+                   table_crap_labels=None,
+                   database_crap_labels=None):
         import pandas as pd
         if table_crap_labels is not None and database_crap_labels is None:
             fm = RandomMapper(
                 self.seed, table_crap_labels)
             data_csv = []
             for i in range(int(self.size)):
                 data_csv += [fm.get_crap()]
             df = pd.DataFrame(data_csv, columns=table_crap_labels.keys())
-            df.to_csv(table_name+'.csv')
+            if self.to_json:
+                with open(table_name+'.json', 'w') as f:
+                    f.write(df.to_json())
+                print('Data written to a json file')
+            elif self.to_parquet:
+                df.to_parquet(table_name + '.parquet',
+                              engine='pyarrow', compression='gzip')
+                print('Data written to a parquet file')
+            else:
+                df.to_csv(table_name+'.csv')
+                print('Data written to a csv file')
         elif table_crap_labels is None and database_crap_labels is not None:
             pass
 
-    def get_dataframe(self, table_name=None, table_crap_labels=None):
+    def get_dataframe(self, table_name=None,
+                      table_crap_labels=None):
         import pandas as pd
         if self.template_table is not None:
             table_name = self.template_table
             self._set_template_table_variables()
             table_crap_labels = self.table_crap_labels
-        if type(table_crap_labels) is str:
+        if isinstance(table_crap_labels, str):
             with open(table_crap_labels, 'r') as f:
                 table_crap_labels = json.load(f)
                 f.close()
         if self.database_instance is not None:
             from sqlalchemy import MetaData, Table
             metadata = MetaData(bind=self.database_instance.engine)
             table = Table(table_name, metadata, autoload=True)
@@ -255,12 +286,16 @@
         data_csv = []
         for i in range(int(self.size)):
             data_csv += [fm.get_crap()]
         return pd.DataFrame(data_csv, columns=table_crap_labels.keys())
 
     def create_mage_project(self):
         self.mage_project = MageProject(
-            project_name=self.mage_project_name, database_config=self.database_config, database_instance=self.database_instance)
+            project_name=self.mage_project_name,
+            database_config=self.database_config,
+            database_instance=self.database_instance)
 
     def create_mage_pipeline(self, table_name, crap_labels):
         self.mage_project.generate_pipeline(
-            seed=self.seed, size=self.size, table_name=table_name, crap_labels=crap_labels)
+            seed=self.seed, size=self.size,
+            table_name=table_name,
+            crap_labels=crap_labels)
```

### Comparing `goodcrap-0.2.0/goodcrap/pipelines/mage.py` & `goodcrap-0.2.1/goodcrap/pipelines/mage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from jinja2 import Environment, FileSystemLoader
-import subprocess
 import os
+import subprocess
+from jinja2 import Environment, FileSystemLoader
 from ..databases.mysql import MySQL
 from ..databases.sqlite import SQLite
 
 
 class MageProject:
     def __init__(self, project_name, database_config, database_instance) -> None:
         from . import templates
@@ -26,16 +26,20 @@
 
         self.project_name = project_name
         retcode = subprocess.call('mage init ' + self.project_name)
         if retcode == 0:
             print('Successfully generating the Mage project', project_name)
 
     def generate_pipeline(self, size, seed, table_name, crap_labels) -> None:
-        # Note: If you are planning to run a pipeline multiple times, then make sure that it does not
-        # have columns that are generated using the faker.unique function. Those columns should be universally unique.
+        '''
+        Note: If you are planning to run a pipeline multiple times, 
+        then make sure that it does nothave columns that are 
+        generated using the faker.unique function. Those columns 
+        should be universally unique.
+        '''
         self.size = size
         self.seed = seed
         self.table_name = table_name
         self.crap_labels = crap_labels
         self.data_loader_context = {
             "size": size,
             "seed": seed,
```

### Comparing `goodcrap-0.2.0/goodcrap/pipelines/templates/data_exporter_mysql.py` & `goodcrap-0.2.1/goodcrap/pipelines/templates/data_exporter_mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Specify your configuration settings in 'io_config.yaml'.
 
     Docs: https://docs.mage.ai/design/data-loading#mysql
     """
     table_name = '{{ table_name }}'  # Specify the name of the table to export data to
     config_path = path.join(get_repo_path(), 'io_config.yaml')
     config_profile = 'default'
-    
+
     with MySQL.with_config(ConfigFileLoader(config_path, config_profile)) as loader:
         loader.export(
             df,
             None,
             table_name,
             index=False,  # Specifies whether to include index in exported table
             if_exists='append',  # Specify resolution policy if table name already exists
```

### Comparing `goodcrap-0.2.0/goodcrap/pipelines/templates/data_loader.py` & `goodcrap-0.2.1/goodcrap/pipelines/templates/data_loader.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.0/goodcrap/pipelines/templates/metadata.yaml` & `goodcrap-0.2.1/goodcrap/pipelines/templates/metadata.yaml`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.0/goodcrap/random_mapper.py` & `goodcrap-0.2.1/goodcrap/random_mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         faker.Faker.seed(self.seed)
         self.faker_generator = []
         table_columns = []
         primary_keys = []
         fks = {}
         if engine is not None and table is not None:
             for f in table.foreign_keys:
-                print('Table has foreign key to', f.column.table)
                 metadata = MetaData(bind=self.engine)
+                # metadata.reflect(self.engine): That's for version > 2
                 rel_table = Table(f.column.table, metadata, autoload=True)
                 results = self.engine.connect().execute(
                     select(rel_table.c[f.column.name])).fetchall()
                 results = [x[0] for x in results]
                 fks[f.column.name] = results
                 # print(fks[f.column.name])
         if engine is not None and table is not None:
```

### Comparing `goodcrap-0.2.0/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json` & `goodcrap-0.2.1/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.0/goodcrap/templates/databases/customers_orders/customers_orders.sql` & `goodcrap-0.2.1/goodcrap/templates/databases/customers_orders/customers_orders.sql`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.0/goodcrap/templates/tables/customers/customers.crap_labels.json` & `goodcrap-0.2.1/goodcrap/templates/tables/customers/customers.crap_labels.json`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.0/goodcrap/templates/tables/customers/customers.sql` & `goodcrap-0.2.1/goodcrap/templates/tables/customers/customers.sql`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.0/goodcrap/templates/tables/orders/orders.sql` & `goodcrap-0.2.1/goodcrap/templates/tables/orders/orders.sql`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.0/goodcrap.egg-info/PKG-INFO` & `goodcrap-0.2.1/goodcrap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: goodcrap
-Version: 0.2.0
+Version: 0.2.1
 Summary: goodcrap creates tables, databases and csv files and fill them with random data
 Home-page: https://github.com/goodcrap/goodcrap
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: gpl-3.0
 Keywords: ai,data engineering,fake data,data science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `goodcrap`
 
-`goodcrap` is a python package that generates data structures (tables, databases and `csv` files) and fill them with random data, or generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures.
+`goodcrap` is a python package that generates data structures (tables, databases and `csv` files) and fill them with random data, generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures, and generate random SQL queries.
 
 ## Motivation
 
-This software enables data engineers to replicate the database schemas at their organisations, and then generate fake data that resemble a random sample of the actual data in their organisation.
+This software enables data engineers to replicate the database schemas at their organisations, and then generate fake data that resemble a random sample of the actual data in their organisation. It also enables them to generate any number of random SQL queries that they can use for testing their analytics pipelines, as well as benchmark their data platforms.
 
 While public datasets, such as those hosted at Google or Kaggle, is a common starting point for people interested in learning data analytics and machine learning, many of these datasets require extensive data cleaning so that they can be usable in analytics pipelines. This makes the use of these datasets difficult for AI learners and practitioners.
 
 Public datasets are also utilized by data engineers who are interested in testing their ETL/ELT pipelines. Those folks are particularly interested in data quantity, more than quality. Most public datasets are limited in quantity, which make them not so useful for testing pipelines or for benchmarking query execution times.
 
 Nowadays, generating random data is increasingly a requirement for data teams. [It is a better alternative to using public datasets that require cleaning](https://motherduck.com/blog/python-faker-duckdb-exploration/).
 
@@ -46,15 +46,15 @@
 
 The simplest use-case scenario is generating a `csv` file with random data. `goodcrap` ships with a number of *template* tables that you can use. For example, let's generate 10,000 records in the `customers` table, using the random seed `3`:
 
 `goodcrap --size 10000 --seed 3 --template_table customers --to_csv`
 
 The file `customers.csv` will be generated. 
 
-`goodcrap` populate databases with crap, in addition to filling `csv` files. You can set `goodcrap` to connect to your database via a database configuration file, the name of which is passed to `goodcrap` via the command line argument `--database_config`. This is a json file that looks like this (for a MySQL database):
+`goodcrap` populate databases with random data, in addition to filling `csv` files. You can set `goodcrap` to connect to your database via a database configuration file, the name of which is passed to `goodcrap` via the command line argument `--database_config`. This is a json file that looks like this (for a MySQL database):
 
 ```json
 {
     "db_type": "mysql",
     "host":"localhost",
     "port":"3306",
     "user":"root",
@@ -203,23 +203,23 @@
     assert output is not None, 'The output is undefined'
 
 ```
 *Note:* If you are planning to run a `Mage` pipeline multiple times, then make sure that it does not have columns that are generated using the faker.unique function. The columns should be universally unique.
 
 ## `goodcrap` generates `Mage` pipelines
 
-`Mage` python files are generated using `Jinja` templates. Here is an example command to generate pipelines for each of the tables in the template database `customers_orders`:
+`Mage` python files are generated using `Jinja` templates. Given that Mage will always be backwards compatible (according to communication with its authors), files and folders generated by `goodcrap` will always be valid. Here is an example command to generate pipelines for each of the tables in the template database `customers_orders`:
 
 `goodcrap --size 1000 --seed 3 --database_config examples\mysql_config --template_database customers_orders --mage_pipeline`
 
 Note that `goodcrap` currently will only generate `Mage` projects if the database configurations are defined.
 
 ## Data warehouses
 
-Some dimensions in data warehouses will required to be filled as part of the testing exercise, but should not be filled with random data. These are the *conformed* dimensions with rigid data, such as the Date, Countries, and Cities dimensions. `goodcrap` will be able to fill these dimensions using the `DimensionFiller` class. Filling these tables will be performed before any other table is populated.
+Some dimensions in data warehouses will required to be filled as part of the testing exercise, but should not be filled with random data. These are the *conformed* dimensions with rigid data, such as the Date, Countries, and Cities dimensions. `goodcrap` will be able to fill these dimensions using the `DimensionFiller` class by providing several options for featurization. Filling these tables will be performed before any other table is populated.
 
 ## Guessing the `crap_labels.json` settings
 
 *in progress*
 
 ## Learning the values from a data sample
```

### Comparing `goodcrap-0.2.0/goodcrap.egg-info/SOURCES.txt` & `goodcrap-0.2.1/goodcrap.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .gitignore
 CHANGELOG.md
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.md
 VERSION
+customers.parquet
 setup.cfg
 setup.py
 .github/workflows/pylint.yml
 examples/mysql_config.json
 examples/sqlite_config.json
 goodcrap/__init__.py
 goodcrap/__main__.py
@@ -19,20 +20,23 @@
 goodcrap.egg-info/PKG-INFO
 goodcrap.egg-info/SOURCES.txt
 goodcrap.egg-info/dependency_links.txt
 goodcrap.egg-info/entry_points.txt
 goodcrap.egg-info/requires.txt
 goodcrap.egg-info/top_level.txt
 goodcrap/crappers/__init__.py
+goodcrap/crappers/queries.py
 goodcrap/data_warehouses/__init__.py
-goodcrap/data_warehouses/dimension_fillers.py
+goodcrap/data_warehouses/dimension_featurizer.py
 goodcrap/databases/__init__.py
 goodcrap/databases/database.py
 goodcrap/databases/mysql.py
+goodcrap/databases/queries.py
 goodcrap/databases/sqlite.py
+goodcrap/pipelines/README.md
 goodcrap/pipelines/__init__.py
 goodcrap/pipelines/mage.py
 goodcrap/pipelines/templates/__init__.py
 goodcrap/pipelines/templates/data_exporter_mysql.py
 goodcrap/pipelines/templates/data_loader.py
 goodcrap/pipelines/templates/metadata.yaml
 goodcrap/templates/__init__.py
```

### Comparing `goodcrap-0.2.0/setup.py` & `goodcrap-0.2.1/setup.py`

 * *Files identical despite different names*

