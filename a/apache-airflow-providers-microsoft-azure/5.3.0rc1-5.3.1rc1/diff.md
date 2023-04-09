# Comparing `tmp/apache-airflow-providers-microsoft-azure-5.3.0rc1.tar.gz` & `tmp/apache-airflow-providers-microsoft-azure-5.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-microsoft-azure-5.3.0rc1.tar", last modified: Sun Apr  2 05:48:58 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-microsoft-azure-5.3.1rc1.tar", last modified: Sun Apr  9 13:49:39 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1.tar` & `apache-airflow-providers-microsoft-azure-5.3.1rc1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:58.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:48:55.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    24636 2023-04-02 05:48:58.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    23015 2023-04-02 05:48:55.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16571 2023-04-02 05:48:55.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8720 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/adx.py
--rw-r--r--   0 root         (0) root         (0)    10986 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/asb.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
--rw-r--r--   0 root         (0) root         (0)    15288 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/batch.py
--rw-r--r--   0 root         (0) root         (0)     6056 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
--rw-r--r--   0 root         (0) root         (0)     4058 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
--rw-r--r--   0 root         (0) root         (0)    14222 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    42973 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
--rw-r--r--   0 root         (0) root         (0)    21695 2023-03-10 19:32:05.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
--rw-r--r--   0 root         (0) root         (0)    12985 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
--rw-r--r--   0 root         (0) root         (0)     7318 2023-03-16 20:46:35.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/synapse.py
--rw-r--r--   0 root         (0) root         (0)    27566 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-03-10 19:31:58.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/adls.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/adx.py
--rw-r--r--   0 root         (0) root         (0)    29576 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/asb.py
--rw-r--r--   0 root         (0) root         (0)    16252 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)    15967 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/container_instances.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    11545 2023-03-27 08:32:49.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/synapse.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7822 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
--rw-r--r--   0 root         (0) root         (0)     5611 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     5957 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/sensors/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:58.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5293 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     4765 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
--rw-r--r--   0 root         (0) root         (0)     4575 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
--rw-r--r--   0 root         (0) root         (0)     8215 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:58.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-03-14 06:24:40.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8863 2023-03-27 08:32:49.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/triggers/wasb.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:58.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)    24636 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2944 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      609 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:48:57.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2359 2023-04-02 05:48:58.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1704 2023-04-02 05:48:55.000000 apache-airflow-providers-microsoft-azure-5.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-09 13:49:34.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    24923 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    23302 2023-04-09 13:49:34.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:38.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:38.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:38.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16620 2023-04-09 13:49:34.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8720 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/adx.py
+-rw-r--r--   0 root         (0) root         (0)    10986 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/asb.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
+-rw-r--r--   0 root         (0) root         (0)    15288 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/batch.py
+-rw-r--r--   0 root         (0) root         (0)     6056 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
+-rw-r--r--   0 root         (0) root         (0)     4058 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
+-rw-r--r--   0 root         (0) root         (0)    14222 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    42973 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)    21695 2023-03-10 19:32:05.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
+-rw-r--r--   0 root         (0) root         (0)    12985 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
+-rw-r--r--   0 root         (0) root         (0)     7318 2023-03-16 20:46:35.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/synapse.py
+-rw-r--r--   0 root         (0) root         (0)    27566 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-03-10 19:31:58.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/adls.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/adx.py
+-rw-r--r--   0 root         (0) root         (0)    29576 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/asb.py
+-rw-r--r--   0 root         (0) root         (0)    16252 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)    15967 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/container_instances.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    11409 2023-04-08 17:35:36.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/synapse.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7822 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     5957 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/sensors/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5293 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     4765 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
+-rw-r--r--   0 root         (0) root         (0)     8215 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-03-14 06:24:40.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8863 2023-03-27 08:32:49.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/triggers/wasb.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    24923 2023-04-09 13:49:38.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-04-09 13:49:38.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:49:38.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-09 13:49:38.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:49:38.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      609 2023-04-09 13:49:38.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 13:49:38.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-04-09 13:49:39.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-04-09 13:49:34.000000 apache-airflow-providers-microsoft-azure-5.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/LICENSE` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/MANIFEST.in` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -23,10 +23,9 @@
 # `MANIFEST_TEMPLATE.py.jinja2` IN the `provider_packages` DIRECTORY
 
 
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.txt
-include README.md
+include CHANGELOG.rst
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/PKG-INFO` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 5.3.0rc1
+Version: 5.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -51,28 +51,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``5.3.0rc1``
+Release: ``5.3.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -149,14 +149,26 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.3.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix AzureDataFactoryPipelineRunLink get_link method (#30514)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 5.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add deferrable 'AzureDataFactoryRunPipelineOperator' (#30147)``
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/README.rst` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``5.3.0rc1``
+Release: ``5.3.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -113,14 +113,26 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.3.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix AzureDataFactoryPipelineRunLink get_link method (#30514)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 5.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add deferrable 'AzureDataFactoryRunPipelineOperator' (#30147)``
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/__init__.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/get_provider_info.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-azure",
         "name": "Microsoft Azure",
         "description": "`Microsoft Azure <https://azure.microsoft.com/>`__\n",
+        "suspended": False,
         "versions": [
+            "5.3.1",
             "5.3.0",
             "5.2.1",
             "5.2.0",
             "5.1.0",
             "5.0.2",
             "5.0.1",
             "5.0.0",
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/__init__.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/adx.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/asb.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/base_azure.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/base_azure.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/batch.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/container_instance.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/container_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/container_registry.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/container_registry.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/container_volume.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/container_volume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/cosmos.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/data_factory.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/data_lake.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/fileshare.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/fileshare.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/synapse.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/hooks/wasb.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/hooks/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/log/__init__.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/__init__.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/adls.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/adx.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/asb.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/batch.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/container_instances.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/container_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/cosmos.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/data_factory.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/data_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,28 +44,27 @@
 
     def get_link(
         self,
         operator: BaseOperator,
         *,
         ti_key: TaskInstanceKey,
     ) -> str:
-        if not isinstance(operator, AzureDataFactoryRunPipelineOperator):
-            self.log.info("The %s is not %s class.", operator.__class__, AzureDataFactoryRunPipelineOperator)
-            return ""
         run_id = XCom.get_value(key="run_id", ti_key=ti_key)
-        conn_id = operator.azure_data_factory_conn_id
+        conn_id = operator.azure_data_factory_conn_id  # type: ignore
         conn = BaseHook.get_connection(conn_id)
         extras = conn.extra_dejson
         subscription_id = get_field(extras, "subscriptionId")
         if not subscription_id:
             raise KeyError(f"Param subscriptionId not found in conn_id '{conn_id}'")
         # Both Resource Group Name and Factory Name can either be declared in the Azure Data Factory
         # connection or passed directly to the operator.
-        resource_group_name = operator.resource_group_name or get_field(extras, "resource_group_name")
-        factory_name = operator.factory_name or get_field(extras, "factory_name")
+        resource_group_name = operator.resource_group_name or get_field(  # type: ignore
+            extras, "resource_group_name"
+        )
+        factory_name = operator.factory_name or get_field(extras, "factory_name")  # type: ignore
         url = (
             f"https://adf.azure.com/en-us/monitoring/pipelineruns/{run_id}"
             f"?factory=/subscriptions/{subscription_id}/"
             f"resourceGroups/{resource_group_name}/providers/Microsoft.DataFactory/"
             f"factories/{factory_name}"
         )
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/synapse.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/secrets/__init__.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/secrets/key_vault.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/secrets/key_vault.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/sensors/__init__.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/sensors/cosmos.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/sensors/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/sensors/data_factory.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/sensors/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/sensors/wasb.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/sensors/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/__init__.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/triggers/__init__.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/triggers/data_factory.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/triggers/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/triggers/wasb.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/triggers/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/airflow/providers/microsoft/azure/utils.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/airflow/providers/microsoft/azure/utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 5.3.0rc1
+Version: 5.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -51,28 +51,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``5.3.0rc1``
+Release: ``5.3.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -149,14 +149,26 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.3.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix AzureDataFactoryPipelineRunLink get_link method (#30514)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 5.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add deferrable 'AzureDataFactoryRunPipelineOperator' (#30147)``
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/pyproject.toml` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -135,18 +135,15 @@
 
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
-"airflow/models/pydantic/taskinstance.py" = ["I002"]
-"airflow/models/pydantic/dag_run.py" = ["I002"]
-"airflow/models/pydantic/dataset.py" = ["I002"]
-"airflow/jobs/pydantic/base_job.py" = ["I002"]
+"airflow/serialization/pydantic/*.py" = ["I002"]
 
 # Ignore pydoc style from these
 "*.pyi" = ["D"]
 "tests/*" = ["D"]
 "scripts/*" = ["D"]
 "dev/*" = ["D"]
 "docs/*" = ["D"]
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/setup.cfg` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/5.3.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-microsoft-azure-5.3.0rc1/setup.py` & `apache-airflow-providers-microsoft-azure-5.3.1rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,27 +22,32 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-microsoft-azure package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.3.0"
+version = "5.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-microsoft-azure setup."""
     setup(
         version=version,
         extras_require={
             "google": ["apache-airflow-providers-google"],
             "oracle": ["apache-airflow-providers-oracle"],
             "sftp": ["apache-airflow-providers-sftp"],
         },
         packages=find_namespace_packages(
-            include=["airflow.providers.microsoft.azure", "airflow.providers.microsoft.azure.*"]
+            include=[
+                "airflow.providers.microsoft.azure",
+                "airflow.providers.microsoft.azure.*",
+                "airflow.providers.microsoft.azure_vendor",
+                "airflow.providers.microsoft.azure_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

