# Comparing `tmp/data-warehouse-client-3.0.0.tar.gz` & `tmp/data-warehouse-client-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-warehouse-client-3.0.0.tar", last modified: Sun Apr  9 15:02:12 2023, max compression
+gzip compressed data, was "data-warehouse-client-3.0.1.tar", last modified: Sun Apr  9 15:47:02 2023, max compression
```

## Comparing `data-warehouse-client-3.0.0.tar` & `data-warehouse-client-3.0.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.424381 data-warehouse-client-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.408380 data-warehouse-client-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.412380 data-warehouse-client-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 15:02:12.424381 data-warehouse-client-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.416381 data-warehouse-client-3.0.0/data_warehouse_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14953 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/auto_generate_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/auto_generate_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/check_bounded_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/check_for_datetime_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/clone_study_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/csv_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    41229 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/data_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/delete_study_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/import_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    34655 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/import_with_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    44090 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/load_warehouse_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/multiple_mg_inserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/print_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/print_metadata_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.420381 data-warehouse-client-3.0.0/data_warehouse_client/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_datetime_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_datetimes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_integer_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_integers.sql
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_real_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_reals.sql
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/core_sql_from_for_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/core_sql_select_for_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_all_measurement_groups.sql
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_all_measurement_groups_and_types_in_a_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_all_table_names.sql
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_boundsdatetime_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_boundsint_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_boundsreal_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_categories_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_category_ids.sql
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurement_group_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurement_groups_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurement_type_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurements_by_cohort.sql
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurements_with_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/get_units_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/insert_datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/insert_measurement.sql
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/insert_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/measurements_lacking_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/measurements_with_invalid_category.sql
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/num_types_in_a_measurement_group.sql
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/ordinal_types_not_matching_category.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/types_in_a_measurement_group.sql
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/sql/update_measurement_group_instance_id.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/study_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/study_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/table_reader_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/table_writer_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/transform_result_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/type_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/data_warehouse_client/warehouse_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.416381 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 15:02:12.000000 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-09 15:02:12.000000 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:02:12.000000 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-09 15:02:12.000000 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 15:02:12.000000 data-warehouse-client-3.0.0/data_warehouse_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.420381 data-warehouse-client-3.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   574842 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/docs/data_warehouse_guide.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.420381 data-warehouse-client-3.0.0/integration_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/integration_test/clone_study_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/integration_test/delete_study_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 15:02:12.424381 data-warehouse-client-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:02:12.424381 data-warehouse-client-3.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/test/test_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-09 15:01:58.000000 data-warehouse-client-3.0.0/test/test_transform_result_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.221954 data-warehouse-client-3.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.221954 data-warehouse-client-3.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.225954 data-warehouse-client-3.0.1/data_warehouse_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/auto_generate_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/auto_generate_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/check_bounded_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/check_for_datetime_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/clone_study_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/csv_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41250 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/data_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/delete_study_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18877 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/import_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34701 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/import_with_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44140 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/load_warehouse_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/multiple_mg_inserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/print_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/print_metadata_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/data_warehouse_client/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_datetime_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_datetimes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_integer_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_integers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_real_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_reals.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/core_sql_from_for_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/core_sql_select_for_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_all_measurement_groups.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_all_measurement_groups_and_types_in_a_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_all_table_names.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_boundsdatetime_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_boundsint_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_boundsreal_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_categories_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_category_ids.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurement_group_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurement_groups_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurement_type_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurements_by_cohort.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurements_with_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_units_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/insert_datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/insert_measurement.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/insert_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/measurements_lacking_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/measurements_with_invalid_category.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/num_types_in_a_measurement_group.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/ordinal_types_not_matching_category.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/types_in_a_measurement_group.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/update_measurement_group_instance_id.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/study_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/study_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/table_reader_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/table_writer_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/transform_result_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/type_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/warehouse_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.225954 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 15:47:02.000000 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-09 15:47:02.000000 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:47:02.000000 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-09 15:47:02.000000 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 15:47:02.000000 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   574842 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/docs/data_warehouse_guide.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/integration_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/integration_test/clone_study_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/integration_test/delete_study_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/test/test_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/test/test_transform_result_format.py
```

### Comparing `data-warehouse-client-3.0.0/.github/workflows/build.yml` & `data-warehouse-client-3.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/.github/workflows/release.yml` & `data-warehouse-client-3.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/.gitignore` & `data-warehouse-client-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/LICENSE` & `data-warehouse-client-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/PKG-INFO` & `data-warehouse-client-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-warehouse-client
-Version: 3.0.0
+Version: 3.0.1
 Summary: This package provides access to the e-Science Central data warehouse that can be used to store, access and analyse data collected in scientific studies, including for healthcare applications
 Home-page: https://github.com/e-science-central/data-warehouse-client
 Author: Paul Watson
 Author-email: paul.watson@ncl.ac.uk
 License: UNKNOWN
 Description: # Data Warehouse Client
```

### Comparing `data-warehouse-client-3.0.0/README.md` & `data-warehouse-client-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/auto_generate_test_cases.py` & `data-warehouse-client-3.0.1/data_warehouse_client/auto_generate_test_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Autogenerate examples to test the data warehouse
 # Valid examples are generated by functions that begin with "valid"
 
-from multiple_mg_inserts import insert_measurement_group_instances
-from load_data import process_measurement_groups
-from type_definitions import LoaderResult, MeasurementGroup, MeasurementType, MeasurementGroupInstance, Source
-from type_definitions import Participant, Study, Trial, Bounds, LoadHelperResult
 from typing import Tuple, List, Optional
 from random import randint, uniform, choice, random
 from string import ascii_lowercase, ascii_uppercase, digits
 from datetime import datetime
-from type_checks import category_ids, int_bounds, real_bounds, datetime_bounds
-from print_metadata_table import create_measurement_group_info
-from check_bounded_values import get_bounds
+
+from data_warehouse_client.check_bounded_values import get_bounds
+from data_warehouse_client.load_data import process_measurement_groups
+from data_warehouse_client.multiple_mg_inserts import insert_measurement_group_instances
+from data_warehouse_client.print_metadata_table import create_measurement_group_info
+from data_warehouse_client.type_checks import category_ids, int_bounds, real_bounds, datetime_bounds
+from data_warehouse_client.type_definitions import MeasurementType, Bounds, LoadHelperResult, Study, MeasurementGroup, \
+    LoaderResult, MeasurementGroupInstance, Source, Participant, Trial
 
 
 def valid_int_generator(measurement_type: MeasurementType, bounds: Bounds) -> int:
     return randint(-2147483648, +2147483647)
 
 
 def valid_real_generator(measurement_type: MeasurementType, bounds: Bounds) -> float:
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/auto_generate_tests.py` & `data-warehouse-client-3.0.1/data_warehouse_client/auto_generate_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from datetime import datetime
 
 # Autogenerate examples to test the data warehouse
 # Valid examples are generated by functions that begin with "valid"
 
-import auto_generate_test_cases
-import data_warehouse
 import pytest
-from type_definitions import Bounds
-from datetime import datetime
-from type_checks import check_int, check_real, check_string, check_boolean, check_datetime, \
+
+from data_warehouse_client import auto_generate_test_cases
+from data_warehouse_client.data_warehouse import DataWarehouse
+from data_warehouse_client.print_metadata_table import create_measurement_group_info
+from data_warehouse_client.type_checks import check_int, check_real, check_string, check_datetime, check_boolean, \
     check_nominal, check_ordinal, check_bounded_int, check_bounded_real, check_bounded_datetime, check_external
-from print_metadata_table import create_measurement_group_info
+from data_warehouse_client.type_definitions import Bounds
 
 
 @pytest.fixture()
 def bounds_ex1() -> Bounds:
     int_bounds = {1: {'minval': 0, 'maxval': 100}}
     real_bounds = {2: {'minval': 0.0, 'maxval': 100.0}}
     start_date = datetime(1900, 1, 1)
@@ -105,15 +106,15 @@
 @pytest.fixture()
 def credentials_full_access_file_name():
     return "dw-credentials-full-access.json"
 
 
 @pytest.fixture()
 def mk_dw_handle_full_access(credentials_full_access_file_name, database_name):
-    data_warehouse_handle = data_warehouse.DataWarehouse(credentials_full_access_file_name, database_name)
+    data_warehouse_handle = DataWarehouse(credentials_full_access_file_name, database_name)
     yield data_warehouse_handle
 
 
 def test_load_test_data_for_all_measurement_groups(mk_dw_handle_full_access, test_study):
     data_warehouse_handle = mk_dw_handle_full_access
     mg_info = create_measurement_group_info(data_warehouse_handle, test_study)
     number_of_measurement_groups = len(mg_info)
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/check_bounded_values.py` & `data-warehouse-client-3.0.1/data_warehouse_client/check_bounded_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from file_utils import process_sql_template
-from type_definitions import Study, MeasurementType, Bounds, DateTime
 from typing import List, Dict
 
+from data_warehouse_client.file_utils import process_sql_template
+from data_warehouse_client.type_definitions import Study, MeasurementType, DateTime, Bounds
+
 
 def get_category_ids(dw, study: Study) -> Dict[MeasurementType, List[int]]:
     """
     Create a dirctory to map from Measurement Type Id to Category Id
     :param dw: data warehouse handle
     :param study: Study id
     :return: Dictionary mapping from Measurement Type to a list of the Category Ids in that Measurement Type
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/check_for_datetime_table.py` & `data-warehouse-client-3.0.1/data_warehouse_client/check_for_datetime_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from data_warehouse_client.file_utils import process_sql_template
 
-# determine if there's a a table called 'boundsdatetime' (this was added in later versions of the warehouse design)
 
-from file_utils import process_sql_template
+# determine if there's a a table called 'boundsdatetime' (this was added in later versions of the warehouse design)
 
 
 def datetimebounds_table_in_dw(dw_handle):
     """
     :param dw_handle: data warehouse handle
     :type dw_handle: database handle (only needs to be read-only)
     :return: True if the database has a table called 'boundsdatetime'
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/clone_study_metadata.py` & `data-warehouse-client-3.0.1/data_warehouse_client/clone_study_metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-
-from table_writer_json import data_warehouse_metadata_tables_to_dictionary, write_tables_in_dw_from_dictionary
+from data_warehouse_client.table_writer_json import data_warehouse_metadata_tables_to_dictionary, \
+    write_tables_in_dw_from_dictionary
 
 
 def clone_study_metadata(dw, source_study_id, dest_study_id):
     """
     Copies all the metadata from one study to another
     :param dw: data warehouse end point
     :param source_study_id: original study
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/csv_io.py` & `data-warehouse-client-3.0.1/data_warehouse_client/csv_io.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/data_warehouse.py` & `data-warehouse-client-3.0.1/data_warehouse_client/data_warehouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 # limitations under the License.
 
 from datetime import datetime
 from sys import exit
 import psycopg2
 from json import load
 from more_itertools import intersperse
-from transform_result_format import form_measurements, form_measurement_group
-from file_utils import process_sql_template
+
+from data_warehouse_client.file_utils import process_sql_template
+from data_warehouse_client.transform_result_format import form_measurements
 
 
 def get_participants_in_result(results):
     """
     find all participants in a set of results
     :param results: a list of measurements. Each measurement is held in a list with the following fields:
                     id,time,study,participant,measurementType,typeName,measurementGroup,
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/delete_study_contents.py` & `data-warehouse-client-3.0.1/data_warehouse_client/delete_study_contents.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from data_warehouse_client.check_for_datetime_table import datetimebounds_table_in_dw
 
-# only run this if you're certain that you want to remove all metadata and measurements from a study!
 
-from check_for_datetime_table import datetimebounds_table_in_dw
+# only run this if you're certain that you want to remove all metadata and measurements from a study!
 
 
 def delete_study_contents(dw, study):
     """
     Deletes all measurements and metadata from a study. Only leave entry in the study table
     Designed to clear out a study before a test that will re-populate it
     :param dw: data warehouse handle
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/file_utils.py` & `data-warehouse-client-3.0.1/data_warehouse_client/file_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from string import Template
+import pkgutil
 
 
 def process_sql_template(filename, mappings=None):
     """
     Reads a templated SQL file and substitutes any variables
     :param filename: the SQL file
     :param mappings: the variables to be substituted
     :return: the text of the SQL query with any variables substituted
     """
-    # https://stackoverflow.com/questions/6028000/how-to-read-a-static-file-from-inside-a-python-package Option 1
-    with open(f"sql/{filename}") as f:
-        file_contents = f.read()
+    # https://stackoverflow.com/questions/6028000/how-to-read-a-static-file-from-inside-a-python-package
+    file_contents = pkgutil.get_data(__name__, f"sql/{filename}").decode("utf-8")
     data = ' '.join(file_contents.replace('\r\n', ' ').split())
     res = Template(data).substitute(mappings)
     return res
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/import_tests.py` & `data-warehouse-client-3.0.1/data_warehouse_client/import_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest  # see https://realpython.com/pytest-python-testing/
-from type_checks import check_int
-from type_definitions import Bounds, LoaderResult, DataToLoad, Loader, MeasurementGroup, LoadHelperResult
 from typing import Dict, List, Tuple
 from datetime import datetime
-import import_with_checks as iwc
-from load_data import load_data
-import data_warehouse
-from check_bounded_values import get_inverse_category_ids_map
 
+from data_warehouse_client.check_bounded_values import get_inverse_category_ids_map
+from data_warehouse_client.data_warehouse import DataWarehouse
+from data_warehouse_client.load_data import load_data
+from data_warehouse_client.type_checks import check_int
+from data_warehouse_client.type_definitions import DataToLoad, Bounds, LoaderResult, MeasurementGroup, LoadHelperResult, \
+    Loader
+from data_warehouse_client import import_with_checks as iwc
 
 @pytest.fixture()
 def walking_test_1() -> DataToLoad:
     data = {
         'visit-date': datetime.now(),
         'visit-code': 'visit3',
         'wb_id': "fred",
@@ -47,15 +48,15 @@
 @pytest.fixture()
 def database_name():
     return "osm_dw"
 
 
 @pytest.fixture()
 def mk_dw_handle(credentials_file_name, database_name):
-    data_warehouse_handle = data_warehouse.DataWarehouse(credentials_file_name, database_name)
+    data_warehouse_handle = DataWarehouse(credentials_file_name, database_name)
     yield data_warehouse_handle
 
 
 @pytest.fixture()
 def test_all_example() -> DataToLoad:
     data = {
         'Int': 4,
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/import_with_checks.py` & `data-warehouse-client-3.0.1/data_warehouse_client/import_with_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from typing import Tuple, List, Optional, Dict, Callable, Any
-from type_checks import check_value_type, category_values, check_string
 from functools import reduce
-from type_definitions import Bounds, ValueTriple, MeasurementGroup, MeasurementType, ValType, DataToLoad,\
-    FieldValue, LoadHelperResult, Loader, LoaderResult
 from itertools import chain
 
+from data_warehouse_client.type_checks import check_value_type, category_values, check_string
+from data_warehouse_client.type_definitions import MeasurementGroup, ValueTriple, MeasurementType, DataToLoad, ValType, \
+    FieldValue, Bounds, Loader, LoadHelperResult, LoaderResult
+
 
 def process_measurement_group(mg_triples):
     """
     takes the result of attempting to load each field in a message group and processes it
     :param mg_triples: [(Success?, [(measurement_type, valtype, value)], Error Message)]
     :return: Success?, [(measurement_type, valtype, value)], [error messages]
     """
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/load_data.py` & `data-warehouse-client-3.0.1/data_warehouse_client/load_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from multiple_mg_inserts import insert_measurement_group_instances
-from check_bounded_values import get_bounds
-from type_definitions import MeasurementGroupInstance, DataToLoad, Source, Participant, Study, Trial, Loader,\
-    Bounds, MeasurementGroup, LoadHelperResult, ValueTriple
 from typing import Tuple, List, Optional, Dict
-from load_warehouse_helpers import process_message_group
+
+from data_warehouse_client.check_bounded_values import get_bounds
+from data_warehouse_client.load_warehouse_helpers import process_message_group
+from data_warehouse_client.multiple_mg_inserts import insert_measurement_group_instances
+from data_warehouse_client.type_definitions import Loader, MeasurementGroup, LoadHelperResult, ValueTriple, DataToLoad, \
+    Study, Bounds, Trial, Participant, Source, MeasurementGroupInstance
 
 
 def get_loader_from_data_name(data_name: str, mapper: Dict[str, Loader]) -> Tuple[bool, Optional[Loader]]:
     """
     map from the data_name to the mapper function - used when process_measurement_groups is the way to ingest data
     :param data_name: the measurement_type_in_the_json
     :param mapper: the dictionary that maps from the event_type to the mapper function
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/load_warehouse_helpers.py` & `data-warehouse-client-3.0.1/data_warehouse_client/load_warehouse_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
 from datetime import datetime
 import unidecode
 from typing import Tuple, List, Any, Callable
 import itertools
-import type_checks
-from type_definitions import MeasurementGroup, LoadHelperResult, LoaderResult, DataToLoad
+
+from data_warehouse_client import type_checks
+from data_warehouse_client.type_definitions import MeasurementGroup, DataToLoad, LoadHelperResult, LoaderResult
 
 
 def process_message_group(mg_triples):
     """
     takes the result of attempting to load each field in a message group and processes it
     :param mg_triples: [(Success?, [(measurement_type, valtype, value)], Error Message)]
     :return: Success?, [(measurement_type, valtype, value)], [error messages]
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/multiple_mg_inserts.py` & `data-warehouse-client-3.0.1/data_warehouse_client/multiple_mg_inserts.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import psycopg2
 from datetime import datetime
-from file_utils import process_sql_template
-from type_checks import check_value_type
-from check_bounded_values import get_bounds
 from typing import Tuple, List, Optional
-from type_definitions import Bounds, Study, MeasurementGroup, ValueTriple, DateTime, Trial, Participant, Source
-from type_definitions import MeasurementGroupInstance, ValType, MeasurementType, Value
+
+from data_warehouse_client.check_bounded_values import get_bounds
+from data_warehouse_client.file_utils import process_sql_template
+from data_warehouse_client.type_checks import check_value_type
+from data_warehouse_client.type_definitions import Study, MeasurementGroup, ValueTriple, Bounds, DateTime, Participant, \
+    Trial, Source, MeasurementType, Value, MeasurementGroupInstance, ValType
 
 
 def insert_measurement_group_instances(data_warehouse_handle,
                                        study: Study,
                                        measurement_group_vals: List[Tuple[MeasurementGroup, List[ValueTriple]]],
                                        bounds: Bounds = None,
                                        time: Optional[DateTime] = None,
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/plot.py` & `data-warehouse-client-3.0.1/data_warehouse_client/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import matplotlib.pyplot as pyplot
 from matplotlib.backends.backend_pdf import PdfPages
-import print_metadata_table
 import datetime
 import numpy as np
 
+from data_warehouse_client import print_metadata_table
+
 
 def plot_measurements(dw, rows, study, measurement_type_id, plot_file):
     """
     Plot the value of a measurement over time.
     :param dw: data warehouse handle
     :param rows: a list of measurements generated by the other client functions. Each measurement is in the form:
                     id,time,study,participant,measurementType,
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/print_io.py` & `data-warehouse-client-3.0.1/data_warehouse_client/print_io.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/print_metadata_table.py` & `data-warehouse-client-3.0.1/data_warehouse_client/print_metadata_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from file_utils import process_sql_template
 from tabulate import tabulate  # https://github.com/astanin/python-tabulate
 import datetime
-from check_for_datetime_table import datetimebounds_table_in_dw
+
+from data_warehouse_client.check_for_datetime_table import datetimebounds_table_in_dw
+from data_warehouse_client.file_utils import process_sql_template
 
 
 def valuetype_to_name():
     return {0: 'Integer', 1: 'Real', 2: 'Text', 3: 'Date Time', 4: 'Boolean',
             5: 'Nominal', 6: 'Ordinal', 7: 'Bounded Integer', 8: 'Bounded Real',
             9: 'Bounded Date Time', 10: 'External'}
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_datetimes.sql` & `data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_datetimes.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_integers.sql` & `data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_integers.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/sql/bounded_reals.sql` & `data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_reals.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/sql/core_sql_from_for_measurements.sql` & `data-warehouse-client-3.0.1/data_warehouse_client/sql/core_sql_from_for_measurements.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/sql/get_measurement_group_info.sql` & `data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurement_group_info.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/study_profile.py` & `data-warehouse-client-3.0.1/data_warehouse_client/study_profile.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/study_summary.py` & `data-warehouse-client-3.0.1/data_warehouse_client/study_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 # Summarise a study
 
 from tabulate import tabulate
-from print_io import print_measurement_group_instances, print_measurement_group_instances_to_file
-from csv_io import export_measurement_groups_as_csv
 from datetime import datetime
 
+from data_warehouse_client.csv_io import export_measurement_groups_as_csv
+from data_warehouse_client.print_io import print_measurement_group_instances, print_measurement_group_instances_to_file
+
 
 def get_instances_per_measurement_group(dw, study):
     """
     Returns the number of instances in all measurement groups in a study
     :param dw: data warehouse handle
     :param study: study id
     :return: number of instances in each measurement group
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/table_reader_json.py` & `data-warehouse-client-3.0.1/data_warehouse_client/table_reader_json.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/table_writer_json.py` & `data-warehouse-client-3.0.1/data_warehouse_client/table_writer_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from json import dump
 from os import path, makedirs
-from check_for_datetime_table import datetimebounds_table_in_dw
+
+from data_warehouse_client.check_for_datetime_table import datetimebounds_table_in_dw
 
 
 def table_to_dictionary(dw, table_name, study_id):
     """
     Read a table and turn it into a dictionary
     Based on code in: https://stackoverflow.com/questions/3286525/return-sql-table-as-json-in-python
     :param dw: data warehouse handle
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/transform_result_format.py` & `data-warehouse-client-3.0.1/data_warehouse_client/transform_result_format.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/type_checks.py` & `data-warehouse-client-3.0.1/data_warehouse_client/type_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
 from typing import Tuple, Any
-from check_bounded_values import check_category_id, check_bounded_datetime_in_bounds,\
-    check_bounded_int_in_bounds, check_bounded_real_in_bounds
-from type_definitions import Bounds, Value, ValType, MeasurementType
+
+from data_warehouse_client.check_bounded_values import check_category_id, check_bounded_int_in_bounds, \
+    check_bounded_real_in_bounds, check_bounded_datetime_in_bounds
+from data_warehouse_client.type_definitions import Bounds, MeasurementType, Value, ValType
 
 
 def int_bounds(bounds: Bounds):
     return bounds[0]
 
 
 def real_bounds(bounds: Bounds):
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/type_definitions.py` & `data-warehouse-client-3.0.1/data_warehouse_client/type_definitions.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client/warehouse_checker.py` & `data-warehouse-client-3.0.1/data_warehouse_client/warehouse_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 # The measurementType is in the measurement group for each measurement
 # The valtype is correct for the measurement type for each measurement
 # the measurement group is valid for the study
 # there are no missing measurement types in a measurement group instance
 # no ordinal, nominal, bounded integer or bounded real values are out of bounds
 
 
-from file_utils import process_sql_template
-from data_warehouse import core_sql_for_measurements
-from print_io import print_measurements, print_measurements_to_file
 from tabulate import tabulate
 from datetime import datetime
-from check_for_datetime_table import datetimebounds_table_in_dw
+
+from data_warehouse_client.check_for_datetime_table import datetimebounds_table_in_dw
+from data_warehouse_client.data_warehouse import core_sql_for_measurements
+from data_warehouse_client.file_utils import process_sql_template
+from data_warehouse_client.print_io import print_measurements, print_measurements_to_file
 
 
 def check_category_exists(dw, study):
     """
     Find measurement types of nominal or ordinal value type without entry in category table
     :param dw: handle to data warehouse
     :param study: study id
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client.egg-info/PKG-INFO` & `data-warehouse-client-3.0.1/data_warehouse_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-warehouse-client
-Version: 3.0.0
+Version: 3.0.1
 Summary: This package provides access to the e-Science Central data warehouse that can be used to store, access and analyse data collected in scientific studies, including for healthcare applications
 Home-page: https://github.com/e-science-central/data-warehouse-client
 Author: Paul Watson
 Author-email: paul.watson@ncl.ac.uk
 License: UNKNOWN
 Description: # Data Warehouse Client
```

### Comparing `data-warehouse-client-3.0.0/data_warehouse_client.egg-info/SOURCES.txt` & `data-warehouse-client-3.0.1/data_warehouse_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/docs/data_warehouse_guide.pdf` & `data-warehouse-client-3.0.1/docs/data_warehouse_guide.pdf`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/integration_test/clone_study_metadata_test.py` & `data-warehouse-client-3.0.1/integration_test/clone_study_metadata_test.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/integration_test/delete_study_test.py` & `data-warehouse-client-3.0.1/integration_test/delete_study_test.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/setup.py` & `data-warehouse-client-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.0/test/test_file_utils.py` & `data-warehouse-client-3.0.1/test/test_file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from unittest import TestCase
+
 from data_warehouse_client import file_utils
 
 
 class TestFileUtils(TestCase):
     def test_process_sql_template(self):
         mappings = {"measurement_group": str(16), "study": str(4)}
         expected_result = "SELECT COUNT(*) FROM measurementtypetogroup WHERE measurementtypetogroup.measurementgroup = 16 AND measurementtypetogroup.study = 4;"
```

### Comparing `data-warehouse-client-3.0.0/test/test_transform_result_format.py` & `data-warehouse-client-3.0.1/test/test_transform_result_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from unittest import TestCase
 
-from data_warehouse_client import transform_result_format
 import datetime
 
+from data_warehouse_client import transform_result_format
+
 
 class TestTransformResultFormat(TestCase):
     def test_form_measurements(self):
         rid = 101
         time = datetime.datetime.now()
         study = 102
         trial = 103
```

