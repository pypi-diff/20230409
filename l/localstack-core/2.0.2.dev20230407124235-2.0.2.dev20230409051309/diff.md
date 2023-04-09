# Comparing `tmp/localstack-core-2.0.2.dev20230407124235.tar.gz` & `tmp/localstack-core-2.0.2.dev20230409051309.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.0.2.dev20230407124235.tar", last modified: Fri Apr  7 12:42:41 2023, max compression
+gzip compressed data, was "localstack-core-2.0.2.dev20230409051309.tar", last modified: Sun Apr  9 05:13:17 2023, max compression
```

## Comparing `localstack-core-2.0.2.dev20230407124235.tar` & `localstack-core-2.0.2.dev20230409051309.tar`

### file list

```diff
@@ -1,835 +1,835 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.976184 localstack-core-2.0.2.dev20230407124235/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-04-07 12:42:41.976184 localstack-core-2.0.2.dev20230407124235/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10815 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-04-07 12:42:35.000000 localstack-core-2.0.2.dev20230407124235/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1890 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    84791 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42769 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   122319 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6035 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.888183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   754298 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55273 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47848 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69896 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35937 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    64389 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   132500 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16662 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14068 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59496 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.892183 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22571 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8786 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.896183 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2075 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6856 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11919 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.896183 localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14226 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49876 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73217 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.896183 localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2211 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7804 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27186 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.896183 localstack-core-2.0.2.dev20230407124235/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18064 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50298 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8214 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.896183 localstack-core-2.0.2.dev20230407124235/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15553 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/contrib/thundra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11624 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.896183 localstack-core-2.0.2.dev20230407124235/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.900183 localstack-core-2.0.2.dev20230407124235/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.900183 localstack-core-2.0.2.dev20230407124235/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2881 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14172 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3524 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5033 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17128 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.900183 localstack-core-2.0.2.dev20230407124235/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.900183 localstack-core-2.0.2.dev20230407124235/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.900183 localstack-core-2.0.2.dev20230407124235/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.900183 localstack-core-2.0.2.dev20230407124235/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.904183 localstack-core-2.0.2.dev20230407124235/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3767 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.904183 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41169 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34409 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12745 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12099 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67662 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.904183 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23585 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.904183 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8672 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.904183 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17805 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4788 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21171 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27269 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12309 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32703 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91859 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72195 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17169 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.908183 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1489 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   152684 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7722 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/urlrouter.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.908183 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1699 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6328 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.908183 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17143 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60765 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8781 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2288 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30425 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20593 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4204 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1916 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5112 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22228 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2270 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2769 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8661 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27162 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3019 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5197 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1382 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10505 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6593 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2650 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5194 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34242 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6479 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2940 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3949 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73346 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6055 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7804 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4406 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21682 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32205 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19028 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/iam/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16218 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11820 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.912183 localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6965 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.916183 localstack-core-2.0.2.dev20230407124235/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34733 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      797 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    46594 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      250 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.916183 localstack-core-2.0.2.dev20230407124235/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.916183 localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24137 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9437 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.916183 localstack-core-2.0.2.dev20230407124235/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.916183 localstack-core-2.0.2.dev20230407124235/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.916183 localstack-core-2.0.2.dev20230407124235/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.916183 localstack-core-2.0.2.dev20230407124235/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2651 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.916183 localstack-core-2.0.2.dev20230407124235/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33392 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12621 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2979 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23108 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60971 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68236 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8940 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5276 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15447 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28951 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21143 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5644 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45694 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    56107 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1666 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24311 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    53186 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6936 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6879 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.920183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.924183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.924183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1292 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2367 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.924183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2270 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.924183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.924183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      658 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.924183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.928183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.928183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.928183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.928183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.928183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.928183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.932183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.936183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.936183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.936183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.936183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.936183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.936183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.944183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.944183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.944183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.944183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.944183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.944183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.944183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3243 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.944183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5976 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.944183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.944183 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.952184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      816 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.952184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.952184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4967 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.952184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.952184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.952184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.952184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3281 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3618 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1161 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1006 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2421 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.952184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.956184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1348 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.956184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.956184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.960184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.960184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4647 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      250 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31024 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6407 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2551 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10302 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4338 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      609 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/transcribe/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/transcribe/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12180 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.964184 localstack-core-2.0.2.dev20230407124235/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.968184 localstack-core-2.0.2.dev20230407124235/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6391 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.968184 localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67790 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4559 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.968184 localstack-core-2.0.2.dev20230407124235/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24927 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.972184 localstack-core-2.0.2.dev20230407124235/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.972184 localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2985 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.976184 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13418 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12903 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11597 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23889 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.976184 localstack-core-2.0.2.dev20230407124235/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4407 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.976184 localstack-core-2.0.2.dev20230407124235/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43017 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28581 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29580 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6852 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4619 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.976184 localstack-core-2.0.2.dev20230407124235/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10057 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.976184 localstack-core-2.0.2.dev20230407124235/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5640 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23504 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-07 12:42:41.976184 localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-04-07 12:42:41.000000 localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36736 2023-04-07 12:42:41.000000 localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-07 12:42:41.000000 localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4968 2023-04-07 12:42:41.000000 localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-07 12:42:38.000000 localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5055 2023-04-07 12:42:38.000000 localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2757 2023-04-07 12:42:41.000000 localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-04-07 12:42:41.000000 localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3116 2023-04-07 12:42:41.976184 localstack-core-2.0.2.dev20230407124235/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-04-07 12:12:49.000000 localstack-core-2.0.2.dev20230407124235/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.433614 localstack-core-2.0.2.dev20230409051309/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-04-09 05:13:17.433614 localstack-core-2.0.2.dev20230409051309/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10815 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.301615 localstack-core-2.0.2.dev20230409051309/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-04-09 05:13:09.000000 localstack-core-2.0.2.dev20230409051309/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1890 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    84791 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42769 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   122319 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6035 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.305615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   754298 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55273 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47848 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69896 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35937 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    64389 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   132500 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16662 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14068 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59496 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.309615 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22571 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8786 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.313615 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2075 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6856 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11919 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.313615 localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14226 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49876 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73217 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.313615 localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2211 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7804 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27186 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.313615 localstack-core-2.0.2.dev20230409051309/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18064 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50298 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8214 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.313615 localstack-core-2.0.2.dev20230409051309/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15553 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/contrib/thundra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11624 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.313615 localstack-core-2.0.2.dev20230409051309/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.317615 localstack-core-2.0.2.dev20230409051309/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.317615 localstack-core-2.0.2.dev20230409051309/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2881 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14172 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3524 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5033 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17128 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.317615 localstack-core-2.0.2.dev20230409051309/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.317615 localstack-core-2.0.2.dev20230409051309/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.317615 localstack-core-2.0.2.dev20230409051309/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.317615 localstack-core-2.0.2.dev20230409051309/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.317615 localstack-core-2.0.2.dev20230409051309/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3767 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.321615 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41169 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34409 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12745 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12099 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67662 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.321615 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23585 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.321615 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8672 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.325615 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17805 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4788 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21171 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27269 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12309 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32703 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91859 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72195 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17169 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.325615 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1489 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   152684 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7722 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/urlrouter.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.325615 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1699 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6328 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.325615 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17143 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60765 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8781 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2288 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.329615 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30425 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20593 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4204 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1916 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5112 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22228 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2270 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2769 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8661 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27162 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3019 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5197 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1382 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10505 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6593 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2650 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5194 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34242 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6479 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2940 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.329615 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.329615 localstack-core-2.0.2.dev20230409051309/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.329615 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3949 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73346 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6055 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7804 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.329615 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4406 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.329615 localstack-core-2.0.2.dev20230409051309/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.329615 localstack-core-2.0.2.dev20230409051309/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.329615 localstack-core-2.0.2.dev20230409051309/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21682 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.329615 localstack-core-2.0.2.dev20230409051309/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32205 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.329615 localstack-core-2.0.2.dev20230409051309/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19028 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/iam/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16218 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11820 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.333615 localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6965 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.333615 localstack-core-2.0.2.dev20230409051309/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34733 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      797 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    46594 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      250 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.333615 localstack-core-2.0.2.dev20230409051309/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.333615 localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24137 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9437 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.333615 localstack-core-2.0.2.dev20230409051309/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.333615 localstack-core-2.0.2.dev20230409051309/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.333615 localstack-core-2.0.2.dev20230409051309/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.333615 localstack-core-2.0.2.dev20230409051309/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2651 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.333615 localstack-core-2.0.2.dev20230409051309/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33392 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.337615 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12621 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2979 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23108 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60971 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68236 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8940 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5276 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15447 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.337615 localstack-core-2.0.2.dev20230409051309/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.337615 localstack-core-2.0.2.dev20230409051309/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28951 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.337615 localstack-core-2.0.2.dev20230409051309/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21143 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.337615 localstack-core-2.0.2.dev20230409051309/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5644 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45694 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    56107 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.337615 localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1666 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24311 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    53186 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6936 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6879 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.337615 localstack-core-2.0.2.dev20230409051309/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.337615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.337615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.337615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1292 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2367 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2270 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      658 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.341615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.345615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.345615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.345615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.345615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.345615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.345615 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.349614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.349614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.349614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.349614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.353614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.353614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.353614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.353614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.353614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.353614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3243 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.353614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5976 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.353614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.357614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.357614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      816 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.361614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.361614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4967 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.361614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.361614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.361614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.361614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3281 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3618 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1161 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1006 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2421 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.361614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.361614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1348 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.361614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.361614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.369614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.369614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.369614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4647 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.369614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.369614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      250 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.369614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.369614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31024 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.369614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.369614 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6407 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2551 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10302 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4338 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.373614 localstack-core-2.0.2.dev20230409051309/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      609 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.373614 localstack-core-2.0.2.dev20230409051309/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.373614 localstack-core-2.0.2.dev20230409051309/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.373614 localstack-core-2.0.2.dev20230409051309/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/transcribe/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/transcribe/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12180 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.373614 localstack-core-2.0.2.dev20230409051309/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.373614 localstack-core-2.0.2.dev20230409051309/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.373614 localstack-core-2.0.2.dev20230409051309/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6391 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.425614 localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65214 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4559 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.425614 localstack-core-2.0.2.dev20230409051309/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24927 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.429614 localstack-core-2.0.2.dev20230409051309/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.433614 localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2985 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.433614 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13418 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12903 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11597 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23889 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.433614 localstack-core-2.0.2.dev20230409051309/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4407 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.433614 localstack-core-2.0.2.dev20230409051309/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43017 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28581 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29580 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6852 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4619 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.433614 localstack-core-2.0.2.dev20230409051309/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10057 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.433614 localstack-core-2.0.2.dev20230409051309/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5640 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23504 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-09 05:13:17.433614 localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-04-09 05:13:17.000000 localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36736 2023-04-09 05:13:17.000000 localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-09 05:13:17.000000 localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4968 2023-04-09 05:13:17.000000 localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-09 05:13:13.000000 localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5055 2023-04-09 05:13:13.000000 localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2757 2023-04-09 05:13:17.000000 localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-04-09 05:13:17.000000 localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3116 2023-04-09 05:13:17.437614 localstack-core-2.0.2.dev20230409051309/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-04-09 04:42:53.000000 localstack-core-2.0.2.dev20230409051309/setup.py
```

### Comparing `localstack-core-2.0.2.dev20230407124235/LICENSE.txt` & `localstack-core-2.0.2.dev20230409051309/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/Makefile` & `localstack-core-2.0.2.dev20230409051309/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/README.md` & `localstack-core-2.0.2.dev20230409051309/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/bin/localstack` & `localstack-core-2.0.2.dev20230409051309/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/bin/localstack-supervisor` & `localstack-core-2.0.2.dev20230409051309/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/accounts.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/acm/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/config/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/core.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/es/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/events/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/iam/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/kms/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/logs/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/route53/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/s3/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/ses/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/sns/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/sts/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/support/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/swf/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/app.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/chain.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/client.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/connect.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/forwarder.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/gateway.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/analytics.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/auth.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/codec.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/cors.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/fallback.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/internal.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/legacy.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/logging.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/proxy.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/region.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/routes.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/service.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/mocking.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/op_router.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/parser.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/serializer.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/service_router.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/protocol/validate.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/proxy.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/scaffold.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/asgi.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/edge.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/hypercorn.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/werkzeug.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/serving/wsgi.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/skeleton.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/spec-patches.json` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/spec.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/aws/trace.py` & `localstack-core-2.0.2.dev20230409051309/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/cli/localstack.py` & `localstack-core-2.0.2.dev20230409051309/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/cli/lpm.py` & `localstack-core-2.0.2.dev20230409051309/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/cli/plugin.py` & `localstack-core-2.0.2.dev20230409051309/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/cli/plugins.py` & `localstack-core-2.0.2.dev20230409051309/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/cli/profiles.py` & `localstack-core-2.0.2.dev20230409051309/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/config.py` & `localstack-core-2.0.2.dev20230409051309/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/constants.py` & `localstack-core-2.0.2.dev20230409051309/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/contrib/thundra.py` & `localstack-core-2.0.2.dev20230409051309/localstack/contrib/thundra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/deprecations.py` & `localstack-core-2.0.2.dev20230409051309/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/extensions/api/aws.py` & `localstack-core-2.0.2.dev20230409051309/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/extensions/api/extension.py` & `localstack-core-2.0.2.dev20230409051309/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/http/adapters.py` & `localstack-core-2.0.2.dev20230409051309/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/http/asgi.py` & `localstack-core-2.0.2.dev20230409051309/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/http/client.py` & `localstack-core-2.0.2.dev20230409051309/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/http/dispatcher.py` & `localstack-core-2.0.2.dev20230409051309/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/http/hypercorn.py` & `localstack-core-2.0.2.dev20230409051309/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/http/proxy.py` & `localstack-core-2.0.2.dev20230409051309/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/http/request.py` & `localstack-core-2.0.2.dev20230409051309/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/http/resource.py` & `localstack-core-2.0.2.dev20230409051309/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/http/response.py` & `localstack-core-2.0.2.dev20230409051309/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/http/router.py` & `localstack-core-2.0.2.dev20230409051309/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/logging/format.py` & `localstack-core-2.0.2.dev20230409051309/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/logging/setup.py` & `localstack-core-2.0.2.dev20230409051309/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/packages/__init__.py` & `localstack-core-2.0.2.dev20230409051309/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/packages/api.py` & `localstack-core-2.0.2.dev20230409051309/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/packages/core.py` & `localstack-core-2.0.2.dev20230409051309/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/packages/debugpy.py` & `localstack-core-2.0.2.dev20230409051309/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/packages/terraform.py` & `localstack-core-2.0.2.dev20230409051309/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/plugins.py` & `localstack-core-2.0.2.dev20230409051309/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/runtime/analytics.py` & `localstack-core-2.0.2.dev20230409051309/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/runtime/hooks.py` & `localstack-core-2.0.2.dev20230409051309/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/runtime/init.py` & `localstack-core-2.0.2.dev20230409051309/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/runtime/main.py` & `localstack-core-2.0.2.dev20230409051309/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/runtime/shutdown.py` & `localstack-core-2.0.2.dev20230409051309/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/acm/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/context.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/helpers.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/integration.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/invocations.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/patches.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/router_asf.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/apigateway/templates.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/api_utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/hooks.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/packages.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/plugins.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/events.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/packages.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/service_models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudformation/stores.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/cloudwatch/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/packages.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/server.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodb/utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/ec2/exceptions.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/ec2/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/ec2/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/edge.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/es/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/events/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/events/scheduler.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/firehose/mappers.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/firehose/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/firehose/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/generic_proxy.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/iam/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/infra.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/internal.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/packages.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/kinesis/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/kms/local_kms_server.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/kms/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/kms/packages.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/kms/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/logs/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/logs/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/messages.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/moto.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/motoserver.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/cluster.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/packages.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/opensearch/versions.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/plugins.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/providers.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/redshift/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/route53/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/route53resolver/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/route53resolver/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/route53resolver/utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/constants.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/cors.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/multipart_content.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/notifications.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/presigned_url.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/s3_listener.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/s3_starter.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/s3_utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/virtual_host.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/s3/website_hosting.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/secretsmanager/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/ses/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sns/constants.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sns/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sns/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sns/publisher.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/constants.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/exceptions.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/query_api.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sqs/utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/ssm/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/resource.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_aws_sdk.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_lambda.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/packages.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/stores.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/sts/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/transcribe/packages.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/transcribe/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/services/transcribe/provider.py` & `localstack-core-2.0.2.dev20230409051309/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/state/core.py` & `localstack-core-2.0.2.dev20230409051309/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/state/inspect.py` & `localstack-core-2.0.2.dev20230409051309/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/state/pickle.py` & `localstack-core-2.0.2.dev20230409051309/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/state/snapshot.py` & `localstack-core-2.0.2.dev20230409051309/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/aws/util.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/filters.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/fixtures.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,53 +135,20 @@
                 endpoint_url = config.get_edge_url()
 
         return SigningHttpClient(signer_factory(creds, service, region), endpoint_url=endpoint_url)
 
     return factory
 
 
-# TODO: remove all these
-
-
-@pytest.fixture(scope="class")
-def dynamodb_client(aws_client):
-    return aws_client.dynamodb
-
-
 @pytest.fixture(scope="class")
 def dynamodb_resource():
     return _resource("dynamodb")
 
 
 @pytest.fixture(scope="class")
-def dynamodbstreams_client(aws_client):
-    return aws_client.dynamodbstreams
-
-
-@pytest.fixture(scope="class")
-def apigateway_client(aws_client):
-    return aws_client.apigateway
-
-
-@pytest.fixture(scope="class")
-def cognito_idp_client(aws_client):
-    return aws_client.cognito_idp
-
-
-@pytest.fixture(scope="class")
-def iam_client(aws_client):
-    return aws_client.iam
-
-
-@pytest.fixture(scope="class")
-def s3_client(aws_client):
-    return aws_client.s3
-
-
-@pytest.fixture(scope="class")
 def s3_vhost_client(aws_client_factory):
     return aws_client_factory(config=botocore.config.Config(s3={"addressing_style": "virtual"})).s3
 
 
 # TODO: remove
 @pytest.fixture(scope="class")
 def s3_presigned_client(aws_client_factory):
@@ -191,194 +158,59 @@
 
 
 @pytest.fixture(scope="class")
 def s3_resource():
     return _resource("s3")
 
 
-@pytest.fixture(scope="class")
-def s3control_client(aws_client):
-    return aws_client.s3control
-
-
-@pytest.fixture(scope="class")
-def sqs_client(aws_client):
-    return aws_client.sqs
-
-
-@pytest.fixture(scope="class")
-def sns_client(aws_client):
-    return aws_client.sns
-
-
-@pytest.fixture(scope="class")
-def cfn_client(aws_client):
-    return aws_client.cloudformation
-
-
-@pytest.fixture(scope="class")
-def ssm_client(aws_client):
-    return aws_client.ssm
-
-
-@pytest.fixture(scope="class")
-def lambda_client(aws_client):
-    return aws_client.awslambda
-
-
-@pytest.fixture(scope="class")
-def kinesis_client(aws_client):
-    return aws_client.kinesis
-
-
-@pytest.fixture(scope="class")
-def kms_client(aws_client):
-    return aws_client.kms
-
-
-@pytest.fixture(scope="class")
-def logs_client(aws_client):
-    return aws_client.logs
-
-
-@pytest.fixture(scope="class")
-def events_client(aws_client):
-    return aws_client.events
-
-
-@pytest.fixture(scope="class")
-def secretsmanager_client(aws_client):
-    return aws_client.secretsmanager
-
-
-@pytest.fixture(scope="class")
-def stepfunctions_client(aws_client):
-    return aws_client.stepfunctions
-
-
-@pytest.fixture(scope="class")
-def ses_client(aws_client):
-    return aws_client.ses
-
-
-@pytest.fixture(scope="class")
-def acm_client(aws_client):
-    return aws_client.acm
-
-
-@pytest.fixture(scope="class")
-def es_client(aws_client):
-    return aws_client.es
-
-
-@pytest.fixture(scope="class")
-def opensearch_client(aws_client):
-    return aws_client.opensearch
-
-
-@pytest.fixture(scope="class")
-def redshift_client(aws_client):
-    return aws_client.redshift
-
-
-@pytest.fixture(scope="class")
-def firehose_client(aws_client):
-    return aws_client.firehose
-
-
-@pytest.fixture(scope="class")
-def cloudwatch_client(aws_client):
-    return aws_client.cloudwatch
-
-
-@pytest.fixture(scope="class")
-def sts_client(aws_client):
-    return aws_client.sts
-
-
-@pytest.fixture(scope="class")
-def ec2_client(aws_client):
-    return aws_client.ec2
-
-
-@pytest.fixture(scope="class")
-def rg_client(aws_client):
-    return aws_client.resource_groups
-
-
-@pytest.fixture(scope="class")
-def rgsa_client(aws_client):
-    return aws_client.resourcegroupstaggingapi
-
-
-@pytest.fixture(scope="class")
-def route53_client(aws_client):
-    return aws_client.route53
-
-
-@pytest.fixture(scope="class")
-def route53resolver_client(aws_client):
-    return aws_client.route53resolver
-
-
-@pytest.fixture(scope="class")
-def transcribe_client(aws_client):
-    return aws_client.transcribe
-
-
-@pytest.fixture(scope="class")
-def ecr_client(aws_client):
-    return aws_client.ecr
-
-
 @pytest.fixture
-def dynamodb_wait_for_table_active(dynamodb_client):
+def dynamodb_wait_for_table_active(aws_client):
     def wait_for_table_active(table_name: str, client=None):
         def wait():
-            return (client or dynamodb_client).describe_table(TableName=table_name)["Table"][
+            return (client or aws_client.dynamodb).describe_table(TableName=table_name)["Table"][
                 "TableStatus"
             ] == "ACTIVE"
 
         poll_condition(wait, timeout=30)
 
     return wait_for_table_active
 
 
 @pytest.fixture
-def dynamodb_create_table_with_parameters(dynamodb_client, dynamodb_wait_for_table_active):
+def dynamodb_create_table_with_parameters(dynamodb_wait_for_table_active, aws_client):
     tables = []
 
     def factory(**kwargs):
         if "TableName" not in kwargs:
             kwargs["TableName"] = f"test-table-{short_uid()}"
 
         tables.append(kwargs["TableName"])
-        response = dynamodb_client.create_table(**kwargs)
+        response = aws_client.dynamodb.create_table(**kwargs)
         dynamodb_wait_for_table_active(kwargs["TableName"])
         return response
 
     yield factory
 
     # cleanup
     for table in tables:
         try:
             # table has to be in ACTIVE state before deletion
             dynamodb_wait_for_table_active(table)
-            dynamodb_client.delete_table(TableName=table)
+            aws_client.dynamodb.delete_table(TableName=table)
         except Exception as e:
             LOG.debug("error cleaning up table %s: %s", table, e)
 
 
 @pytest.fixture
-def dynamodb_create_table(dynamodb_client, dynamodb_wait_for_table_active):
+def dynamodb_create_table(dynamodb_wait_for_table_active, aws_client):
     # beware, this swallows exception in create_dynamodb_table utility function
     tables = []
 
     def factory(**kwargs):
-        kwargs["client"] = dynamodb_client
+        kwargs["client"] = aws_client.dynamodb
         if "table_name" not in kwargs:
             kwargs["table_name"] = f"test-table-{short_uid()}"
         if "partition_key" not in kwargs:
             kwargs["partition_key"] = "id"
 
         tables.append(kwargs["table_name"])
 
@@ -387,28 +219,28 @@
     yield factory
 
     # cleanup
     for table in tables:
         try:
             # table has to be in ACTIVE state before deletion
             dynamodb_wait_for_table_active(table)
-            dynamodb_client.delete_table(TableName=table)
+            aws_client.dynamodb.delete_table(TableName=table)
         except Exception as e:
             LOG.debug("error cleaning up table %s: %s", table, e)
 
 
 @pytest.fixture
-def s3_create_bucket(s3_client, s3_resource):
+def s3_create_bucket(s3_resource, aws_client):
     buckets = []
 
     def factory(**kwargs) -> str:
         if "Bucket" not in kwargs:
             kwargs["Bucket"] = "test-bucket-%s" % short_uid()
 
-        s3_client.create_bucket(**kwargs)
+        aws_client.s3.create_bucket(**kwargs)
         buckets.append(kwargs["Bucket"])
         return kwargs["Bucket"]
 
     yield factory
 
     # cleanup
     for bucket in buckets:
@@ -418,69 +250,71 @@
             bucket.object_versions.all().delete()
             bucket.delete()
         except Exception as e:
             LOG.debug("error cleaning up bucket %s: %s", bucket, e)
 
 
 @pytest.fixture
-def s3_bucket(s3_client, s3_create_bucket) -> str:
-    region = s3_client.meta.region_name
+def s3_bucket(s3_create_bucket, aws_client) -> str:
+    region = aws_client.s3.meta.region_name
     kwargs = {}
     if region != "us-east-1":
         kwargs["CreateBucketConfiguration"] = {"LocationConstraint": region}
     return s3_create_bucket(**kwargs)
 
 
 @pytest.fixture
-def sqs_create_queue(sqs_client):
+def sqs_create_queue(aws_client):
     queue_urls = []
 
     def factory(**kwargs):
         if "QueueName" not in kwargs:
             kwargs["QueueName"] = "test-queue-%s" % short_uid()
 
-        response = sqs_client.create_queue(**kwargs)
+        response = aws_client.sqs.create_queue(**kwargs)
         url = response["QueueUrl"]
         queue_urls.append(url)
 
         return url
 
     yield factory
 
     # cleanup
     for queue_url in queue_urls:
         try:
-            sqs_client.delete_queue(QueueUrl=queue_url)
+            aws_client.sqs.delete_queue(QueueUrl=queue_url)
         except Exception as e:
             LOG.debug("error cleaning up queue %s: %s", queue_url, e)
 
 
 @pytest.fixture
-def sqs_receive_messages_delete(sqs_client):
+def sqs_receive_messages_delete(aws_client):
     def factory(
         queue_url: str,
         expected_messages: Optional[int] = None,
         wait_time: Optional[int] = 5,
     ):
-        response = sqs_client.receive_message(
+        response = aws_client.sqs.receive_message(
             QueueUrl=queue_url,
             MessageAttributeNames=["All"],
             VisibilityTimeout=0,
             WaitTimeSeconds=wait_time,
         )
         messages = []
         for m in response["Messages"]:
             message = json.loads(to_str(m["Body"]))
             messages.append(message)
 
         if expected_messages is not None:
             assert len(messages) == expected_messages
 
         for message in response["Messages"]:
-            sqs_client.delete_message(QueueUrl=queue_url, ReceiptHandle=message["ReceiptHandle"])
+            aws_client.sqs.delete_message(
+                QueueUrl=queue_url, ReceiptHandle=message["ReceiptHandle"]
+            )
 
         return messages
 
     return factory
 
 
 @pytest.fixture
@@ -505,114 +339,114 @@
 
 @pytest.fixture
 def sqs_queue(sqs_create_queue):
     return sqs_create_queue()
 
 
 @pytest.fixture
-def sqs_queue_arn(sqs_client):
+def sqs_queue_arn(aws_client):
     def _get_arn(queue_url: str) -> str:
-        return sqs_client.get_queue_attributes(QueueUrl=queue_url, AttributeNames=["QueueArn"])[
+        return aws_client.sqs.get_queue_attributes(QueueUrl=queue_url, AttributeNames=["QueueArn"])[
             "Attributes"
         ]["QueueArn"]
 
     return _get_arn
 
 
 @pytest.fixture
-def sqs_queue_exists(sqs_client):
+def sqs_queue_exists(aws_client):
     def _queue_exists(queue_url: str) -> bool:
         """
         Checks whether a queue with the given queue URL exists.
         :param queue_url: the queue URL
         :return: true if the queue exists, false otherwise
         """
         try:
-            result = sqs_client.get_queue_url(QueueName=queue_url.split("/")[-1])
+            result = aws_client.sqs.get_queue_url(QueueName=queue_url.split("/")[-1])
             return result.get("QueueUrl") == queue_url
         except ClientError as e:
             if "NonExistentQueue" in e.response["Error"]["Code"]:
                 return False
             raise
 
     yield _queue_exists
 
 
 @pytest.fixture
-def sns_create_topic(sns_client):
+def sns_create_topic(aws_client):
     topic_arns = []
 
     def _create_topic(**kwargs):
         if "Name" not in kwargs:
             kwargs["Name"] = "test-topic-%s" % short_uid()
-        response = sns_client.create_topic(**kwargs)
+        response = aws_client.sns.create_topic(**kwargs)
         topic_arns.append(response["TopicArn"])
         return response
 
     yield _create_topic
 
     for topic_arn in topic_arns:
         try:
-            sns_client.delete_topic(TopicArn=topic_arn)
+            aws_client.sns.delete_topic(TopicArn=topic_arn)
         except Exception as e:
             LOG.debug("error cleaning up topic %s: %s", topic_arn, e)
 
 
 @pytest.fixture
-def sns_wait_for_topic_delete(sns_client):
+def sns_wait_for_topic_delete(aws_client):
     def wait_for_topic_delete(topic_arn: str) -> None:
         def wait():
             try:
-                sns_client.get_topic_attributes(TopicArn=topic_arn)
+                aws_client.sns.get_topic_attributes(TopicArn=topic_arn)
                 return False
             except Exception as e:
                 if "NotFound" in e.response["Error"]["Code"]:
                     return True
 
                 raise
 
         poll_condition(wait, timeout=30)
 
     return wait_for_topic_delete
 
 
 @pytest.fixture
-def sns_subscription(sns_client):
+def sns_subscription(aws_client):
     sub_arns = []
 
     def _create_sub(**kwargs):
         if kwargs.get("ReturnSubscriptionArn") is None:
             kwargs["ReturnSubscriptionArn"] = True
 
         # requires 'TopicArn', 'Protocol', and 'Endpoint'
-        response = sns_client.subscribe(**kwargs)
+        response = aws_client.sns.subscribe(**kwargs)
         sub_arn = response["SubscriptionArn"]
         sub_arns.append(sub_arn)
         return response
 
     yield _create_sub
 
     for sub_arn in sub_arns:
         try:
-            sns_client.unsubscribe(SubscriptionArn=sub_arn)
+            aws_client.sns.unsubscribe(SubscriptionArn=sub_arn)
         except Exception as e:
             LOG.debug(f"error cleaning up subscription {sub_arn}: {e}")
 
 
 @pytest.fixture
-def sns_topic(sns_client, sns_create_topic):
+def sns_topic(sns_create_topic, aws_client):
     topic_arn = sns_create_topic()["TopicArn"]
-    return sns_client.get_topic_attributes(TopicArn=topic_arn)
+    return aws_client.sns.get_topic_attributes(TopicArn=topic_arn)
 
 
 @pytest.fixture
-def sns_allow_topic_sqs_queue(sqs_client):
+def sns_allow_topic_sqs_queue(aws_client):
     def _allow_sns_topic(sqs_queue_url, sqs_queue_arn, sns_topic_arn) -> None:
         # allow topic to write to sqs queue
-        sqs_client.set_queue_attributes(
+        aws_client.sqs.set_queue_attributes(
             QueueUrl=sqs_queue_url,
             Attributes={
                 "Policy": json.dumps(
                     {
                         "Statement": [
                             {
                                 "Effect": "Allow",
@@ -627,47 +461,47 @@
             },
         )
 
     return _allow_sns_topic
 
 
 @pytest.fixture
-def sns_create_sqs_subscription(sns_client, sqs_client, sns_allow_topic_sqs_queue, sqs_queue_arn):
+def sns_create_sqs_subscription(sns_allow_topic_sqs_queue, sqs_queue_arn, aws_client):
     subscriptions = []
 
     def _factory(topic_arn: str, queue_url: str, **kwargs) -> Dict[str, str]:
         queue_arn = sqs_queue_arn(queue_url=queue_url)
 
         # connect sns topic to sqs
-        subscription = sns_client.subscribe(
+        subscription = aws_client.sns.subscribe(
             TopicArn=topic_arn, Protocol="sqs", Endpoint=queue_arn, **kwargs
         )
         subscription_arn = subscription["SubscriptionArn"]
 
         # allow topic to write to sqs queue
         sns_allow_topic_sqs_queue(
             sqs_queue_url=queue_url, sqs_queue_arn=queue_arn, sns_topic_arn=topic_arn
         )
 
         subscriptions.append(subscription_arn)
-        return sns_client.get_subscription_attributes(SubscriptionArn=subscription_arn)[
+        return aws_client.sns.get_subscription_attributes(SubscriptionArn=subscription_arn)[
             "Attributes"
         ]
 
     yield _factory
 
     for arn in subscriptions:
         try:
-            sns_client.unsubscribe(SubscriptionArn=arn)
+            aws_client.sns.unsubscribe(SubscriptionArn=arn)
         except Exception as e:
             LOG.error("error cleaning up subscription %s: %s", arn, e)
 
 
 @pytest.fixture
-def sns_create_http_endpoint(sns_client, sns_create_topic, sns_subscription):
+def sns_create_http_endpoint(sns_create_topic, sns_subscription, aws_client):
     http_servers = []
 
     def _create_http_endpoint(
         raw_message_delivery: bool = False,
     ) -> Tuple[str, str, str, HTTPServer]:
         server = HTTPServer()
         server.start()
@@ -689,22 +523,22 @@
                 "numMaxDelayRetries": 0,
                 "backoffFunction": "linear",
             },
             "sicklyRetryPolicy": None,
             "throttlePolicy": {"maxReceivesPerSecond": 1000},
             "guaranteed": False,
         }
-        sns_client.set_subscription_attributes(
+        aws_client.sns.set_subscription_attributes(
             SubscriptionArn=subscription_arn,
             AttributeName="DeliveryPolicy",
             AttributeValue=json.dumps(delivery_policy),
         )
 
         if raw_message_delivery:
-            sns_client.set_subscription_attributes(
+            aws_client.sns.set_subscription_attributes(
                 SubscriptionArn=subscription_arn,
                 AttributeName="RawMessageDelivery",
                 AttributeValue="true",
             )
 
         return topic_arn, subscription_arn, endpoint_url, server
 
@@ -712,39 +546,39 @@
 
     for http_server in http_servers:
         if http_server.is_running():
             http_server.stop()
 
 
 @pytest.fixture
-def route53_hosted_zone(route53_client):
+def route53_hosted_zone(aws_client):
     hosted_zones = []
 
     def factory(**kwargs):
         if "Name" not in kwargs:
             kwargs["Name"] = f"www.{short_uid()}.com."
         if "CallerReference" not in kwargs:
             kwargs["CallerReference"] = f"caller-ref-{short_uid()}"
-        response = route53_client.create_hosted_zone(
+        response = aws_client.route53.create_hosted_zone(
             Name=kwargs["Name"], CallerReference=kwargs["CallerReference"]
         )
         hosted_zones.append(response["HostedZone"]["Id"])
         return response
 
     yield factory
 
     for zone in hosted_zones:
         try:
-            route53_client.delete_hosted_zone(Id=zone)
+            aws_client.route53.delete_hosted_zone(Id=zone)
         except Exception as e:
             LOG.debug(f"error cleaning up route53 HostedZone {zone}: {e}")
 
 
 @pytest.fixture
-def transcribe_create_job(transcribe_client, s3_client, s3_bucket):
+def transcribe_create_job(s3_bucket, aws_client):
     job_names = []
 
     def _create_job(audio_file: str, params: Optional[dict[str, Any]] = None) -> str:
         s3_key = "test-clip.wav"
 
         if not params:
             params = {}
@@ -756,87 +590,89 @@
             params["LanguageCode"] = "en-GB"
 
         if "Media" not in params:
             params["Media"] = {"MediaFileUri": f"s3://{s3_bucket}/{s3_key}"}
 
         # upload test wav to a s3 bucket
         with open(audio_file, "rb") as f:
-            s3_client.upload_fileobj(f, s3_bucket, s3_key)
+            aws_client.s3.upload_fileobj(f, s3_bucket, s3_key)
 
-        response = transcribe_client.start_transcription_job(**params)
+        response = aws_client.transcribe.start_transcription_job(**params)
 
         job_name = response["TranscriptionJob"]["TranscriptionJobName"]
         job_names.append(job_name)
 
         return job_name
 
     yield _create_job
 
     for job_name in job_names:
         with contextlib.suppress(ClientError):
-            transcribe_client.delete_transcription_job(TranscriptionJobName=job_name)
+            aws_client.transcribe.delete_transcription_job(TranscriptionJobName=job_name)
 
 
 @pytest.fixture
-def kinesis_create_stream(kinesis_client):
+def kinesis_create_stream(aws_client):
     stream_names = []
 
     def _create_stream(**kwargs):
         if "StreamName" not in kwargs:
             kwargs["StreamName"] = f"test-stream-{short_uid()}"
-        kinesis_client.create_stream(**kwargs)
+        aws_client.kinesis.create_stream(**kwargs)
         stream_names.append(kwargs["StreamName"])
         return kwargs["StreamName"]
 
     yield _create_stream
 
     for stream_name in stream_names:
         try:
-            kinesis_client.delete_stream(StreamName=stream_name, EnforceConsumerDeletion=True)
+            aws_client.kinesis.delete_stream(StreamName=stream_name, EnforceConsumerDeletion=True)
         except Exception as e:
             LOG.debug("error cleaning up kinesis stream %s: %s", stream_name, e)
 
 
 @pytest.fixture
-def wait_for_stream_ready(kinesis_client):
+def wait_for_stream_ready(aws_client):
     def _wait_for_stream_ready(stream_name: str):
         def is_stream_ready():
-            describe_stream_response = kinesis_client.describe_stream(StreamName=stream_name)
+            describe_stream_response = aws_client.kinesis.describe_stream(StreamName=stream_name)
             return describe_stream_response["StreamDescription"]["StreamStatus"] in [
                 "ACTIVE",
                 "UPDATING",
             ]
 
         poll_condition(is_stream_ready)
 
     return _wait_for_stream_ready
 
 
 @pytest.fixture
-def wait_for_delivery_stream_ready(firehose_client):
+def wait_for_delivery_stream_ready(aws_client):
     def _wait_for_stream_ready(delivery_stream_name: str):
         def is_stream_ready():
-            describe_stream_response = firehose_client.describe_delivery_stream(
+            describe_stream_response = aws_client.firehose.describe_delivery_stream(
                 DeliveryStreamName=delivery_stream_name
             )
             return (
                 describe_stream_response["DeliveryStreamDescription"]["DeliveryStreamStatus"]
                 == "ACTIVE"
             )
 
         poll_condition(is_stream_ready)
 
     return _wait_for_stream_ready
 
 
 @pytest.fixture
-def wait_for_dynamodb_stream_ready(dynamodbstreams_client):
+def wait_for_dynamodb_stream_ready(aws_client):
     def _wait_for_stream_ready(stream_arn: str):
         def is_stream_ready():
-            describe_stream_response = dynamodbstreams_client.describe_stream(StreamArn=stream_arn)
+            describe_stream_response = aws_client.dynamodbstreams.describe_stream(
+                StreamArn=stream_arn
+            )
             return describe_stream_response["StreamDescription"]["StreamStatus"] == "ENABLED"
 
         poll_condition(is_stream_ready)
 
     return _wait_for_stream_ready
 
 
@@ -890,38 +726,38 @@
             LOG.debug("error cleaning up KMS key %s: %s", key_id, e)
 
 
 # kms_create_key fixture is used here not just to be able to create aliases without a key specified,
 # but also to make sure that kms_create_key gets executed before and teared down after kms_create_alias -
 # to make sure that we clean up aliases before keys get cleaned up.
 @pytest.fixture()
-def kms_create_alias(kms_client, kms_create_key):
+def kms_create_alias(kms_create_key, aws_client):
     aliases = []
 
     def _create_alias(**kwargs):
         if "AliasName" not in kwargs:
             kwargs["AliasName"] = f"alias/{short_uid()}"
         if "TargetKeyId" not in kwargs:
             kwargs["TargetKeyId"] = kms_create_key()["KeyId"]
 
-        kms_client.create_alias(**kwargs)
+        aws_client.kms.create_alias(**kwargs)
         aliases.append(kwargs["AliasName"])
         return kwargs["AliasName"]
 
     yield _create_alias
 
     for alias in aliases:
         try:
-            kms_client.delete_alias(AliasName=alias)
+            aws_client.kms.delete_alias(AliasName=alias)
         except Exception as e:
             LOG.debug("error cleaning up KMS alias %s: %s", alias, e)
 
 
 @pytest.fixture()
-def kms_create_grant(kms_client, kms_create_key):
+def kms_create_grant(kms_create_key, aws_client):
     grants = []
 
     def _create_grant(**kwargs):
         # Just a random ARN, since KMS in LocalStack currently doesn't validate GranteePrincipal,
         # but some GranteePrincipal is required to create a grant.
         GRANTEE_PRINCIPAL_ARN = (
             "arn:aws:kms:eu-central-1:123456789876:key/198a5a78-52c3-489f-ac70-b06a4d11027a"
@@ -930,99 +766,99 @@
         if "Operations" not in kwargs:
             kwargs["Operations"] = ["Decrypt", "Encrypt"]
         if "GranteePrincipal" not in kwargs:
             kwargs["GranteePrincipal"] = GRANTEE_PRINCIPAL_ARN
         if "KeyId" not in kwargs:
             kwargs["KeyId"] = kms_create_key()["KeyId"]
 
-        grant_id = kms_client.create_grant(**kwargs)["GrantId"]
+        grant_id = aws_client.kms.create_grant(**kwargs)["GrantId"]
         grants.append((grant_id, kwargs["KeyId"]))
         return grant_id, kwargs["KeyId"]
 
     yield _create_grant
 
     for grant_id, key_id in grants:
         try:
-            kms_client.retire_grant(GrantId=grant_id, KeyId=key_id)
+            aws_client.kms.retire_grant(GrantId=grant_id, KeyId=key_id)
         except Exception as e:
             LOG.debug("error cleaning up KMS grant %s: %s", grant_id, e)
 
 
 @pytest.fixture
 def kms_key(kms_create_key):
     return kms_create_key()
 
 
 @pytest.fixture
-def kms_grant_and_key(kms_client, kms_key, sts_client):
-    user_arn = sts_client.get_caller_identity()["Arn"]
+def kms_grant_and_key(kms_key, aws_client):
+    user_arn = aws_client.sts.get_caller_identity()["Arn"]
 
     return [
-        kms_client.create_grant(
+        aws_client.kms.create_grant(
             KeyId=kms_key["KeyId"],
             GranteePrincipal=user_arn,
             Operations=["Decrypt", "Encrypt"],
         ),
         kms_key,
     ]
 
 
 @pytest.fixture
-def opensearch_wait_for_cluster(opensearch_client):
+def opensearch_wait_for_cluster(aws_client):
     def _wait_for_cluster(domain_name: str):
         def finished_processing():
-            status = opensearch_client.describe_domain(DomainName=domain_name)["DomainStatus"]
+            status = aws_client.opensearch.describe_domain(DomainName=domain_name)["DomainStatus"]
             return status["Processing"] is False
 
         assert poll_condition(
             finished_processing, timeout=5 * 60
         ), f"could not start domain: {domain_name}"
 
     return _wait_for_cluster
 
 
 @pytest.fixture
-def opensearch_create_domain(opensearch_client, opensearch_wait_for_cluster):
+def opensearch_create_domain(opensearch_wait_for_cluster, aws_client):
     domains = []
 
     def factory(**kwargs) -> str:
         if "DomainName" not in kwargs:
             kwargs["DomainName"] = f"test-domain-{short_uid()}"
 
-        opensearch_client.create_domain(**kwargs)
+        aws_client.opensearch.create_domain(**kwargs)
 
         opensearch_wait_for_cluster(domain_name=kwargs["DomainName"])
 
         domains.append(kwargs["DomainName"])
         return kwargs["DomainName"]
 
     yield factory
 
     # cleanup
     for domain in domains:
         try:
-            opensearch_client.delete_domain(DomainName=domain)
+            aws_client.opensearch.delete_domain(DomainName=domain)
         except Exception as e:
             LOG.debug("error cleaning up domain %s: %s", domain, e)
 
 
 @pytest.fixture
 def opensearch_domain(opensearch_create_domain) -> str:
     return opensearch_create_domain()
 
 
 @pytest.fixture
-def opensearch_endpoint(opensearch_client, opensearch_domain) -> str:
-    status = opensearch_client.describe_domain(DomainName=opensearch_domain)["DomainStatus"]
+def opensearch_endpoint(opensearch_domain, aws_client) -> str:
+    status = aws_client.opensearch.describe_domain(DomainName=opensearch_domain)["DomainStatus"]
     assert "Endpoint" in status
     return f"https://{status['Endpoint']}"
 
 
 @pytest.fixture
-def opensearch_document_path(opensearch_client, opensearch_endpoint):
+def opensearch_document_path(opensearch_endpoint, aws_client):
     document = {
         "first_name": "Boba",
         "last_name": "Fett",
         "age": 41,
         "about": "I'm just a simple man, trying to make my way in the universe.",
         "interests": ["mandalorian armor", "tusken culture"],
     }
@@ -1034,33 +870,33 @@
     )
     assert response.status_code == 201, f"could not create document at: {document_path}"
     return document_path
 
 
 # Cleanup fixtures
 @pytest.fixture
-def cleanup_stacks(cfn_client):
+def cleanup_stacks(aws_client):
     def _cleanup_stacks(stacks: List[str]) -> None:
         stacks = ensure_list(stacks)
         for stack in stacks:
             try:
-                cfn_client.delete_stack(StackName=stack)
+                aws_client.cloudformation.delete_stack(StackName=stack)
             except Exception:
                 LOG.debug(f"Failed to cleanup stack '{stack}'")
 
     return _cleanup_stacks
 
 
 @pytest.fixture
-def cleanup_changesets(cfn_client):
+def cleanup_changesets(aws_client):
     def _cleanup_changesets(changesets: List[str]) -> None:
         changesets = ensure_list(changesets)
         for cs in changesets:
             try:
-                cfn_client.delete_change_set(ChangeSetName=cs)
+                aws_client.cloudformation.delete_change_set(ChangeSetName=cs)
             except Exception:
                 LOG.debug(f"Failed to cleanup changeset '{cs}'")
 
     return _cleanup_changesets
 
 
 # Helpers for Cfn
@@ -1076,20 +912,19 @@
     outputs: Dict[str, str]
 
     destroy: Callable[[], None]
 
 
 @pytest.fixture
 def deploy_cfn_template(
-    cfn_client,
-    lambda_client,
     cleanup_stacks,
     cleanup_changesets,
     is_change_set_created_and_available,
     is_change_set_finished,
+    aws_client,
 ):
     state = []
 
     def _deploy(
         *,
         is_update: Optional[bool] = False,
         stack_name: Optional[str] = None,
@@ -1106,15 +941,15 @@
         stack_name = stack_name or f"stack-{short_uid()}"
         change_set_name = change_set_name or f"change-set-{short_uid()}"
 
         if template_path is not None:
             template = load_template_file(template_path)
         template_rendered = render_template(template, **(template_mapping or {}))
 
-        response = cfn_client.create_change_set(
+        response = aws_client.cloudformation.create_change_set(
             StackName=stack_name,
             ChangeSetName=change_set_name,
             TemplateBody=template_rendered,
             Capabilities=["CAPABILITY_AUTO_EXPAND", "CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"],
             ChangeSetType=("UPDATE" if is_update else "CREATE"),
             Parameters=[
                 {
@@ -1125,27 +960,31 @@
             ],
         )
         change_set_id = response["Id"]
         stack_id = response["StackId"]
         state.append({"stack_id": stack_id, "change_set_id": change_set_id})
 
         assert wait_until(is_change_set_created_and_available(change_set_id), _max_wait=60)
-        cfn_client.execute_change_set(ChangeSetName=change_set_id)
+        aws_client.cloudformation.execute_change_set(ChangeSetName=change_set_id)
         assert wait_until(is_change_set_finished(change_set_id), _max_wait=max_wait or 60)
 
-        outputs = cfn_client.describe_stacks(StackName=stack_id)["Stacks"][0].get("Outputs", [])
+        outputs = aws_client.cloudformation.describe_stacks(StackName=stack_id)["Stacks"][0].get(
+            "Outputs", []
+        )
 
         mapped_outputs = {o["OutputKey"]: o.get("OutputValue") for o in outputs}
 
         def _destroy_stack():
-            cfn_client.delete_stack(StackName=stack_id)
+            aws_client.cloudformation.delete_stack(StackName=stack_id)
 
             def _await_stack_delete():
                 return (
-                    cfn_client.describe_stacks(StackName=stack_id)["Stacks"][0]["StackStatus"]
+                    aws_client.cloudformation.describe_stacks(StackName=stack_id)["Stacks"][0][
+                        "StackStatus"
+                    ]
                     == "DELETE_COMPLETE"
                 )
 
             assert wait_until(_await_stack_delete, _max_wait=max_wait or 60)
             # TODO: fix in localstack. stack should only be in DELETE_COMPLETE state after all resources have been deleted
             time.sleep(2)
 
@@ -1164,58 +1003,58 @@
         except Exception as e:
             LOG.debug(
                 f"Failed cleaning up change set {entry_change_set_id=} and stack {entry_stack_id=}: {e}"
             )
 
 
 @pytest.fixture
-def is_change_set_created_and_available(cfn_client):
+def is_change_set_created_and_available(aws_client):
     def _is_change_set_created_and_available(change_set_id: str):
         def _inner():
-            change_set = cfn_client.describe_change_set(ChangeSetName=change_set_id)
+            change_set = aws_client.cloudformation.describe_change_set(ChangeSetName=change_set_id)
             return (
                 # TODO: CREATE_FAILED should also not lead to further retries
                 change_set.get("Status") == "CREATE_COMPLETE"
                 and change_set.get("ExecutionStatus") == "AVAILABLE"
             )
 
         return _inner
 
     return _is_change_set_created_and_available
 
 
 @pytest.fixture
-def is_change_set_failed_and_unavailable(cfn_client):
+def is_change_set_failed_and_unavailable(aws_client):
     def _is_change_set_created_and_available(change_set_id: str):
         def _inner():
-            change_set = cfn_client.describe_change_set(ChangeSetName=change_set_id)
+            change_set = aws_client.cloudformation.describe_change_set(ChangeSetName=change_set_id)
             return (
                 # TODO: CREATE_FAILED should also not lead to further retries
                 change_set.get("Status") == "FAILED"
                 and change_set.get("ExecutionStatus") == "UNAVAILABLE"
             )
 
         return _inner
 
     return _is_change_set_created_and_available
 
 
 @pytest.fixture
-def is_stack_created(cfn_client):
-    return _has_stack_status(cfn_client, ["CREATE_COMPLETE", "CREATE_FAILED"])
+def is_stack_created(aws_client):
+    return _has_stack_status(aws_client.cloudformation, ["CREATE_COMPLETE", "CREATE_FAILED"])
 
 
 @pytest.fixture
-def is_stack_updated(cfn_client):
-    return _has_stack_status(cfn_client, ["UPDATE_COMPLETE", "UPDATE_FAILED"])
+def is_stack_updated(aws_client):
+    return _has_stack_status(aws_client.cloudformation, ["UPDATE_COMPLETE", "UPDATE_FAILED"])
 
 
 @pytest.fixture
-def is_stack_deleted(cfn_client):
-    return _has_stack_status(cfn_client, ["DELETE_COMPLETE"])
+def is_stack_deleted(aws_client):
+    return _has_stack_status(aws_client.cloudformation, ["DELETE_COMPLETE"])
 
 
 def _has_stack_status(cfn_client, statuses: List[str]):
     def _has_status(stack_id: str):
         def _inner():
             resp = cfn_client.describe_stacks(StackName=stack_id)
             s = resp["Stacks"][0]  # since the lookup  uses the id we can only get a single response
@@ -1223,38 +1062,38 @@
 
         return _inner
 
     return _has_status
 
 
 @pytest.fixture
-def is_change_set_finished(cfn_client):
+def is_change_set_finished(aws_client):
     def _is_change_set_finished(change_set_id: str, stack_name: Optional[str] = None):
         def _inner():
             kwargs = {"ChangeSetName": change_set_id}
             if stack_name:
                 kwargs["StackName"] = stack_name
 
-            check_set = cfn_client.describe_change_set(**kwargs)
+            check_set = aws_client.cloudformation.describe_change_set(**kwargs)
 
             if check_set.get("ExecutionStatus") == "ROLLBACK_COMPLETE":
                 LOG.warning("Change set failed")
                 raise ShortCircuitWaitException()
 
             return check_set.get("ExecutionStatus") == "EXECUTE_COMPLETE"
 
         return _inner
 
     return _is_change_set_finished
 
 
 @pytest.fixture
-def wait_until_lambda_ready(lambda_client):
+def wait_until_lambda_ready(aws_client):
     def _wait_until_ready(function_name: str, qualifier: str = None, client=None):
-        client = client or lambda_client
+        client = client or aws_client.awslambda
 
         def _is_not_pending():
             kwargs = {}
             if qualifier:
                 kwargs["Qualifier"] = qualifier
             try:
                 result = (
@@ -1304,28 +1143,26 @@
         }
     ]
 }
 """.strip()
 
 
 @pytest.fixture
-def create_lambda_function_aws(
-    lambda_client,
-):
+def create_lambda_function_aws(aws_client):
     lambda_arns = []
 
     def _create_lambda_function(**kwargs):
         def _create_function():
-            resp = lambda_client.create_function(**kwargs)
+            resp = aws_client.awslambda.create_function(**kwargs)
             lambda_arns.append(resp["FunctionArn"])
 
             def _is_not_pending():
                 try:
                     result = (
-                        lambda_client.get_function(FunctionName=resp["FunctionName"])[
+                        aws_client.awslambda.get_function(FunctionName=resp["FunctionName"])[
                             "Configuration"
                         ]["State"]
                         != "Pending"
                     )
                     return result
                 except Exception as e:
                     LOG.error(e)
@@ -1338,15 +1175,15 @@
         # localstack should normally not require the retries and will just continue here
         return retry(_create_function, retries=3, sleep=4)
 
     yield _create_lambda_function
 
     for arn in lambda_arns:
         try:
-            lambda_client.delete_function(FunctionName=arn)
+            aws_client.awslambda.delete_function(FunctionName=arn)
         except Exception:
             LOG.debug(f"Unable to delete function {arn=} in cleanup")
 
 
 @pytest.fixture
 def create_lambda_function(aws_client, wait_until_lambda_ready, lambda_su_role):
     lambda_arns_and_clients = []
@@ -1388,199 +1225,199 @@
         try:
             logs_client.delete_log_group(logGroupName=log_group_name)
         except Exception:
             LOG.debug(f"Unable to delete log group {log_group_name} in cleanup")
 
 
 @pytest.fixture
-def check_lambda_logs(logs_client):
+def check_lambda_logs(aws_client):
     def _check_logs(func_name: str, expected_lines: List[str] = None) -> List[str]:
         if not expected_lines:
             expected_lines = []
-        log_events = get_lambda_logs(func_name, logs_client=logs_client)
+        log_events = get_lambda_logs(func_name, logs_client=aws_client.logs)
         log_messages = [e["message"] for e in log_events]
         for line in expected_lines:
             if ".*" in line:
                 found = [re.match(line, m, flags=re.DOTALL) for m in log_messages]
                 if any(found):
                     continue
             assert line in log_messages
         return log_messages
 
     return _check_logs
 
 
 @pytest.fixture
-def create_policy(iam_client):
+def create_policy(aws_client):
     policy_arns = []
 
     def _create_policy(*args, **kwargs):
         if "PolicyName" not in kwargs:
             kwargs["PolicyName"] = f"policy-{short_uid()}"
-        response = iam_client.create_policy(*args, **kwargs)
+        response = aws_client.iam.create_policy(*args, **kwargs)
         policy_arn = response["Policy"]["Arn"]
         policy_arns.append(policy_arn)
         return response
 
     yield _create_policy
 
     for policy_arn in policy_arns:
         try:
-            iam_client.delete_policy(PolicyArn=policy_arn)
+            aws_client.iam.delete_policy(PolicyArn=policy_arn)
         except Exception:
             LOG.debug("Could not delete policy '%s' during test cleanup", policy_arn)
 
 
 @pytest.fixture
-def create_user(iam_client):
+def create_user(aws_client):
     usernames = []
 
     def _create_user(**kwargs):
         if "UserName" not in kwargs:
             kwargs["UserName"] = f"user-{short_uid()}"
-        response = iam_client.create_user(**kwargs)
+        response = aws_client.iam.create_user(**kwargs)
         usernames.append(response["User"]["UserName"])
         return response
 
     yield _create_user
 
     for username in usernames:
-        inline_policies = iam_client.list_user_policies(UserName=username)["PolicyNames"]
+        inline_policies = aws_client.iam.list_user_policies(UserName=username)["PolicyNames"]
         for inline_policy in inline_policies:
             try:
-                iam_client.delete_user_policy(UserName=username, PolicyName=inline_policy)
+                aws_client.iam.delete_user_policy(UserName=username, PolicyName=inline_policy)
             except Exception:
                 LOG.debug(
                     "Could not delete user policy '%s' from '%s' during cleanup",
                     inline_policy,
                     username,
                 )
-        attached_policies = iam_client.list_attached_user_policies(UserName=username)[
+        attached_policies = aws_client.iam.list_attached_user_policies(UserName=username)[
             "AttachedPolicies"
         ]
         for attached_policy in attached_policies:
             try:
-                iam_client.detach_user_policy(
+                aws_client.iam.detach_user_policy(
                     UserName=username, PolicyArn=attached_policy["PolicyArn"]
                 )
             except Exception:
                 LOG.debug(
                     "Error detaching policy '%s' from user '%s'",
                     attached_policy["PolicyArn"],
                     username,
                 )
-        access_keys = iam_client.list_access_keys(UserName=username)["AccessKeyMetadata"]
+        access_keys = aws_client.iam.list_access_keys(UserName=username)["AccessKeyMetadata"]
         for access_key in access_keys:
             try:
-                iam_client.delete_access_key(
+                aws_client.iam.delete_access_key(
                     UserName=username, AccessKeyId=access_key["AccessKeyId"]
                 )
             except Exception:
                 LOG.debug(
                     "Error deleting access key '%s' from user '%s'",
                     access_key["AccessKeyId"],
                     username,
                 )
 
         try:
-            iam_client.delete_user(UserName=username)
+            aws_client.iam.delete_user(UserName=username)
         except Exception as e:
             LOG.debug("Error deleting user '%s' during test cleanup: %s", username, e)
 
 
 @pytest.fixture
-def wait_and_assume_role(sts_client):
+def wait_and_assume_role(aws_client):
     def _wait_and_assume_role(role_arn: str, session_name: str = None):
         if not session_name:
             session_name = f"session-{short_uid()}"
 
         def assume_role():
-            return sts_client.assume_role(RoleArn=role_arn, RoleSessionName=session_name)[
+            return aws_client.sts.assume_role(RoleArn=role_arn, RoleSessionName=session_name)[
                 "Credentials"
             ]
 
         # need to retry a couple of times before we are allowed to assume this role in AWS
         keys = retry(assume_role, sleep=5, retries=4)
         return keys
 
     return _wait_and_assume_role
 
 
 @pytest.fixture
-def create_role(iam_client):
+def create_role(aws_client):
     role_names = []
 
     def _create_role(**kwargs):
         if not kwargs.get("RoleName"):
             kwargs["RoleName"] = f"role-{short_uid()}"
-        result = iam_client.create_role(**kwargs)
+        result = aws_client.iam.create_role(**kwargs)
         role_names.append(result["Role"]["RoleName"])
         return result
 
     yield _create_role
 
     for role_name in role_names:
         # detach policies
-        attached_policies = iam_client.list_attached_role_policies(RoleName=role_name)[
+        attached_policies = aws_client.iam.list_attached_role_policies(RoleName=role_name)[
             "AttachedPolicies"
         ]
         for attached_policy in attached_policies:
             try:
-                iam_client.detach_role_policy(
+                aws_client.iam.detach_role_policy(
                     RoleName=role_name, PolicyArn=attached_policy["PolicyArn"]
                 )
             except Exception:
                 LOG.debug(
                     "Could not detach role policy '%s' from '%s' during cleanup",
                     attached_policy["PolicyArn"],
                     role_name,
                 )
-        role_policies = iam_client.list_role_policies(RoleName=role_name)["PolicyNames"]
+        role_policies = aws_client.iam.list_role_policies(RoleName=role_name)["PolicyNames"]
         for role_policy in role_policies:
             try:
-                iam_client.delete_role_policy(RoleName=role_name, PolicyName=role_policy)
+                aws_client.iam.delete_role_policy(RoleName=role_name, PolicyName=role_policy)
             except Exception:
                 LOG.debug(
                     "Could not delete role policy '%s' from '%s' during cleanup",
                     role_policy,
                     role_name,
                 )
         try:
-            iam_client.delete_role(RoleName=role_name)
+            aws_client.iam.delete_role(RoleName=role_name)
         except Exception:
             LOG.debug("Could not delete role '%s' during cleanup", role_name)
 
 
 @pytest.fixture
-def create_parameter(ssm_client):
+def create_parameter(aws_client):
     params = []
 
     def _create_parameter(**kwargs):
         params.append(kwargs["Name"])
-        return ssm_client.put_parameter(**kwargs)
+        return aws_client.ssm.put_parameter(**kwargs)
 
     yield _create_parameter
 
     for param in params:
-        ssm_client.delete_parameter(Name=param)
+        aws_client.ssm.delete_parameter(Name=param)
 
 
 @pytest.fixture
-def create_secret(secretsmanager_client):
+def create_secret(aws_client):
     items = []
 
     def _create_parameter(**kwargs):
-        create_response = secretsmanager_client.create_secret(**kwargs)
+        create_response = aws_client.secretsmanager.create_secret(**kwargs)
         items.append(create_response["ARN"])
         return create_response
 
     yield _create_parameter
 
     for item in items:
-        secretsmanager_client.delete_secret(SecretId=item, ForceDeleteWithoutRecovery=True)
+        aws_client.secretsmanager.delete_secret(SecretId=item, ForceDeleteWithoutRecovery=True)
 
 
 # TODO Figure out how to make cert creation tests pass against AWS.
 #
 # We would like to have localstack tests to pass not just against localstack, but also against AWS to make sure
 # our emulation is correct. Unfortunately, with certificate creation there are some issues.
 #
@@ -1655,111 +1492,115 @@
 
     run_safe(aws_client.iam.detach_role_policy(RoleName=role_name, PolicyArn=policy_arn))
     run_safe(aws_client.iam.delete_role(RoleName=role_name))
     run_safe(aws_client.iam.delete_policy(PolicyArn=policy_arn))
 
 
 @pytest.fixture
-def create_iam_role_with_policy(iam_client):
+def create_iam_role_with_policy(aws_client):
     roles = {}
 
     def _create_role_and_policy(**kwargs):
         role = kwargs["RoleName"]
         policy = kwargs["PolicyName"]
         role_policy = json.dumps(kwargs["RoleDefinition"])
 
-        result = iam_client.create_role(RoleName=role, AssumeRolePolicyDocument=role_policy)
+        result = aws_client.iam.create_role(RoleName=role, AssumeRolePolicyDocument=role_policy)
         role_arn = result["Role"]["Arn"]
         policy_document = json.dumps(kwargs["PolicyDefinition"])
-        iam_client.put_role_policy(RoleName=role, PolicyName=policy, PolicyDocument=policy_document)
+        aws_client.iam.put_role_policy(
+            RoleName=role, PolicyName=policy, PolicyDocument=policy_document
+        )
         roles[role] = policy
         return role_arn
 
     yield _create_role_and_policy
 
     for role_name, policy_name in roles.items():
-        iam_client.delete_role_policy(RoleName=role_name, PolicyName=policy_name)
-        iam_client.delete_role(RoleName=role_name)
+        aws_client.iam.delete_role_policy(RoleName=role_name, PolicyName=policy_name)
+        aws_client.iam.delete_role(RoleName=role_name)
 
 
 @pytest.fixture
-def firehose_create_delivery_stream(firehose_client, wait_for_delivery_stream_ready):
+def firehose_create_delivery_stream(wait_for_delivery_stream_ready, aws_client):
     delivery_streams = {}
 
     def _create_delivery_stream(**kwargs):
         if "DeliveryStreamName" not in kwargs:
             kwargs["DeliveryStreamName"] = f"test-delivery-stream-{short_uid()}"
 
-        delivery_stream = firehose_client.create_delivery_stream(**kwargs)
+        delivery_stream = aws_client.firehose.create_delivery_stream(**kwargs)
         delivery_streams.update({kwargs["DeliveryStreamName"]: delivery_stream})
         wait_for_delivery_stream_ready(kwargs["DeliveryStreamName"])
         return delivery_stream
 
     yield _create_delivery_stream
 
     for delivery_stream_name in delivery_streams.keys():
-        firehose_client.delete_delivery_stream(DeliveryStreamName=delivery_stream_name)
+        aws_client.firehose.delete_delivery_stream(DeliveryStreamName=delivery_stream_name)
 
 
 @pytest.fixture
-def events_create_rule(events_client):
+def events_create_rule(aws_client):
     rules = []
 
     def _create_rule(**kwargs):
         rule_name = kwargs["Name"]
         bus_name = kwargs.get("EventBusName", "")
         pattern = kwargs.get("EventPattern", {})
         schedule = kwargs.get("ScheduleExpression", "")
-        rule_arn = events_client.put_rule(
+        rule_arn = aws_client.events.put_rule(
             Name=rule_name,
             EventBusName=bus_name,
             EventPattern=json.dumps(pattern),
             ScheduleExpression=schedule,
         )["RuleArn"]
         rules.append({"name": rule_name, "bus": bus_name})
         return rule_arn
 
     yield _create_rule
 
     for rule in rules:
-        targets = events_client.list_targets_by_rule(Rule=rule["name"], EventBusName=rule["bus"])[
-            "Targets"
-        ]
+        targets = aws_client.events.list_targets_by_rule(
+            Rule=rule["name"], EventBusName=rule["bus"]
+        )["Targets"]
 
         targetIds = [target["Id"] for target in targets]
         if len(targetIds) > 0:
-            events_client.remove_targets(Rule=rule["name"], EventBusName=rule["bus"], Ids=targetIds)
+            aws_client.events.remove_targets(
+                Rule=rule["name"], EventBusName=rule["bus"], Ids=targetIds
+            )
 
-        events_client.delete_rule(Name=rule["name"], EventBusName=rule["bus"])
+        aws_client.events.delete_rule(Name=rule["name"], EventBusName=rule["bus"])
 
 
 @pytest.fixture
-def ses_configuration_set(ses_client):
+def ses_configuration_set(aws_client):
     configuration_set_names = []
 
     def factory(name: str) -> None:
-        ses_client.create_configuration_set(
+        aws_client.ses.create_configuration_set(
             ConfigurationSet={
                 "Name": name,
             },
         )
         configuration_set_names.append(name)
 
     yield factory
 
     for configuration_set_name in configuration_set_names:
-        ses_client.delete_configuration_set(ConfigurationSetName=configuration_set_name)
+        aws_client.ses.delete_configuration_set(ConfigurationSetName=configuration_set_name)
 
 
 @pytest.fixture
-def ses_configuration_set_sns_event_destination(ses_client):
+def ses_configuration_set_sns_event_destination(aws_client):
     event_destinations = []
 
     def factory(config_set_name: str, event_destination_name: str, topic_arn: str) -> None:
-        ses_client.create_configuration_set_event_destination(
+        aws_client.ses.create_configuration_set_event_destination(
             ConfigurationSetName=config_set_name,
             EventDestination={
                 "Name": event_destination_name,
                 "Enabled": True,
                 "MatchingEventTypes": ["send", "bounce", "delivery", "open", "click"],
                 "SNSDestination": {
                     "TopicARN": topic_arn,
@@ -1767,90 +1608,90 @@
             },
         )
         event_destinations.append((config_set_name, event_destination_name))
 
     yield factory
 
     for (created_config_set_name, created_event_destination_name) in event_destinations:
-        ses_client.delete_configuration_set_event_destination(
+        aws_client.ses.delete_configuration_set_event_destination(
             ConfigurationSetName=created_config_set_name,
             EventDestinationName=created_event_destination_name,
         )
 
 
 @pytest.fixture
-def ses_email_template(ses_client):
+def ses_email_template(aws_client):
     template_names = []
 
     def factory(name: str, contents: str, subject: str = f"Email template {short_uid()}"):
-        ses_client.create_template(
+        aws_client.ses.create_template(
             Template={
                 "TemplateName": name,
                 "SubjectPart": subject,
                 "TextPart": contents,
             }
         )
         template_names.append(name)
 
     yield factory
 
     for template_name in template_names:
-        ses_client.delete_template(TemplateName=template_name)
+        aws_client.ses.delete_template(TemplateName=template_name)
 
 
 @pytest.fixture
-def ses_verify_identity(ses_client):
+def ses_verify_identity(aws_client):
     identities = []
 
     def factory(email_address: str) -> None:
-        ses_client.verify_email_identity(EmailAddress=email_address)
+        aws_client.ses.verify_email_identity(EmailAddress=email_address)
 
     yield factory
 
     for identity in identities:
-        ses_client.delete_identity(Identity=identity)
+        aws_client.ses.delete_identity(Identity=identity)
 
 
 @pytest.fixture
-def ec2_create_security_group(ec2_client):
+def ec2_create_security_group(aws_client):
     ec2_sgs = []
 
     def factory(ports=None, **kwargs):
         if "GroupName" not in kwargs:
             kwargs["GroupName"] = f"test-sg-{short_uid()}"
-        security_group = ec2_client.create_security_group(**kwargs)
+        security_group = aws_client.ec2.create_security_group(**kwargs)
 
         permissions = [
             {
                 "FromPort": port,
                 "IpProtocol": "tcp",
                 "IpRanges": [{"CidrIp": "0.0.0.0/0"}],
                 "ToPort": port,
             }
             for port in ports or []
         ]
-        ec2_client.authorize_security_group_ingress(
+        aws_client.ec2.authorize_security_group_ingress(
             GroupName=kwargs["GroupName"],
             IpPermissions=permissions,
         )
 
         ec2_sgs.append(security_group["GroupId"])
         return security_group
 
     yield factory
 
     for sg_group_id in ec2_sgs:
         try:
-            ec2_client.delete_security_group(GroupId=sg_group_id)
+            aws_client.ec2.delete_security_group(GroupId=sg_group_id)
         except Exception as e:
             LOG.debug("Error cleaning up EC2 security group: %s, %s", sg_group_id, e)
 
 
 @pytest.fixture
-def cleanups(ec2_client):
+def cleanups(aws_client):
     cleanup_fns = []
 
     yield cleanup_fns
 
     for cleanup_callback in cleanup_fns[::-1]:
         try:
             cleanup_callback()
@@ -1946,32 +1787,32 @@
     for rest_api_id, region_name in rest_apis:
         with contextlib.suppress(Exception):
             apigateway_client = aws_client_factory(region_name=region_name).apigateway
             apigateway_client.delete_rest_api(restApiId=rest_api_id)
 
 
 @pytest.fixture
-def appsync_create_api(appsync_client):
+def appsync_create_api(aws_client):
     graphql_apis = []
 
     def factory(**kwargs):
         if "name" not in kwargs:
             kwargs["name"] = f"graphql-api-testing-name-{short_uid()}"
         if not kwargs.get("authenticationType"):
             kwargs["authenticationType"] = "API_KEY"
 
-        result = appsync_client.create_graphql_api(**kwargs)["graphqlApi"]
+        result = aws_client.appsync.create_graphql_api(**kwargs)["graphqlApi"]
         graphql_apis.append(result["apiId"])
         return result
 
     yield factory
 
     for api in graphql_apis:
         try:
-            appsync_client.delete_graphql_api(apiId=api)
+            aws_client.appsync.delete_graphql_api(apiId=api)
         except Exception as e:
             LOG.debug(f"Error cleaning up AppSync API: {api}, {e}")
 
 
 @pytest.fixture
 def assert_host_customisation(monkeypatch):
     hostname_external = f"external-host-{short_uid()}"
@@ -2092,44 +1933,44 @@
         policy_arn = response["Policy"]["Arn"]
         return policy_arn
 
     return _create_policy_with_doc
 
 
 @pytest.fixture
-def create_role_with_policy(iam_client, sts_client, create_role, create_policy_generated_document):
+def create_role_with_policy(create_role, create_policy_generated_document, aws_client):
     def _create_role_with_policy(effect, actions, assume_policy_doc, resource=None, attach=True):
         role_name = f"role-{short_uid()}"
         result = create_role(RoleName=role_name, AssumeRolePolicyDocument=assume_policy_doc)
         role_arn = result["Role"]["Arn"]
         policy_name = f"p-{short_uid()}"
 
         if attach:
             # create role and attach role policy
             policy_arn = create_policy_generated_document(
                 effect, actions, policy_name=policy_name, resource=resource
             )
-            iam_client.attach_role_policy(RoleName=role_name, PolicyArn=policy_arn)
+            aws_client.iam.attach_role_policy(RoleName=role_name, PolicyArn=policy_arn)
         else:
             # put role policy
             policy_document = create_policy_doc(effect, actions, resource=resource)
             policy_document = json.dumps(policy_document)
-            iam_client.put_role_policy(
+            aws_client.iam.put_role_policy(
                 RoleName=role_name, PolicyName=policy_name, PolicyDocument=policy_document
             )
 
         return role_name, role_arn
 
     return _create_role_with_policy
 
 
 @pytest.fixture
-def create_user_with_policy(iam_client, create_policy_generated_document, create_user):
+def create_user_with_policy(create_policy_generated_document, create_user, aws_client):
     def _create_user_with_policy(effect, actions, resource=None):
         policy_arn = create_policy_generated_document(effect, actions, resource=resource)
         username = f"user-{short_uid()}"
         create_user(UserName=username)
-        iam_client.attach_user_policy(UserName=username, PolicyArn=policy_arn)
-        keys = iam_client.create_access_key(UserName=username)["AccessKey"]
+        aws_client.iam.attach_user_policy(UserName=username, PolicyArn=policy_arn)
+        keys = aws_client.iam.create_access_key(UserName=username)["AccessKey"]
         return username, keys
 
     return _create_user_with_policy
```

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/snapshot.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/pytest/util.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/snapshots/prototype.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/snapshots/report.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/snapshots/transformer.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.0.2.dev20230409051309/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/cli.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/client.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/events.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/logger.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/metadata.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/publisher.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/archives.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/asyncio.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/auth.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/arns.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/aws_models.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/aws_responses.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/aws_stack.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/client.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/client_types.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/queries.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/request_context.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/resources.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/aws/templating.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/bootstrap.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/collections.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/common.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/config_listener.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/container_networking.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/container_utils/container_client.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/coverage_docs.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/crypto.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/diagnose.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/docker_utils.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/files.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/functions.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/http.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/json.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/net.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/numbers.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/objects.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/patch.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/platform.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/run.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/scheduler.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/server/http2_server.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/server/proxy_server.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/serving.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/ssl.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/strings.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/sync.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/tagging.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/tail.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/testutil.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/threads.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/time.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/urls.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/venv.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack/utils/xml.py` & `localstack-core-2.0.2.dev20230409051309/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/plux.json` & `localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/plux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9084928229665071%*

 * *Differences: {"'localstack.hooks.on_infra_start'": '{insert: [(0, '*

 * *                                      "'_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event'), "*

 * *                                      '(1, '*

 * *                                      "'_publish_container_info=localstack.runtime.analytics:_publish_container_info'), "*

 * *                                      '(2, '*

 * *                                      "'validate_configuration=localstack.services.awslambda.plugins: […]*

```diff
@@ -53,36 +53,36 @@
         "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
     ],
     "localstack.hooks.on_infra_shutdown": [
         "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
-        "deprecation_warnings=localstack.plugins:deprecation_warnings",
-        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
+        "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
+        "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
         "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
-        "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
-        "_publish_container_info=localstack.runtime.analytics:_publish_container_info"
+        "deprecation_warnings=localstack.plugins:deprecation_warnings",
+        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
         "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "ffmpeg/community=localstack.services.transcribe.plugins:ffmpeg_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
         "terraform/community=localstack.packages.plugins:terraform_package",
-        "ffmpeg/community=localstack.services.transcribe.plugins:ffmpeg_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages"
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package"
     ]
 }
```

### Comparing `localstack-core-2.0.2.dev20230407124235/localstack_core.egg-info/requires.txt` & `localstack-core-2.0.2.dev20230409051309/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/pyproject.toml` & `localstack-core-2.0.2.dev20230409051309/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.2.dev20230407124235/setup.cfg` & `localstack-core-2.0.2.dev20230409051309/setup.cfg`

 * *Files identical despite different names*

