# Comparing `tmp/apache-airflow-providers-amazon-7.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-amazon-7.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-amazon-7.4.0rc1.tar", last modified: Sun Apr  2 05:46:51 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-amazon-7.4.1rc1.tar", last modified: Sun Apr  9 13:48:06 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-7.4.0rc1.tar` & `apache-airflow-providers-amazon-7.4.1rc1.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-7.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1237 2023-04-02 05:46:46.000000 apache-airflow-providers-amazon-7.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-7.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    52692 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    50871 2023-04-02 05:46:46.000000 apache-airflow-providers-amazon-7.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:50.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:50.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:50.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:50.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:50.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12935 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    44515 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    19189 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)     9644 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7641 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    22191 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    13816 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     6281 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13561 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    42450 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    57278 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:50.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:50.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     6826 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)     1217 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/aws_lambda.py
--rw-r--r--   0 root         (0) root         (0)    13603 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    30225 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    31781 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    46887 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     8343 2023-02-24 21:43:25.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    29868 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    28216 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8052 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    49835 2023-03-01 07:06:45.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16132 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     9198 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    18537 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2768 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     5857 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8639 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5036 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9198 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4569 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6185 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3499 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3666 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     7690 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20348 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/waiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)     1378 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)    36763 2023-04-02 05:46:46.000000 apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    52692 2023-04-02 05:46:49.000000 apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7266 2023-04-02 05:46:49.000000 apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:46:49.000000 apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-02 05:46:49.000000 apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:46:49.000000 apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      777 2023-04-02 05:46:49.000000 apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:46:49.000000 apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-amazon-7.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-04-02 05:46:51.000000 apache-airflow-providers-amazon-7.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2182 2023-04-02 05:46:46.000000 apache-airflow-providers-amazon-7.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:06.000000 apache-airflow-providers-amazon-7.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-7.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-04-09 13:48:01.000000 apache-airflow-providers-amazon-7.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-7.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    53299 2023-04-09 13:48:06.000000 apache-airflow-providers-amazon-7.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    51478 2023-04-09 13:48:01.000000 apache-airflow-providers-amazon-7.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12935 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    44515 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    19189 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)     9644 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7641 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    22191 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    13816 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13561 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    42450 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    57278 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     6826 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)     1217 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/aws_lambda.py
+-rw-r--r--   0 root         (0) root         (0)    13603 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    30225 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    31781 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    46887 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     8343 2023-02-24 21:43:25.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    29868 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    28218 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8052 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    49835 2023-03-01 07:06:45.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16132 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9198 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    18537 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     5857 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8639 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     5036 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9198 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4569 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6185 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     7690 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20348 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/waiter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:05.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)    36812 2023-04-09 13:48:01.000000 apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:06.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    53299 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7266 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      777 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 13:48:04.000000 apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-amazon-7.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-04-09 13:48:06.000000 apache-airflow-providers-amazon-7.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-04-09 13:48:00.000000 apache-airflow-providers-amazon-7.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/LICENSE` & `apache-airflow-providers-amazon-7.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/MANIFEST.in` & `apache-airflow-providers-amazon-7.4.1rc1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -26,10 +26,9 @@
 
 include airflow/providers/amazon/aws/hooks/batch_waiters.json
 include airflow/providers/amazon/aws/waiters/*.json
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.txt
-include README.md
+include CHANGELOG.rst
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/PKG-INFO` & `apache-airflow-providers-amazon-7.4.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 7.4.0rc1
+Version: 7.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -60,28 +60,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``7.4.0rc1``
+Release: ``7.4.1rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -158,14 +158,36 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.4.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix 'RedshiftResumeClusterOperator' deferrable implementation (#30370)``
+
+Misc
+~~~~
+
+* ``Add more info to quicksight error messages (#30466)``
+* ``add template field for s3 bucket (#30472)``
+* ``Add s3_bucket to template fields in SFTP to S3 operator (#30444)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add AWS deferrable BatchOperator (#29300)``
+   * ``Revert "Add AWS deferrable BatchOperator (#29300)" (#30489)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 7.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add deferrable mode to 'RedshiftResumeClusterOperator' (#30090)``
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/README.rst` & `apache-airflow-providers-amazon-7.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``7.4.0rc1``
+Release: ``7.4.1rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -113,14 +113,36 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.4.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix 'RedshiftResumeClusterOperator' deferrable implementation (#30370)``
+
+Misc
+~~~~
+
+* ``Add more info to quicksight error messages (#30466)``
+* ``add template field for s3 bucket (#30472)``
+* ``Add s3_bucket to template fields in SFTP to S3 operator (#30444)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add AWS deferrable BatchOperator (#29300)``
+   * ``Revert "Add AWS deferrable BatchOperator (#29300)" (#30489)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 7.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add deferrable mode to 'RedshiftResumeClusterOperator' (#30090)``
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,18 +109,34 @@
         :return: An QuickSight Ingestion Status
         """
         try:
             describe_ingestion_response = self.get_conn().describe_ingestion(
                 AwsAccountId=aws_account_id, DataSetId=data_set_id, IngestionId=ingestion_id
             )
             return describe_ingestion_response["Ingestion"]["IngestionStatus"]
-        except KeyError:
-            raise AirflowException("Could not get status of the Amazon QuickSight Ingestion")
-        except ClientError:
-            raise AirflowException("AWS request failed, check logs for more info")
+        except KeyError as e:
+            raise AirflowException(f"Could not get status of the Amazon QuickSight Ingestion: {e}")
+        except ClientError as e:
+            raise AirflowException(f"AWS request failed: {e}")
+
+    def get_error_info(self, aws_account_id: str, data_set_id: str, ingestion_id: str) -> dict | None:
+        """
+        Gets info about the error if any.
+
+        :param aws_account_id: An AWS Account ID
+        :param data_set_id: QuickSight Data Set ID
+        :param ingestion_id: QuickSight Ingestion ID
+        :return: Error info dict containing the error type (key 'Type') and message (key 'Message')
+            if available. Else, returns None.
+        """
+        describe_ingestion_response = self.get_conn().describe_ingestion(
+            AwsAccountId=aws_account_id, DataSetId=data_set_id, IngestionId=ingestion_id
+        )
+        # using .get() to get None if the key is not present, instead of an exception.
+        return describe_ingestion_response["Ingestion"].get("ErrorInfo")
 
     def wait_for_state(
         self,
         aws_account_id: str,
         data_set_id: str,
         ingestion_id: str,
         target_state: set,
@@ -137,17 +153,19 @@
             will check the status of QuickSight Ingestion
         :return: response of describe_ingestion call after Ingestion is is done
         """
         sec = 0
         status = self.get_status(aws_account_id, data_set_id, ingestion_id)
         while status in self.NON_TERMINAL_STATES and status != target_state:
             self.log.info("Current status is %s", status)
-            time.sleep(check_interval)
-            sec += check_interval
             if status in self.FAILED_STATES:
-                raise AirflowException("The Amazon QuickSight Ingestion failed!")
+                info = self.get_error_info(aws_account_id, data_set_id, ingestion_id)
+                raise AirflowException(f"The Amazon QuickSight Ingestion failed. Error info: {info}")
             if status == "CANCELLED":
                 raise AirflowException("The Amazon QuickSight SPICE ingestion cancelled!")
+            # wait and try again
+            time.sleep(check_interval)
+            sec += check_interval
             status = self.get_status(aws_account_id, data_set_id, ingestion_id)
 
         self.log.info("QuickSight Ingestion completed")
         return status
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/aws_lambda.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
                 timeout=self.execution_timeout,
                 trigger=RedshiftClusterTrigger(
                     task_id=self.task_id,
                     poll_interval=self.poll_interval,
                     aws_conn_id=self.aws_conn_id,
                     cluster_identifier=self.cluster_identifier,
                     attempts=self._attempts,
-                    operation_type="pause_cluster",
+                    operation_type="resume_cluster",
                 ),
                 method_name="execute_complete",
             )
         else:
             while self._attempts >= 1:
                 try:
                     redshift_hook.get_conn().resume_cluster(ClusterIdentifier=self.cluster_identifier)
@@ -466,15 +466,15 @@
         """
         if event:
             if "status" in event and event["status"] == "error":
                 msg = f"{event['status']}: {event['message']}"
                 raise AirflowException(msg)
             elif "status" in event and event["status"] == "success":
                 self.log.info("%s completed successfully.", self.task_id)
-                self.log.info("Paused cluster successfully")
+                self.log.info("Resumed cluster successfully")
         else:
             raise AirflowException("No event received from trigger")
 
 
 class RedshiftPauseClusterOperator(BaseOperator):
     """
     Pause an AWS Redshift Cluster if it has status `available`.
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/redshift_sql.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,16 @@
         self.log.info("Poking for Amazon QuickSight Ingestion ID: %s", self.ingestion_id)
         aws_account_id = self.sts_hook.get_account_number()
         quicksight_ingestion_state = self.quicksight_hook.get_status(
             aws_account_id, self.data_set_id, self.ingestion_id
         )
         self.log.info("QuickSight Status: %s", quicksight_ingestion_state)
         if quicksight_ingestion_state in self.errored_statuses:
-            raise AirflowException("The QuickSight Ingestion failed!")
+            error = self.quicksight_hook.get_error_info(aws_account_id, self.data_set_id, self.ingestion_id)
+            raise AirflowException(f"The QuickSight Ingestion failed. Error info: {error}")
         return quicksight_ingestion_state == self.success_status
 
     @cached_property
     def quicksight_hook(self):
         return QuickSightHook(aws_conn_id=self.aws_conn_id)
 
     @cached_property
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     :param aws_conn_id: aws connection to use
     :param s3_bucket: The targeted s3 bucket. This is the S3 bucket from
         where the file is downloaded.
     :param s3_key: The targeted s3 key. This is the specified file path for
         downloading the file from S3.
     """
 
-    template_fields: Sequence[str] = ("s3_key", "sftp_path")
+    template_fields: Sequence[str] = ("s3_key", "sftp_path", "s3_bucket")
 
     def __init__(
         self,
         *,
         s3_bucket: str,
         s3_key: str,
         sftp_path: str,
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         the file is uploaded.
     :param s3_key: The targeted s3 key. This is the specified path for
         uploading the file to S3.
     :param use_temp_file: If True, copies file first to local,
         if False streams file from SFTP to S3.
     """
 
-    template_fields: Sequence[str] = ("s3_key", "sftp_path")
+    template_fields: Sequence[str] = ("s3_key", "sftp_path", "s3_bucket")
 
     def __init__(
         self,
         *,
         s3_bucket: str,
         s3_key: str,
         sftp_path: str,
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,12 +66,22 @@
                         poll_interval=self.poll_interval,
                     )
                     if response.get("status") == "success":
                         yield TriggerEvent(response)
                     else:
                         if self.attempts < 1:
                             yield TriggerEvent({"status": "error", "message": f"{self.task_id} failed"})
+                elif self.operation_type == "resume_cluster":
+                    response = await hook.resume_cluster(
+                        cluster_identifier=self.cluster_identifier,
+                        polling_period_seconds=self.poll_interval,
+                    )
+                    if response:
+                        yield TriggerEvent(response)
+                    else:
+                        error_message = f"{self.task_id} failed"
+                        yield TriggerEvent({"status": "error", "message": error_message})
                 else:
                     yield TriggerEvent(f"{self.operation_type} is not supported")
             except Exception as e:
                 if self.attempts < 1:
                     yield TriggerEvent({"status": "error", "message": str(e)})
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-7.4.1rc1/airflow/providers/amazon/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-amazon",
         "name": "Amazon",
         "description": "Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).\n",
+        "suspended": False,
         "versions": [
+            "7.4.1",
             "7.4.0",
             "7.3.0",
             "7.2.1",
             "7.2.0",
             "7.1.0",
             "7.0.0",
             "6.2.0",
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 7.4.0rc1
+Version: 7.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -60,28 +60,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``7.4.0rc1``
+Release: ``7.4.1rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -158,14 +158,36 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.4.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix 'RedshiftResumeClusterOperator' deferrable implementation (#30370)``
+
+Misc
+~~~~
+
+* ``Add more info to quicksight error messages (#30466)``
+* ``add template field for s3 bucket (#30472)``
+* ``Add s3_bucket to template fields in SFTP to S3 operator (#30444)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add AWS deferrable BatchOperator (#29300)``
+   * ``Revert "Add AWS deferrable BatchOperator (#29300)" (#30489)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 7.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add deferrable mode to 'RedshiftResumeClusterOperator' (#30090)``
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-7.4.1rc1/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/pyproject.toml` & `apache-airflow-providers-amazon-7.4.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/setup.cfg` & `apache-airflow-providers-amazon-7.4.1rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/7.4.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-amazon-7.4.0rc1/setup.py` & `apache-airflow-providers-amazon-7.4.1rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-amazon package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "7.4.0"
+version = "7.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-amazon setup."""
     setup(
         version=version,
         extras_require={
@@ -43,13 +43,20 @@
             "imap": ["apache-airflow-providers-imap"],
             "mongo": ["apache-airflow-providers-mongo"],
             "salesforce": ["apache-airflow-providers-salesforce"],
             "ssh": ["apache-airflow-providers-ssh"],
             "pandas": ["pandas>=0.17.1"],
             "aiobotocore": ["aiobotocore>=2.1.1"],
         },
-        packages=find_namespace_packages(include=["airflow.providers.amazon", "airflow.providers.amazon.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.amazon",
+                "airflow.providers.amazon.*",
+                "airflow.providers.amazon_vendor",
+                "airflow.providers.amazon_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

