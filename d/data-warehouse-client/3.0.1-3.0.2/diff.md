# Comparing `tmp/data-warehouse-client-3.0.1.tar.gz` & `tmp/data-warehouse-client-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-warehouse-client-3.0.1.tar", last modified: Sun Apr  9 15:47:02 2023, max compression
+gzip compressed data, was "data-warehouse-client-3.0.2.tar", last modified: Sun Apr  9 18:03:51 2023, max compression
```

## Comparing `data-warehouse-client-3.0.1.tar` & `data-warehouse-client-3.0.2.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.221954 data-warehouse-client-3.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.221954 data-warehouse-client-3.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.225954 data-warehouse-client-3.0.1/data_warehouse_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/auto_generate_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/auto_generate_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/check_bounded_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/check_for_datetime_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/clone_study_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/csv_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    41250 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/data_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/delete_study_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18877 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/import_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    34701 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/import_with_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    44140 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/load_warehouse_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/multiple_mg_inserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/print_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/print_metadata_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/data_warehouse_client/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_datetime_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_datetimes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_integer_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_integers.sql
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_real_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_reals.sql
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/core_sql_from_for_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/core_sql_select_for_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_all_measurement_groups.sql
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_all_measurement_groups_and_types_in_a_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_all_table_names.sql
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_boundsdatetime_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_boundsint_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_boundsreal_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_categories_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_category_ids.sql
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurement_group_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurement_groups_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurement_type_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurements_by_cohort.sql
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurements_with_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/get_units_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/insert_datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/insert_measurement.sql
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/insert_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/measurements_lacking_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/measurements_with_invalid_category.sql
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/num_types_in_a_measurement_group.sql
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/ordinal_types_not_matching_category.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/types_in_a_measurement_group.sql
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/sql/update_measurement_group_instance_id.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/study_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/study_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/table_reader_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/table_writer_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/transform_result_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/type_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/data_warehouse_client/warehouse_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.225954 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 15:47:02.000000 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-09 15:47:02.000000 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:47:02.000000 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-09 15:47:02.000000 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 15:47:02.000000 data-warehouse-client-3.0.1/data_warehouse_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   574842 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/docs/data_warehouse_guide.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/integration_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/integration_test/clone_study_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/integration_test/delete_study_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:02.233954 data-warehouse-client-3.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/test/test_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-09 15:46:52.000000 data-warehouse-client-3.0.1/test/test_transform_result_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.661648 data-warehouse-client-3.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.661648 data-warehouse-client-3.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.665648 data-warehouse-client-3.0.2/data_warehouse_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/auto_generate_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/auto_generate_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/check_bounded_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/check_for_datetime_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/clone_study_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/csv_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41274 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/data_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/delete_study_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/import_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34701 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/import_with_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44140 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/load_warehouse_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/multiple_mg_inserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/print_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/print_metadata_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/data_warehouse_client/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_datetime_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_datetimes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_integer_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_integers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_real_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_reals.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/core_sql_from_for_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/core_sql_select_for_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_all_measurement_groups.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_all_measurement_groups_and_types_in_a_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_all_table_names.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_boundsdatetime_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_boundsint_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_boundsreal_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_categories_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_category_ids.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurement_group_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurement_groups_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurement_type_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurements_by_cohort.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurements_with_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_units_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/insert_datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/insert_measurement.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/insert_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/measurements_lacking_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/measurements_with_invalid_category.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/num_types_in_a_measurement_group.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/ordinal_types_not_matching_category.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/types_in_a_measurement_group.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/update_measurement_group_instance_id.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/study_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/study_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/table_reader_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/table_writer_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/transform_result_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/type_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/warehouse_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.665648 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 18:03:51.000000 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-09 18:03:51.000000 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:03:51.000000 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-09 18:03:51.000000 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 18:03:51.000000 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   574842 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/docs/data_warehouse_guide.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/integration_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/integration_test/clone_study_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/integration_test/delete_study_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/test/test_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/test/test_transform_result_format.py
```

### Comparing `data-warehouse-client-3.0.1/.github/workflows/build.yml` & `data-warehouse-client-3.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/.github/workflows/release.yml` & `data-warehouse-client-3.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/.gitignore` & `data-warehouse-client-3.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/LICENSE` & `data-warehouse-client-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/PKG-INFO` & `data-warehouse-client-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-warehouse-client
-Version: 3.0.1
+Version: 3.0.2
 Summary: This package provides access to the e-Science Central data warehouse that can be used to store, access and analyse data collected in scientific studies, including for healthcare applications
 Home-page: https://github.com/e-science-central/data-warehouse-client
 Author: Paul Watson
 Author-email: paul.watson@ncl.ac.uk
 License: UNKNOWN
 Description: # Data Warehouse Client
```

### Comparing `data-warehouse-client-3.0.1/README.md` & `data-warehouse-client-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/auto_generate_test_cases.py` & `data-warehouse-client-3.0.2/data_warehouse_client/auto_generate_test_cases.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/auto_generate_tests.py` & `data-warehouse-client-3.0.2/data_warehouse_client/auto_generate_tests.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/check_bounded_values.py` & `data-warehouse-client-3.0.2/data_warehouse_client/check_bounded_values.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/check_for_datetime_table.py` & `data-warehouse-client-3.0.2/data_warehouse_client/check_for_datetime_table.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/clone_study_metadata.py` & `data-warehouse-client-3.0.2/data_warehouse_client/clone_study_metadata.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/csv_io.py` & `data-warehouse-client-3.0.2/data_warehouse_client/csv_io.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/data_warehouse.py` & `data-warehouse-client-3.0.2/data_warehouse_client/data_warehouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from datetime import datetime
 from sys import exit
 import psycopg2
 from json import load
 from more_itertools import intersperse
 
 from data_warehouse_client.file_utils import process_sql_template
-from data_warehouse_client.transform_result_format import form_measurements
+from data_warehouse_client.transform_result_format import form_measurements, form_measurement_group
 
 
 def get_participants_in_result(results):
     """
     find all participants in a set of results
     :param results: a list of measurements. Each measurement is held in a list with the following fields:
                     id,time,study,participant,measurementType,typeName,measurementGroup,
```

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/delete_study_contents.py` & `data-warehouse-client-3.0.2/data_warehouse_client/delete_study_contents.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/file_utils.py` & `data-warehouse-client-3.0.2/data_warehouse_client/file_utils.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/import_tests.py` & `data-warehouse-client-3.0.2/data_warehouse_client/import_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 from typing import Dict, List, Tuple
 from datetime import datetime
 
 from data_warehouse_client.check_bounded_values import get_inverse_category_ids_map
 from data_warehouse_client.data_warehouse import DataWarehouse
 from data_warehouse_client.load_data import load_data
 from data_warehouse_client.type_checks import check_int
-from data_warehouse_client.type_definitions import DataToLoad, Bounds, LoaderResult, MeasurementGroup, LoadHelperResult, \
-    Loader
+from data_warehouse_client.type_definitions import DataToLoad, Bounds, LoaderResult, MeasurementGroup, \
+    LoadHelperResult, Loader
 from data_warehouse_client import import_with_checks as iwc
 
+
 @pytest.fixture()
 def walking_test_1() -> DataToLoad:
     data = {
         'visit-date': datetime.now(),
         'visit-code': 'visit3',
         'wb_id': "fred",
         'Turn_Id': 2345,
```

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/import_with_checks.py` & `data-warehouse-client-3.0.2/data_warehouse_client/import_with_checks.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/load_data.py` & `data-warehouse-client-3.0.2/data_warehouse_client/load_data.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/load_warehouse_helpers.py` & `data-warehouse-client-3.0.2/data_warehouse_client/load_warehouse_helpers.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/multiple_mg_inserts.py` & `data-warehouse-client-3.0.2/data_warehouse_client/multiple_mg_inserts.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/plot.py` & `data-warehouse-client-3.0.2/data_warehouse_client/plot.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/print_io.py` & `data-warehouse-client-3.0.2/data_warehouse_client/print_io.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/print_metadata_table.py` & `data-warehouse-client-3.0.2/data_warehouse_client/print_metadata_table.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_datetimes.sql` & `data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_datetimes.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_integers.sql` & `data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_integers.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/sql/bounded_reals.sql` & `data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_reals.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/sql/core_sql_from_for_measurements.sql` & `data-warehouse-client-3.0.2/data_warehouse_client/sql/core_sql_from_for_measurements.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/sql/get_measurement_group_info.sql` & `data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurement_group_info.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/study_profile.py` & `data-warehouse-client-3.0.2/data_warehouse_client/study_profile.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/study_summary.py` & `data-warehouse-client-3.0.2/data_warehouse_client/study_summary.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/table_reader_json.py` & `data-warehouse-client-3.0.2/data_warehouse_client/table_reader_json.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/table_writer_json.py` & `data-warehouse-client-3.0.2/data_warehouse_client/table_writer_json.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/transform_result_format.py` & `data-warehouse-client-3.0.2/data_warehouse_client/transform_result_format.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/type_checks.py` & `data-warehouse-client-3.0.2/data_warehouse_client/type_checks.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/type_definitions.py` & `data-warehouse-client-3.0.2/data_warehouse_client/type_definitions.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client/warehouse_checker.py` & `data-warehouse-client-3.0.2/data_warehouse_client/warehouse_checker.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client.egg-info/PKG-INFO` & `data-warehouse-client-3.0.2/data_warehouse_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-warehouse-client
-Version: 3.0.1
+Version: 3.0.2
 Summary: This package provides access to the e-Science Central data warehouse that can be used to store, access and analyse data collected in scientific studies, including for healthcare applications
 Home-page: https://github.com/e-science-central/data-warehouse-client
 Author: Paul Watson
 Author-email: paul.watson@ncl.ac.uk
 License: UNKNOWN
 Description: # Data Warehouse Client
```

### Comparing `data-warehouse-client-3.0.1/data_warehouse_client.egg-info/SOURCES.txt` & `data-warehouse-client-3.0.2/data_warehouse_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 data_warehouse_client/type_definitions.py
 data_warehouse_client/warehouse_checker.py
 data_warehouse_client.egg-info/PKG-INFO
 data_warehouse_client.egg-info/SOURCES.txt
 data_warehouse_client.egg-info/dependency_links.txt
 data_warehouse_client.egg-info/requires.txt
 data_warehouse_client.egg-info/top_level.txt
+data_warehouse_client/sql/__init__.py
 data_warehouse_client/sql/bounded_datetime_measurement_types_without_bounds.sql
 data_warehouse_client/sql/bounded_datetimes.sql
 data_warehouse_client/sql/bounded_integer_measurement_types_without_bounds.sql
 data_warehouse_client/sql/bounded_integers.sql
 data_warehouse_client/sql/bounded_real_measurement_types_without_bounds.sql
 data_warehouse_client/sql/bounded_reals.sql
 data_warehouse_client/sql/core_sql_from_for_measurements.sql
```

### Comparing `data-warehouse-client-3.0.1/docs/data_warehouse_guide.pdf` & `data-warehouse-client-3.0.2/docs/data_warehouse_guide.pdf`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/integration_test/clone_study_metadata_test.py` & `data-warehouse-client-3.0.2/integration_test/clone_study_metadata_test.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/integration_test/delete_study_test.py` & `data-warehouse-client-3.0.2/integration_test/delete_study_test.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/setup.py` & `data-warehouse-client-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/test/test_file_utils.py` & `data-warehouse-client-3.0.2/test/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.1/test/test_transform_result_format.py` & `data-warehouse-client-3.0.2/test/test_transform_result_format.py`

 * *Files identical despite different names*

