# Comparing `tmp/phidata-1.5.5.tar.gz` & `tmp/phidata-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-1.5.5.tar", last modified: Fri Apr  7 20:22:52 2023, max compression
+gzip compressed data, was "phidata-1.5.6.tar", last modified: Sun Apr  9 17:04:10 2023, max compression
```

## Comparing `phidata-1.5.5.tar` & `phidata-1.5.6.tar`

### file list

```diff
@@ -1,497 +1,507 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.021928 phidata-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-07 20:22:32.000000 phidata-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-07 20:22:52.021928 phidata-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-07 20:22:32.000000 phidata-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.977928 phidata-1.5.5/phidata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.977928 phidata-1.5.5/phidata/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.977928 phidata-1.5.5/phidata/airflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/airflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.977928 phidata-1.5.5/phidata/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.977928 phidata-1.5.5/phidata/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.977928 phidata-1.5.5/phidata/app/alertmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.977928 phidata-1.5.5/phidata/app/amundsen/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/amundsen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/amundsen/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/amundsen/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/amundsen/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.977928 phidata-1.5.5/phidata/app/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/assistant/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/cadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/databox/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/databox/databox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/db/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/db/base_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48622 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/grafana/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/k8s/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/k8s/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/k8s/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/nodeexporter/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47922 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/phidata_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.981928 phidata-1.5.5/phidata/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53160 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.985928 phidata-1.5.5/phidata/app/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.985928 phidata-1.5.5/phidata/app/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.985928 phidata-1.5.5/phidata/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/server/api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/server/app_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    58078 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/server/server_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.985928 phidata-1.5.5/phidata/app/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49371 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/spark/spark_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.985928 phidata-1.5.5/phidata/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.985928 phidata-1.5.5/phidata/app/superset/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/superset/superset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/superset/superset_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/superset/superset_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.985928 phidata-1.5.5/phidata/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.985928 phidata-1.5.5/phidata/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/asset/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/asset/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/asset/data_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/asset/local/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/asset/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/asset/local/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/aws/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/aws/create/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/create/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/aws/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/aws/resource/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.989928 phidata-1.5.5/phidata/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.993928 phidata-1.5.5/phidata/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.993928 phidata-1.5.5/phidata/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.993928 phidata-1.5.5/phidata/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.993928 phidata-1.5.5/phidata/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.993928 phidata-1.5.5/phidata/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.993928 phidata-1.5.5/phidata/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.993928 phidata-1.5.5/phidata/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/iam/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.993928 phidata-1.5.5/phidata/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.993928 phidata-1.5.5/phidata/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.993928 phidata-1.5.5/phidata/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.997928 phidata-1.5.5/phidata/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/s3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/s3/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/aws/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.997928 phidata-1.5.5/phidata/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/checks/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/checks/not_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.997928 phidata-1.5.5/phidata/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/decorators/validate_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.997928 phidata-1.5.5/phidata/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.997928 phidata-1.5.5/phidata/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/resource/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/resource/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.997928 phidata-1.5.5/phidata/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.997928 phidata-1.5.5/phidata/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/exceptions/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/exceptions/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/exceptions/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.997928 phidata-1.5.5/phidata/infra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/infra/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/infra/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/infra/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/infra/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.001928 phidata-1.5.5/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.005928 phidata-1.5.5/phidata/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.009928 phidata-1.5.5/phidata/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.009928 phidata-1.5.5/phidata/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.009928 phidata-1.5.5/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.009928 phidata-1.5.5/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.009928 phidata-1.5.5/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.009928 phidata-1.5.5/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.009928 phidata-1.5.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/k8s/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/utils/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/k8s/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/product/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/product/data_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/table/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/local/local_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/local/parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/table/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/s3/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/s3/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/table/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/sql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/task/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/task/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/task/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/task/aws/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.013928 phidata-1.5.5/phidata/task/aws/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/task/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/task/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/task/download/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/download/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/task/download/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/download/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/download/url/to_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/download/url/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/task/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/task/plot/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/plot/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/python_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/task/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/task/run/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/run/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/run/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/task_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/task/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/task/upload/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/upload/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.017928 phidata-1.5.5/phidata/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/types/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/types/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/types/phidata_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.021928 phidata-1.5.5/phidata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/env_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/prep_infra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/print_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/utils/workspace_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.021928 phidata-1.5.5/phidata/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/workflow/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.021928 phidata-1.5.5/phidata/workflow/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/workflow/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.021928 phidata-1.5.5/phidata/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-07 20:22:32.000000 phidata-1.5.5/phidata/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:51.977928 phidata-1.5.5/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-07 20:22:51.000000 phidata-1.5.5/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-04-07 20:22:51.000000 phidata-1.5.5/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:22:51.000000 phidata-1.5.5/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 20:22:51.000000 phidata-1.5.5/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 20:22:51.000000 phidata-1.5.5/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-07 20:22:32.000000 phidata-1.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:22:52.021928 phidata-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-07 20:22:32.000000 phidata-1.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:52.021928 phidata-1.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-07 20:22:32.000000 phidata-1.5.5/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.329632 phidata-1.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-09 17:03:50.000000 phidata-1.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-09 17:04:10.329632 phidata-1.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-09 17:03:50.000000 phidata-1.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.277631 phidata-1.5.6/phidata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.277631 phidata-1.5.6/phidata/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.277631 phidata-1.5.6/phidata/airflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.277631 phidata-1.5.6/phidata/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.277631 phidata-1.5.6/phidata/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.277631 phidata-1.5.6/phidata/app/alertmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.281631 phidata-1.5.6/phidata/app/amundsen/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/amundsen/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.281631 phidata-1.5.6/phidata/app/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/assistant/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.281631 phidata-1.5.6/phidata/app/cadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.281631 phidata-1.5.6/phidata/app/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/databox/databox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.281631 phidata-1.5.6/phidata/app/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/db/base_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.281631 phidata-1.5.6/phidata/app/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.281631 phidata-1.5.6/phidata/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.281631 phidata-1.5.6/phidata/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.281631 phidata-1.5.6/phidata/app/grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/grafana/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.281631 phidata-1.5.6/phidata/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.285632 phidata-1.5.6/phidata/app/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/k8s/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/k8s/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/k8s/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.285632 phidata-1.5.6/phidata/app/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.285632 phidata-1.5.6/phidata/app/nodeexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/phidata_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.285632 phidata-1.5.6/phidata/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53160 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.285632 phidata-1.5.6/phidata/app/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.285632 phidata-1.5.6/phidata/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.285632 phidata-1.5.6/phidata/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/server/api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/server/app_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58186 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/server/server_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.285632 phidata-1.5.6/phidata/app/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/spark/spark_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.285632 phidata-1.5.6/phidata/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.289631 phidata-1.5.6/phidata/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/superset/superset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/superset/superset_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.289631 phidata-1.5.6/phidata/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.289631 phidata-1.5.6/phidata/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.289631 phidata-1.5.6/phidata/asset/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/asset/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/asset/data_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.289631 phidata-1.5.6/phidata/asset/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/asset/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/asset/local/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.289631 phidata-1.5.6/phidata/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.289631 phidata-1.5.6/phidata/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.289631 phidata-1.5.6/phidata/aws/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.293631 phidata-1.5.6/phidata/aws/create/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/create/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.293631 phidata-1.5.6/phidata/aws/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.293631 phidata-1.5.6/phidata/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.293631 phidata-1.5.6/phidata/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.293631 phidata-1.5.6/phidata/aws/resource/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.293631 phidata-1.5.6/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.293631 phidata-1.5.6/phidata/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.293631 phidata-1.5.6/phidata/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.293631 phidata-1.5.6/phidata/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.297632 phidata-1.5.6/phidata/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.297632 phidata-1.5.6/phidata/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-09 17:03:50.000000 phidata-1.5.6/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.297632 phidata-1.5.6/phidata/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.297632 phidata-1.5.6/phidata/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.297632 phidata-1.5.6/phidata/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.297632 phidata-1.5.6/phidata/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.297632 phidata-1.5.6/phidata/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.297632 phidata-1.5.6/phidata/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.297632 phidata-1.5.6/phidata/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/s3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/s3/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/aws/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.301632 phidata-1.5.6/phidata/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/checks/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/checks/not_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.301632 phidata-1.5.6/phidata/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/decorators/validate_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.301632 phidata-1.5.6/phidata/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.301632 phidata-1.5.6/phidata/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/resource/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/resource/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.301632 phidata-1.5.6/phidata/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.301632 phidata-1.5.6/phidata/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/exceptions/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/exceptions/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/exceptions/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.305631 phidata-1.5.6/phidata/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/infra/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/infra/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/infra/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/infra/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.305631 phidata-1.5.6/phidata/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.305631 phidata-1.5.6/phidata/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.305631 phidata-1.5.6/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.305631 phidata-1.5.6/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.305631 phidata-1.5.6/phidata/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.305631 phidata-1.5.6/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.305631 phidata-1.5.6/phidata/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.305631 phidata-1.5.6/phidata/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.309632 phidata-1.5.6/phidata/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.309632 phidata-1.5.6/phidata/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.309632 phidata-1.5.6/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.309632 phidata-1.5.6/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.309632 phidata-1.5.6/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.309632 phidata-1.5.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.309632 phidata-1.5.6/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.309632 phidata-1.5.6/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.309632 phidata-1.5.6/phidata/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.313632 phidata-1.5.6/phidata/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.313632 phidata-1.5.6/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.313632 phidata-1.5.6/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.313632 phidata-1.5.6/phidata/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.313632 phidata-1.5.6/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.313632 phidata-1.5.6/phidata/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/k8s/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/utils/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/k8s/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.317632 phidata-1.5.6/phidata/llm/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/llm/duckdb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/product/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/product/data_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/table/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/local/local_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/local/parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/table/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/s3/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/s3/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/sql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/task/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/task/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/task/aws/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/task/aws/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/task/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.321632 phidata-1.5.6/phidata/task/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.325632 phidata-1.5.6/phidata/task/download/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.325632 phidata-1.5.6/phidata/task/download/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/download/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/download/url/to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.325632 phidata-1.5.6/phidata/task/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.325632 phidata-1.5.6/phidata/task/plot/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/plot/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/python_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.325632 phidata-1.5.6/phidata/task/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.325632 phidata-1.5.6/phidata/task/run/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/run/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/task_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.325632 phidata-1.5.6/phidata/task/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.325632 phidata-1.5.6/phidata/task/upload/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.325632 phidata-1.5.6/phidata/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/types/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/types/phidata_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.329632 phidata-1.5.6/phidata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/env_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/prep_infra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/utils/workspace_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.329632 phidata-1.5.6/phidata/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/workflow/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.329632 phidata-1.5.6/phidata/workflow/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.329632 phidata-1.5.6/phidata/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-09 17:03:51.000000 phidata-1.5.6/phidata/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.277631 phidata-1.5.6/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-09 17:04:10.000000 phidata-1.5.6/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-04-09 17:04:10.000000 phidata-1.5.6/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:04:10.000000 phidata-1.5.6/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 17:04:10.000000 phidata-1.5.6/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 17:04:10.000000 phidata-1.5.6/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-09 17:03:51.000000 phidata-1.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 17:04:10.329632 phidata-1.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-09 17:03:51.000000 phidata-1.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:10.329632 phidata-1.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-09 17:03:51.000000 phidata-1.5.6/tests/test_placeholder.py
```

### Comparing `phidata-1.5.5/LICENSE` & `phidata-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/airflow/operators/empty.py` & `phidata-1.5.6/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/airflow/airflow_base.py` & `phidata-1.5.6/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/airflow/airflow_flower.py` & `phidata-1.5.6/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/airflow/airflow_manager.py` & `phidata-1.5.6/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/airflow/airflow_scheduler.py` & `phidata-1.5.6/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/airflow/airflow_webserver.py` & `phidata-1.5.6/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/airflow/airflow_worker.py` & `phidata-1.5.6/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/alertmanager/alertmanager.py` & `phidata-1.5.6/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/amundsen/frontend.py` & `phidata-1.5.6/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/amundsen/metadata.py` & `phidata-1.5.6/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/amundsen/search.py` & `phidata-1.5.6/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/assistant/assistant.py` & `phidata-1.5.6/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/cadvisor/cadvisor.py` & `phidata-1.5.6/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/databox/databox.py` & `phidata-1.5.6/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/db/base_db.py` & `phidata-1.5.6/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/elastic/elastic_app.py` & `phidata-1.5.6/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/elasticsearch/elasticsearch.py` & `phidata-1.5.6/phidata/app/elasticsearch/elasticsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,19 +524,19 @@
 
         # if open_container_port = True
         if self.args.open_container_port:
             container_ports[
                 str(self.args.container_port)
             ] = self.args.container_host_port
 
-        container_cmd: List[str]
+        container_cmd: List[str] = []
         if isinstance(self.args.command, str):
-            container_cmd = self.args.command.split(" ")
-        else:
-            container_cmd = self.args.command
+            container_cmd.extend(self.args.command.split(" "))
+        elif isinstance(self.args.command, list):
+            container_cmd.extend(self.args.command)
 
         # if self.args.discovery is not None:
         #     container_cmd.append(f"--discovery{str(self.args.discovery)}")
 
         # Create the container
         docker_container = DockerContainer(
             name=self.get_container_name(),
```

### Comparing `phidata-1.5.5/phidata/app/fastapi/fastapi.py` & `phidata-1.5.6/phidata/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/grafana/grafana.py` & `phidata-1.5.6/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/group.py` & `phidata-1.5.6/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/jupyter/jupyter_hub.py` & `phidata-1.5.6/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/jupyter/jupyter_lab.py` & `phidata-1.5.6/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/k8s/app.py` & `phidata-1.5.6/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/k8s/dir.py` & `phidata-1.5.6/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/k8s/url.py` & `phidata-1.5.6/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/neo4j/neo4j.py` & `phidata-1.5.6/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/nodeexporter/nodeexporter.py` & `phidata-1.5.6/phidata/app/nodeexporter/nodeexporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -933,21 +933,20 @@
             envs_from_secret=[secret.secret_name for secret in secrets]
             if len(secrets) > 0
             else None,
             ports=ports if len(ports) > 0 else None,
             volumes=volumes if len(volumes) > 0 else None,
             labels=container_labels,
         )
-        containers.insert(0, node - exporter_container)
+        containers.insert(0, nodeexporter_container)
 
         # Set default container for kubectl commands
         # https://kubernetes.io/docs/reference/labels-annotations-taints/#kubectl-kubernetes-io-default-container
         pod_annotations = {
-            "kubectl.kubernetes.io/default-container": node
-            - exporter_container.container_name,
+            "kubectl.kubernetes.io/default-container": nodeexporter_container.container_name,
         }
         if self.args.pod_annotations is not None and isinstance(
             self.args.pod_annotations, dict
         ):
             pod_annotations.update(self.args.pod_annotations)
 
         deploy_labels: Dict[str, Any] = common_labels or {}
@@ -972,15 +971,15 @@
             volumes=volumes if len(volumes) > 0 else None,
             labels=deploy_labels,
             pod_annotations=pod_annotations,
             topology_spread_key=self.args.topology_spread_key,
             topology_spread_max_skew=self.args.topology_spread_max_skew,
             topology_spread_when_unsatisfiable=self.args.topology_spread_when_unsatisfiable,
         )
-        deployments.append(node - exporter_deployment)
+        deployments.append(nodeexporter_deployment)
 
         # Create the services
         if self.args.create_service:
             service_labels: Dict[str, Any] = common_labels or {}
             if self.args.service_labels is not None and isinstance(
                 self.args.service_labels, dict
             ):
@@ -988,15 +987,15 @@
 
             _service = CreateService(
                 service_name=self.get_service_name(),
                 app_name=app_name,
                 namespace=ns_name,
                 service_account_name=sa_name,
                 service_type=self.args.service_type,
-                deployment=node - exporter_deployment,
+                deployment=nodeexporter_deployment,
                 ports=ports if len(ports) > 0 else None,
                 labels=service_labels,
             )
             services.append(_service)
 
         # Create the K8sResourceGroup
         k8s_resource_group = CreateK8sResourceGroup(
```

### Comparing `phidata-1.5.5/phidata/app/phidata_app.py` & `phidata-1.5.6/phidata/app/phidata_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/postgres/postgres_db.py` & `phidata-1.5.6/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/prometheus/prometheus.py` & `phidata-1.5.6/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/redis/redis.py` & `phidata-1.5.6/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/server/api_server.py` & `phidata-1.5.6/phidata/app/server/api_server.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/server/app_server.py` & `phidata-1.5.6/phidata/app/server/app_server.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/server/server_base.py` & `phidata-1.5.6/phidata/app/server/server_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1163,20 +1163,22 @@
                 skip_delete=self.args.skip_delete,
                 wait_for_creation=self.args.wait_for_creation,
                 wait_for_deletion=self.args.wait_for_deletion,
             )
 
         # Get VPC ID from subnets
         vpc_ids = set()
-        for subnet in self.args.aws_subnets:
-            _vpc = Subnet(id=subnet).get_vpc_id()
-            vpc_ids.add(_vpc)
-            if len(vpc_ids) != 1:
-                raise ValueError("Subnets must be in the same VPC")
-        vpc_id = vpc_ids.pop() if len(vpc_ids) == 1 else None
+        vpc_id = None
+        if self.args.aws_subnets is not None:
+            for subnet in self.args.aws_subnets:
+                _vpc = Subnet(id=subnet).get_vpc_id()
+                vpc_ids.add(_vpc)
+                if len(vpc_ids) != 1:
+                    raise ValueError("Subnets must be in the same VPC")
+            vpc_id = vpc_ids.pop() if len(vpc_ids) == 1 else None
 
         # -*- Create Target Group
         target_group = TargetGroup(
             name=f"{app_name}-tg",
             port=self.get_container_port(),
             protocol="HTTP",
             vpc_id=vpc_id,
@@ -1233,15 +1235,15 @@
             requires_compatibilities=[self.args.ecs_launch_type],
             skip_create=self.args.skip_create,
             skip_delete=self.args.skip_delete,
             wait_for_creation=self.args.wait_for_creation,
             wait_for_deletion=self.args.wait_for_deletion,
         )
 
-        aws_vpc_config = {}
+        aws_vpc_config: Dict[str, Any] = {}
         if self.args.aws_subnets is not None:
             aws_vpc_config["subnets"] = self.args.aws_subnets
         if self.args.aws_security_groups is not None:
             aws_vpc_config["securityGroups"] = self.args.aws_security_groups
         if self.args.assign_public_ip:
             aws_vpc_config["assignPublicIp"] = "ENABLED"
```

### Comparing `phidata-1.5.5/phidata/app/spark/spark_base.py` & `phidata-1.5.6/phidata/app/spark/spark_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,19 +542,19 @@
 
         # if open_container_port = True
         if self.args.open_container_port:
             container_ports[
                 str(self.args.container_port)
             ] = self.args.container_host_port
 
-        container_cmd: List[str]
+        container_cmd: List[str] = []
         if isinstance(self.args.command, str):
-            container_cmd = self.args.command.split(" ")
-        else:
-            container_cmd = self.args.command
+            container_cmd.extend(self.args.command.split(" "))
+        elif isinstance(self.args.command, list):
+            container_cmd.extend(self.args.command)
 
         if self.args.cores is not None:
             container_cmd.append(f"--cores {str(self.args.cores)}")
 
         if self.args.memory is not None:
             container_cmd.append(f"--memory {str(self.args.memory)}")
```

### Comparing `phidata-1.5.5/phidata/app/spark/spark_driver.py` & `phidata-1.5.6/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/spark/spark_worker.py` & `phidata-1.5.6/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/streamlit/streamlit.py` & `phidata-1.5.6/phidata/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/superset/superset_base.py` & `phidata-1.5.6/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/superset/superset_init.py` & `phidata-1.5.6/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/superset/superset_webserver.py` & `phidata-1.5.6/phidata/app/superset/superset_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/superset/superset_worker.py` & `phidata-1.5.6/phidata/app/superset/superset_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/superset/superset_worker_beat.py` & `phidata-1.5.6/phidata/app/superset/superset_worker_beat.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/traefik/crds.py` & `phidata-1.5.6/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/traefik/ingress_route.py` & `phidata-1.5.6/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/app/traefik/router.py` & `phidata-1.5.6/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/asset/aws/aws_asset.py` & `phidata-1.5.6/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/asset/data_asset.py` & `phidata-1.5.6/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/asset/local/file.py` & `phidata-1.5.6/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/asset/local/local_asset.py` & `phidata-1.5.6/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/api_client.py` & `phidata-1.5.6/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/athena/query.py` & `phidata-1.5.6/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/config.py` & `phidata-1.5.6/phidata/aws/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/create/iam/eks_admin_role.py` & `phidata-1.5.6/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/create/iam/role.py` & `phidata-1.5.6/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/enums/manager_status.py` & `phidata-1.5.6/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/manager.py` & `phidata-1.5.6/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/acm/certificate.py` & `phidata-1.5.6/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/athena/query.py` & `phidata-1.5.6/phidata/aws/resource/athena/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 
 class AthenaQueryExecution(AwsResource):
     """
     # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#client
     """
 
-    resource_type = "AthenaQueryExecution"
-    service_name = "athena"
+    resource_type: str = "AthenaQueryExecution"
+    service_name: str = "athena"
 
     # The SQL query statements to be executed.
     query_string: str
     # A unique case-sensitive string used to ensure the request to create the query
     # is idempotent (executes only once). If another StartQueryExecution request is received,
     # the same response is returned and another query is not created. If a parameter
     # has changed, for example, the QueryString , an error is returned.
```

### Comparing `phidata-1.5.5/phidata/aws/resource/base.py` & `phidata-1.5.6/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/cloudformation/stack.py` & `phidata-1.5.6/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/ec2/subnet.py` & `phidata-1.5.6/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/ec2/volume.py` & `phidata-1.5.6/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/ecs/cluster.py` & `phidata-1.5.6/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/ecs/container.py` & `phidata-1.5.6/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/ecs/service.py` & `phidata-1.5.6/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/ecs/task_definition.py` & `phidata-1.5.6/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/ecs/volume.py` & `phidata-1.5.6/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/eks/addon.py` & `phidata-1.5.6/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/eks/cluster.py` & `phidata-1.5.6/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/eks/fargate_profile.py` & `phidata-1.5.6/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/eks/kubeconfig.py` & `phidata-1.5.6/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/eks/node_group.py` & `phidata-1.5.6/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/elasticache/cluster.py` & `phidata-1.5.6/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-1.5.6/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/elb/listener.py` & `phidata-1.5.6/phidata/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/elb/load_balancer.py` & `phidata-1.5.6/phidata/aws/resource/elb/load_balancer.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         elb = self._read(aws_client)
         if elb is None:
             print_error(
                 f"Error reading {self.get_resource_type()}. Please get DNS name manually."
             )
         else:
             dns_name = elb.get("DNSName", None)
-            print_info(f"LoadBalancer DNS: {dns_name}")
+            print_info(f"LoadBalancer DNS: http://{dns_name}")
         return True
 
     def _read(self, aws_client: AwsApiClient) -> Optional[Any]:
         """Returns the LoadBalancer
 
         Args:
             aws_client: The AwsApiClient for the current LoadBalancer
```

### Comparing `phidata-1.5.5/phidata/aws/resource/elb/target_group.py` & `phidata-1.5.6/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/emr/cluster.py` & `phidata-1.5.6/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/glue/crawler.py` & `phidata-1.5.6/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/group.py` & `phidata-1.5.6/phidata/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/iam/group.py` & `phidata-1.5.6/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/iam/policy.py` & `phidata-1.5.6/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/iam/role.py` & `phidata-1.5.6/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/rds/db_cluster.py` & `phidata-1.5.6/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/rds/db_instance.py` & `phidata-1.5.6/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-1.5.6/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/s3/bucket.py` & `phidata-1.5.6/phidata/aws/resource/s3/bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 
 class S3Bucket(AwsResource):
     """
     # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#service-resource
     """
 
-    resource_type = "s3.Bucket"
-    service_name = "s3"
+    resource_type: str = "s3"
+    service_name: str = "s3"
 
     # name of bucket
     name: str
     # The canned ACL to apply to the bucket.
     acl: Optional[
         Literal["private", "public-read", "public-read-write", "authenticated-read"]
     ] = None
```

### Comparing `phidata-1.5.5/phidata/aws/resource/secret/manager.py` & `phidata-1.5.6/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/types.py` & `phidata-1.5.6/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/resource/utils.py` & `phidata-1.5.6/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/s3/csv_dataset.py` & `phidata-1.5.6/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/s3/dataset.py` & `phidata-1.5.6/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/s3/dataset_base.py` & `phidata-1.5.6/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/aws/s3/object.py` & `phidata-1.5.6/phidata/aws/s3/object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 from pathlib import Path
 from typing import Optional
 from typing_extensions import Literal
 
 from phidata.asset.local.file import LocalFile
-from phidata.asset.data_asset import DataAsset, DataAssetArgs
+from phidata.asset.aws.aws_asset import AwsAsset, AwsAssetArgs
 from phidata.aws.resource.s3.bucket import S3Bucket
 from phidata.utils.log import logger
 
 
-class S3ObjectArgs(DataAssetArgs):
+class S3ObjectArgs(AwsAssetArgs):
     key: str
     bucket: S3Bucket
+    bucket_name: Optional[str] = None
 
 
-class S3Object(DataAsset):
+class S3Object(AwsAsset):
     def __init__(
         self,
         key: str,
-        bucket: S3Bucket,
+        bucket: Optional[S3Bucket] = None,
+        bucket_name: Optional[str] = None,
         version: Optional[str] = None,
         enabled: bool = True,
     ) -> None:
         super().__init__()
         try:
+            _bucket = bucket
+            if _bucket is None and bucket_name is not None:
+                _bucket = S3Bucket(name=bucket_name)
+
+            if _bucket is None:
+                logger.error(f"Bucket for {key} unavailable")
+                return
+
             self.args: S3ObjectArgs = S3ObjectArgs(
                 key=key,
-                bucket=bucket,
+                bucket=_bucket,
+                bucket_name=bucket_name,
                 name=key,
                 version=version,
                 enabled=enabled,
             )
         except Exception as e:
             logger.error(f"Args for {self.__class__.__name__} are not valid")
             raise
```

### Comparing `phidata-1.5.5/phidata/aws/worker.py` & `phidata-1.5.6/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/base.py` & `phidata-1.5.6/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/checks/check.py` & `phidata-1.5.6/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/checks/not_empty.py` & `phidata-1.5.6/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/constants.py` & `phidata-1.5.6/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/decorators/timer.py` & `phidata-1.5.6/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/decorators/validate_env.py` & `phidata-1.5.6/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/api_client.py` & `phidata-1.5.6/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/args.py` & `phidata-1.5.6/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/config.py` & `phidata-1.5.6/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/enums.py` & `phidata-1.5.6/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/manager.py` & `phidata-1.5.6/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/resource/base.py` & `phidata-1.5.6/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/resource/container.py` & `phidata-1.5.6/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/resource/group.py` & `phidata-1.5.6/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/resource/image.py` & `phidata-1.5.6/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/resource/network.py` & `phidata-1.5.6/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/resource/types.py` & `phidata-1.5.6/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/resource/utils.py` & `phidata-1.5.6/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/resource/volume.py` & `phidata-1.5.6/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/utils/container.py` & `phidata-1.5.6/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/docker/worker.py` & `phidata-1.5.6/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/infra/args.py` & `phidata-1.5.6/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/infra/config.py` & `phidata-1.5.6/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/infra/resource.py` & `phidata-1.5.6/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/api_client.py` & `phidata-1.5.6/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/args.py` & `phidata-1.5.6/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/config.py` & `phidata-1.5.6/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.5.6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.5.6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/apps/v1/deployment.py` & `phidata-1.5.6/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/common/port.py` & `phidata-1.5.6/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/core/v1/config_map.py` & `phidata-1.5.6/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/core/v1/container.py` & `phidata-1.5.6/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/core/v1/namespace.py` & `phidata-1.5.6/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-1.5.6/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-1.5.6/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/core/v1/secret.py` & `phidata-1.5.6/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/core/v1/service.py` & `phidata-1.5.6/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/core/v1/service_account.py` & `phidata-1.5.6/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/core/v1/volume.py` & `phidata-1.5.6/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-1.5.6/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/group.py` & `phidata-1.5.6/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/kubeconfig.py` & `phidata-1.5.6/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-1.5.6/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.5.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.5.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-1.5.6/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/enums/api_version.py` & `phidata-1.5.6/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/enums/kind.py` & `phidata-1.5.6/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/enums/manager_status.py` & `phidata-1.5.6/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/enums/pv.py` & `phidata-1.5.6/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/manager.py` & `phidata-1.5.6/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.5.6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.5.6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-1.5.6/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-1.5.6/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 class DeploymentStrategy(K8sObject):
     """
     # https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.23/#deploymentstrategy-v1-apps
     """
 
     resource_type: str = "DeploymentStrategy"
 
-    rolling_update: RollingUpdateDeployment = Field(None, alias="rollingUpdate")
+    rolling_update: RollingUpdateDeployment = Field(
+        RollingUpdateDeployment(), alias="rollingUpdate"
+    )
     type: Literal["Recreate", "RollingUpdate"] = "RollingUpdate"
 
     def get_k8s_object(self) -> V1DeploymentStrategy:
         # Return a V1DeploymentStrategy object
         # https://github.com/kubernetes-client/python/blob/master/kubernetes/client/models/v1_deployment_strategy.py
         _v1_deployment_strategy = V1DeploymentStrategy(
             rolling_update=self.rolling_update.get_k8s_object(),
```

### Comparing `phidata-1.5.5/phidata/k8s/resource/base.py` & `phidata-1.5.6/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/config_map.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/container.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/namespace.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/pod.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/secret.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/service.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/service_account.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/toleration.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/volume.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-1.5.6/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/group.py` & `phidata-1.5.6/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/kubeconfig.py` & `phidata-1.5.6/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-1.5.6/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     # https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.23/#labelselector-v1-meta
     """
 
     resource_type: str = "LabelSelector"
 
     # matchLabels is a map of {key,value} pairs.
-    match_labels: Dict[str, str] = Field(None, alias="matchLabels")
+    match_labels: Optional[Dict[str, str]] = Field(None, alias="matchLabels")
 
     def get_k8s_object(self) -> V1LabelSelector:
         # Return a V1LabelSelector object
         # https://github.com/kubernetes-client/python/blob/master/kubernetes/client/models/v1_label_selector.py
         _v1_label_selector = V1LabelSelector(
             match_labels=self.match_labels,
         )
```

### Comparing `phidata-1.5.5/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-1.5.6/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-1.5.6/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.5.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.5.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-1.5.6/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/types.py` & `phidata-1.5.6/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/resource/utils.py` & `phidata-1.5.6/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/utils/pod.py` & `phidata-1.5.6/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/k8s/worker.py` & `phidata-1.5.6/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/product/data_product.py` & `phidata-1.5.6/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/table/local/csv.py` & `phidata-1.5.6/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/table/local/local_table.py` & `phidata-1.5.6/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/table/local/parquet.py` & `phidata-1.5.6/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/table/s3/csv.py` & `phidata-1.5.6/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/table/s3/parquet.py` & `phidata-1.5.6/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/table/s3/s3_table.py` & `phidata-1.5.6/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/table/sql/postgres.py` & `phidata-1.5.6/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/table/sql/sql_table.py` & `phidata-1.5.6/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/aws/athena/run_query.py` & `phidata-1.5.6/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/aws/emr/create_cluster.py` & `phidata-1.5.6/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/aws/emr/delete_cluster.py` & `phidata-1.5.6/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/aws/glue/start_crawler.py` & `phidata-1.5.6/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/decorator.py` & `phidata-1.5.6/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/download/s3/to_file.py` & `phidata-1.5.6/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/download/url/to_file.py` & `phidata-1.5.6/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/download/url/to_s3.py` & `phidata-1.5.6/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/download/url/to_sql.py` & `phidata-1.5.6/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/plot/sql/query.py` & `phidata-1.5.6/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/python_task.py` & `phidata-1.5.6/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/run/sql/query.py` & `phidata-1.5.6/phidata/task/run/sql/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         sql_table: SqlTable,
         show_sample_data: bool = False,
         load_result_to: Optional[SqlTable] = None,
         if_exists: Optional[Literal["fail", "replace", "append"]] = None,
         index: Optional[bool] = None,
         index_label: Optional[Union[str, List[str]]] = None,
         chunksize: Optional[int] = None,
-        name: str = "run_sql_query",
+        name: str = "run_duckdb_query",
         task_id: Optional[str] = None,
         dag_id: Optional[str] = None,
         version: Optional[str] = None,
         enabled: bool = True,
     ):
         super().__init__()
         try:
```

### Comparing `phidata-1.5.5/phidata/task/task.py` & `phidata-1.5.6/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/task_relatives.py` & `phidata-1.5.6/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/upload/file/to_s3.py` & `phidata-1.5.6/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/task/upload/file/to_sql.py` & `phidata-1.5.6/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/types/airflow.py` & `phidata-1.5.6/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/types/context.py` & `phidata-1.5.6/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/types/phidata_runtime.py` & `phidata-1.5.6/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/cli_console.py` & `phidata-1.5.6/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/common.py` & `phidata-1.5.6/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/compare.py` & `phidata-1.5.6/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/context.py` & `phidata-1.5.6/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/dttm.py` & `phidata-1.5.6/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/enums.py` & `phidata-1.5.6/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/env_file.py` & `phidata-1.5.6/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/env_var.py` & `phidata-1.5.6/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/filesystem.py` & `phidata-1.5.6/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/log.py` & `phidata-1.5.6/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/prep_infra_config.py` & `phidata-1.5.6/phidata/utils/prep_infra_config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/print_table.py` & `phidata-1.5.6/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/utils/workspace_path.py` & `phidata-1.5.6/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/workflow/decorator.py` & `phidata-1.5.6/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/workflow/workflow.py` & `phidata-1.5.6/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/workflow/workflow_relatives.py` & `phidata-1.5.6/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/workspace/config.py` & `phidata-1.5.6/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata/workspace/settings.py` & `phidata-1.5.6/phidata/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-1.5.5/phidata.egg-info/SOURCES.txt` & `phidata-1.5.6/phidata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,22 @@
 phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
 phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
 phidata/k8s/resource/storage_k8s_io/__init__.py
 phidata/k8s/resource/storage_k8s_io/v1/__init__.py
 phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
 phidata/k8s/utils/__init__.py
 phidata/k8s/utils/pod.py
+phidata/llm/__init__.py
+phidata/llm/duckdb/__init__.py
+phidata/llm/duckdb/agent.py
+phidata/llm/duckdb/chain.py
+phidata/llm/duckdb/connection.py
+phidata/llm/duckdb/loader.py
+phidata/llm/duckdb/query.py
+phidata/llm/duckdb/tool.py
 phidata/product/__init__.py
 phidata/product/data_product.py
 phidata/table/__init__.py
 phidata/table/local/__init__.py
 phidata/table/local/csv.py
 phidata/table/local/local_table.py
 phidata/table/local/parquet.py
```

### Comparing `phidata-1.5.5/pyproject.toml` & `phidata-1.5.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phidata"
-version = "1.5.5"
+version = "1.5.6"
 description = "Building blocks for Data Engineering"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
@@ -31,14 +31,17 @@
 documentation = "https://www.docs.phidata.com"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.mypy]
+plugins = [
+  "pydantic.mypy"
+]
 check_untyped_defs = true
 no_implicit_optional = true
 warn_unused_configs = true
 exclude = [
   "phidata/asset/dev", # exclude dev assets from mypy
   "phidata/workflow/dev", # exclude dev workflows from mypy
   "phidata/product/dev", # exclude dev products from mypy
```

