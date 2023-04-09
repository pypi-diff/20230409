# Comparing `tmp/data-warehouse-client-2.0.9.tar.gz` & `tmp/data-warehouse-client-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-warehouse-client-2.0.9.tar", last modified: Thu Mar  2 16:05:46 2023, max compression
+gzip compressed data, was "data-warehouse-client-3.0.0.tar", last modified: Sun Apr  9 15:02:12 2023, max compression
```

## Comparing `data-warehouse-client-2.0.9.tar` & `data-warehouse-client-3.0.0.tar`

### file list

```diff
@@ -1,68 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 16:05:46.710313 data-warehouse-client-2.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 16:05:46.694313 data-warehouse-client-2.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 16:05:46.698313 data-warehouse-client-2.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-03-02 16:05:46.710313 data-warehouse-client-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 16:05:46.702313 data-warehouse-client-2.0.9/data_warehouse_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/clone_study_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/csv_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    41428 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/data_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/delete_study_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35838 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/load_warehouse_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/print_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/print_metadata_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sample_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 16:05:46.710313 data-warehouse-client-2.0.9/data_warehouse_client/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/bounded_integer_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/bounded_integers.sql
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/bounded_real_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/bounded_reals.sql
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/core_sql_from_for_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/core_sql_select_for_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_all_measurement_groups.sql
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_all_measurement_groups_and_types_in_a_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_boundsint_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_boundsreal_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_categories_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_measurement_group_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_measurement_groups_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_measurement_type_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_measurements_by_cohort.sql
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_measurements_with_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/get_units_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/measurements_lacking_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/measurements_with_invalid_category.sql
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/num_types_in_a_measurement_group.sql
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/ordinal_types_not_matching_category.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/sql/types_in_a_measurement_group.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/study_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/study_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/table_reader_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/table_writer_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/transform_result_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/data_warehouse_client/warehouse_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 16:05:46.706313 data-warehouse-client-2.0.9/data_warehouse_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-03-02 16:05:46.000000 data-warehouse-client-2.0.9/data_warehouse_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-02 16:05:46.000000 data-warehouse-client-2.0.9/data_warehouse_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 16:05:46.000000 data-warehouse-client-2.0.9/data_warehouse_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-02 16:05:46.000000 data-warehouse-client-2.0.9/data_warehouse_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-02 16:05:46.000000 data-warehouse-client-2.0.9/data_warehouse_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 16:05:46.710313 data-warehouse-client-2.0.9/integration_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/integration_test/clone_study_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/integration_test/delete_study_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 16:05:46.710313 data-warehouse-client-2.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 16:05:46.710313 data-warehouse-client-2.0.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/test/test_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-02 16:05:34.000000 data-warehouse-client-2.0.9/test/test_transform_result_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.424381 data-warehouse-client-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.408380 data-warehouse-client-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.412380 data-warehouse-client-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 15:02:12.424381 data-warehouse-client-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.416381 data-warehouse-client-3.0.0/data_warehouse_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14953 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/auto_generate_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/auto_generate_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/check_bounded_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/check_for_datetime_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/clone_study_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/csv_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41229 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/data_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/delete_study_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/import_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34655 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/import_with_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44090 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/load_warehouse_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/multiple_mg_inserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/print_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/print_metadata_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.420381 data-warehouse-client-3.0.0/data_warehouse_client/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_datetime_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_datetimes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_integer_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_integers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_real_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_reals.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/core_sql_from_for_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/core_sql_select_for_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_all_measurement_groups.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_all_measurement_groups_and_types_in_a_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_all_table_names.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_boundsdatetime_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_boundsint_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_boundsreal_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_categories_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_category_ids.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurement_group_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurement_groups_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurement_type_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurements_by_cohort.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurements_with_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_units_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/insert_datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/insert_measurement.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/insert_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/measurements_lacking_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/measurements_with_invalid_category.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/num_types_in_a_measurement_group.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/ordinal_types_not_matching_category.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/types_in_a_measurement_group.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/update_measurement_group_instance_id.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/study_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/study_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/table_reader_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/table_writer_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/transform_result_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/type_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/warehouse_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.416381 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 15:02:12.000000 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-09 15:02:12.000000 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:02:12.000000 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-09 15:02:12.000000 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 15:02:12.000000 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.420381 data-warehouse-client-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   574842 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/docs/data_warehouse_guide.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.420381 data-warehouse-client-3.0.0/integration_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/integration_test/clone_study_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/integration_test/delete_study_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 15:02:12.424381 data-warehouse-client-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.424381 data-warehouse-client-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/test/test_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/test/test_transform_result_format.py
```

### Comparing `data-warehouse-client-2.0.9/.github/workflows/build.yml` & `data-warehouse-client-3.0.0/.github/workflows/build.yml`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# This workflow will install Python dependencies, run tests and lint with a single version of Python
-# For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
-
-name: Build application
-
-on: [push]
-jobs:
-  build:
-
-    runs-on: ubuntu-latest
-
-    steps:
-      - uses: actions/checkout@v2
-      - name: Set up Python 3.8
-        uses: actions/setup-python@v2
-        with:
-          python-version: 3.8
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          pip install -r requirements.txt
-          pip install flake8
-      - name: Lint with flake8
-        run: |
-          # stop the build if there are Python syntax errors or undefined names
-          flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-          # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-          flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
-      - name: Run tests
-        run: |
-          python -m unittest -v
+# This workflow will install Python dependencies, run tests and lint with a single version of Python
+# For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
+
+name: Build application
+
+on: [push]
+jobs:
+  build:
+
+    runs-on: ubuntu-latest
+
+    steps:
+      - uses: actions/checkout@v2
+      - name: Set up Python 3.8
+        uses: actions/setup-python@v2
+        with:
+          python-version: 3.8
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install -r requirements.txt
+          pip install flake8
+      - name: Lint with flake8
+        run: |
+          # stop the build if there are Python syntax errors or undefined names
+          flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
+          # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
+          flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+      - name: Run tests
+        run: |
+          python -m unittest -v
```

### Comparing `data-warehouse-client-2.0.9/.gitignore` & `data-warehouse-client-3.0.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -150,9 +150,11 @@
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 scratchpad.py
-*.pdf
 /data_warehouse_client/production-db-credentials-full-access.json
+data_warehouse_client/dw-credentials-full-access.json
+data_warehouse_client/dw-credentials-read-only.json
+/data_warehouse_client/sql/Data Warehouse Schema.sql
```

### Comparing `data-warehouse-client-2.0.9/LICENSE` & `data-warehouse-client-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-2.0.9/PKG-INFO` & `data-warehouse-client-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-warehouse-client
-Version: 2.0.9
+Version: 3.0.0
 Summary: This package provides access to the e-Science Central data warehouse that can be used to store, access and analyse data collected in scientific studies, including for healthcare applications
 Home-page: https://github.com/e-science-central/data-warehouse-client
 Author: Paul Watson
 Author-email: paul.watson@ncl.ac.uk
 License: UNKNOWN
 Description: # Data Warehouse Client
         
@@ -39,20 +39,23 @@
         2.	Descriptive information about the types of measurement is stored in the warehouse so that tools or humans 
         can interpret the data stored there.
         3.	The design is optimised for query performance. In several cases, this has led to denormalization
          (duplication of data) to reduce the need for expensive joins.
         4.	It must support a security regime to restrict each user’s access 
         to the data collected in studies.
         
+        
         For more information see: 
         P. Watson and H. Hiden, "The e-Science Central Study Data Platform"
         2022 IEEE 18th International Conference on e-Science (e-Science),
         Salt Lake City, UT, USA, 2022, pp. 55-64, doi: 10.1109/eScience55777.2022.00020.
         https://scholar.google.co.uk/citations?view_op=view_citation&hl=en&user=KQJg3lwAAAAJ&sortby=pubdate&citation_for_view=KQJg3lwAAAAJ:z0_F5_TITjQC
         
+        For more documentation see [A Data Warehouse for Storing and Analysing Study Data](docs/data_warehouse_guide.pdf).
+        
         # Running Instructions
         
         To install from PyPi, run:
         
         pip install data-warehouse-client
         
         In directory in which your executable is run, create a `db-credentials.json` file containing database
```

### Comparing `data-warehouse-client-2.0.9/README.md` & `data-warehouse-client-3.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,23 @@
 2.	Descriptive information about the types of measurement is stored in the warehouse so that tools or humans 
 can interpret the data stored there.
 3.	The design is optimised for query performance. In several cases, this has led to denormalization
  (duplication of data) to reduce the need for expensive joins.
 4.	It must support a security regime to restrict each user’s access 
 to the data collected in studies.
 
+
 For more information see: 
 P. Watson and H. Hiden, "The e-Science Central Study Data Platform"
 2022 IEEE 18th International Conference on e-Science (e-Science),
 Salt Lake City, UT, USA, 2022, pp. 55-64, doi: 10.1109/eScience55777.2022.00020.
 https://scholar.google.co.uk/citations?view_op=view_citation&hl=en&user=KQJg3lwAAAAJ&sortby=pubdate&citation_for_view=KQJg3lwAAAAJ:z0_F5_TITjQC
 
+For more documentation see [A Data Warehouse for Storing and Analysing Study Data](docs/data_warehouse_guide.pdf).
+
 # Running Instructions
 
 To install from PyPi, run:
 
 pip install data-warehouse-client
 
 In directory in which your executable is run, create a `db-credentials.json` file containing database
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/clone_study_metadata.py` & `data-warehouse-client-3.0.0/data_warehouse_client/clone_study_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from data_warehouse_client import table_writer_json
+from table_writer_json import data_warehouse_metadata_tables_to_dictionary, write_tables_in_dw_from_dictionary
 
 
 def clone_study_metadata(dw, source_study_id, dest_study_id):
     """
     Copies all the metadata from one study to another
     :param dw: data warehouse end point
     :param source_study_id: original study
     :param dest_study_id: destination study
     :return total rows inserted
     """
     # extract existing metadata
-    tbls = table_writer_json.data_warehouse_metadata_tables_to_dictionary(dw, source_study_id)
+    tbls = data_warehouse_metadata_tables_to_dictionary(dw, source_study_id)
     for table in tbls:  # for each table
         for row in tbls[table]:  # for each row
             row.update({'study': dest_study_id})  # update all occurrences of study to the destination study
-    return table_writer_json.write_tables_in_dw_from_dictionary(dw, tbls)  # write the result to the warehouse
+    return write_tables_in_dw_from_dictionary(dw, tbls)  # write the result to the warehouse
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/csv_io.py` & `data-warehouse-client-3.0.0/data_warehouse_client/csv_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,35 +9,34 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from typing import List
-import csv
+from csv import writer
 
 
 def export_measurements_as_csv(rows, fname):
     """
     Stores measurements returned by queries in a CSV file
     The input rows must be in the format produced by:
         getMeasurements or getMeasurementsWithValueTest
         The output file has a header row, followed by a row for each measurement. This has the columns:
             id,time,study,participant,measurementType,typeName,measurementGroup, groupInstance,trial,valType,value
     :param rows: a list of rows returned by getMeasurements, getMeasurementsWithValueTest or
                     getMeasurementGroupInstancesWithValueTests
     :param fname: the filename of the output CSV file
     """
     with open(fname, "w", newline="", encoding="utf-8") as f:
-        writer = csv.writer(f)
-        writer.writerow(
+        wr = writer(f)
+        wr.writerow(
             ["Id", "Time", "Study", "Participant", "Measurement Type", "Measurement Type Name", "Measurement Group",
              "Measurement Group Instance", "Trial", "Value Type", "Value"])
-        writer.writerows(rows)
+        wr.writerows(rows)
 
 
 def export_measurement_groups_as_csv(header, instances, fname):
     """
     Stores measurements returned by formMeasurementGroups in a CSV file
     The input rows must be in the format produced by formMeasurementGroups
     The output file has a header row, followed by a row for each measurement group instance. The table has columns:
@@ -45,10 +44,10 @@
                 value1, value2....
             where value n is the value for the nth measurement in the instance (ordered by measurement type)
     :param header: a list of column names
     :param instances: a list of instances returned by formatMeasurementGroup
     :param fname: the filename of the output CSV file
     """
     with open(fname, "w", newline="", encoding="utf-8") as f:
-        writer = csv.writer(f)
-        writer.writerow(header)
-        writer.writerows(instances)
+        wr = writer(f)
+        wr.writerow(header)
+        wr.writerows(instances)
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/data_warehouse.py` & `data-warehouse-client-3.0.0/data_warehouse_client/data_warehouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import datetime
-import sys
+from datetime import datetime
+from sys import exit
 import psycopg2
-import json
+from json import load
 from more_itertools import intersperse
-from data_warehouse_client import transform_result_format
-
-from data_warehouse_client import file_utils
+from transform_result_format import form_measurements, form_measurement_group
+from file_utils import process_sql_template
 
 
 def get_participants_in_result(results):
     """
     find all participants in a set of results
     :param results: a list of measurements. Each measurement is held in a list with the following fields:
                     id,time,study,participant,measurementType,typeName,measurementGroup,
@@ -39,15 +38,16 @@
     A helper function that returns the data warehouse field that holds measurement values of the type
     specified in the parameter
     :param val_type: the type of measurement
     :return: the database field holding the measurement value
     """
     val_types = {0: "measurement.valinteger", 1: "measurement.valreal", 2: "textvalue.textval",
                  3: "datetimevalue.datetimeval", 4: "measurement.valinteger", 5: "measurement.valinteger",
-                 6: "measurement.valinteger", 7: "measurement.valinteger", 8: "measurement.valreal"}
+                 6: "measurement.valinteger", 7: "measurement.valinteger", 8: "measurement.valreal",
+                 9: "datetimevalue.datetimeval", 10: "textvalue.textval"}
     try:
         return val_types[val_type]
     except KeyError:
         print("Error: valType out of range: ", val_type)
         return None
 
 
@@ -72,15 +72,15 @@
 
 
 def core_sql_from_for_measurements():
     """
     Creates the from clause used by many of the functions that query the data warehouse
     :return: the from clause used by several of the functions that query the data warehouse
     """
-    return file_utils.process_sql_template("core_sql_from_for_measurements.sql")
+    return process_sql_template("core_sql_from_for_measurements.sql")
 
 
 def core_sql_for_where_clauses(study: int, participant: int, measurement_type: int, measurement_group: int,
                                group_instance: int, trial: int, start_time, end_time):
     """
     Returns the where clauses used by many of the functions that query the data warehouse to filter out rows
     according to the criteria passed as parameters. A value of -1 for any parameter means that no filter is
@@ -149,15 +149,15 @@
 
 
 def core_sql_select_for_measurements():
     """
      Creates the select clause used by many of the functions that query the data warehouse
      :return: the select clause used by several of the functions that query the data warehouse
      """
-    return file_utils.process_sql_template("core_sql_select_for_measurements.sql")
+    return process_sql_template("core_sql_select_for_measurements.sql")
 
 
 def core_sql_for_measurements():
     """
     Creates the select and from clauses used by many of the functions that query the data warehouse
     :return: the select and from clauses used by several of the functions that query the data warehouse
     """
@@ -169,25 +169,25 @@
         # construct a connection to the warehouse
         self.credentialsFile = credentials_file
         self.dbName = db_name
         # load credentials
         print("Loading credentials..")
         try:
             with open(self.credentialsFile, 'r') as fIn:
-                creds = json.load(fIn)
+                creds = load(fIn)
         except Exception as e:
-            sys.exit("Unable to load the credential's file! Exiting.\n" + str(e))
+            exit("Unable to load the credential's file! Exiting.\n" + str(e))
 
         print("Connecting to the database..")
         # establish connection
         conn_string = f"dbname={self.dbName} user={creds['user']} host={creds['IP']} password={creds['pass']}"
         try:
             self.dbConnection = psycopg2.connect(conn_string)
         except Exception as e:
-            sys.exit("Unable to connect to the database! Exiting.\n" + str(e))
+            exit("Unable to connect to the database! Exiting.\n" + str(e))
         print("Init successful! Running queries.\n")
 
     def get_measurements(self, study, participant=-1, measurement_type=-1, measurement_group=-1, group_instance=-1,
                          trial=-1, start_time=-1, end_time=-1):
         """
         This function returns all measurements in the data warehouse that meet the optional criteria specified
         in the keyword arguments.
@@ -204,17 +204,17 @@
         :return: a list of measurements. Each measurement is held in a list with the following fields:
             id,time,study,participant,measurementType,typeName,measurementGroup, groupInstance,trial,valType,value
         """
         (where_clause, first_condition) = core_sql_for_where_clauses(study, participant, measurement_type,
                                                                      measurement_group,
                                                                      group_instance, trial, start_time, end_time)
         mappings = {"core_sql": core_sql_for_measurements(), "where_clause": where_clause}
-        query = file_utils.process_sql_template("get_measurements.sql", mappings)
+        query = process_sql_template("get_measurements.sql", mappings)
         raw_results = self.return_query_result(query)
-        return transform_result_format.form_measurements(raw_results)
+        return form_measurements(raw_results)
 
     def aggregate_measurements(self, study, measurement_type, aggregation, participant=-1, measurement_group=-1,
                                group_instance=-1, trial=-1, start_time=-1, end_time=-1):
         """
 
         :param measurement_type: the type of the measurements to be aggregated
         :param study: a study id
@@ -259,17 +259,17 @@
         mt_info = self.get_measurement_type_info(study, measurement_type)
         val_type = mt_info[0][2]  # find the value type of the measurement
         # Add a clause to test the field that is relevant to the type of the measurement
         condition = " WHERE " if first_condition else " AND "
         cond = make_value_test(val_type, value_test_condition)
         mappings = {"core_sql": core_sql_for_measurements(), "where_clause": where_clause, "condition": condition,
                     "cond": cond}
-        query = file_utils.process_sql_template("get_measurements_with_value.sql", mappings)
+        query = process_sql_template("get_measurements_with_value.sql", mappings)
         raw_results = self.return_query_result(query)
-        return transform_result_format.form_measurements(raw_results)
+        return form_measurements(raw_results)
 
     def get_measurements_by_cohort(self, study, cohort_id, participant=-1, measurement_type=-1,
                                    measurement_group=-1, group_instance=-1, trial=-1, start_time=-1, end_time=-1):
         """
         Find all measurements in a cohort that meet the criteria.
         :param cohort_id: the value of the category in measurementType 181 that represents the condition
         :param study: a study id
@@ -285,39 +285,39 @@
         """
         (where_clause, first_condition) = core_sql_for_where_clauses(study, participant, measurement_type,
                                                                      measurement_group,
                                                                      group_instance, trial, start_time, end_time)
         condition = " WHERE " if first_condition else " AND "
         mappings = {"core_sql": core_sql_for_measurements(), "where_clause": where_clause, "condition": condition,
                     "cohort_id": str(cohort_id), "study": str(study)}
-        query = file_utils.process_sql_template("get_measurements_by_cohort.sql", mappings)
+        query = process_sql_template("get_measurements_by_cohort.sql", mappings)
         raw_results = self.return_query_result(query)
-        return transform_result_format.form_measurements(raw_results)
+        return form_measurements(raw_results)
 
     def num_types_in_a_measurement_group(self, study, measurement_group):
         """
         A helper function that returns the number of measurement types in a measurement group
         :param study: study id
         :param measurement_group: measurement group id
         :return: number of measurement types in the measurement group
         """
         mappings = {"measurement_group": str(measurement_group), "study": str(study)}
-        query = file_utils.process_sql_template("num_types_in_a_measurement_group.sql", mappings)
+        query = process_sql_template("num_types_in_a_measurement_group.sql", mappings)
         num_types = self.return_query_result(query)
         return num_types[0][0]
 
     def get_types_in_a_measurement_group(self, study, measurement_group):
         """
         A helper function that returns the names of the measurement types in a measurement group
         :param study: study id
         :param measurement_group: measurement group id
         :return: list of names of the measurement types in the measurement group
         """
         mappings = {"measurement_group": str(measurement_group), "study": str(study)}
-        query = file_utils.process_sql_template("types_in_a_measurement_group.sql", mappings)
+        query = process_sql_template("types_in_a_measurement_group.sql", mappings)
         type_names = self.return_query_result(query)
         return type_names
 
     def mk_value_tests(self, value_test_conditions, study):
         """
         Helper function used to creat a Where clause to find measurements that fail the conditions
         :param value_test_conditions:   a list where each element is takes the following form:
@@ -367,16 +367,16 @@
         outer_query = core_sql_for_measurements()
         outer_query += " " + w
         if len(value_test_conditions) > 0:
             outer_query += " AND measurement.groupinstance NOT IN (" + problem_q + ")"
         outer_query += " ORDER BY groupinstance, measurementtype"
         outer_query += ";"
         raw_results = self.return_query_result(outer_query)
-        formed_measurements = transform_result_format.form_measurements(raw_results)
-        return transform_result_format.form_measurement_group(self, study, measurement_group, formed_measurements)
+        formed_measurements = form_measurements(raw_results)
+        return form_measurement_group(self, study, measurement_group, formed_measurements)
 
     def get_measurement_group_instances_for_cohort(self, study, measurement_group, participants, value_test_conditions,
                                                    trial=-1, start_time=-1, end_time=-1):
         """
         Return all instances of a measurement group in which one or more of the measurements within the
             instance meet some specified criteria for the specified cohort of participants
         :param measurement_group: a measurement group
@@ -405,26 +405,26 @@
         outer_query = core_sql_for_measurements()
         outer_query += where_clause
         if len(value_test_conditions) > 0:
             outer_query += " AND measurement.groupinstance NOT IN (" + problem_q + ")"
         outer_query += " ORDER BY groupinstance, measurementtype"
         outer_query += ";"
         raw_results = self.return_query_result(outer_query)
-        formed_measurements = transform_result_format.form_measurements(raw_results)
-        return transform_result_format.form_measurement_group(self, study, measurement_group, formed_measurements)
+        formed_measurements = form_measurements(raw_results)
+        return form_measurement_group(self, study, measurement_group, formed_measurements)
 
     def get_measurement_type_info(self, study, measurement_type_id):
         """
         Returns information on a measurement type
         :param study: the study id
         :param measurement_type_id: the id of a measurement type
         :return: a list containing the elements: id, description, value type, units name
         """
         mappings = {"measurement_type_id": str(measurement_type_id), "study": str(study)}
-        query = file_utils.process_sql_template("get_measurement_type_info.sql", mappings)
+        query = process_sql_template("get_measurement_type_info.sql", mappings)
         return self.return_query_result(query)
 
     def return_query_result(self, query_text):
         """
         executes an SQL query. It is used for SELECT queries.
         :param query_text: the SQL
         :return: the result as a list of rows.
@@ -456,45 +456,45 @@
     def get_all_measurement_groups(self, study):
         """
         A helper function that returns information on all the measurement groups in a study
         :param study: the study id
         :return: a list of [measurement group id, measurement group description]
         """
         mappings = {"study": str(study)}
-        query = file_utils.process_sql_template("get_all_measurement_groups.sql", mappings)
+        query = process_sql_template("get_all_measurement_groups.sql", mappings)
         return self.return_query_result(query)
 
     def get_all_measurement_groups_and_types_in_a_study(self, study):
         """
         A helper function that returns information on all the measurement groups and types in a study
         :param study: the study id
         :return: a list of rows. Each row is a list whose elements are: measurement group id, measurement type id
                    and the name of the measurement type
         """
         # Return all measurement groups and measurement types in a study
         mappings = {"study": str(study)}
-        query = file_utils.process_sql_template("get_all_measurement_groups_and_types_in_a_study.sql", mappings)
+        query = process_sql_template("get_all_measurement_groups_and_types_in_a_study.sql", mappings)
         return self.return_query_result(query)
 
     def insert_measurement_group(self, study, measurement_group, values,
-                                 time=-1, trial=None, participant=None, source=None, cursor=None):  # None maps to SQL NULL
+                                 time=-1, trial=None, participant=None, source=None, cursor=None):
         """
          Insert one measurement group
          :param study: the study id
          :param measurement_group: the measurement group
          :param values: a list of the values from the measurement group in the form (measurementType,valType,value)
          :param time: the time the measurement was taken. It defaults to the current time
          :param trial: optional trial id
          :param participant: optional participant id
          :param source: optional source
          :param cursor: database cursor
          :return success boolean, the measurement group instance, error message
          """
         if time == -1:  # use the current date and time if none is specified
-            time = datetime.datetime.now()  # use the current date and time if none is specified
+            time = datetime.now()  # use the current date and time if none is specified
 
         group_instance = 0   # used temporarily for the first measurement inserted in the measurement group
         insert_error = False  # will be set to true if there is an error inserting any measurement in the group
         if cursor is None:     # no cursor has been passed into the function, so create one
             cur = self.dbConnection.cursor()
         else:
             cur = cursor
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/delete_study_contents.py` & `data-warehouse-client-3.0.0/data_warehouse_client/delete_study_contents.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,57 +10,69 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # only run this if you're certain that you want to remove all metadata and measurements from a study!
 
+from check_for_datetime_table import datetimebounds_table_in_dw
+
 
 def delete_study_contents(dw, study):
     """
     Deletes all measurements and metadata from a study. Only leave entry in the study table
     Designed to clear out a study before a test that will re-populate it
     :param dw: data warehouse handle
     :param study: study id
     """
-    for tab in table_names_to_delete():
+    for tab in table_names_to_delete(dw):
         dw.exec_sql_with_no_return("DELETE FROM " + tab + " WHERE study = " + str(study))
 
 
 def delete_study_measurements(dw, study):
     """
     Deletes all measurements from a study. Only leave entries in the study and trial tables
     Designed to clear out a study before a test that will re-populate it
     :param dw: data warehouse handle
     :param study: study id
     """
     for tab in measurement_table_names():
         dw.exec_sql_with_no_return("DELETE FROM " + tab + " WHERE study = " + str(study))
 
 
-def table_names_to_delete():
+def table_names_to_delete(dw):
     """
+    :param dw: data warehouse handle
     :return: the names of all the tables in the data warehouse in a study to be deleted (all but study)
     """
-    return measurement_table_names() + metadata_table_names()
+    return measurement_table_names() + metadata_table_names(dw)
 
 
 def measurement_table_names():
     """
     :return: the names of all the tables in the data warehouse that hold measurements
     """
     return ['textvalue', 'datetimevalue', 'measurement']
 
 
-def metadata_table_names():
+def metadata_table_names(dw):
     """
+    :param dw: data warehouse handle
     :return: the names of all the tables in the data warehouse that hold metadata
     """
-    return ['measurementtypetogroup', 'boundsreal', 'boundsint', 'category', 'measurementtype', 'units',
-            'measurementgroup', 'source', 'sourcetype', 'participant', 'trial']
+    if datetimebounds_table_in_dw(dw):
+        return ['measurementtypetogroup',
+                'boundsreal', 'boundsint', 'boundsdatetime',
+                'category', 'measurementtype', 'units',
+                'measurementgroup', 'source', 'sourcetype', 'participant', 'trial']
+    else:
+        return ['measurementtypetogroup',
+                'boundsreal', 'boundsint',
+                'category', 'measurementtype', 'units',
+                'measurementgroup', 'source', 'sourcetype', 'participant', 'trial']
 
 
 def delete_study_completely(dw, study):
     """
     Deletes everything in a study: use with care
     :param dw: data warehouse handle
     :param study: study id
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/load_warehouse_helpers.py` & `data-warehouse-client-3.0.0/data_warehouse_client/load_warehouse_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
 from datetime import datetime
 import unidecode
+from typing import Tuple, List, Any, Callable
+import itertools
+import type_checks
+from type_definitions import MeasurementGroup, LoadHelperResult, LoaderResult, DataToLoad
 
 
 def process_message_group(mg_triples):
     """
     takes the result of attempting to load each field in a message group and processes it
-    :param mg_triples: list of (successful load?, ((measurement_ttpe, valtype, value)))
-    :return: Success?, the list of (measurement_type, valtype, value) triples, the error message list
+    :param mg_triples: [(Success?, [(measurement_type, valtype, value)], Error Message)]
+    :return: Success?, [(measurement_type, valtype, value)], [error messages]
     """
     success_index = 0
     triple_index = 1
     error_message_index = 2
     oks = list(map(lambda r: r[success_index], mg_triples))     # get a list of the bools indicating success
     triples = list(map(lambda r: r[triple_index], mg_triples))  # get a list of the triples
     if functools.reduce(lambda x, y: x and y, oks):             # if all value in message group are correct....
@@ -52,42 +56,42 @@
     :param jfield: the field name
     :param measurement_type: the measurement type
     :param data: the data in which the field is missing
     :param val_type: the correct type of the field
     :return: error message
     """
     return f'Wrong type for {jfield} (measurement type {measurement_type}) in data {data};' +\
-           f'it should be a {type_names(val_type)} (value type {val_type})'
+           f' it should be a {type_names(val_type)} (value type {val_type})'
 
 
 def type_names(val_type):
     """
     return the name of a type represented by a number
     :param val_type: int representing a type in the warehouse
     :return: name
     """
     if val_type in [0, 5, 6, 7]:  # 5 and 6 are there for ordinals and nominals created from id
         return "integer"
     elif val_type in [1, 8]:
         return "real"
-    elif val_type == 3:
+    elif val_type in [3, 9]:
         return "datetime"
     elif val_type == 4:
         return "boolean"
     else:
         return "string"
 
 
 def convert_epoch_in_ms_to_string(timestamp_in_ms):
     """
     converts timestamp in ms epoch format to string
     :param timestamp_in_ms: epoch timestamp in ms
     :return: well_formed, date time string
     """
-    if check_int(timestamp_in_ms):
+    if type_checks.check_int(timestamp_in_ms):
         timestamp_in_sec = int(timestamp_in_ms)//1000
         try:
             time_val = datetime.fromtimestamp(timestamp_in_sec)
             return True, str(time_val)
         except Exception:
             return False, None
     else:
@@ -99,78 +103,14 @@
     converts timestamp in ms epoch format to string
     :param val: posix timestamp
     :return: well_formed, date time string
     """
     return True, val.replace('T', ' ')
 
 
-def check_int(string):
-    """
-    Check if a string represents an integer
-    :param string: string
-    :return: True if the string represents an integer
-    """
-    try:
-        val = int(string)
-        return True
-    except ValueError:
-        return False
-
-
-def check_real(string):
-    """
-    Check if a string represents a real
-    :param string: string
-    :return: True if the string represents a real
-    """
-    try:
-        val = float(string)
-        return True
-    except ValueError:
-        return False
-
-
-def check_datetime(string):
-    """
-    Check if a string represents a datetime
-    :param string: string
-    :return: True if the string represents a datetime
-    """
-    return True  # need to add checking later
-
-
-def check_boolean(string):
-    """
-    Check if a string represents a boolean
-    :param string: 
-    :return: True if the string represents a boolean
-    """
-    return string in ['T', 'Y', 'F', 'N', '0', '1', 0, 1]
-
-
-def type_check(val, val_type):
-    """
-    Check the type of a value retrieved from a field
-    :param val: value
-    :param val_type: the type is should be
-    :return: True if the value has the right type, False otherwise
-    """
-    if val_type in [0, 5, 6, 7]:  # 5 and 6 are there for ordinals and nominals created from id
-        well_typed = check_int(val)
-    elif val_type in [1, 8]:
-        well_typed = check_real(val)
-    elif val_type == 3:
-        well_typed = check_datetime(val)
-    elif val_type == 4:
-        well_typed = check_boolean(val)
-    else:
-        well_typed = True  # everything else is a string
-    return well_typed
-
-
 def get_and_check_value(measurement_type, val_type, data, jfield, optional):
     """
     check if a value exists, and if so its type
     :param measurement_type: measurement type of jfield in the data warehouse
     :param val_type: the type of the value to be stored
     :param data: json that contains the jfield
     :param jfield: the name of the field
@@ -183,15 +123,15 @@
         exists = False
         well_typed = False  # default
     elif val == "":
         exists = False
         well_typed = False  # default
     else:
         exists = True
-        well_typed = type_check(val, val_type)
+        well_typed = type_checks.type_check(val, val_type)
     if (not optional) and (not exists):
         error_message = missing_mandatory_type_error_message(jfield, measurement_type, data)
     elif exists and (not well_typed):
         error_message = wrong_type_error_message(jfield, measurement_type, data, val_type)
     return exists, well_typed, val, error_message
 
 
@@ -524,17 +464,17 @@
     :param jfield: the name of the field
     :return : Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
     """
     (exists, well_formed, val, error_messsage) = get_and_check_value(measurement_type, 4, data, jfield, False)
     # val_type is set to 2 for checking as the field is expected to be a string ("T" or "Y") or ("F" or "N")
     if exists and well_formed:
         if val in ['0', 'N', 'F', 0]:
-            val01 = mk_bool_string(False)
+            val01 = mk_bool(False)
         else:
-            val01 = mk_bool_string(True)  # must be 'Y' or 'T' or '1' or 1
+            val01 = mk_bool(True)  # must be 'Y' or 'T' or '1' or 1
         return True, [(measurement_type, 4, val01)], ""
     else:
         return False, [], error_messsage
 
 
 def mk_optional_boolean(measurement_type, data, jfield):
     """
@@ -542,21 +482,21 @@
     If not then return an empty list.
         :param measurement_type:    measurement type of jfield in the data warehouse
         :param data:                json that may contain the jfield
         :param jfield:              the name of the field
         :return                     if the field exists then a list is returned holding the appropriate entry
                                     if the field doesn't exist then an empty list is returned
         """
-    (exists, well_formed, val, error_message) = get_and_check_value(measurement_type, 2, data, jfield, True)
+    (exists, well_formed, val, error_message) = get_and_check_value(measurement_type, 4, data, jfield, True)
     # val_type is set to 2 for checking as the field is expected to be a string "T" or "F"
     if exists and well_formed:
         if val in ['0', 'N', 'F', 0]:
-            val01 = mk_bool_string(False)
+            val01 = mk_bool(False)
         else:
-            val01 = mk_bool_string(True)  # must be 'Y' or 'T' or '1' or 1
+            val01 = mk_bool(True)  # must be 'Y' or 'T' or '1' or 1
         return True, [(measurement_type, 4, val01)], ""
     elif exists and not well_formed:
         return False, [], error_message
     else:
         return True, [], ""  # it's optional so OK if the field is not found
 
 
@@ -665,14 +605,94 @@
     :param data: the json structure
     :param jfield: the name of the field
     :return: Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
     """
     return mk_basic_field(measurement_type, 6, data, jfield)
 
 
+def mk_categorical_from_id_with_id_check(measurement_type, data, jfield, id_list, val_type, optional: bool):
+    """
+    :param measurement_type: the id of the measurementtype that will hold the value
+    :param data: the json structure
+    :param jfield: the name of the field
+    :param id_list: list containing the acceptable value of the id
+    :param val_type: 5 for nominal, 6 for ordinal
+    :param optional: boolean that is True if the id is optional
+    :return: Success?, [(measurement_type, valtype, value for the jfield in the data)], error_message
+    """
+    if optional:
+        success, result, error_message = mk_optional_basic_field(measurement_type, val_type, data, jfield)
+    else:
+        success, result, error_message = mk_basic_field(measurement_type, val_type, data, jfield)
+    if success and result != []:  # need to check if value returned is in bounds
+        (measurement_type_returned, val_type_returned, value) = result[0]  # pick the triple from the singleton list
+        if value in id_list:
+            return True, result, ""  # acceptable id value
+        else:  # id is out of range
+            return False, [], f'Category id error for {jfield} (measurement type {measurement_type}) in data: {data}'
+    else:  # in all other cases just return without a check (as no result was returned)
+        return success, result, error_message
+
+
+def mk_nominal_from_id_with_id_check(measurement_type, data, jfield, id_list):
+    """
+    make a nominal triple (measurement_type, 5, value) where the id is stored in the jfield
+    Check it's in range
+    :param measurement_type: the id of the measurementtype that will hold the value
+    :param data: the json structure
+    :param jfield: the name of the field
+    :param id_list: list containing the acceptable value of the id
+    :return: Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
+    """
+    nominal_valtype: int = 5
+    return mk_categorical_from_id_with_id_check(measurement_type, data, jfield, id_list, nominal_valtype, False)
+
+
+def mk_optional_nominal_from_id_with_id_check(measurement_type, data, jfield, id_list):
+    """
+    make a nominal triple (measurement_type, 5, value) where the id is stored in the jfield
+    Check it's in range
+    :param measurement_type: the id of the measurementtype that will hold the value
+    :param data: the json structure
+    :param jfield: the name of the field
+    :param id_list: list containing the acceptable value of the id
+    :return: Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
+    """
+    nominal_valtype: int = 5
+    return mk_categorical_from_id_with_id_check(measurement_type, data, jfield, id_list, nominal_valtype, True)
+
+
+def mk_ordinal_from_id_with_id_check(measurement_type, data, jfield, id_list):
+    """
+    make a nominal triple (measurement_type, 6, value) where the id is stored in the jfield
+    Check it's in range
+    :param measurement_type: the id of the measurementtype that will hold the value
+    :param data: the json structure
+    :param jfield: the name of the field
+    :param id_list: list containing the acceptable value of the id
+    :return: Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
+    """
+    ordinal_valtype: int = 6
+    return mk_categorical_from_id_with_id_check(measurement_type, data, jfield, id_list, ordinal_valtype, False)
+
+
+def mk_optional_ordinal_from_id_with_id_check(measurement_type, data, jfield, id_list):
+    """
+    make an odinal triple (measurement_type, 6, value) where the id is stored in the jfield
+    Check it's in range
+    :param measurement_type: the id of the measurementtype that will hold the value
+    :param data: the json structure
+    :param jfield: the name of the field
+    :param id_list: list containing the acceptable value of the id
+    :return: Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
+    """
+    ordinal_valtype: int = 6
+    return mk_categorical_from_id_with_id_check(measurement_type, data, jfield, id_list, ordinal_valtype, True)
+
+
 def mk_optional_nominal_from_dict(measurement_type, data, jfield, cat_dict):
     """
     If the jfield exists in the data then return [(measurement_ttpe, valtype, value for the jfield in the data)].
     If not then return an empty list.
     :param measurement_type: the id of the measurementtype that hold the value if it exists
     :param data: the json structure
     :param jfield: the name of the optional field
@@ -729,14 +749,26 @@
     """
     if bool_val:
         return '1'
     else:
         return '0'
 
 
+def mk_bool(bool_val: bool) -> int:
+    """
+    COnvert a boolean value to an integer ready to be inserted into the measurement table
+    :param bool_val: boolean
+    :return: integer (0 = False, 1 = True)
+    """
+    if bool_val:
+        return 1
+    else:
+        return 0
+
+
 def split_enum(measurement_types, data, jfield, valuelist):
     """
     ENUMS (Sets of values) are not represented directly in the warehouse. Instead they are represented as one boolean
     measurementtype per value. This function takes a json list of values and creates the list of measurements from it -
     one for each type.
     :param measurement_types: the list of measurement_types of the measurements into which the booleans are to be stored
     :param data: the json structure
@@ -752,15 +784,15 @@
         exists = False
     elif values == "":
         exists = False
     else:
         exists = True
     if exists:
         for (measurement_type, value) in zip(measurement_types, valuelist):
-            res = res + [(measurement_type, 4, mk_bool_string(value in values))]  # the 4 is because the type is boolean
+            res = res + [(measurement_type, 4, mk_bool(value in values))]  # the 4 is because the type is boolean
         return True, res, ""
     else:
         return False, [], f'Missing Mandatory ENUM field {jfield} for measurement_types {measurement_types} in {data}'
 
 
 def split_optional_enum(measurement_types, data, jfield, valuelist):
     """
@@ -781,20 +813,133 @@
         exists = False
     elif values == "":
         exists = False
     else:
         exists = True
     if exists:
         for (measurement_type, value) in zip(measurement_types, valuelist):
-            res = res + [(measurement_type, 4, mk_bool_string(value in values))]  # the 4 is because the type is boolean
+            res = res + [(measurement_type, 4, mk_bool(value in values))]  # the 4 is because the type is boolean
         return True, res, ""
     else:
         return True, [], ""  # Field doesn't exist, which is OK as this is an optional field
 
 
+def mk_bounded_datetime(measurement_type, data, jfield):
+    """
+    create a (measurement_type, valtype, value for the jfield in the data) triple for a bounded datetime
+    :param measurement_type: measurement type of jfield in the data warehouse
+    :param data: json that may contain the jfield
+    :param jfield: the name of the field
+    :return: Error free?, [(measurement_type, valtype, value for the jfield in the data)], error_message
+    """
+    bounded_datetime_type = 9
+    return mk_basic_field(measurement_type, bounded_datetime_type, data, jfield)
+
+
+def mk_optional_bounded_datetime(measurement_type, data, jfield):
+    """
+    If the jfield exists in the data then return [(measurement_ttpe, valtype, value for the jfield in the data)].
+    If not then return an empty list.
+        :param measurement_type:    measurement type of jfield in the data warehouse
+        :param data:                json that may contain the jfield
+        :param jfield:              the name of the field
+        :return                     Error free?, if field exists then a list is returned holding the appropriate entry
+                                    if the field doesn't exist then an empty list is returned, Error message
+        """
+    bounded_datetime_type = 9
+    return mk_optional_basic_field(measurement_type, bounded_datetime_type, data, jfield)
+
+
+def mk_optional_external(measurement_type, data, jfield):
+    """
+    If the jfield exists in the data then return [(measurement_ttpe, valtype, value for the jfield in the data)].
+    If not then return an empty list.
+        :param measurement_type:    measurement type of jfield in the data warehouse
+        :param data:                json that may contain the jfield
+        :param jfield:              the name of the field
+        :return                     Error free?, if field exists then a list is returned holding the appropriate entry
+                                    if the field doesn't exist then an empty list is returned, Error message
+        """
+    external_type = 10
+    return mk_optional_basic_field(measurement_type, external_type, data, jfield)
+
+
+def mk_external(measurement_type, data, jfield):
+    """
+    create a (measurement_type, valtype, value for the jfield in the data) triple for an external reference
+    :param measurement_type: measurement type of jfield in the data warehouse
+    :param data: json that may contain the jfield
+    :param jfield: the name of the field
+    :return: Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
+    """
+    external_type = 10
+    return mk_basic_field(measurement_type, external_type, data, jfield)
+
+
+def concat(ls: List[List[Any]]) -> List[Any]:
+    """
+    Concatenate a list of lists
+    :param ls:  list of lists
+    :return: list
+    """
+    return list(itertools.chain.from_iterable(ls))
+
+
+def load_a_list(data: DataToLoad,
+                jfield: str,
+                loader: Callable[[DataToLoad], LoaderResult],
+                mg_id: MeasurementGroup,
+                optional: bool) ->\
+        List[Tuple[MeasurementGroup, List[LoadHelperResult]]]:
+    """
+    Load a list within data loaded into the
+    :param data: data to load into warehouse - held in a Dictionary
+    :param jfield: name of the field in the Dictionary
+    :param loader: function to load the data
+    :param mg_id: measurement group id - only used if the jfield is not found
+    :param optional: True if the list is optional
+    :return: list of measurement group ids and the values to load into them
+    """
+    list_val: List[DataToLoad] = data.get(jfield)   # extract the list field
+    if list_val is None:  # missing field
+        if optional:
+            return []    # if optional then it's not an error
+        else:   # there should have been a list, so flag an error
+            return [(mg_id, [(False, [], f'Missing mandatory field {jfield} (list expected) in data: {data}')])]
+    else:  # the list exists
+        # create a single, combined list and ignore the optional fields (Time, Trial, Participant, Source)
+        return concat(list(map(lambda e: loader(e)[0], list_val)))
+
+
+def load_list(data: DataToLoad, jfield: str, loader: Callable[[DataToLoad], LoaderResult],
+              mg_id: MeasurementGroup) -> List[Tuple[MeasurementGroup, List[LoadHelperResult]]]:
+    """
+
+    :param data: data to load into warehouse - held in a Dictionary
+    :param jfield: name of the field in the Dictionary
+    :param loader: function to load the data
+    :param mg_id: measurement group id - only used if the jfield is not found
+    :return: list of measurement group ids and the values to load into them
+    """
+    return load_a_list(data, jfield, loader, mg_id, False)
+
+
+def load_optional_list(data: DataToLoad, jfield: str, loader, mg_id: MeasurementGroup) ->\
+        List[Tuple[MeasurementGroup, List[LoadHelperResult]]]:
+    """
+
+    :param data: data to load into warehouse - held in a Dictionary
+    :param jfield: name of the field in the Dictionary
+    :param loader: function to load the data
+    :param mg_id: measurement group id - only used if the jfield is not found
+    :return: list of measurement group ids and the values to load into them
+    """
+    return load_a_list(data, jfield, loader, mg_id, True)
+
+
 def get_converter_fn(event_type, mapper_dict):
     """
     map from the event_type to the mapper function and message group
     :param event_type: the e-Science Central event type
     :param mapper_dict: the dictionary that maps from the event_type to the mapper function and message group
     :return: (boolean indicating if the event_type is found, mapper function, measurement group
     """
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/plot.py` & `data-warehouse-client-3.0.0/data_warehouse_client/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from data_warehouse_client import data_warehouse
 import matplotlib.pyplot as pyplot
 from matplotlib.backends.backend_pdf import PdfPages
 import print_metadata_table
 import datetime
 import numpy as np
 
 
@@ -122,15 +121,7 @@
                     pyplot.bar(['False', 'True'], [f_count, t_count])
                     pyplot.title(f'{mg_name} ({mg_id}) / {mt_name} ({mt_id})')
                     pyplot.close()
                     pdf.savefig(fig)
 #              else:
                     # print('No Measurements Recorded', file=f)
     pdf.close()
-
-
-# test it out
-#  dw_handle = data_warehouse.DataWarehouse("db-credentials-read-only.json", "datawarehouse")
-#
-#  study_id = 8
-#
-#  plot_distributions(dw_handle, study_id)
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/print_io.py` & `data-warehouse-client-3.0.0/data_warehouse_client/print_io.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/print_metadata_table.py` & `data-warehouse-client-3.0.0/data_warehouse_client/print_metadata_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from data_warehouse_client import file_utils
+from file_utils import process_sql_template
 from tabulate import tabulate  # https://github.com/astanin/python-tabulate
 import datetime
+from check_for_datetime_table import datetimebounds_table_in_dw
 
 
 def valuetype_to_name():
     return {0: 'Integer', 1: 'Real', 2: 'Text', 3: 'Date Time', 4: 'Boolean',
-            5: 'Nominal', 6: 'Ordinal', 7: 'Bounded Integer', 8: 'Bounded Real'}
+            5: 'Nominal', 6: 'Ordinal', 7: 'Bounded Integer', 8: 'Bounded Real',
+            9: 'Bounded Date Time', 10: 'External'}
 
 
 def mk_txt_report_file_name(f_dir, report_name, time_string):
     return f_dir + report_name + time_string + ".txt"
 
 
 def print_metadata_tables_to_file(dw, study_id):
@@ -48,14 +50,17 @@
                 upper_bound = ''
                 if mt_info['intbounds'] != {}:
                     lower_bound = mt_info['intbounds']['minval']
                     upper_bound = mt_info['intbounds']['maxval']
                 elif mt_info['realbounds'] != {}:
                     lower_bound = mt_info['realbounds']['minval']
                     upper_bound = mt_info['realbounds']['maxval']
+                elif mt_info['datetimebounds'] != {}:
+                    lower_bound = mt_info['datetimebounds']['minval']
+                    upper_bound = mt_info['datetimebounds']['maxval']
                 if mt_info['units'] is None:
                     units_prnt = ""
                 else:
                     units_prnt = mt_info['units']
                 row = [mt_info['name'], mt_id, valuetype_to_name()[mt_info['valtype']],
                        mt_info['optional'], units_prnt, lower_bound, upper_bound, cats]
                 rows = rows + [row]
@@ -80,14 +85,17 @@
             upper_bound = ''
             if mt_info['intbounds'] != {}:
                 lower_bound = mt_info['intbounds']['minval']
                 upper_bound = mt_info['intbounds']['maxval']
             elif mt_info['realbounds'] != {}:
                 lower_bound = mt_info['realbounds']['minval']
                 upper_bound = mt_info['realbounds']['maxval']
+            elif mt_info['datetimebounds'] != {}:
+                lower_bound = mt_info['datetimebounds']['minval']
+                upper_bound = mt_info['datetimebounds']['maxval']
             if mt_info['units'] is None:
                 units_prnt = ""
             else:
                 units_prnt = mt_info['units']
             row = [mt_info['name'], mt_id, valuetype_to_name()[mt_info['valtype']],
                    mt_info['optional'], units_prnt, lower_bound, upper_bound, cats]
             rows = rows + [row]
@@ -110,43 +118,52 @@
 def create_measurement_group_info(dw, study):
     """
     Creates a dictionary with each entry a measurement group
     :param dw: data warehouse handle
     :param study: study id
     :return:
     """
-    q1 = file_utils.process_sql_template("get_measurement_group_info.sql", {"study": study})
+    q1 = process_sql_template("get_measurement_group_info.sql", {"study": study})
     r1 = dw.return_query_result(q1)  # return a list of (measurementgroup, measurementtype, name, valtype, optional)
 
-    q2 = file_utils.process_sql_template("get_categories_in_study.sql", {"study": study})
+    q2 = process_sql_template("get_categories_in_study.sql", {"study": study})
     r2 = dw.return_query_result(q2)
 
     cats = {}
     for mt in set([row[0] for row in r2]):
         cats[mt] = dict(map(lambda t: (t[2], t[1]),  filter(lambda r: r[0] == mt, r2)))
 
-    q3 = file_utils.process_sql_template("get_boundsint_in_study.sql", {"study": study})
+    q3 = process_sql_template("get_boundsint_in_study.sql", {"study": study})
     r3 = dw.return_query_result(q3)
     int_bounds = {}
     for [mt_id, minval, maxval] in r3:
         int_bounds[mt_id] = {'minval': minval, 'maxval': maxval}
 
-    q4 = file_utils.process_sql_template("get_boundsreal_in_study.sql", {"study": study})
+    q4 = process_sql_template("get_boundsreal_in_study.sql", {"study": study})
     r4 = dw.return_query_result(q4)
     real_bounds = {}
     for [mt_id, minval, maxval] in r4:
         real_bounds[mt_id] = {'minval': minval, 'maxval': maxval}
 
-    q5 = file_utils.process_sql_template("get_measurement_groups_in_study.sql", {"study": study})
+    if datetimebounds_table_in_dw(dw):
+        q4a = process_sql_template("get_boundsdatetime_in_study.sql", {"study": study})
+        r4a = dw.return_query_result(q4a)
+        datetime_bounds = {}
+        for [mt_id, minval, maxval] in r4a:
+            datetime_bounds[mt_id] = {'minval': minval, 'maxval': maxval}
+    else:
+        datetime_bounds = {}
+
+    q5 = process_sql_template("get_measurement_groups_in_study.sql", {"study": study})
     r5 = dw.return_query_result(q5)
     mg_names = {}
     for [mg_id, mg_name] in r5:
         mg_names[mg_id] = mg_name
 
-    q6 = file_utils.process_sql_template("get_units_in_study.sql", {"study": study})
+    q6 = process_sql_template("get_units_in_study.sql", {"study": study})
     r6 = dw.return_query_result(q6)
     unit_name = {}
     for [mt_id, unit_description] in r6:
         unit_name[mt_id] = unit_description
 
     mg_info = {}
     for mg in set([row[0] for row in r1]):
@@ -163,17 +180,23 @@
             else:
                 int_bounds_val = intbounds
             realbounds = real_bounds.get(ms_type)
             if realbounds is None:
                 real_bounds_val = {}
             else:
                 real_bounds_val = realbounds
+            datetimebounds = datetime_bounds.get(ms_type)
+            if datetimebounds is None:
+                datetime_bounds_val = {}
+            else:
+                datetime_bounds_val = datetimebounds
             unitname = unit_name.get(ms_type)
             if unitname is None:
                 units_val = None
             else:
                 units_val = unitname
             mt_info = {'name': name, 'valtype': valtype, 'optional': mk_optional(optional), 'units': units_val,
-                       'categories': cat_val, 'intbounds': int_bounds_val, 'realbounds': real_bounds_val}
+                       'categories': cat_val, 'intbounds': int_bounds_val, 'realbounds': real_bounds_val,
+                       'datetimebounds': datetime_bounds_val}
             mt_info_all[ms_type] = mt_info
         mg_info[mg] = {'name': mg_names[mg], 'message_types': mt_info_all}
     return mg_info
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/sql/bounded_integers.sql` & `data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_integers.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/sql/bounded_reals.sql` & `data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_reals.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/sql/core_sql_from_for_measurements.sql` & `data-warehouse-client-3.0.0/data_warehouse_client/sql/core_sql_from_for_measurements.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/sql/get_measurement_group_info.sql` & `data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurement_group_info.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/study_profile.py` & `data-warehouse-client-3.0.0/data_warehouse_client/study_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import pandas as pd
 import pandas_profiling as pp
-import datetime
+from datetime import datetime
 
 
 def mk_html_report_file_name(f_dir, report_name, time_string):
     return f_dir + report_name + time_string + ".html"
 
 
 def profile_all_measurement_groups(dw, study, report_dir, select_participants=False, participants=[],
@@ -32,15 +32,15 @@
     :param select_participants: select a subset of participants to be included in the profile
     :param participants: list of participants to be included in the profile if select_participants is true
     :param select_trials: select a subset of trials to be included in the profile
     :param trials: list of trials to be included in the profile if select_trials is true
     :param hide_trial_column: don't include the Trial column (useful for studies where trial is not used)
     :param filename_prefix: optional string to add to front of filename
     """
-    timestamp = datetime.datetime.now()                        # use the current date and time in the filenames
+    timestamp = datetime.now()                        # use the current date and time in the filenames
     time_fname_str = timestamp.strftime('%Y-%m-%dh%Hm%Ms%S')   # format the date time string used in the filename
     measurement_groups = dw.get_all_measurement_groups(study)  # get all the measurement groups in the study
 
     for [mg_id, mg_name] in measurement_groups:                # for each measurement group
         (header, instances) = dw.get_measurement_group_instances(study, mg_id, [])   # extract header and all instances
         df_full = pd.DataFrame(instances, columns=header)                            # create a pandas data frame
         if select_participants:   # select participants
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/study_summary.py` & `data-warehouse-client-3.0.0/data_warehouse_client/study_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 # Summarise a study
 
 from tabulate import tabulate
-from data_warehouse_client import print_io
-from data_warehouse_client import csv_io
-import datetime
+from print_io import print_measurement_group_instances, print_measurement_group_instances_to_file
+from csv_io import export_measurement_groups_as_csv
+from datetime import datetime
 
 
 def get_instances_per_measurement_group(dw, study):
     """
     Returns the number of instances in all measurement groups in a study
     :param dw: data warehouse handle
     :param study: study id
@@ -46,15 +46,15 @@
     print(f'All Measurement Group Instances in Study {study}')
     measurement_groups = dw.get_all_measurement_groups(study)
     print()
     for [mg_id, mg_name] in measurement_groups:
         (header, instances) = dw.get_measurement_group_instances(study, mg_id, [])
         if len(instances) > 0:
             print(f'All measurements in group {mg_id} ({mg_name}) for Study {study} \n')
-            print_io.print_measurement_group_instances(header, instances)
+            print_measurement_group_instances(header, instances)
             print()
 
 
 def print_study_summary(dw, study):
     """
     Print a summary of the number of participants and the total instances in each measgeurement group in a study
     :param dw: data warehouse handle
@@ -94,44 +94,44 @@
 def print_all_instances_in_a_study_to_file(dw, study):
     """
     Print to a file all instances in a study - don't print for measurement groups that have no measurements
     :param dw: data warehouse handle
     :param study: study id
     """
     file_dir = "reports/"
-    timestamp = datetime.datetime.now()  # use the current date and time if none is specified
+    timestamp = datetime.now()  # use the current date and time if none is specified
     time_fname_str = timestamp.strftime('%Y-%m-%dh%Hm%Ms%S')
     fname = mk_txt_report_file_name(file_dir, "study-instances-", time_fname_str)
     with open(fname, "w", encoding="utf-8") as f:
         print(f'All Measurement Group Instances in Study {study}\n', file=f)
         measurement_groups = dw.get_all_measurement_groups(study)
         for [mg_id, mg_name] in measurement_groups:
             (header, instances) = dw.get_measurement_group_instances(study, mg_id, [])
             if len(instances) > 0:
                 print(f'All measurements in group {mg_id} ({mg_name}) for Study {study} \n', file=f)
-                print_io.print_measurement_group_instances_to_file(header, instances, f)
+                print_measurement_group_instances_to_file(header, instances, f)
                 print('\n', file=f)
 
 
 def print_all_instances_in_a_study_to_csv_files(dw, study):
     """
     Print all instances in a study to a set of csvs - one per measurement group
     Now depreciated. Use print_instances_in_a_study_to_csv_files
     :param dw: data warehouse handle
     :param study: study id
     """
     file_dir = "reports/"
-    timestamp = datetime.datetime.now()  # use the current date and time if none is specified
+    timestamp = datetime.now()  # use the current date and time if none is specified
     time_fname_str = timestamp.strftime('%Y-%m-%dh%Hm%Ms%S')
     measurement_groups = dw.get_all_measurement_groups(study)
     for [mg_id, mg_name] in measurement_groups:
         (header, instances) = dw.get_measurement_group_instances(study, mg_id, [])
         if len(instances) > 0:
             fname = mk_csv_report_file_name(file_dir, "study-instances-" + mg_name + "-", time_fname_str)
-            csv_io.export_measurement_groups_as_csv(header, instances, fname)
+            export_measurement_groups_as_csv(header, instances, fname)
 
 
 def mk_participants_dictionary(dw, study):
     """
     Create a dictionary containing mapping from participant_id to local_id for all the participants in a study
     :param dw: data warehouse handle
     :param study: study_id
@@ -156,75 +156,75 @@
     :param participants: list of participants to be included in the profile if select_participants is true
     :param local_participant_id: include the local participant id if this boolean is True
     :param filename_prefix: optional string to add to front of filename
     :param print_empty_files: optional boolean to print csv files with no instances in them
     """
     if local_participant_id:
         participant_local_id = mk_participants_dictionary(dw, study)   # create a dictionary mapping from id to local id
-    timestamp = datetime.datetime.now()  # use the current date and time if none is specified
+    timestamp = datetime.now()  # use the current date and time if none is specified
     time_fname_str = timestamp.strftime('%Y-%m-%dh%Hm%Ms%S')
     participant_index = 3  # the participant_id is in position 3 of the list
     measurement_groups = dw.get_all_measurement_groups(study)
     for [mg_id, mg_name] in measurement_groups:
         (header, all_instances) = dw.get_measurement_group_instances(study, mg_id, [])
         if select_participants:  # select participants
-            instances = list(filter(lambda instance: instance[participant_index] in participants, all_instances))
+            instances = list(filter(lambda inst: inst[participant_index] in participants, all_instances))
         else:
             instances = all_instances
         if (len(instances) > 0) or print_empty_files:   # if there are some instances in the measurement group
                                                         #  or if files should be created even if there are no instances
             fname = mk_csv_report_file_name(report_dir, filename_prefix +
                                             "study-instances-" + mg_name + "-", time_fname_str)
             if local_participant_id:
                 instances_with_local_participant_id = []
                 extended_header = ['Local Participant'] + header
                 for instance in instances:  # add the local participant id to the start of each row
                     participant_id = instance[participant_index]  # get unique participant id
                     local_participant = participant_local_id[participant_id]  # get the local participant id
                     instances_with_local_participant_id = instances_with_local_participant_id +\
                                                           [[local_participant] + instance]
-                    csv_io.export_measurement_groups_as_csv(extended_header, instances_with_local_participant_id, fname)
+                    export_measurement_groups_as_csv(extended_header, instances_with_local_participant_id, fname)
             else:  # don't include local id
-                csv_io.export_measurement_groups_as_csv(header, instances, fname)
+                export_measurement_groups_as_csv(header, instances, fname)
 
 
 def print_all_instances_in_a_study_with_local_participant_id_to_csv_files(dw, study):
     """
     Print all instances in a study to a set of csvs - one per measurement group - including participants
     This is now depreciated. Use print_instances_in_a_study_to_csv_files
     :param dw: data warehouse handle
     :param study: study id
     """
     file_dir = "reports/"
     participant_id_index = 3
-    timestamp = datetime.datetime.now()  # use the current date and time if none is specified
+    timestamp = datetime.now()  # use the current date and time if none is specified
     time_fname_str = timestamp.strftime('%Y-%m-%dh%Hm%Ms%S')
     measurement_groups = dw.get_all_measurement_groups(study)
     for [mg_id, mg_name] in measurement_groups:
         (header, instances) = dw.get_measurement_group_instances(study, mg_id, [])
         extended_header = ['Local Participant'] + header
         if len(instances) > 0:  # if there are some instances in the measurement group
             fname = mk_csv_report_file_name(file_dir, "study-instances-" + mg_name + "-", time_fname_str)
             instances_with_local_participant_id = []
             for instance in instances:  # add the local participant id to the start of each row
                 participant_id = instance[participant_id_index]  # get unique participant id
                 (success, part) = dw.get_participant_by_id(study, participant_id)  # get local participant id
                 instances_with_local_participant_id = instances_with_local_participant_id + [[part] + instance]
-            csv_io.export_measurement_groups_as_csv(extended_header, instances_with_local_participant_id, fname)
+            export_measurement_groups_as_csv(extended_header, instances_with_local_participant_id, fname)
 
 
 def print_study_summary_to_file(dw, study):
     """
     Print to a file a summary of the number of participants and the total instances in each measurement group in a study
     :param dw: data warehouse handle
     :param study: study id
     :return:
     """
     file_dir = "reports/"
-    timestamp = datetime.datetime.now()  # use the current date and time if none is specified
+    timestamp = datetime.now()  # use the current date and time if none is specified
     time_fname_str = timestamp.strftime('%Y-%m-%dh%Hm%Ms%S')
     fname = mk_txt_report_file_name(file_dir, "study-summary-", time_fname_str)
     with open(fname, "w", encoding="utf-8") as f:
         print(f'Summary of Study {study}', file=f)
         # Get Number of Participants
         n_participants = len(dw.get_participants(study))
         print(f'Number of Participants in Study {study}: {n_participants}', file=f)
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/table_reader_json.py` & `data-warehouse-client-3.0.0/data_warehouse_client/table_reader_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
+from json import load
 
 
 def read_json_tables(file_name):
     """
     Reads a table stored in a json file
     :param file_name: filename in which to store the output (in directory output)
     :return a list of dictionaries - one for each row of the table
     """
     try:
         with open(file_name, 'r') as jIn:
-            j = json.load(jIn)
+            j = load(jIn)
             return j
     except Exception as e:
         print("Unable to load the json file! Exiting: \n" + str(e))
     return j
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/table_writer_json.py` & `data-warehouse-client-3.0.0/data_warehouse_client/table_writer_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
-import os
+from json import dump
+from os import path, makedirs
+from check_for_datetime_table import datetimebounds_table_in_dw
 
 
 def table_to_dictionary(dw, table_name, study_id):
     """
     Read a table and turn it into a dictionary
     Based on code in: https://stackoverflow.com/questions/3286525/return-sql-table-as-json-in-python
     :param dw: data warehouse handle
@@ -51,34 +52,38 @@
 def data_warehouse_metadata_tables_to_dictionary(dw, study_id):
     """
     Writes the data warehouse metadata tables into a dictionary
     :param dw: data warehouse handle
     :param study_id: the study id
     :return a dictionary of tables, each a list of dictionaries - one for each row of the table
     """
-    return tables_to_dictionary(dw, study_id, metadata_table_names())
+    return tables_to_dictionary(dw, study_id, metadata_table_names(dw))
 
 
-def metadata_table_names():
+def metadata_table_names(dw):
     """
     :return: the names of all the metadata tables in the data warehouse
     """
-    return ["trial", "units", "measurementtype", "measurementgroup", "sourcetype", "boundsreal",
-            "boundsint", "category", "measurementtypetogroup"]
+    if datetimebounds_table_in_dw(dw):   # include 'datetimebounds'
+        return ["trial", "units", "measurementtype", "measurementgroup", "sourcetype", "boundsreal",
+                "boundsint", "boundsdatetime", "category", "measurementtypetogroup"]
+    else:  # exclude 'datetimebounds'
+        return ["trial", "units", "measurementtype", "measurementgroup", "sourcetype", "boundsreal",
+                "boundsint", "category", "measurementtypetogroup"]
 
 
 def dictionary_to_json_file(d, file_name):
     """
     write dictionary to file in json format
     :param d: dictionary
     :param file_name: output filename
     """
-    os.makedirs(os.path.dirname(file_name), exist_ok=True)
+    makedirs(path.dirname(file_name), exist_ok=True)
     with open(file_name, 'w') as json_file:
-        json.dump(d, json_file)
+        dump(d, json_file)
 
 
 def data_warehouse_metadata_tables_to_file(dw, study_id, file_name):
     """
     Write a set of data warehouse tables into a file
     :param dw: data warehouse handle
     :param study_id: the study id
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/transform_result_format.py` & `data-warehouse-client-3.0.0/data_warehouse_client/transform_result_format.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,18 @@
             row_out[r][value_index] = rows[r][14]
         elif rows[r][val_type_index] == 6:  # ordinal
             row_out[r][value_index] = rows[r][14]
         elif rows[r][val_type_index] == 7:  # boundedint
             row_out[r][value_index] = rows[r][10]
         elif rows[r][val_type_index] == 8:  # boundedreal
             row_out[r][value_index] = rows[r][11]
+        elif rows[r][val_type_index] == 9:  # bounded datetime
+            row_out[r][value_index] = rows[r][13]
+        elif rows[r][val_type_index] == 10:  # external
+            row_out[r][value_index] = rows[r][12]
         else:
             print("typeval error of ", rows[r][9], " for id", rows[r][0], " study ", rows[r][2])
     return row_out
 
 
 def form_measurement_group(dw, study, measurement_group, rows):
     """
@@ -74,18 +78,18 @@
             where value n is the value for the nth measurement in the instance (ordered by measurement type)
             "None" is used if a value is missing)
     """
     result_rows = []
     if len(rows) > 0:
         measurement_group: int = rows[0][6]   # get the measurement group from the first measurement
         mts = dw.get_type_ids_in_measurement_group(study, measurement_group)  # get all the measurement type ids
-        # Create a dictionary entry for each instance hoding the common values and the measurement values
+        # Create a dictionary entry for each instance holding the common values and the measurement values
         result_values = {}  # the measurement values
-        result_common = {}  # the common values returned for each instance: instance, time of 1st measurement,
-                            #                                               study, participant, measurementGroup, trial
+        result_common = {}  # the common values returned for each instance:
+                            # instance, time of 1st measurement, study, participant, measurementGroup, trial
         for (row_id, time, study_id, participant, mt, tn, mg, mgi, trial, val_type, value) in rows:
             if not (mgi in result_common):           # it's a new instance
                 result_common.update({mgi: [mgi, time, study, participant, mg, trial]})  # store the common values
                 result_values.update({mgi: {}})                                          # create empty values for inst
             result_values[mgi][mt] = value  # add values to the dictionary               # add the value
         # Write out the list of measurement groups
         for instance in result_values:               # for each instance
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client/warehouse_checker.py` & `data-warehouse-client-3.0.0/data_warehouse_client/warehouse_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,102 +18,127 @@
 # The measurementType is in the measurement group for each measurement
 # The valtype is correct for the measurement type for each measurement
 # the measurement group is valid for the study
 # there are no missing measurement types in a measurement group instance
 # no ordinal, nominal, bounded integer or bounded real values are out of bounds
 
 
-from data_warehouse_client import file_utils
-from data_warehouse_client import data_warehouse
-from data_warehouse_client import print_io
+from file_utils import process_sql_template
+from data_warehouse import core_sql_for_measurements
+from print_io import print_measurements, print_measurements_to_file
 from tabulate import tabulate
-import datetime
+from datetime import datetime
+from check_for_datetime_table import datetimebounds_table_in_dw
 
 
 def check_category_exists(dw, study):
     """
     Find measurement types of nominal or ordinal value type without entry in category table
     :param dw: handle to data warehouse
     :param study: study id
     :return: the ids and names of measurement types in the study that fail the test
     """
     mappings = {"study": str(study)}
-    query = file_utils.process_sql_template("ordinal_types_not_matching_category.sql", mappings)
+    query = process_sql_template("ordinal_types_not_matching_category.sql", mappings)
     return dw.return_query_result(query)
 
 
 def check_integer_bounds_exist(dw, study):
     """
     Find measurement types of bounded integer value type without entry in boundsinteger table
     :param dw: handle to data warehouse
     :param study: study id
     :return: the ids and names of measurement types in the study that fail the test
     """
     mappings = {"study": str(study)}
-    query = file_utils.process_sql_template("bounded_integer_measurement_types_without_bounds.sql", mappings)
+    query = process_sql_template("bounded_integer_measurement_types_without_bounds.sql", mappings)
     return dw.return_query_result(query)
 
 
 def check_real_bounds_exist(dw, study):
     """
     Find measurement types of bounded real value type without entry in boundsreal table
     :param dw: handle to data warehouse
     :param study: study id
     :return: the ids and names of measurement types in the study that fail the test
     """
     mappings = {"study": str(study)}
-    query = file_utils.process_sql_template("bounded_real_measurement_types_without_bounds.sql", mappings)
+    query = process_sql_template("bounded_real_measurement_types_without_bounds.sql", mappings)
+    return dw.return_query_result(query)
+
+
+def check_datetime_bounds_exist(dw, study):
+    """
+    Find measurement types of bounded datetime value type without entry in boundsreal table
+    :param dw: handle to data warehouse
+    :param study: study id
+    :return: the ids and names of measurement types in the study that fail the test
+    """
+    mappings = {"study": str(study)}
+    query = process_sql_template("bounded_datetime_measurement_types_without_bounds.sql", mappings)
     return dw.return_query_result(query)
 
 
 def check_valtype_matches_values(dw, study):
     """
     Find measurements that lack a value
     :param dw: handle to data warehouse
     :param study: study id
     :return: the measurements in the study that fail the test
     """
-    mappings = {"study": str(study), "core_sql": data_warehouse.core_sql_for_measurements()}
-    query = file_utils.process_sql_template("measurements_lacking_value.sql", mappings)
+    mappings = {"study": str(study), "core_sql": core_sql_for_measurements()}
+    query = process_sql_template("measurements_lacking_value.sql", mappings)
     return dw.return_query_result(query)
 
 
 def check_category_in_range(dw, study):
     """
     Returns the ids of measurements that refer to a non-existent category
     :param dw: handle to data warehouse
     :param study: study id
     :return: the ids of measurements in the study that fail the test
     """
-    mappings = {"study": str(study), "core_sql": data_warehouse.core_sql_for_measurements()}
-    query = file_utils.process_sql_template("measurements_lacking_value.sql", mappings)
+    mappings = {"study": str(study), "core_sql": core_sql_for_measurements()}
+    query = process_sql_template("measurements_lacking_value.sql", mappings)
     return dw.return_query_result(query)
 
 
 def check_bounded_integers(dw, study):
     """
     Returns the ids of measurements that hold bounded integers that are out of range
     :param dw: handle to data warehouse
     :param study: study id
     :return: the ids of measurements in the study that fail the test
     """
     mappings = {"study": str(study)}
-    query = file_utils.process_sql_template("bounded_integers.sql", mappings)
+    query = process_sql_template("bounded_integers.sql", mappings)
     return dw.return_query_result(query)
 
 
 def check_bounded_reals(dw, study):
     """
     Returns the ids of measurements that hold bounded reals that are out of range
     :param dw: handle to data warehouse
     :param study: study id
     :return: the ids of measurements in the study that fail the test
     """
     mappings = {"study": str(study)}
-    query = file_utils.process_sql_template("bounded_reals.sql", mappings)
+    query = process_sql_template("bounded_reals.sql", mappings)
+    return dw.return_query_result(query)
+
+
+def check_bounded_datetimes(dw, study):
+    """
+    Returns the ids of measurements that hold bounded reals that are out of range
+    :param dw: handle to data warehouse
+    :param study: study id
+    :return: the ids of measurements in the study that fail the test
+    """
+    mappings = {"study": str(study)}
+    query = process_sql_template("bounded_datetimes.sql", mappings)
     return dw.return_query_result(query)
 
 
 def print_check_warehouse(dw, study):
     """
     Prints on stdout the results of all the tests that check the warehouse for errors
     :param dw: handle to data warehouse
@@ -150,15 +175,15 @@
     print(f'- Check Measurements')
     print()
 
     print(f'-- Measurements where the Value Type does not match the values stored in the Measurement Table')
     r1 = check_valtype_matches_values(dw, study)
     n_invalid_entries = len(r1)
     if n_invalid_entries > 0:
-        print_io.print_measurements(r1)
+        print_measurements(r1)
     print(f'({n_invalid_entries} invalid entries)')
 
     print(f'-- Measurements declared as ordinal or nominal that refer to a non-existent category')
     r3 = check_category_in_range(dw, study)
     n_errors = len(r3)
     if n_errors > 0:
         print(tabulate(r3, headers=['Measurement Id']))
@@ -175,15 +200,24 @@
     print()
     print(f'-- Measurements declared as Bounded Reals whose value is outside of the bounds')
     r5 = check_bounded_reals(dw, study)
     n_errors = len(r5)
     if n_errors > 0:
         print(tabulate(r5, headers=['Id', 'Value', 'MeasurementType', 'Group', 'Min', 'Max', 'Participant']))
     print(f'({n_errors} measurements)')
+
     print()
+    if datetimebounds_table_in_dw(dw):
+        print(f'-- Measurements declared as Bounded Datetimes whose value is outside of the bounds')
+        r5 = check_bounded_datetimes(dw, study)
+        n_errors = len(r5)
+        if n_errors > 0:
+            print(tabulate(r5, headers=['Id', 'Value', 'MeasurementType', 'Group', 'Min', 'Max', 'Participant']))
+        print(f'({n_errors} measurements)')
+        print()
 
 
 def mk_txt_report_file_name(f_dir, report_name, time_string):
     return f_dir + report_name + time_string + ".txt"
 
 
 def print_check_warehouse_to_file(dw, study):
@@ -191,15 +225,15 @@
     Prints to a file the results of all the tests that check the warehouse for errors
     :param dw: handle to data warehouse
     :param study: study id
     :return:
     """
 
     file_dir = "reports/"
-    timestamp = datetime.datetime.now()  # use the current date and time if none is specified
+    timestamp = datetime.now()  # use the current date and time if none is specified
     time_fname_str = timestamp.strftime('%Y-%m-%dh%Hm%Ms%S')
     fname = mk_txt_report_file_name(file_dir, "warehouse-check-", time_fname_str)
 
     with open(fname, "w", encoding="utf-8") as f:
         print(f'Check Study {study}\n', file=f)
 
         print(f'- Check Metadata\n', file=f)
@@ -227,31 +261,41 @@
 
         print(f'- Check Measurements\n', file=f)
 
         print(f'-- Measurements where the Value Type does not match the values stored in the Measurement Table', file=f)
         r1 = check_valtype_matches_values(dw, study)
         n_invalid_entries = len(r1)
         if n_invalid_entries > 0:
-            print_io.print_measurements_to_file(r1, f)
+            print_measurements_to_file(r1, f)
         print(f'({n_invalid_entries} invalid entries)\n', file=f)
 
         print(f'-- Measurements declared as ordinal or nominal that refer to a non-existent category', file=f)
         r3 = check_category_in_range(dw, study)
         n_errors = len(r3)
         if n_errors > 0:
             print(tabulate(r3, headers=['Measurement Id']), file=f)
         print(f'({n_errors} measurements)\n', file=f)
 
         print(f'-- Measurements declared as Bounded Integers whose value is outside of the bounds', file=f)
         r4 = check_bounded_integers(dw, study)
         n_errors = len(r4)
         if n_errors > 0:
-            print(tabulate(r4, headers=['Id', 'Value']), file=f)
+            print(tabulate(r4, headers=['Id', 'Value', 'MeasurementType', 'Group', 'Min', 'Max', 'Participant']),
+                  file=f)
         print(f'({n_errors} measurements)\n', file=f)
 
         print(f'-- Measurements declared as Bounded Reals whose value is outside of the bounds', file=f)
         r5 = check_bounded_reals(dw, study)
         n_errors = len(r5)
         if n_errors > 0:
             print(tabulate(r5, headers=['Id', 'Value', 'MeasurementType', 'Group', 'Min', 'Max', 'Participant']),
                   file=f)
         print(f'({n_errors} measurements)\n', file=f)
+
+        if datetimebounds_table_in_dw(dw):
+            print(f'-- Measurements declared as Bounded Datetimes whose value is outside of the bounds', file=f)
+            r5 = check_bounded_datetimes(dw, study)
+            n_errors = len(r5)
+            if n_errors > 0:
+                print(tabulate(r5, headers=['Id', 'Value', 'MeasurementType', 'Group', 'Min', 'Max', 'Participant']),
+                      file=f)
+            print(f'({n_errors} measurements)\n', file=f)
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client.egg-info/PKG-INFO` & `data-warehouse-client-3.0.0/data_warehouse_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-warehouse-client
-Version: 2.0.9
+Version: 3.0.0
 Summary: This package provides access to the e-Science Central data warehouse that can be used to store, access and analyse data collected in scientific studies, including for healthcare applications
 Home-page: https://github.com/e-science-central/data-warehouse-client
 Author: Paul Watson
 Author-email: paul.watson@ncl.ac.uk
 License: UNKNOWN
 Description: # Data Warehouse Client
         
@@ -39,20 +39,23 @@
         2.	Descriptive information about the types of measurement is stored in the warehouse so that tools or humans 
         can interpret the data stored there.
         3.	The design is optimised for query performance. In several cases, this has led to denormalization
          (duplication of data) to reduce the need for expensive joins.
         4.	It must support a security regime to restrict each user’s access 
         to the data collected in studies.
         
+        
         For more information see: 
         P. Watson and H. Hiden, "The e-Science Central Study Data Platform"
         2022 IEEE 18th International Conference on e-Science (e-Science),
         Salt Lake City, UT, USA, 2022, pp. 55-64, doi: 10.1109/eScience55777.2022.00020.
         https://scholar.google.co.uk/citations?view_op=view_citation&hl=en&user=KQJg3lwAAAAJ&sortby=pubdate&citation_for_view=KQJg3lwAAAAJ:z0_F5_TITjQC
         
+        For more documentation see [A Data Warehouse for Storing and Analysing Study Data](docs/data_warehouse_guide.pdf).
+        
         # Running Instructions
         
         To install from PyPi, run:
         
         pip install data-warehouse-client
         
         In directory in which your executable is run, create a `db-credentials.json` file containing database
```

### Comparing `data-warehouse-client-2.0.9/data_warehouse_client.egg-info/SOURCES.txt` & `data-warehouse-client-3.0.0/data_warehouse_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,57 +2,76 @@
 LICENSE
 README.md
 requirements.txt
 setup.py
 .github/workflows/build.yml
 .github/workflows/release.yml
 data_warehouse_client/__init__.py
+data_warehouse_client/auto_generate_test_cases.py
+data_warehouse_client/auto_generate_tests.py
+data_warehouse_client/check_bounded_values.py
+data_warehouse_client/check_for_datetime_table.py
 data_warehouse_client/clone_study_metadata.py
 data_warehouse_client/csv_io.py
 data_warehouse_client/data_warehouse.py
 data_warehouse_client/delete_study_contents.py
 data_warehouse_client/file_utils.py
+data_warehouse_client/import_tests.py
+data_warehouse_client/import_with_checks.py
+data_warehouse_client/load_data.py
 data_warehouse_client/load_warehouse_helpers.py
+data_warehouse_client/multiple_mg_inserts.py
 data_warehouse_client/plot.py
 data_warehouse_client/print_io.py
 data_warehouse_client/print_metadata_table.py
 data_warehouse_client/requirements.txt
-data_warehouse_client/sample_queries.py
 data_warehouse_client/study_profile.py
 data_warehouse_client/study_summary.py
 data_warehouse_client/table_reader_json.py
 data_warehouse_client/table_writer_json.py
 data_warehouse_client/transform_result_format.py
+data_warehouse_client/type_checks.py
+data_warehouse_client/type_definitions.py
 data_warehouse_client/warehouse_checker.py
 data_warehouse_client.egg-info/PKG-INFO
 data_warehouse_client.egg-info/SOURCES.txt
 data_warehouse_client.egg-info/dependency_links.txt
 data_warehouse_client.egg-info/requires.txt
 data_warehouse_client.egg-info/top_level.txt
+data_warehouse_client/sql/bounded_datetime_measurement_types_without_bounds.sql
+data_warehouse_client/sql/bounded_datetimes.sql
 data_warehouse_client/sql/bounded_integer_measurement_types_without_bounds.sql
 data_warehouse_client/sql/bounded_integers.sql
 data_warehouse_client/sql/bounded_real_measurement_types_without_bounds.sql
 data_warehouse_client/sql/bounded_reals.sql
 data_warehouse_client/sql/core_sql_from_for_measurements.sql
 data_warehouse_client/sql/core_sql_select_for_measurements.sql
 data_warehouse_client/sql/get_all_measurement_groups.sql
 data_warehouse_client/sql/get_all_measurement_groups_and_types_in_a_study.sql
+data_warehouse_client/sql/get_all_table_names.sql
+data_warehouse_client/sql/get_boundsdatetime_in_study.sql
 data_warehouse_client/sql/get_boundsint_in_study.sql
 data_warehouse_client/sql/get_boundsreal_in_study.sql
 data_warehouse_client/sql/get_categories_in_study.sql
+data_warehouse_client/sql/get_category_ids.sql
 data_warehouse_client/sql/get_measurement_group_info.sql
 data_warehouse_client/sql/get_measurement_groups_in_study.sql
 data_warehouse_client/sql/get_measurement_type_info.sql
 data_warehouse_client/sql/get_measurements.sql
 data_warehouse_client/sql/get_measurements_by_cohort.sql
 data_warehouse_client/sql/get_measurements_with_value.sql
 data_warehouse_client/sql/get_units_in_study.sql
+data_warehouse_client/sql/insert_datetime.sql
+data_warehouse_client/sql/insert_measurement.sql
+data_warehouse_client/sql/insert_text.sql
 data_warehouse_client/sql/measurements_lacking_value.sql
 data_warehouse_client/sql/measurements_with_invalid_category.sql
 data_warehouse_client/sql/num_types_in_a_measurement_group.sql
 data_warehouse_client/sql/ordinal_types_not_matching_category.sql
 data_warehouse_client/sql/types_in_a_measurement_group.sql
+data_warehouse_client/sql/update_measurement_group_instance_id.sql
+docs/data_warehouse_guide.pdf
 integration_test/clone_study_metadata_test.py
 integration_test/delete_study_test.py
 test/__init__.py
 test/test_file_utils.py
 test/test_transform_result_format.py
```

### Comparing `data-warehouse-client-2.0.9/integration_test/clone_study_metadata_test.py` & `data-warehouse-client-3.0.0/integration_test/clone_study_metadata_test.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-2.0.9/integration_test/delete_study_test.py` & `data-warehouse-client-3.0.0/integration_test/delete_study_test.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-2.0.9/setup.py` & `data-warehouse-client-3.0.0/setup.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="data-warehouse-client",
-    version="0.0.3",
-    author="Paul Watson",
-    author_email="paul.watson@ncl.ac.uk",
-    description="This package provides access to the e-Science Central data warehouse that can be used to store, "
-                "access and analyse data collected in scientific studies, including for healthcare applications",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/e-science-central/data-warehouse-client",
-    packages=["data_warehouse_client"],
-    package_dir={'data_warehouse_client': 'data_warehouse_client'},
-    package_data={'data_warehouse_client':['sql/*.sql']},
-    use_scm_version=True,
-    setup_requires=['setuptools_scm'],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    install_requires=[
-        "more-itertools",
-        "matplotlib",
-        "psycopg2",
-        "tabulate"
-    ],
-    python_requires='>=3.6',
-)
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="data-warehouse-client",
+    version="0.0.3",
+    author="Paul Watson",
+    author_email="paul.watson@ncl.ac.uk",
+    description="This package provides access to the e-Science Central data warehouse that can be used to store, "
+                "access and analyse data collected in scientific studies, including for healthcare applications",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/e-science-central/data-warehouse-client",
+    packages=["data_warehouse_client"],
+    package_dir={'data_warehouse_client': 'data_warehouse_client'},
+    package_data={'data_warehouse_client':['sql/*.sql']},
+    use_scm_version=True,
+    setup_requires=['setuptools_scm'],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
+    ],
+    install_requires=[
+        "more-itertools",
+        "matplotlib",
+        "psycopg2",
+        "tabulate"
+    ],
+    python_requires='>=3.6',
+)
```

### Comparing `data-warehouse-client-2.0.9/test/test_file_utils.py` & `data-warehouse-client-3.0.0/test/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-2.0.9/test/test_transform_result_format.py` & `data-warehouse-client-3.0.0/test/test_transform_result_format.py`

 * *Files identical despite different names*

