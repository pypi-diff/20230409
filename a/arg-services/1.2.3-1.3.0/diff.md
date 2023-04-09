# Comparing `tmp/arg_services-1.2.3.tar.gz` & `tmp/arg_services-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arg_services-1.2.3.tar", max compression
+gzip compressed data, was "arg_services-1.3.0.tar", max compression
```

## Comparing `arg_services-1.2.3.tar` & `arg_services-1.3.0.tar`

### file list

```diff
@@ -1,82 +1,81 @@
--rw-r--r--   0        0        0     1067 2023-03-10 16:24:52.497019 arg_services-1.2.3/LICENSE
--rw-r--r--   0        0        0      657 2023-03-10 16:24:52.497019 arg_services-1.2.3/README.md
--rw-r--r--   0        0        0      671 2023-03-10 16:25:46.377964 arg_services-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     7288 2023-03-10 16:25:45.885955 arg_services-1.2.3/src/arg_services/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.869955 arg_services-1.2.3/src/arg_services/cbr/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.869955 arg_services-1.2.3/src/arg_services/cbr/v1beta/__init__.py
--rw-r--r--   0        0        0     6689 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/adaptation_pb2.py
--rw-r--r--   0        0        0    12124 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
--rw-r--r--   0        0        0     2783 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
--rw-r--r--   0        0        0      806 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
--rw-r--r--   0        0        0     3301 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/casebase_pb2.py
--rw-r--r--   0        0        0     3094 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/casebase_pb2.pyi
--rw-r--r--   0        0        0     2792 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
--rw-r--r--   0        0        0      806 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
--rw-r--r--   0        0        0     2428 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/model_pb2.py
--rw-r--r--   0        0        0     2515 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/model_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/model_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
--rw-r--r--   0        0        0     6015 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/retrieval_pb2.py
--rw-r--r--   0        0        0    10993 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
--rw-r--r--   0        0        0     2807 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
--rw-r--r--   0        0        0      815 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.869955 arg_services-1.2.3/src/arg_services/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.873955 arg_services-1.2.3/src/arg_services/graph/v1/__init__.py
--rw-r--r--   0        0        0    11386 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/graph/v1/graph_pb2.py
--rw-r--r--   0        0        0    33449 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/graph/v1/graph_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/graph/v1/graph_pb2_grpc.py
--rw-r--r--   0        0        0      151 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/graph/v1/graph_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.873955 arg_services-1.2.3/src/arg_services/mining/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.873955 arg_services-1.2.3/src/arg_services/mining/v1beta/__init__.py
--rw-r--r--   0        0        0     4793 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     6692 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     4625 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0     1237 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     5843 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     8973 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     4721 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0     1298 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     4035 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/graph_construction_pb2.py
--rw-r--r--   0        0        0     3932 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
--rw-r--r--   0        0        0     3092 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
--rw-r--r--   0        0        0      961 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
--rw-r--r--   0        0        0     3673 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     4057 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     2896 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0      856 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0     2839 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/mining_pb2.py
--rw-r--r--   0        0        0     2419 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/mining_pb2.pyi
--rw-r--r--   0        0        0     2834 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/mining_pb2_grpc.py
--rw-r--r--   0        0        0      821 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.865955 arg_services-1.2.3/src/arg_services/mining_explanation/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.865955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/__init__.py
--rw-r--r--   0        0        0     3256 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     3359 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     3044 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0      916 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     4339 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     5167 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     3110 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0      961 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     3718 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     3980 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     3112 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0      960 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.877955 arg_services-1.2.3/src/arg_services/nlp/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.877955 arg_services-1.2.3/src/arg_services/nlp/v1/__init__.py
--rw-r--r--   0        0        0     8532 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/nlp/v1/nlp_pb2.py
--rw-r--r--   0        0        0    27577 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/nlp/v1/nlp_pb2.pyi
--rw-r--r--   0        0        0     6344 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/nlp/v1/nlp_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.877955 arg_services-1.2.3/src/google/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 16:25:45.881955 arg_services-1.2.3/src/google/api/__init__.py
--rw-r--r--   0        0        0     1794 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/google/api/annotations_pb2.py
--rw-r--r--   0        0        0     1047 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0      627 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/google/api/annotations_pb2_grpc.pyi
--rw-r--r--   0        0        0     2540 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/google/api/http_pb2.py
--rw-r--r--   0        0        0    18274 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      627 2023-03-10 16:25:45.857955 arg_services-1.2.3/src/google/api/http_pb2_grpc.pyi
--rw-r--r--   0        0        0     1866 1970-01-01 00:00:00.000000 arg_services-1.2.3/setup.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 arg_services-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-09 09:56:51.694542 arg_services-1.3.0/LICENSE
+-rw-r--r--   0        0        0      657 2023-04-09 09:56:51.694542 arg_services-1.3.0/README.md
+-rw-r--r--   0        0        0      671 2023-04-09 09:57:28.058345 arg_services-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7288 2023-04-09 09:57:27.274349 arg_services-1.3.0/src/arg_services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.262349 arg_services-1.3.0/src/arg_services/cbr/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.262349 arg_services-1.3.0/src/arg_services/cbr/v1beta/__init__.py
+-rw-r--r--   0        0        0     6996 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2.py
+-rw-r--r--   0        0        0    12124 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
+-rw-r--r--   0        0        0     2783 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
+-rw-r--r--   0        0        0      806 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3416 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2.py
+-rw-r--r--   0        0        0     3094 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi
+-rw-r--r--   0        0        0     2792 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
+-rw-r--r--   0        0        0      806 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2519 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2.py
+-rw-r--r--   0        0        0     2515 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8286 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2.py
+-rw-r--r--   0        0        0    15179 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
+-rw-r--r--   0        0        0     4628 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
+-rw-r--r--   0        0        0     1252 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.258350 arg_services-1.3.0/src/arg_services/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.258350 arg_services-1.3.0/src/arg_services/graph/v1/__init__.py
+-rw-r--r--   0        0        0    11861 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2.py
+-rw-r--r--   0        0        0    33449 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2_grpc.py
+-rw-r--r--   0        0        0      151 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.262349 arg_services-1.3.0/src/arg_services/mining/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.266349 arg_services-1.3.0/src/arg_services/mining/v1beta/__init__.py
+-rw-r--r--   0        0        0     5028 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     6692 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     4625 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0     1237 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6102 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     8973 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     4721 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0     1298 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4150 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2.py
+-rw-r--r--   0        0        0     3932 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
+-rw-r--r--   0        0        0     3092 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
+-rw-r--r--   0        0        0      961 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3812 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     4057 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     2896 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0      856 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2930 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2.py
+-rw-r--r--   0        0        0     2419 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2.pyi
+-rw-r--r--   0        0        0     2834 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py
+-rw-r--r--   0        0        0      821 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.266349 arg_services-1.3.0/src/arg_services/mining_explanation/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.266349 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/__init__.py
+-rw-r--r--   0        0        0     3371 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     3359 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     3044 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0      916 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4502 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     5167 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     3110 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0      961 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3857 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     3980 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     3112 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0      960 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.270349 arg_services-1.3.0/src/arg_services/nlp/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.270349 arg_services-1.3.0/src/arg_services/nlp/v1/__init__.py
+-rw-r--r--   0        0        0     9005 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2.py
+-rw-r--r--   0        0        0    27846 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2.pyi
+-rw-r--r--   0        0        0     6344 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.270349 arg_services-1.3.0/src/google/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:57:27.274349 arg_services-1.3.0/src/google/api/__init__.py
+-rw-r--r--   0        0        0     1813 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0     1047 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0      627 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/annotations_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2631 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/http_pb2.py
+-rw-r--r--   0        0        0    18295 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      627 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/http_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 arg_services-1.3.0/PKG-INFO
```

### Comparing `arg_services-1.2.3/LICENSE` & `arg_services-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/README.md` & `arg_services-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/pyproject.toml` & `arg_services-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "arg-services"
-version = "1.2.3"
+version = "1.3.0"
 description = "gRPC definitions for microservice-based argumentation machines"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/arg-services-python"
 include = ["src/**/*"]
 packages = [
     { include = "arg_services", from = "src" },
     { include = "google", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-grpcio = "^1.51.1"
-protobuf = "^4.21.12"
-grpcio-reflection = "^1.51.1"
-grpc-stubs = "^1.24.12"
+grpcio = "^1.53.0"
+protobuf = "^4.22.1"
+grpcio-reflection = "^1.53.0"
+grpc-stubs = "^1.53.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `arg_services-1.2.3/src/arg_services/__init__.py` & `arg_services-1.3.0/src/arg_services/__init__.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/adaptation_pb2.py` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,44 +16,45 @@
 from arg_services.nlp.v1 import nlp_pb2 as arg__services_dot_nlp_dot_v1_dot_nlp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(arg_services/cbr/v1beta/adaptation.proto\x12\x17\x61rg_services.cbr.v1beta\x1a#arg_services/cbr/v1beta/model.proto\x1a\'arg_services/cbr/v1beta/retrieval.proto\x1a\x1d\x61rg_services/nlp/v1/nlp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\xae\x03\n\x0c\x41\x64\x61ptRequest\x12\x46\n\x05\x63\x61ses\x18\x02 \x03(\x0b\x32\x30.arg_services.cbr.v1beta.AdaptRequest.CasesEntryR\x05\x63\x61ses\x12=\n\x05query\x18\x03 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05query\x12=\n\nnlp_config\x18\x05 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\tnlpConfig\x12@\n\tdirection\x18\x06 \x01(\x0e\x32\".arg_services.cbr.v1beta.DirectionR\tdirection\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x65\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x41\n\x05value\x18\x02 \x01(\x0b\x32+.arg_services.cbr.v1beta.AdaptedCaseRequestR\x05value:\x02\x38\x01\"\xf1\x01\n\rAdaptResponse\x12G\n\x05\x63\x61ses\x18\x01 \x03(\x0b\x32\x31.arg_services.cbr.v1beta.AdaptResponse.CasesEntryR\x05\x63\x61ses\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x66\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x42\n\x05value\x18\x02 \x01(\x0b\x32,.arg_services.cbr.v1beta.AdaptedCaseResponseR\x05value:\x02\x38\x01\"\xdc\x01\n\x12\x41\x64\x61ptedCaseRequest\x12;\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x04\x63\x61se\x12\x33\n\x05rules\x18\x02 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x05rules\x12H\n\x07mapping\x18\x03 \x01(\x0b\x32).arg_services.cbr.v1beta.RetrievedMappingH\x00R\x07mapping\x88\x01\x01\x42\n\n\x08_mapping\"\xd2\x03\n\x13\x41\x64\x61ptedCaseResponse\x12;\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x04\x63\x61se\x12O\n\x12\x65xtracted_concepts\x18\x02 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x11\x65xtractedConcepts\x12O\n\x12\x64iscarded_concepts\x18\x03 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x11\x64iscardedConcepts\x12\x42\n\rapplied_rules\x18\x04 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0c\x61ppliedRules\x12\x46\n\x0f\x64iscarded_rules\x18\x05 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0e\x64iscardedRules\x12P\n\x0frule_candidates\x18\x06 \x03(\x0b\x32\'.arg_services.cbr.v1beta.RuleCandidatesR\x0eruleCandidates\"z\n\x04Rule\x12\x38\n\x06source\x18\x01 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06source\x12\x38\n\x06target\x18\x02 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06target\"e\n\x07\x43oncept\x12\x14\n\x05lemma\x18\x01 \x01(\tR\x05lemma\x12.\n\x03pos\x18\x02 \x01(\x0e\x32\x1c.arg_services.cbr.v1beta.PosR\x03pos\x12\x14\n\x05score\x18\x03 \x01(\x01R\x05score\"\x84\x01\n\x0eRuleCandidates\x12\x38\n\x06source\x18\x01 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06source\x12\x38\n\x06target\x18\x02 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06target*z\n\tDirection\x12\x19\n\x15\x44IRECTION_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x44IRECTION_GENERALIZATION\x10\x01\x12\x1c\n\x18\x44IRECTION_SPECIALIZATION\x10\x02\x12\x16\n\x12\x44IRECTION_COMBINED\x10\x03*Y\n\x03Pos\x12\x13\n\x0fPOS_UNSPECIFIED\x10\x00\x12\x0c\n\x08POS_NOUN\x10\x01\x12\x0c\n\x08POS_VERB\x10\x02\x12\x11\n\rPOS_ADJECTIVE\x10\x03\x12\x0e\n\nPOS_ADVERB\x10\x04\x32\x89\x01\n\x11\x41\x64\x61ptationService\x12t\n\x05\x41\x64\x61pt\x12%.arg_services.cbr.v1beta.AdaptRequest\x1a&.arg_services.cbr.v1beta.AdaptResponse\"\x1c\x82\xd3\xe4\x93\x02\x16:\x01*\"\x11/cbr/v1beta/adaptB\xa8\x01\n\x1b\x63om.arg_services.cbr.v1betaB\x0f\x41\x64\x61ptationProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.cbr.v1beta.adaptation_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.cbr.v1beta.adaptation_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.arg_services.cbr.v1betaB\017AdaptationProtoP\001\242\002\003ACX\252\002\026ArgServices.Cbr.V1beta\312\002\026ArgServices\\Cbr\\V1beta\342\002\"ArgServices\\Cbr\\V1beta\\GPBMetadata\352\002\030ArgServices::Cbr::V1beta'
   _ADAPTREQUEST_CASESENTRY._options = None
   _ADAPTREQUEST_CASESENTRY._serialized_options = b'8\001'
   _ADAPTRESPONSE_CASESENTRY._options = None
   _ADAPTRESPONSE_CASESENTRY._serialized_options = b'8\001'
   _ADAPTATIONSERVICE.methods_by_name['Adapt']._options = None
   _ADAPTATIONSERVICE.methods_by_name['Adapt']._serialized_options = b'\202\323\344\223\002\026:\001*\"\021/cbr/v1beta/adapt'
-  _DIRECTION._serialized_start=1969
-  _DIRECTION._serialized_end=2091
-  _POS._serialized_start=2093
-  _POS._serialized_end=2182
-  _ADAPTREQUEST._serialized_start=239
-  _ADAPTREQUEST._serialized_end=669
-  _ADAPTREQUEST_CASESENTRY._serialized_start=568
-  _ADAPTREQUEST_CASESENTRY._serialized_end=669
-  _ADAPTRESPONSE._serialized_start=672
-  _ADAPTRESPONSE._serialized_end=913
-  _ADAPTRESPONSE_CASESENTRY._serialized_start=811
-  _ADAPTRESPONSE_CASESENTRY._serialized_end=913
-  _ADAPTEDCASEREQUEST._serialized_start=916
-  _ADAPTEDCASEREQUEST._serialized_end=1136
-  _ADAPTEDCASERESPONSE._serialized_start=1139
-  _ADAPTEDCASERESPONSE._serialized_end=1605
-  _RULE._serialized_start=1607
-  _RULE._serialized_end=1729
-  _CONCEPT._serialized_start=1731
-  _CONCEPT._serialized_end=1832
-  _RULECANDIDATES._serialized_start=1835
-  _RULECANDIDATES._serialized_end=1967
-  _ADAPTATIONSERVICE._serialized_start=2185
-  _ADAPTATIONSERVICE._serialized_end=2322
+  _globals['_DIRECTION']._serialized_start=1969
+  _globals['_DIRECTION']._serialized_end=2091
+  _globals['_POS']._serialized_start=2093
+  _globals['_POS']._serialized_end=2182
+  _globals['_ADAPTREQUEST']._serialized_start=239
+  _globals['_ADAPTREQUEST']._serialized_end=669
+  _globals['_ADAPTREQUEST_CASESENTRY']._serialized_start=568
+  _globals['_ADAPTREQUEST_CASESENTRY']._serialized_end=669
+  _globals['_ADAPTRESPONSE']._serialized_start=672
+  _globals['_ADAPTRESPONSE']._serialized_end=913
+  _globals['_ADAPTRESPONSE_CASESENTRY']._serialized_start=811
+  _globals['_ADAPTRESPONSE_CASESENTRY']._serialized_end=913
+  _globals['_ADAPTEDCASEREQUEST']._serialized_start=916
+  _globals['_ADAPTEDCASEREQUEST']._serialized_end=1136
+  _globals['_ADAPTEDCASERESPONSE']._serialized_start=1139
+  _globals['_ADAPTEDCASERESPONSE']._serialized_end=1605
+  _globals['_RULE']._serialized_start=1607
+  _globals['_RULE']._serialized_end=1729
+  _globals['_CONCEPT']._serialized_start=1731
+  _globals['_CONCEPT']._serialized_end=1832
+  _globals['_RULECANDIDATES']._serialized_start=1835
+  _globals['_RULECANDIDATES']._serialized_end=1967
+  _globals['_ADAPTATIONSERVICE']._serialized_start=2185
+  _globals['_ADAPTATIONSERVICE']._serialized_end=2322
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/adaptation_pb2.pyi` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/casebase_pb2.py` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 from arg_services.cbr.v1beta import model_pb2 as arg__services_dot_cbr_dot_v1beta_dot_model__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&arg_services/cbr/v1beta/casebase.proto\x12\x17\x61rg_services.cbr.v1beta\x1a#arg_services/cbr/v1beta/model.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\xc8\x01\n\x0f\x43\x61sebaseRequest\x12\x41\n\x07include\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.CasebaseFilterR\x07include\x12\x41\n\x07\x65xclude\x18\x02 \x01(\x0b\x32\'.arg_services.cbr.v1beta.CasebaseFilterR\x07\x65xclude\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xc1\x01\n\x10\x43\x61sebaseResponse\x12J\n\x05\x63\x61ses\x18\x01 \x03(\x0b\x32\x34.arg_services.cbr.v1beta.CasebaseResponse.CasesEntryR\x05\x63\x61ses\x1a\x61\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12=\n\x05value\x18\x02 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05value:\x02\x38\x01\x32\x94\x01\n\x0f\x43\x61sebaseService\x12\x80\x01\n\x08\x43\x61sebase\x12(.arg_services.cbr.v1beta.CasebaseRequest\x1a).arg_services.cbr.v1beta.CasebaseResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/cbr/v1beta/casebaseB\xa6\x01\n\x1b\x63om.arg_services.cbr.v1betaB\rCasebaseProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.cbr.v1beta.casebase_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.cbr.v1beta.casebase_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.arg_services.cbr.v1betaB\rCasebaseProtoP\001\242\002\003ACX\252\002\026ArgServices.Cbr.V1beta\312\002\026ArgServices\\Cbr\\V1beta\342\002\"ArgServices\\Cbr\\V1beta\\GPBMetadata\352\002\030ArgServices::Cbr::V1beta'
   _CASEBASERESPONSE_CASESENTRY._options = None
   _CASEBASERESPONSE_CASESENTRY._serialized_options = b'8\001'
   _CASEBASESERVICE.methods_by_name['Casebase']._options = None
   _CASEBASESERVICE.methods_by_name['Casebase']._serialized_options = b'\202\323\344\223\002\031:\001*\"\024/cbr/v1beta/casebase'
-  _CASEBASEREQUEST._serialized_start=165
-  _CASEBASEREQUEST._serialized_end=365
-  _CASEBASERESPONSE._serialized_start=368
-  _CASEBASERESPONSE._serialized_end=561
-  _CASEBASERESPONSE_CASESENTRY._serialized_start=464
-  _CASEBASERESPONSE_CASESENTRY._serialized_end=561
-  _CASEBASESERVICE._serialized_start=564
-  _CASEBASESERVICE._serialized_end=712
+  _globals['_CASEBASEREQUEST']._serialized_start=165
+  _globals['_CASEBASEREQUEST']._serialized_end=365
+  _globals['_CASEBASERESPONSE']._serialized_start=368
+  _globals['_CASEBASERESPONSE']._serialized_end=561
+  _globals['_CASEBASERESPONSE_CASESENTRY']._serialized_start=464
+  _globals['_CASEBASERESPONSE_CASESENTRY']._serialized_end=561
+  _globals['_CASEBASESERVICE']._serialized_start=564
+  _globals['_CASEBASESERVICE']._serialized_end=712
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/casebase_pb2.pyi` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/model_pb2.py` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 
 
 from arg_services.graph.v1 import graph_pb2 as arg__services_dot_graph_dot_v1_dot_graph__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#arg_services/cbr/v1beta/model.proto\x12\x17\x61rg_services.cbr.v1beta\x1a!arg_services/graph/v1/graph.proto\"X\n\x0e\x41nnotatedGraph\x12\x32\n\x05graph\x18\x01 \x01(\x0b\x32\x1c.arg_services.graph.v1.GraphR\x05graph\x12\x12\n\x04text\x18\x02 \x01(\tR\x04text\"\xc2\x01\n\x0e\x43\x61sebaseFilter\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x14\n\x05\x63\x61ses\x18\x02 \x01(\tR\x05\x63\x61ses\x12K\n\x06kwargs\x18\x03 \x03(\x0b\x32\x33.arg_services.cbr.v1beta.CasebaseFilter.KwargsEntryR\x06kwargs\x1a\x39\n\x0bKwargsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\xa3\x01\n\x1b\x63om.arg_services.cbr.v1betaB\nModelProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.cbr.v1beta.model_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.cbr.v1beta.model_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.arg_services.cbr.v1betaB\nModelProtoP\001\242\002\003ACX\252\002\026ArgServices.Cbr.V1beta\312\002\026ArgServices\\Cbr\\V1beta\342\002\"ArgServices\\Cbr\\V1beta\\GPBMetadata\352\002\030ArgServices::Cbr::V1beta'
   _CASEBASEFILTER_KWARGSENTRY._options = None
   _CASEBASEFILTER_KWARGSENTRY._serialized_options = b'8\001'
-  _ANNOTATEDGRAPH._serialized_start=99
-  _ANNOTATEDGRAPH._serialized_end=187
-  _CASEBASEFILTER._serialized_start=190
-  _CASEBASEFILTER._serialized_end=384
-  _CASEBASEFILTER_KWARGSENTRY._serialized_start=327
-  _CASEBASEFILTER_KWARGSENTRY._serialized_end=384
+  _globals['_ANNOTATEDGRAPH']._serialized_start=99
+  _globals['_ANNOTATEDGRAPH']._serialized_end=187
+  _globals['_CASEBASEFILTER']._serialized_start=190
+  _globals['_CASEBASEFILTER']._serialized_end=384
+  _globals['_CASEBASEFILTER_KWARGSENTRY']._serialized_start=327
+  _globals['_CASEBASEFILTER_KWARGSENTRY']._serialized_end=384
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/model_pb2.pyi` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/retrieval_pb2.pyi` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -128,52 +128,51 @@
 global___RetrieveRequest = RetrieveRequest
 
 @typing_extensions.final
 class RetrieveResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     QUERY_RESPONSES_FIELD_NUMBER: builtins.int
+    EXTRAS_FIELD_NUMBER: builtins.int
     @property
     def query_responses(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___QueryResponse]: ...
+    @property
+    def extras(self) -> google.protobuf.struct_pb2.Struct: ...
     def __init__(
         self,
         *,
         query_responses: collections.abc.Iterable[global___QueryResponse] | None = ...,
+        extras: google.protobuf.struct_pb2.Struct | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["query_responses", b"query_responses"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["extras", b"extras"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["extras", b"extras", "query_responses", b"query_responses"]) -> None: ...
 
 global___RetrieveResponse = RetrieveResponse
 
 @typing_extensions.final
 class QueryResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SEMANTIC_RANKING_FIELD_NUMBER: builtins.int
     STRUCTURAL_RANKING_FIELD_NUMBER: builtins.int
     STRUCTURAL_MAPPING_FIELD_NUMBER: builtins.int
-    EXTRAS_FIELD_NUMBER: builtins.int
     @property
     def semantic_ranking(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RetrievedCase]: ...
     @property
     def structural_ranking(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RetrievedCase]: ...
     @property
     def structural_mapping(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RetrievedMapping]: ...
-    @property
-    def extras(self) -> google.protobuf.struct_pb2.Struct:
-        """Implementation-specific information can be encoded here"""
     def __init__(
         self,
         *,
         semantic_ranking: collections.abc.Iterable[global___RetrievedCase] | None = ...,
         structural_ranking: collections.abc.Iterable[global___RetrievedCase] | None = ...,
         structural_mapping: collections.abc.Iterable[global___RetrievedMapping] | None = ...,
-        extras: google.protobuf.struct_pb2.Struct | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["extras", b"extras"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["extras", b"extras", "semantic_ranking", b"semantic_ranking", "structural_mapping", b"structural_mapping", "structural_ranking", b"structural_ranking"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["semantic_ranking", b"semantic_ranking", "structural_mapping", b"structural_mapping", "structural_ranking", b"structural_ranking"]) -> None: ...
 
 global___QueryResponse = QueryResponse
 
 @typing_extensions.final
 class RetrievedCase(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -233,7 +232,91 @@
         query_id: builtins.str = ...,
         case_id: builtins.str = ...,
         similarity: builtins.float = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["case_id", b"case_id", "query_id", b"query_id", "similarity", b"similarity"]) -> None: ...
 
 global___MappedElement = MappedElement
+
+@typing_extensions.final
+class SimilaritiesRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    CASES_FIELD_NUMBER: builtins.int
+    QUERY_FIELD_NUMBER: builtins.int
+    NLP_CONFIG_FIELD_NUMBER: builtins.int
+    STRUCTURAL_FIELD_NUMBER: builtins.int
+    MAPPING_ALGORITHM_FIELD_NUMBER: builtins.int
+    MAPPING_ALGORITHM_VARIANT_FIELD_NUMBER: builtins.int
+    SCHEME_HANDLING_FIELD_NUMBER: builtins.int
+    EXTRAS_FIELD_NUMBER: builtins.int
+    @property
+    def cases(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[arg_services.cbr.v1beta.model_pb2.AnnotatedGraph]: ...
+    @property
+    def query(self) -> arg_services.cbr.v1beta.model_pb2.AnnotatedGraph: ...
+    @property
+    def nlp_config(self) -> arg_services.nlp.v1.nlp_pb2.NlpConfig: ...
+    structural: builtins.bool
+    mapping_algorithm: global___MappingAlgorithm.ValueType
+    mapping_algorithm_variant: builtins.int
+    scheme_handling: global___SchemeHandling.ValueType
+    @property
+    def extras(self) -> google.protobuf.struct_pb2.Struct: ...
+    def __init__(
+        self,
+        *,
+        cases: collections.abc.Iterable[arg_services.cbr.v1beta.model_pb2.AnnotatedGraph] | None = ...,
+        query: arg_services.cbr.v1beta.model_pb2.AnnotatedGraph | None = ...,
+        nlp_config: arg_services.nlp.v1.nlp_pb2.NlpConfig | None = ...,
+        structural: builtins.bool = ...,
+        mapping_algorithm: global___MappingAlgorithm.ValueType = ...,
+        mapping_algorithm_variant: builtins.int = ...,
+        scheme_handling: global___SchemeHandling.ValueType = ...,
+        extras: google.protobuf.struct_pb2.Struct | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["extras", b"extras", "nlp_config", b"nlp_config", "query", b"query"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cases", b"cases", "extras", b"extras", "mapping_algorithm", b"mapping_algorithm", "mapping_algorithm_variant", b"mapping_algorithm_variant", "nlp_config", b"nlp_config", "query", b"query", "scheme_handling", b"scheme_handling", "structural", b"structural"]) -> None: ...
+
+global___SimilaritiesRequest = SimilaritiesRequest
+
+@typing_extensions.final
+class SimilaritiesResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    SIMILARITIES_FIELD_NUMBER: builtins.int
+    EXTRAS_FIELD_NUMBER: builtins.int
+    @property
+    def similarities(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SimilarityResponse]: ...
+    @property
+    def extras(self) -> google.protobuf.struct_pb2.Struct: ...
+    def __init__(
+        self,
+        *,
+        similarities: collections.abc.Iterable[global___SimilarityResponse] | None = ...,
+        extras: google.protobuf.struct_pb2.Struct | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["extras", b"extras"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["extras", b"extras", "similarities", b"similarities"]) -> None: ...
+
+global___SimilaritiesResponse = SimilaritiesResponse
+
+@typing_extensions.final
+class SimilarityResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    SEMANTIC_SIMILARITY_FIELD_NUMBER: builtins.int
+    STRUCTURAL_SIMILARITY_FIELD_NUMBER: builtins.int
+    STRUCTURAL_MAPPING_FIELD_NUMBER: builtins.int
+    semantic_similarity: builtins.float
+    structural_similarity: builtins.float
+    @property
+    def structural_mapping(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RetrievedMapping]: ...
+    def __init__(
+        self,
+        *,
+        semantic_similarity: builtins.float = ...,
+        structural_similarity: builtins.float = ...,
+        structural_mapping: collections.abc.Iterable[global___RetrievedMapping] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["semantic_similarity", b"semantic_similarity", "structural_mapping", b"structural_mapping", "structural_similarity", b"structural_similarity"]) -> None: ...
+
+global___SimilarityResponse = SimilarityResponse
```

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from arg_services.cbr.v1beta import retrieval_pb2 as arg__services_dot_cbr_dot_v1beta_dot_retrieval__pb2
+from arg_services.mining_explanation.v1beta import entailment_pb2 as arg__services_dot_mining__explanation_dot_v1beta_dot_entailment__pb2
 
 
-class RetrievalServiceStub(object):
+class EntailmentExplanationServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.Retrieve = channel.unary_unary(
-                '/arg_services.cbr.v1beta.RetrievalService/Retrieve',
-                request_serializer=arg__services_dot_cbr_dot_v1beta_dot_retrieval__pb2.RetrieveRequest.SerializeToString,
-                response_deserializer=arg__services_dot_cbr_dot_v1beta_dot_retrieval__pb2.RetrieveResponse.FromString,
+        self.Entailments = channel.unary_unary(
+                '/arg_services.mining_explanation.v1beta.EntailmentExplanationService/Entailments',
+                request_serializer=arg__services_dot_mining__explanation_dot_v1beta_dot_entailment__pb2.EntailmentsRequest.SerializeToString,
+                response_deserializer=arg__services_dot_mining__explanation_dot_v1beta_dot_entailment__pb2.EntailmentsResponse.FromString,
                 )
 
 
-class RetrievalServiceServicer(object):
+class EntailmentExplanationServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def Retrieve(self, request, context):
+    def Entailments(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_RetrievalServiceServicer_to_server(servicer, server):
+def add_EntailmentExplanationServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'Retrieve': grpc.unary_unary_rpc_method_handler(
-                    servicer.Retrieve,
-                    request_deserializer=arg__services_dot_cbr_dot_v1beta_dot_retrieval__pb2.RetrieveRequest.FromString,
-                    response_serializer=arg__services_dot_cbr_dot_v1beta_dot_retrieval__pb2.RetrieveResponse.SerializeToString,
+            'Entailments': grpc.unary_unary_rpc_method_handler(
+                    servicer.Entailments,
+                    request_deserializer=arg__services_dot_mining__explanation_dot_v1beta_dot_entailment__pb2.EntailmentsRequest.FromString,
+                    response_serializer=arg__services_dot_mining__explanation_dot_v1beta_dot_entailment__pb2.EntailmentsResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'arg_services.cbr.v1beta.RetrievalService', rpc_method_handlers)
+            'arg_services.mining_explanation.v1beta.EntailmentExplanationService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class RetrievalService(object):
+class EntailmentExplanationService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def Retrieve(request,
+    def Entailments(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/arg_services.cbr.v1beta.RetrievalService/Retrieve',
-            arg__services_dot_cbr_dot_v1beta_dot_retrieval__pb2.RetrieveRequest.SerializeToString,
-            arg__services_dot_cbr_dot_v1beta_dot_retrieval__pb2.RetrieveResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/arg_services.mining_explanation.v1beta.EntailmentExplanationService/Entailments',
+            arg__services_dot_mining__explanation_dot_v1beta_dot_entailment__pb2.EntailmentsRequest.SerializeToString,
+            arg__services_dot_mining__explanation_dot_v1beta_dot_entailment__pb2.EntailmentsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `arg_services-1.2.3/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,27 @@
 
 class RetrievalServiceStub:
     def __init__(self, channel: grpc.Channel) -> None: ...
     Retrieve: grpc.UnaryUnaryMultiCallable[
         arg_services.cbr.v1beta.retrieval_pb2.RetrieveRequest,
         arg_services.cbr.v1beta.retrieval_pb2.RetrieveResponse,
     ]
+    Similarities: grpc.UnaryUnaryMultiCallable[
+        arg_services.cbr.v1beta.retrieval_pb2.SimilaritiesRequest,
+        arg_services.cbr.v1beta.retrieval_pb2.SimilaritiesResponse,
+    ]
 
 class RetrievalServiceServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def Retrieve(
         self,
         request: arg_services.cbr.v1beta.retrieval_pb2.RetrieveRequest,
         context: grpc.ServicerContext,
     ) -> arg_services.cbr.v1beta.retrieval_pb2.RetrieveResponse: ...
+    @abc.abstractmethod
+    def Similarities(
+        self,
+        request: arg_services.cbr.v1beta.retrieval_pb2.SimilaritiesRequest,
+        context: grpc.ServicerContext,
+    ) -> arg_services.cbr.v1beta.retrieval_pb2.SimilaritiesResponse: ...
 
 def add_RetrievalServiceServicer_to_server(servicer: RetrievalServiceServicer, server: grpc.Server) -> None: ...
```

### Comparing `arg_services-1.2.3/src/arg_services/graph/v1/graph_pb2.py` & `arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,62 +13,63 @@
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!arg_services/graph/v1/graph.proto\x12\x15\x61rg_services.graph.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xb3\x08\n\x05Graph\x12=\n\x05nodes\x18\x01 \x03(\x0b\x32\'.arg_services.graph.v1.Graph.NodesEntryR\x05nodes\x12=\n\x05\x65\x64ges\x18\x02 \x03(\x0b\x32\'.arg_services.graph.v1.Graph.EdgesEntryR\x05\x65\x64ges\x12I\n\tresources\x18\x03 \x03(\x0b\x32+.arg_services.graph.v1.Graph.ResourcesEntryR\tresources\x12R\n\x0cparticipants\x18\x04 \x03(\x0b\x32..arg_services.graph.v1.Graph.ParticipantsEntryR\x0cparticipants\x12\x46\n\x08\x61nalysts\x18\x05 \x03(\x0b\x32*.arg_services.graph.v1.Graph.AnalystsEntryR\x08\x61nalysts\x12$\n\x0bmajor_claim\x18\x06 \x01(\tH\x00R\nmajorClaim\x88\x01\x01\x12%\n\x0eschema_version\x18\x07 \x01(\rR\rschemaVersion\x12\'\n\x0flibrary_version\x18\x08 \x01(\tR\x0elibraryVersion\x12;\n\x08metadata\x18\x0e \x01(\x0b\x32\x1f.arg_services.graph.v1.MetadataR\x08metadata\x12\x33\n\x08userdata\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x08userdata\x1aU\n\nNodesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.arg_services.graph.v1.NodeR\x05value:\x02\x38\x01\x1aU\n\nEdgesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.arg_services.graph.v1.EdgeR\x05value:\x02\x38\x01\x1a]\n\x0eResourcesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x35\n\x05value\x18\x02 \x01(\x0b\x32\x1f.arg_services.graph.v1.ResourceR\x05value:\x02\x38\x01\x1a\x63\n\x11ParticipantsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x38\n\x05value\x18\x02 \x01(\x0b\x32\".arg_services.graph.v1.ParticipantR\x05value:\x02\x38\x01\x1a[\n\rAnalystsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32\x1e.arg_services.graph.v1.AnalystR\x05value:\x02\x38\x01\x42\x0e\n\x0c_major_claim\"v\n\x08Metadata\x12\x34\n\x07\x63reated\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x34\n\x07updated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07updated\"\x97\x02\n\x08Resource\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12\x19\n\x05title\x18\x02 \x01(\tH\x00R\x05title\x88\x01\x01\x12\x1b\n\x06source\x18\x03 \x01(\tH\x01R\x06source\x88\x01\x01\x12\x38\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ttimestamp\x12;\n\x08metadata\x18\x0e \x01(\x0b\x32\x1f.arg_services.graph.v1.MetadataR\x08metadata\x12\x33\n\x08userdata\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x08userdataB\x08\n\x06_titleB\t\n\x07_source\"\xea\x02\n\x0bParticipant\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1f\n\x08username\x18\x02 \x01(\tH\x00R\x08username\x88\x01\x01\x12\x19\n\x05\x65mail\x18\x03 \x01(\tH\x01R\x05\x65mail\x88\x01\x01\x12\x15\n\x03url\x18\x04 \x01(\tH\x02R\x03url\x88\x01\x01\x12\x1f\n\x08location\x18\x05 \x01(\tH\x03R\x08location\x88\x01\x01\x12%\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x04R\x0b\x64\x65scription\x88\x01\x01\x12;\n\x08metadata\x18\x0e \x01(\x0b\x32\x1f.arg_services.graph.v1.MetadataR\x08metadata\x12\x33\n\x08userdata\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x08userdataB\x0b\n\t_usernameB\x08\n\x06_emailB\x06\n\x04_urlB\x0b\n\t_locationB\x0e\n\x0c_description\"w\n\x07\x41nalyst\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x19\n\x05\x65mail\x18\x02 \x01(\tH\x00R\x05\x65mail\x88\x01\x01\x12\x33\n\x08userdata\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x08userdataB\x08\n\x06_email\"\xa8\x01\n\x04\x45\x64ge\x12\x16\n\x06source\x18\x01 \x01(\tR\x06source\x12\x16\n\x06target\x18\x02 \x01(\tR\x06target\x12;\n\x08metadata\x18\x0e \x01(\x0b\x32\x1f.arg_services.graph.v1.MetadataR\x08metadata\x12\x33\n\x08userdata\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x08userdata\"\xec\x01\n\x04Node\x12\x31\n\x04\x61tom\x18\x01 \x01(\x0b\x32\x1b.arg_services.graph.v1.AtomH\x00R\x04\x61tom\x12\x37\n\x06scheme\x18\x02 \x01(\x0b\x32\x1d.arg_services.graph.v1.SchemeH\x00R\x06scheme\x12;\n\x08metadata\x18\x0e \x01(\x0b\x32\x1f.arg_services.graph.v1.MetadataR\x08metadata\x12\x33\n\x08userdata\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x08userdataB\x06\n\x04type\"\x91\x01\n\x04\x41tom\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12>\n\treference\x18\x02 \x01(\x0b\x32 .arg_services.graph.v1.ReferenceR\treference\x12%\n\x0bparticipant\x18\x03 \x01(\tH\x00R\x0bparticipant\x88\x01\x01\x42\x0e\n\x0c_participant\"u\n\tReference\x12\x1f\n\x08resource\x18\x01 \x01(\tH\x00R\x08resource\x88\x01\x01\x12\x1b\n\x06offset\x18\x02 \x01(\rH\x01R\x06offset\x88\x01\x01\x12\x12\n\x04text\x18\x03 \x01(\tR\x04textB\x0b\n\t_resourceB\t\n\x07_offset\"\xba\x02\n\x06Scheme\x12:\n\x07support\x18\x01 \x01(\x0e\x32\x1e.arg_services.graph.v1.SupportH\x00R\x07support\x12\x37\n\x06\x61ttack\x18\x02 \x01(\x0e\x32\x1d.arg_services.graph.v1.AttackH\x00R\x06\x61ttack\x12\x43\n\npreference\x18\x03 \x01(\x0e\x32!.arg_services.graph.v1.PreferenceH\x00R\npreference\x12=\n\x08rephrase\x18\x04 \x01(\x0e\x32\x1f.arg_services.graph.v1.RephraseH\x00R\x08rephrase\x12/\n\x13premise_descriptors\x18\x0f \x03(\tR\x12premiseDescriptorsB\x06\n\x04type*\x95\x0f\n\x07Support\x12\x13\n\x0fSUPPORT_DEFAULT\x10\x00\x12\x1c\n\x18SUPPORT_POSITION_TO_KNOW\x10\x01\x12\x1a\n\x16SUPPORT_EXPERT_OPINION\x10\x02\x12\x1d\n\x19SUPPORT_WITNESS_TESTIMONY\x10\x03\x12\x1b\n\x17SUPPORT_POPULAR_OPINION\x10\x04\x12\x1c\n\x18SUPPORT_POPULAR_PRACTICE\x10\x05\x12\x13\n\x0fSUPPORT_EXAMPLE\x10\x06\x12\x13\n\x0fSUPPORT_ANALOGY\x10\x07\x12,\n(SUPPORT_PRACTICAL_REASONING_FROM_ANALOGY\x10\x08\x12\x17\n\x13SUPPORT_COMPOSITION\x10\t\x12\x14\n\x10SUPPORT_DIVISION\x10\n\x12\x17\n\x13SUPPORT_OPPOSITIONS\x10\x0b\x12\"\n\x1eSUPPORT_RHETORICAL_OPPOSITIONS\x10\x0c\x12\x18\n\x14SUPPORT_ALTERNATIVES\x10\r\x12!\n\x1dSUPPORT_VERBAL_CLASSIFICATION\x10\x0e\x12,\n(SUPPORT_VERBAL_CLASSIFICATION_DEFINITION\x10\x0f\x12+\n\'SUPPORT_VERBAL_CLASSIFICATION_VAGUENESS\x10\x10\x12/\n+SUPPORT_VERBAL_CLASSIFICATION_ARBITRARINESS\x10\x11\x12)\n%SUPPORT_INTERACTION_OF_ACT_AND_PERSON\x10\x12\x12\x12\n\x0eSUPPORT_VALUES\x10\x13\x12\x1b\n\x17SUPPORT_POSITIVE_VALUES\x10=\x12\x1b\n\x17SUPPORT_NEGATIVE_VALUES\x10>\x12\x15\n\x11SUPPORT_SACRIFICE\x10\x14\x12%\n!SUPPORT_THE_GROUP_AND_ITS_MEMBERS\x10\x15\x12\x1f\n\x1bSUPPORT_PRACTICAL_REASONING\x10\x16\x12*\n&SUPPORT_TWO_PERSON_PRACTICAL_REASONING\x10\x17\x12\x11\n\rSUPPORT_WASTE\x10\x18\x12\x16\n\x12SUPPORT_SUNK_COSTS\x10\x19\x12\x15\n\x11SUPPORT_IGNORANCE\x10\x1a\x12\x1f\n\x1bSUPPORT_EPISTEMIC_IGNORANCE\x10\x1b\x12\x1b\n\x17SUPPORT_CAUSE_TO_EFFECT\x10\x1c\x12 \n\x1cSUPPORT_CORRELATION_TO_CAUSE\x10\x1d\x12\x10\n\x0cSUPPORT_SIGN\x10\x1e\x12\x15\n\x11SUPPORT_ABDUCTIVE\x10\x1f\x12\"\n\x1eSUPPORT_EVIDENCE_TO_HYPOTHESIS\x10 \x12\x18\n\x14SUPPORT_CONSEQUENCES\x10!\x12!\n\x1dSUPPORT_POSITIVE_CONSEQUENCES\x10?\x12!\n\x1dSUPPORT_NEGATIVE_CONSEQUENCES\x10@\x12\"\n\x1eSUPPORT_PRAGMATIC_ALTERNATIVES\x10\"\x12\x12\n\x0eSUPPORT_THREAT\x10#\x12\x17\n\x13SUPPORT_FEAR_APPEAL\x10$\x12\x19\n\x15SUPPORT_DANGER_APPEAL\x10%\x12\x19\n\x15SUPPORT_NEED_FOR_HELP\x10&\x12\x14\n\x10SUPPORT_DISTRESS\x10\'\x12\x16\n\x12SUPPORT_COMMITMENT\x10(\x12\x13\n\x0fSUPPORT_ETHOTIC\x10)\x12\x1e\n\x1aSUPPORT_GENERIC_AD_HOMINEM\x10*\x12#\n\x1fSUPPORT_PRAGMATIC_INCONSISTENCY\x10+\x12#\n\x1fSUPPORT_INCONSISTENT_COMMITMENT\x10,\x12%\n!SUPPORT_CIRCUMSTANTIAL_AD_HOMINEM\x10-\x12\x10\n\x0cSUPPORT_BIAS\x10.\x12\x1b\n\x17SUPPORT_BIAS_AD_HOMINEM\x10/\x12\x16\n\x12SUPPORT_GRADUALISM\x10\x30\x12\x1a\n\x16SUPPORT_SLIPPERY_SLOPE\x10\x31\x12$\n SUPPORT_PRECEDENT_SLIPPERY_SLOPE\x10\x32\x12\"\n\x1eSUPPORT_SORITES_SLIPPERY_SLOPE\x10\x33\x12!\n\x1dSUPPORT_VERBAL_SLIPPERY_SLOPE\x10\x34\x12\x1f\n\x1bSUPPORT_FULL_SLIPPERY_SLOPE\x10\x35\x12$\n SUPPORT_CONSTITUTIVE_RULE_CLAIMS\x10\x36\x12\x11\n\rSUPPORT_RULES\x10\x37\x12\x1c\n\x18SUPPORT_EXCEPTIONAL_CASE\x10\x38\x12\x15\n\x11SUPPORT_PRECEDENT\x10\x39\x12\x1b\n\x17SUPPORT_PLEA_FOR_EXCUSE\x10:\x12\x16\n\x12SUPPORT_PERCEPTION\x10;\x12\x12\n\x0eSUPPORT_MEMORY\x10<*\x1c\n\x06\x41ttack\x12\x12\n\x0e\x41TTACK_DEFAULT\x10\x00*$\n\nPreference\x12\x16\n\x12PREFERENCE_DEFAULT\x10\x00* \n\x08Rephrase\x12\x14\n\x10REPHRASE_DEFAULT\x10\x00\x42\x99\x01\n\x19\x63om.arg_services.graph.v1B\nGraphProtoP\x01\xa2\x02\x03\x41GX\xaa\x02\x14\x41rgServices.Graph.V1\xca\x02\x14\x41rgServices\\Graph\\V1\xe2\x02 ArgServices\\Graph\\V1\\GPBMetadata\xea\x02\x16\x41rgServices::Graph::V1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.graph.v1.graph_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.graph.v1.graph_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\031com.arg_services.graph.v1B\nGraphProtoP\001\242\002\003AGX\252\002\024ArgServices.Graph.V1\312\002\024ArgServices\\Graph\\V1\342\002 ArgServices\\Graph\\V1\\GPBMetadata\352\002\026ArgServices::Graph::V1'
   _GRAPH_NODESENTRY._options = None
   _GRAPH_NODESENTRY._serialized_options = b'8\001'
   _GRAPH_EDGESENTRY._options = None
   _GRAPH_EDGESENTRY._serialized_options = b'8\001'
   _GRAPH_RESOURCESENTRY._options = None
   _GRAPH_RESOURCESENTRY._serialized_options = b'8\001'
   _GRAPH_PARTICIPANTSENTRY._options = None
   _GRAPH_PARTICIPANTSENTRY._serialized_options = b'8\001'
   _GRAPH_ANALYSTSENTRY._options = None
   _GRAPH_ANALYSTSENTRY._serialized_options = b'8\001'
-  _SUPPORT._serialized_start=3084
-  _SUPPORT._serialized_end=5025
-  _ATTACK._serialized_start=5027
-  _ATTACK._serialized_end=5055
-  _PREFERENCE._serialized_start=5057
-  _PREFERENCE._serialized_end=5093
-  _REPHRASE._serialized_start=5095
-  _REPHRASE._serialized_end=5127
-  _GRAPH._serialized_start=124
-  _GRAPH._serialized_end=1199
-  _GRAPH_NODESENTRY._serialized_start=722
-  _GRAPH_NODESENTRY._serialized_end=807
-  _GRAPH_EDGESENTRY._serialized_start=809
-  _GRAPH_EDGESENTRY._serialized_end=894
-  _GRAPH_RESOURCESENTRY._serialized_start=896
-  _GRAPH_RESOURCESENTRY._serialized_end=989
-  _GRAPH_PARTICIPANTSENTRY._serialized_start=991
-  _GRAPH_PARTICIPANTSENTRY._serialized_end=1090
-  _GRAPH_ANALYSTSENTRY._serialized_start=1092
-  _GRAPH_ANALYSTSENTRY._serialized_end=1183
-  _METADATA._serialized_start=1201
-  _METADATA._serialized_end=1319
-  _RESOURCE._serialized_start=1322
-  _RESOURCE._serialized_end=1601
-  _PARTICIPANT._serialized_start=1604
-  _PARTICIPANT._serialized_end=1966
-  _ANALYST._serialized_start=1968
-  _ANALYST._serialized_end=2087
-  _EDGE._serialized_start=2090
-  _EDGE._serialized_end=2258
-  _NODE._serialized_start=2261
-  _NODE._serialized_end=2497
-  _ATOM._serialized_start=2500
-  _ATOM._serialized_end=2645
-  _REFERENCE._serialized_start=2647
-  _REFERENCE._serialized_end=2764
-  _SCHEME._serialized_start=2767
-  _SCHEME._serialized_end=3081
+  _globals['_SUPPORT']._serialized_start=3084
+  _globals['_SUPPORT']._serialized_end=5025
+  _globals['_ATTACK']._serialized_start=5027
+  _globals['_ATTACK']._serialized_end=5055
+  _globals['_PREFERENCE']._serialized_start=5057
+  _globals['_PREFERENCE']._serialized_end=5093
+  _globals['_REPHRASE']._serialized_start=5095
+  _globals['_REPHRASE']._serialized_end=5127
+  _globals['_GRAPH']._serialized_start=124
+  _globals['_GRAPH']._serialized_end=1199
+  _globals['_GRAPH_NODESENTRY']._serialized_start=722
+  _globals['_GRAPH_NODESENTRY']._serialized_end=807
+  _globals['_GRAPH_EDGESENTRY']._serialized_start=809
+  _globals['_GRAPH_EDGESENTRY']._serialized_end=894
+  _globals['_GRAPH_RESOURCESENTRY']._serialized_start=896
+  _globals['_GRAPH_RESOURCESENTRY']._serialized_end=989
+  _globals['_GRAPH_PARTICIPANTSENTRY']._serialized_start=991
+  _globals['_GRAPH_PARTICIPANTSENTRY']._serialized_end=1090
+  _globals['_GRAPH_ANALYSTSENTRY']._serialized_start=1092
+  _globals['_GRAPH_ANALYSTSENTRY']._serialized_end=1183
+  _globals['_METADATA']._serialized_start=1201
+  _globals['_METADATA']._serialized_end=1319
+  _globals['_RESOURCE']._serialized_start=1322
+  _globals['_RESOURCE']._serialized_end=1601
+  _globals['_PARTICIPANT']._serialized_start=1604
+  _globals['_PARTICIPANT']._serialized_end=1966
+  _globals['_ANALYST']._serialized_start=1968
+  _globals['_ANALYST']._serialized_end=2087
+  _globals['_EDGE']._serialized_start=2090
+  _globals['_EDGE']._serialized_end=2258
+  _globals['_NODE']._serialized_start=2261
+  _globals['_NODE']._serialized_end=2497
+  _globals['_ATOM']._serialized_start=2500
+  _globals['_ATOM']._serialized_end=2645
+  _globals['_REFERENCE']._serialized_start=2647
+  _globals['_REFERENCE']._serialized_end=2764
+  _globals['_SCHEME']._serialized_start=2767
+  _globals['_SCHEME']._serialized_end=3081
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/graph/v1/graph_pb2.pyi` & `arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/adu_pb2.py` & `arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,38 +13,39 @@
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$arg_services/mining/v1beta/adu.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"Z\n\x13SegmentationRequest\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x88\x01\n\x14SegmentationResponse\x12?\n\x08segments\x18\x01 \x03(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"E\n\x07Segment\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12\x14\n\x05start\x18\x02 \x01(\x04R\x05start\x12\x10\n\x03\x65nd\x18\x03 \x01(\x04R\x03\x65nd\"\xe2\x01\n\x15\x43lassificationRequest\x12[\n\x08segments\x18\x01 \x03(\x0b\x32?.arg_services.mining.v1beta.ClassificationRequest.SegmentsEntryR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a;\n\rSegmentsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"~\n\x16\x43lassificationResponse\x12\x33\n\x04\x61\x64us\x18\x01 \x03(\x0b\x32\x1f.arg_services.mining.v1beta.AduR\x04\x61\x64us\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"_\n\x03\x41\x64u\x12\x1d\n\nsegment_id\x18\x01 \x01(\tR\tsegmentId\x12\x39\n\x06tokens\x18\x02 \x03(\x0b\x32!.arg_services.mining.v1beta.TokenR\x06tokens\"[\n\x05Token\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12$\n\rargumentative\x18\x02 \x01(\x08R\rargumentative\x12\x18\n\x07keyword\x18\x03 \x01(\x08R\x07keyword2\xd4\x02\n\nAduService\x12\x9d\x01\n\x0cSegmentation\x12/.arg_services.mining.v1beta.SegmentationRequest\x1a\x30.arg_services.mining.v1beta.SegmentationResponse\"*\x82\xd3\xe4\x93\x02$:\x01*\"\x1f/mining/v1beta/adu/segmentation\x12\xa5\x01\n\x0e\x43lassification\x12\x31.arg_services.mining.v1beta.ClassificationRequest\x1a\x32.arg_services.mining.v1beta.ClassificationResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/mining/v1beta/adu/classificationB\xb0\x01\n\x1e\x63om.arg_services.mining.v1betaB\x08\x41\x64uProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.adu_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.adu_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.arg_services.mining.v1betaB\010AduProtoP\001\242\002\003AMX\252\002\031ArgServices.Mining.V1beta\312\002\031ArgServices\\Mining\\V1beta\342\002%ArgServices\\Mining\\V1beta\\GPBMetadata\352\002\033ArgServices::Mining::V1beta'
   _CLASSIFICATIONREQUEST_SEGMENTSENTRY._options = None
   _CLASSIFICATIONREQUEST_SEGMENTSENTRY._serialized_options = b'8\001'
   _ADUSERVICE.methods_by_name['Segmentation']._options = None
   _ADUSERVICE.methods_by_name['Segmentation']._serialized_options = b'\202\323\344\223\002$:\001*\"\037/mining/v1beta/adu/segmentation'
   _ADUSERVICE.methods_by_name['Classification']._options = None
   _ADUSERVICE.methods_by_name['Classification']._serialized_options = b'\202\323\344\223\002&:\001*\"!/mining/v1beta/adu/classification'
-  _SEGMENTATIONREQUEST._serialized_start=128
-  _SEGMENTATIONREQUEST._serialized_end=218
-  _SEGMENTATIONRESPONSE._serialized_start=221
-  _SEGMENTATIONRESPONSE._serialized_end=357
-  _SEGMENT._serialized_start=359
-  _SEGMENT._serialized_end=428
-  _CLASSIFICATIONREQUEST._serialized_start=431
-  _CLASSIFICATIONREQUEST._serialized_end=657
-  _CLASSIFICATIONREQUEST_SEGMENTSENTRY._serialized_start=598
-  _CLASSIFICATIONREQUEST_SEGMENTSENTRY._serialized_end=657
-  _CLASSIFICATIONRESPONSE._serialized_start=659
-  _CLASSIFICATIONRESPONSE._serialized_end=785
-  _ADU._serialized_start=787
-  _ADU._serialized_end=882
-  _TOKEN._serialized_start=884
-  _TOKEN._serialized_end=975
-  _ADUSERVICE._serialized_start=978
-  _ADUSERVICE._serialized_end=1318
+  _globals['_SEGMENTATIONREQUEST']._serialized_start=128
+  _globals['_SEGMENTATIONREQUEST']._serialized_end=218
+  _globals['_SEGMENTATIONRESPONSE']._serialized_start=221
+  _globals['_SEGMENTATIONRESPONSE']._serialized_end=357
+  _globals['_SEGMENT']._serialized_start=359
+  _globals['_SEGMENT']._serialized_end=428
+  _globals['_CLASSIFICATIONREQUEST']._serialized_start=431
+  _globals['_CLASSIFICATIONREQUEST']._serialized_end=657
+  _globals['_CLASSIFICATIONREQUEST_SEGMENTSENTRY']._serialized_start=598
+  _globals['_CLASSIFICATIONREQUEST_SEGMENTSENTRY']._serialized_end=657
+  _globals['_CLASSIFICATIONRESPONSE']._serialized_start=659
+  _globals['_CLASSIFICATIONRESPONSE']._serialized_end=785
+  _globals['_ADU']._serialized_start=787
+  _globals['_ADU']._serialized_end=882
+  _globals['_TOKEN']._serialized_start=884
+  _globals['_TOKEN']._serialized_end=975
+  _globals['_ADUSERVICE']._serialized_start=978
+  _globals['_ADUSERVICE']._serialized_end=1318
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/adu_pb2.pyi` & `arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/adu_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/entailment_pb2.py` & `arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,40 +14,41 @@
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from arg_services.mining.v1beta import adu_pb2 as arg__services_dot_mining_dot_v1beta_dot_adu__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+arg_services/mining/v1beta/entailment.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a$arg_services/mining/v1beta/adu.proto\x1a\x1cgoogle/api/annotations.proto\"\x90\x01\n\x11\x45ntailmentRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12\x18\n\x07premise\x18\x02 \x01(\tR\x07premise\x12\x14\n\x05\x63laim\x18\x03 \x01(\tR\x05\x63laim\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xee\x01\n\x12\x45ntailmentResponse\x12S\n\x0f\x65ntailment_type\x18\x01 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x0e\x65ntailmentType\x12R\n\x0bpredictions\x18\x02 \x03(\x0b\x32\x30.arg_services.mining.v1beta.EntailmentPredictionR\x0bpredictions\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x9d\x02\n\x12\x45ntailmentsRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12X\n\x08segments\x18\x02 \x03(\x0b\x32<.arg_services.mining.v1beta.EntailmentsRequest.SegmentsEntryR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a`\n\rSegmentsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x05value:\x02\x38\x01\"\x8e\x01\n\x13\x45ntailmentsResponse\x12\x46\n\x07results\x18\x01 \x03(\x0b\x32,.arg_services.mining.v1beta.EntailmentResultR\x07results\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xae\x01\n\x10\x45ntailmentResult\x12\x46\n\nentailment\x18\x01 \x01(\x0b\x32&.arg_services.mining.v1beta.EntailmentR\nentailment\x12R\n\x0bpredictions\x18\x02 \x03(\x0b\x32\x30.arg_services.mining.v1beta.EntailmentPredictionR\x0bpredictions\"\x86\x01\n\nEntailment\x12\x1d\n\npremise_id\x18\x01 \x01(\tR\tpremiseId\x12\x19\n\x08\x63laim_id\x18\x02 \x01(\tR\x07\x63laimId\x12>\n\x04type\x18\x03 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x04type\"x\n\x14\x45ntailmentPrediction\x12 \n\x0bprobability\x18\x01 \x01(\x01R\x0bprobability\x12>\n\x04type\x18\x02 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x04type*\x91\x01\n\x0e\x45ntailmentType\x12\x1f\n\x1b\x45NTAILMENT_TYPE_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x45NTAILMENT_TYPE_ENTAILMENT\x10\x01\x12!\n\x1d\x45NTAILMENT_TYPE_CONTRADICTION\x10\x02\x12\x1b\n\x17\x45NTAILMENT_TYPE_NEUTRAL\x10\x03\x32\xbf\x02\n\x11\x45ntailmentService\x12\x91\x01\n\nEntailment\x12-.arg_services.mining.v1beta.EntailmentRequest\x1a..arg_services.mining.v1beta.EntailmentResponse\"$\x82\xd3\xe4\x93\x02\x1e:\x01*\"\x19/mining/v1beta/entailment\x12\x95\x01\n\x0b\x45ntailments\x12..arg_services.mining.v1beta.EntailmentsRequest\x1a/.arg_services.mining.v1beta.EntailmentsResponse\"%\x82\xd3\xe4\x93\x02\x1f:\x01*\"\x1a/mining/v1beta/entailmentsB\xb7\x01\n\x1e\x63om.arg_services.mining.v1betaB\x0f\x45ntailmentProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.entailment_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.entailment_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.arg_services.mining.v1betaB\017EntailmentProtoP\001\242\002\003AMX\252\002\031ArgServices.Mining.V1beta\312\002\031ArgServices\\Mining\\V1beta\342\002%ArgServices\\Mining\\V1beta\\GPBMetadata\352\002\033ArgServices::Mining::V1beta'
   _ENTAILMENTSREQUEST_SEGMENTSENTRY._options = None
   _ENTAILMENTSREQUEST_SEGMENTSENTRY._serialized_options = b'8\001'
   _ENTAILMENTSERVICE.methods_by_name['Entailment']._options = None
   _ENTAILMENTSERVICE.methods_by_name['Entailment']._serialized_options = b'\202\323\344\223\002\036:\001*\"\031/mining/v1beta/entailment'
   _ENTAILMENTSERVICE.methods_by_name['Entailments']._options = None
   _ENTAILMENTSERVICE.methods_by_name['Entailments']._serialized_options = b'\202\323\344\223\002\037:\001*\"\032/mining/v1beta/entailments'
-  _ENTAILMENTTYPE._serialized_start=1431
-  _ENTAILMENTTYPE._serialized_end=1576
-  _ENTAILMENTREQUEST._serialized_start=174
-  _ENTAILMENTREQUEST._serialized_end=318
-  _ENTAILMENTRESPONSE._serialized_start=321
-  _ENTAILMENTRESPONSE._serialized_end=559
-  _ENTAILMENTSREQUEST._serialized_start=562
-  _ENTAILMENTSREQUEST._serialized_end=847
-  _ENTAILMENTSREQUEST_SEGMENTSENTRY._serialized_start=751
-  _ENTAILMENTSREQUEST_SEGMENTSENTRY._serialized_end=847
-  _ENTAILMENTSRESPONSE._serialized_start=850
-  _ENTAILMENTSRESPONSE._serialized_end=992
-  _ENTAILMENTRESULT._serialized_start=995
-  _ENTAILMENTRESULT._serialized_end=1169
-  _ENTAILMENT._serialized_start=1172
-  _ENTAILMENT._serialized_end=1306
-  _ENTAILMENTPREDICTION._serialized_start=1308
-  _ENTAILMENTPREDICTION._serialized_end=1428
-  _ENTAILMENTSERVICE._serialized_start=1579
-  _ENTAILMENTSERVICE._serialized_end=1898
+  _globals['_ENTAILMENTTYPE']._serialized_start=1431
+  _globals['_ENTAILMENTTYPE']._serialized_end=1576
+  _globals['_ENTAILMENTREQUEST']._serialized_start=174
+  _globals['_ENTAILMENTREQUEST']._serialized_end=318
+  _globals['_ENTAILMENTRESPONSE']._serialized_start=321
+  _globals['_ENTAILMENTRESPONSE']._serialized_end=559
+  _globals['_ENTAILMENTSREQUEST']._serialized_start=562
+  _globals['_ENTAILMENTSREQUEST']._serialized_end=847
+  _globals['_ENTAILMENTSREQUEST_SEGMENTSENTRY']._serialized_start=751
+  _globals['_ENTAILMENTSREQUEST_SEGMENTSENTRY']._serialized_end=847
+  _globals['_ENTAILMENTSRESPONSE']._serialized_start=850
+  _globals['_ENTAILMENTSRESPONSE']._serialized_end=992
+  _globals['_ENTAILMENTRESULT']._serialized_start=995
+  _globals['_ENTAILMENTRESULT']._serialized_end=1169
+  _globals['_ENTAILMENT']._serialized_start=1172
+  _globals['_ENTAILMENT']._serialized_end=1306
+  _globals['_ENTAILMENTPREDICTION']._serialized_start=1308
+  _globals['_ENTAILMENTPREDICTION']._serialized_end=1428
+  _globals['_ENTAILMENTSERVICE']._serialized_start=1579
+  _globals['_ENTAILMENTSERVICE']._serialized_end=1898
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/entailment_pb2.pyi` & `arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/entailment_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/graph_construction_pb2.py` & `arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 from arg_services.mining.v1beta import entailment_pb2 as arg__services_dot_mining_dot_v1beta_dot_entailment__pb2
 from arg_services.graph.v1 import graph_pb2 as arg__services_dot_graph_dot_v1_dot_graph__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3arg_services/mining/v1beta/graph_construction.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a$arg_services/mining/v1beta/adu.proto\x1a+arg_services/mining/v1beta/entailment.proto\x1a!arg_services/graph/v1/graph.proto\x1a\x1cgoogle/api/annotations.proto\"\x89\x03\n\x18GraphConstructionRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12R\n\x04\x61\x64us\x18\x02 \x03(\x0b\x32>.arg_services.mining.v1beta.GraphConstructionRequest.AdusEntryR\x04\x61\x64us\x12$\n\x0emajor_claim_id\x18\x03 \x01(\tR\x0cmajorClaimId\x12H\n\x0b\x65ntailments\x18\x04 \x03(\x0b\x32&.arg_services.mining.v1beta.EntailmentR\x0b\x65ntailments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\\\n\tAdusEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x05value:\x02\x38\x01\"\x80\x01\n\x19GraphConstructionResponse\x12\x32\n\x05graph\x18\x01 \x01(\x0b\x32\x1c.arg_services.graph.v1.GraphR\x05graph\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras2\xcb\x01\n\x18GraphConstructionService\x12\xae\x01\n\x11GraphConstruction\x12\x34.arg_services.mining.v1beta.GraphConstructionRequest\x1a\x35.arg_services.mining.v1beta.GraphConstructionResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/mining/v1beta/graph_constructionB\xbe\x01\n\x1e\x63om.arg_services.mining.v1betaB\x16GraphConstructionProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.graph_construction_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.graph_construction_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.arg_services.mining.v1betaB\026GraphConstructionProtoP\001\242\002\003AMX\252\002\031ArgServices.Mining.V1beta\312\002\031ArgServices\\Mining\\V1beta\342\002%ArgServices\\Mining\\V1beta\\GPBMetadata\352\002\033ArgServices::Mining::V1beta'
   _GRAPHCONSTRUCTIONREQUEST_ADUSENTRY._options = None
   _GRAPHCONSTRUCTIONREQUEST_ADUSENTRY._serialized_options = b'8\001'
   _GRAPHCONSTRUCTIONSERVICE.methods_by_name['GraphConstruction']._options = None
   _GRAPHCONSTRUCTIONSERVICE.methods_by_name['GraphConstruction']._serialized_options = b'\202\323\344\223\002&:\001*\"!/mining/v1beta/graph_construction'
-  _GRAPHCONSTRUCTIONREQUEST._serialized_start=262
-  _GRAPHCONSTRUCTIONREQUEST._serialized_end=655
-  _GRAPHCONSTRUCTIONREQUEST_ADUSENTRY._serialized_start=563
-  _GRAPHCONSTRUCTIONREQUEST_ADUSENTRY._serialized_end=655
-  _GRAPHCONSTRUCTIONRESPONSE._serialized_start=658
-  _GRAPHCONSTRUCTIONRESPONSE._serialized_end=786
-  _GRAPHCONSTRUCTIONSERVICE._serialized_start=789
-  _GRAPHCONSTRUCTIONSERVICE._serialized_end=992
+  _globals['_GRAPHCONSTRUCTIONREQUEST']._serialized_start=262
+  _globals['_GRAPHCONSTRUCTIONREQUEST']._serialized_end=655
+  _globals['_GRAPHCONSTRUCTIONREQUEST_ADUSENTRY']._serialized_start=563
+  _globals['_GRAPHCONSTRUCTIONREQUEST_ADUSENTRY']._serialized_end=655
+  _globals['_GRAPHCONSTRUCTIONRESPONSE']._serialized_start=658
+  _globals['_GRAPHCONSTRUCTIONRESPONSE']._serialized_end=786
+  _globals['_GRAPHCONSTRUCTIONSERVICE']._serialized_start=789
+  _globals['_GRAPHCONSTRUCTIONSERVICE']._serialized_end=992
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/graph_construction_pb2.pyi` & `arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/major_claim_pb2.py` & `arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from arg_services.mining.v1beta import adu_pb2 as arg__services_dot_mining_dot_v1beta_dot_adu__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,arg_services/mining/v1beta/major_claim.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a$arg_services/mining/v1beta/adu.proto\x1a\x1cgoogle/api/annotations.proto\"\xb1\x02\n\x11MajorClaimRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12W\n\x08segments\x18\x02 \x03(\x0b\x32;.arg_services.mining.v1beta.MajorClaimRequest.SegmentsEntryR\x08segments\x12\x14\n\x05limit\x18\x04 \x01(\x04R\x05limit\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a`\n\rSegmentsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x05value:\x02\x38\x01\"\x8d\x01\n\x12MajorClaimResponse\x12\x46\n\x07ranking\x18\x01 \x03(\x0b\x32,.arg_services.mining.v1beta.MajorClaimResultR\x07ranking\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"D\n\x10MajorClaimResult\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12 \n\x0bprobability\x18\x02 \x01(\x01R\x0bprobability2\xa8\x01\n\x11MajorClaimService\x12\x92\x01\n\nMajorClaim\x12-.arg_services.mining.v1beta.MajorClaimRequest\x1a..arg_services.mining.v1beta.MajorClaimResponse\"%\x82\xd3\xe4\x93\x02\x1f:\x01*\"\x1a/mining/v1beta/major_claimB\xb7\x01\n\x1e\x63om.arg_services.mining.v1betaB\x0fMajorClaimProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.major_claim_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.major_claim_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.arg_services.mining.v1betaB\017MajorClaimProtoP\001\242\002\003AMX\252\002\031ArgServices.Mining.V1beta\312\002\031ArgServices\\Mining\\V1beta\342\002%ArgServices\\Mining\\V1beta\\GPBMetadata\352\002\033ArgServices::Mining::V1beta'
   _MAJORCLAIMREQUEST_SEGMENTSENTRY._options = None
   _MAJORCLAIMREQUEST_SEGMENTSENTRY._serialized_options = b'8\001'
   _MAJORCLAIMSERVICE.methods_by_name['MajorClaim']._options = None
   _MAJORCLAIMSERVICE.methods_by_name['MajorClaim']._serialized_options = b'\202\323\344\223\002\037:\001*\"\032/mining/v1beta/major_claim'
-  _MAJORCLAIMREQUEST._serialized_start=175
-  _MAJORCLAIMREQUEST._serialized_end=480
-  _MAJORCLAIMREQUEST_SEGMENTSENTRY._serialized_start=384
-  _MAJORCLAIMREQUEST_SEGMENTSENTRY._serialized_end=480
-  _MAJORCLAIMRESPONSE._serialized_start=483
-  _MAJORCLAIMRESPONSE._serialized_end=624
-  _MAJORCLAIMRESULT._serialized_start=626
-  _MAJORCLAIMRESULT._serialized_end=694
-  _MAJORCLAIMSERVICE._serialized_start=697
-  _MAJORCLAIMSERVICE._serialized_end=865
+  _globals['_MAJORCLAIMREQUEST']._serialized_start=175
+  _globals['_MAJORCLAIMREQUEST']._serialized_end=480
+  _globals['_MAJORCLAIMREQUEST_SEGMENTSENTRY']._serialized_start=384
+  _globals['_MAJORCLAIMREQUEST_SEGMENTSENTRY']._serialized_end=480
+  _globals['_MAJORCLAIMRESPONSE']._serialized_start=483
+  _globals['_MAJORCLAIMRESPONSE']._serialized_end=624
+  _globals['_MAJORCLAIMRESULT']._serialized_start=626
+  _globals['_MAJORCLAIMRESULT']._serialized_end=694
+  _globals['_MAJORCLAIMSERVICE']._serialized_start=697
+  _globals['_MAJORCLAIMSERVICE']._serialized_end=865
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/major_claim_pb2.pyi` & `arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/mining_pb2.py` & `arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from arg_services.graph.v1 import graph_pb2 as arg__services_dot_graph_dot_v1_dot_graph__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'arg_services/mining/v1beta/mining.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a!arg_services/graph/v1/graph.proto\x1a\x1cgoogle/api/annotations.proto\"[\n\x12RunPipelineRequest\x12\x14\n\x05texts\x18\x01 \x03(\tR\x05texts\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"|\n\x13RunPipelineResponse\x12\x34\n\x06graphs\x18\x01 \x03(\x0b\x32\x1c.arg_services.graph.v1.GraphR\x06graphs\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras2\xa8\x01\n\rMiningService\x12\x96\x01\n\x0bRunPipeline\x12..arg_services.mining.v1beta.RunPipelineRequest\x1a/.arg_services.mining.v1beta.RunPipelineResponse\"&\x82\xd3\xe4\x93\x02 :\x01*\"\x1b/mining/v1beta/run_pipelineB\xb3\x01\n\x1e\x63om.arg_services.mining.v1betaB\x0bMiningProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.mining_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.mining_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.arg_services.mining.v1betaB\013MiningProtoP\001\242\002\003AMX\252\002\031ArgServices.Mining.V1beta\312\002\031ArgServices\\Mining\\V1beta\342\002%ArgServices\\Mining\\V1beta\\GPBMetadata\352\002\033ArgServices::Mining::V1beta'
   _MININGSERVICE.methods_by_name['RunPipeline']._options = None
   _MININGSERVICE.methods_by_name['RunPipeline']._serialized_options = b'\202\323\344\223\002 :\001*\"\033/mining/v1beta/run_pipeline'
-  _RUNPIPELINEREQUEST._serialized_start=166
-  _RUNPIPELINEREQUEST._serialized_end=257
-  _RUNPIPELINERESPONSE._serialized_start=259
-  _RUNPIPELINERESPONSE._serialized_end=383
-  _MININGSERVICE._serialized_start=386
-  _MININGSERVICE._serialized_end=554
+  _globals['_RUNPIPELINEREQUEST']._serialized_start=166
+  _globals['_RUNPIPELINEREQUEST']._serialized_end=257
+  _globals['_RUNPIPELINERESPONSE']._serialized_start=259
+  _globals['_RUNPIPELINERESPONSE']._serialized_end=383
+  _globals['_MININGSERVICE']._serialized_start=386
+  _globals['_MININGSERVICE']._serialized_end=554
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/mining_pb2.pyi` & `arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/mining_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/adu_pb2.py` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0arg_services/mining_explanation/v1beta/adu.proto\x12&arg_services.mining_explanation.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\x80\x01\n\x15\x43lassificationRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12\x1a\n\x08segments\x18\x02 \x03(\tR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x96\x01\n\x16\x43lassificationResponse\x12K\n\x08segments\x18\x01 \x03(\x0b\x32/.arg_services.mining_explanation.v1beta.SegmentR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"L\n\x07Segment\x12\'\n\x0fkeyword_markers\x18\x01 \x03(\x08R\x0ekeywordMarkers\x12\x18\n\x07\x63lauses\x18\x02 \x03(\tR\x07\x63lauses2\xe3\x01\n\x15\x41\x64uExplanationService\x12\xc9\x01\n\x0e\x43lassification\x12=.arg_services.mining_explanation.v1beta.ClassificationRequest\x1a>.arg_services.mining_explanation.v1beta.ClassificationResponse\"8\x82\xd3\xe4\x93\x02\x32:\x01*\"-/mining_explanation/v1beta/adu/classificationB\xe8\x01\n*com.arg_services.mining_explanation.v1betaB\x08\x41\x64uProtoP\x01\xa2\x02\x03\x41MX\xaa\x02$ArgServices.MiningExplanation.V1beta\xca\x02$ArgServices\\MiningExplanation\\V1beta\xe2\x02\x30\x41rgServices\\MiningExplanation\\V1beta\\GPBMetadata\xea\x02&ArgServices::MiningExplanation::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining_explanation.v1beta.adu_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining_explanation.v1beta.adu_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n*com.arg_services.mining_explanation.v1betaB\010AduProtoP\001\242\002\003AMX\252\002$ArgServices.MiningExplanation.V1beta\312\002$ArgServices\\MiningExplanation\\V1beta\342\0020ArgServices\\MiningExplanation\\V1beta\\GPBMetadata\352\002&ArgServices::MiningExplanation::V1beta'
   _ADUEXPLANATIONSERVICE.methods_by_name['Classification']._options = None
   _ADUEXPLANATIONSERVICE.methods_by_name['Classification']._serialized_options = b'\202\323\344\223\0022:\001*\"-/mining_explanation/v1beta/adu/classification'
-  _CLASSIFICATIONREQUEST._serialized_start=153
-  _CLASSIFICATIONREQUEST._serialized_end=281
-  _CLASSIFICATIONRESPONSE._serialized_start=284
-  _CLASSIFICATIONRESPONSE._serialized_end=434
-  _SEGMENT._serialized_start=436
-  _SEGMENT._serialized_end=512
-  _ADUEXPLANATIONSERVICE._serialized_start=515
-  _ADUEXPLANATIONSERVICE._serialized_end=742
+  _globals['_CLASSIFICATIONREQUEST']._serialized_start=153
+  _globals['_CLASSIFICATIONREQUEST']._serialized_end=281
+  _globals['_CLASSIFICATIONRESPONSE']._serialized_start=284
+  _globals['_CLASSIFICATIONRESPONSE']._serialized_end=434
+  _globals['_SEGMENT']._serialized_start=436
+  _globals['_SEGMENT']._serialized_end=512
+  _globals['_ADUEXPLANATIONSERVICE']._serialized_start=515
+  _globals['_ADUEXPLANATIONSERVICE']._serialized_end=742
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/entailment_pb2.py` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,30 +14,31 @@
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from arg_services.mining.v1beta import entailment_pb2 as arg__services_dot_mining_dot_v1beta_dot_entailment__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7arg_services/mining_explanation/v1beta/entailment.proto\x12&arg_services.mining_explanation.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a+arg_services/mining/v1beta/entailment.proto\x1a\x1cgoogle/api/annotations.proto\"\xb7\x01\n\x12\x45ntailmentsRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12T\n\x0b\x65ntailments\x18\x02 \x03(\x0b\x32\x32.arg_services.mining_explanation.v1beta.EntailmentR\x0b\x65ntailments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x9a\x01\n\x13\x45ntailmentsResponse\x12R\n\x07results\x18\x01 \x03(\x0b\x32\x38.arg_services.mining_explanation.v1beta.EntailmentResultR\x07results\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"|\n\nEntailment\x12\x18\n\x07premise\x18\x01 \x01(\tR\x07premise\x12\x14\n\x05\x63laim\x18\x02 \x01(\tR\x05\x63laim\x12>\n\x04type\x18\x03 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x04type\"\x95\x02\n\x10\x45ntailmentResult\x12n\n\x0csimilarities\x18\x01 \x03(\x0b\x32J.arg_services.mining_explanation.v1beta.EntailmentResult.SimilaritiesEntryR\x0csimilarities\x12)\n\x10keywords_premise\x18\x02 \x03(\x08R\x0fkeywordsPremise\x12%\n\x0ekeywords_claim\x18\x03 \x03(\x08R\rkeywordsClaim\x1a?\n\x11SimilaritiesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x01R\x05value:\x02\x38\x01\x32\xda\x01\n\x1c\x45ntailmentExplanationService\x12\xb9\x01\n\x0b\x45ntailments\x12:.arg_services.mining_explanation.v1beta.EntailmentsRequest\x1a;.arg_services.mining_explanation.v1beta.EntailmentsResponse\"1\x82\xd3\xe4\x93\x02+:\x01*\"&/mining_explanation/v1beta/entailmentsB\xef\x01\n*com.arg_services.mining_explanation.v1betaB\x0f\x45ntailmentProtoP\x01\xa2\x02\x03\x41MX\xaa\x02$ArgServices.MiningExplanation.V1beta\xca\x02$ArgServices\\MiningExplanation\\V1beta\xe2\x02\x30\x41rgServices\\MiningExplanation\\V1beta\\GPBMetadata\xea\x02&ArgServices::MiningExplanation::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining_explanation.v1beta.entailment_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining_explanation.v1beta.entailment_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n*com.arg_services.mining_explanation.v1betaB\017EntailmentProtoP\001\242\002\003AMX\252\002$ArgServices.MiningExplanation.V1beta\312\002$ArgServices\\MiningExplanation\\V1beta\342\0020ArgServices\\MiningExplanation\\V1beta\\GPBMetadata\352\002&ArgServices::MiningExplanation::V1beta'
   _ENTAILMENTRESULT_SIMILARITIESENTRY._options = None
   _ENTAILMENTRESULT_SIMILARITIESENTRY._serialized_options = b'8\001'
   _ENTAILMENTEXPLANATIONSERVICE.methods_by_name['Entailments']._options = None
   _ENTAILMENTEXPLANATIONSERVICE.methods_by_name['Entailments']._serialized_options = b'\202\323\344\223\002+:\001*\"&/mining_explanation/v1beta/entailments'
-  _ENTAILMENTSREQUEST._serialized_start=205
-  _ENTAILMENTSREQUEST._serialized_end=388
-  _ENTAILMENTSRESPONSE._serialized_start=391
-  _ENTAILMENTSRESPONSE._serialized_end=545
-  _ENTAILMENT._serialized_start=547
-  _ENTAILMENT._serialized_end=671
-  _ENTAILMENTRESULT._serialized_start=674
-  _ENTAILMENTRESULT._serialized_end=951
-  _ENTAILMENTRESULT_SIMILARITIESENTRY._serialized_start=888
-  _ENTAILMENTRESULT_SIMILARITIESENTRY._serialized_end=951
-  _ENTAILMENTEXPLANATIONSERVICE._serialized_start=954
-  _ENTAILMENTEXPLANATIONSERVICE._serialized_end=1172
+  _globals['_ENTAILMENTSREQUEST']._serialized_start=205
+  _globals['_ENTAILMENTSREQUEST']._serialized_end=388
+  _globals['_ENTAILMENTSRESPONSE']._serialized_start=391
+  _globals['_ENTAILMENTSRESPONSE']._serialized_end=545
+  _globals['_ENTAILMENT']._serialized_start=547
+  _globals['_ENTAILMENT']._serialized_end=671
+  _globals['_ENTAILMENTRESULT']._serialized_start=674
+  _globals['_ENTAILMENTRESULT']._serialized_end=951
+  _globals['_ENTAILMENTRESULT_SIMILARITIESENTRY']._serialized_start=888
+  _globals['_ENTAILMENTRESULT_SIMILARITIESENTRY']._serialized_end=951
+  _globals['_ENTAILMENTEXPLANATIONSERVICE']._serialized_start=954
+  _globals['_ENTAILMENTEXPLANATIONSERVICE']._serialized_end=1172
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,28 +13,29 @@
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8arg_services/mining_explanation/v1beta/major_claim.proto\x12&arg_services.mining_explanation.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\x83\x01\n\x11MajorClaimRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12!\n\x0cmajor_claims\x18\x02 \x03(\tR\x0bmajorClaims\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xa2\x01\n\x12MajorClaimResponse\x12[\n\x0cmajor_claims\x18\x01 \x03(\x0b\x32\x38.arg_services.mining_explanation.v1beta.MajorClaimResultR\x0bmajorClaims\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xdf\x01\n\x10MajorClaimResult\x12n\n\x0csimilarities\x18\x01 \x03(\x0b\x32J.arg_services.mining_explanation.v1beta.MajorClaimResult.SimilaritiesEntryR\x0csimilarities\x12\x1a\n\x08keywords\x18\x02 \x03(\x08R\x08keywords\x1a?\n\x11SimilaritiesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x01R\x05value:\x02\x38\x01\x32\xc0\x01\n\x1cMajorClaimExplanationService\x12\x9f\x01\n\nMajorClaim\x12\x39.arg_services.mining_explanation.v1beta.MajorClaimRequest\x1a:.arg_services.mining_explanation.v1beta.MajorClaimResponse\"\x1a\x82\xd3\xe4\x93\x02\x14:\x01*\"\x0f/nlp/v1/vectorsB\xef\x01\n*com.arg_services.mining_explanation.v1betaB\x0fMajorClaimProtoP\x01\xa2\x02\x03\x41MX\xaa\x02$ArgServices.MiningExplanation.V1beta\xca\x02$ArgServices\\MiningExplanation\\V1beta\xe2\x02\x30\x41rgServices\\MiningExplanation\\V1beta\\GPBMetadata\xea\x02&ArgServices::MiningExplanation::V1betab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining_explanation.v1beta.major_claim_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining_explanation.v1beta.major_claim_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n*com.arg_services.mining_explanation.v1betaB\017MajorClaimProtoP\001\242\002\003AMX\252\002$ArgServices.MiningExplanation.V1beta\312\002$ArgServices\\MiningExplanation\\V1beta\342\0020ArgServices\\MiningExplanation\\V1beta\\GPBMetadata\352\002&ArgServices::MiningExplanation::V1beta'
   _MAJORCLAIMRESULT_SIMILARITIESENTRY._options = None
   _MAJORCLAIMRESULT_SIMILARITIESENTRY._serialized_options = b'8\001'
   _MAJORCLAIMEXPLANATIONSERVICE.methods_by_name['MajorClaim']._options = None
   _MAJORCLAIMEXPLANATIONSERVICE.methods_by_name['MajorClaim']._serialized_options = b'\202\323\344\223\002\024:\001*\"\017/nlp/v1/vectors'
-  _MAJORCLAIMREQUEST._serialized_start=161
-  _MAJORCLAIMREQUEST._serialized_end=292
-  _MAJORCLAIMRESPONSE._serialized_start=295
-  _MAJORCLAIMRESPONSE._serialized_end=457
-  _MAJORCLAIMRESULT._serialized_start=460
-  _MAJORCLAIMRESULT._serialized_end=683
-  _MAJORCLAIMRESULT_SIMILARITIESENTRY._serialized_start=620
-  _MAJORCLAIMRESULT_SIMILARITIESENTRY._serialized_end=683
-  _MAJORCLAIMEXPLANATIONSERVICE._serialized_start=686
-  _MAJORCLAIMEXPLANATIONSERVICE._serialized_end=878
+  _globals['_MAJORCLAIMREQUEST']._serialized_start=161
+  _globals['_MAJORCLAIMREQUEST']._serialized_end=292
+  _globals['_MAJORCLAIMRESPONSE']._serialized_start=295
+  _globals['_MAJORCLAIMRESPONSE']._serialized_end=457
+  _globals['_MAJORCLAIMRESULT']._serialized_start=460
+  _globals['_MAJORCLAIMRESULT']._serialized_end=683
+  _globals['_MAJORCLAIMRESULT_SIMILARITIESENTRY']._serialized_start=620
+  _globals['_MAJORCLAIMRESULT_SIMILARITIESENTRY']._serialized_end=683
+  _globals['_MAJORCLAIMEXPLANATIONSERVICE']._serialized_start=686
+  _globals['_MAJORCLAIMEXPLANATIONSERVICE']._serialized_end=878
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/nlp/v1/nlp_pb2.py` & `arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,56 +11,57 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x61rg_services/nlp/v1/nlp.proto\x12\x13\x61rg_services.nlp.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\xec\x01\n\tNlpConfig\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12\x1f\n\x0bspacy_model\x18\x02 \x01(\tR\nspacyModel\x12N\n\x10\x65mbedding_models\x18\x03 \x03(\x0b\x32#.arg_services.nlp.v1.EmbeddingModelR\x0f\x65mbeddingModels\x12R\n\x11similarity_method\x18\x04 \x01(\x0e\x32%.arg_services.nlp.v1.SimilarityMethodR\x10similarityMethod\"\xbf\x01\n\x13SimilaritiesRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12?\n\x0btext_tuples\x18\x02 \x03(\x0b\x32\x1e.arg_services.nlp.v1.TextTupleR\ntextTuples\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"k\n\x14SimilaritiesResponse\x12\"\n\x0csimilarities\x18\x01 \x03(\x01R\x0csimilarities\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"7\n\tTextTuple\x12\x14\n\x05text1\x18\x01 \x01(\tR\x05text1\x12\x14\n\x05text2\x18\x02 \x01(\tR\x05text2\"!\n\x07Strings\x12\x16\n\x06values\x18\x01 \x03(\tR\x06values\"\xc5\x03\n\rDocBinRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12\x14\n\x05texts\x18\x02 \x03(\tR\x05texts\x12\x41\n\nattributes\x18\x03 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x01R\nattributes\x88\x01\x01\x12\x43\n\renabled_pipes\x18\x04 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x00R\x0c\x65nabledPipes\x12\x45\n\x0e\x64isabled_pipes\x18\x05 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x00R\rdisabledPipes\x12N\n\x10\x65mbedding_levels\x18\x06 \x03(\x0e\x32#.arg_services.nlp.v1.EmbeddingLevelR\x0f\x65mbeddingLevels\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtrasB\x07\n\x05pipesB\r\n\x0b_attributes\"Y\n\x0e\x44ocBinResponse\x12\x16\n\x06\x64ocbin\x18\x01 \x01(\x0cR\x06\x64ocbin\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xdf\x01\n\x0eVectorsRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12\x14\n\x05texts\x18\x02 \x03(\tR\x05texts\x12N\n\x10\x65mbedding_levels\x18\x03 \x03(\x0e\x32#.arg_services.nlp.v1.EmbeddingLevelR\x0f\x65mbeddingLevels\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x81\x01\n\x0fVectorsResponse\x12=\n\x07vectors\x18\x01 \x03(\x0b\x32#.arg_services.nlp.v1.VectorResponseR\x07vectors\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xea\x01\n\x0eVectorResponse\x12\x37\n\x08\x64ocument\x18\x01 \x01(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\x08\x64ocument\x12\x33\n\x06tokens\x18\x02 \x03(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\x06tokens\x12\x39\n\tsentences\x18\x03 \x03(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\tsentences\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\" \n\x06Vector\x12\x16\n\x06vector\x18\x01 \x03(\x01R\x06vector\"\xd8\x01\n\x0e\x45mbeddingModel\x12\x41\n\nmodel_type\x18\x01 \x01(\x0e\x32\".arg_services.nlp.v1.EmbeddingTypeR\tmodelType\x12\x1d\n\nmodel_name\x18\x02 \x01(\tR\tmodelName\x12\x41\n\x0cpooling_type\x18\x03 \x01(\x0e\x32\x1c.arg_services.nlp.v1.PoolingH\x00R\x0bpoolingType\x12\x16\n\x05pmean\x18\x04 \x01(\x01H\x00R\x05pmeanB\t\n\x07pooling*\xe0\x02\n\x10SimilarityMethod\x12!\n\x1dSIMILARITY_METHOD_UNSPECIFIED\x10\x00\x12\x1c\n\x18SIMILARITY_METHOD_COSINE\x10\x01\x12%\n!SIMILARITY_METHOD_DYNAMAX_JACCARD\x10\x02\x12%\n!SIMILARITY_METHOD_MAXPOOL_JACCARD\x10\x03\x12\"\n\x1eSIMILARITY_METHOD_DYNAMAX_DICE\x10\x04\x12$\n SIMILARITY_METHOD_DYNAMAX_OTSUKA\x10\x05\x12\x19\n\x15SIMILARITY_METHOD_WMD\x10\x06\x12\x1a\n\x16SIMILARITY_METHOD_EDIT\x10\x07\x12\x1d\n\x19SIMILARITY_METHOD_JACCARD\x10\x08\x12\x1d\n\x19SIMILARITY_METHOD_ANGULAR\x10\t*\x8a\x01\n\x0e\x45mbeddingLevel\x12\x1f\n\x1b\x45MBEDDING_LEVEL_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x45MBEDDING_LEVEL_DOCUMENT\x10\x01\x12\x1a\n\x16\x45MBEDDING_LEVEL_TOKENS\x10\x02\x12\x1d\n\x19\x45MBEDDING_LEVEL_SENTENCES\x10\x03*\xc6\x01\n\x07Pooling\x12\x17\n\x13POOLING_UNSPECIFIED\x10\x00\x12\x10\n\x0cPOOLING_MEAN\x10\x01\x12\x0f\n\x0bPOOLING_MAX\x10\x02\x12\x0f\n\x0bPOOLING_MIN\x10\x03\x12\x0f\n\x0bPOOLING_SUM\x10\x04\x12\x11\n\rPOOLING_FIRST\x10\x05\x12\x10\n\x0cPOOLING_LAST\x10\x06\x12\x12\n\x0ePOOLING_MEDIAN\x10\x07\x12\x11\n\rPOOLING_GMEAN\x10\x08\x12\x11\n\rPOOLING_HMEAN\x10\t*\xb7\x01\n\rEmbeddingType\x12\x1e\n\x1a\x45MBEDDING_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x45MBEDDING_TYPE_SPACY\x10\x01\x12\x1f\n\x1b\x45MBEDDING_TYPE_TRANSFORMERS\x10\x02\x12(\n$EMBEDDING_TYPE_SENTENCE_TRANSFORMERS\x10\x03\x12!\n\x1d\x45MBEDDING_TYPE_TENSORFLOW_HUB\x10\x04\x32\xf3\x02\n\nNlpService\x12p\n\x07Vectors\x12#.arg_services.nlp.v1.VectorsRequest\x1a$.arg_services.nlp.v1.VectorsResponse\"\x1a\x82\xd3\xe4\x93\x02\x14:\x01*\"\x0f/nlp/v1/vectors\x12\x84\x01\n\x0cSimilarities\x12(.arg_services.nlp.v1.SimilaritiesRequest\x1a).arg_services.nlp.v1.SimilaritiesResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/nlp/v1/similarities\x12l\n\x06\x44ocBin\x12\".arg_services.nlp.v1.DocBinRequest\x1a#.arg_services.nlp.v1.DocBinResponse\"\x19\x82\xd3\xe4\x93\x02\x13:\x01*\"\x0e/nlp/v1/docbinB\x8d\x01\n\x17\x63om.arg_services.nlp.v1B\x08NlpProtoP\x01\xa2\x02\x03\x41NX\xaa\x02\x12\x41rgServices.Nlp.V1\xca\x02\x12\x41rgServices\\Nlp\\V1\xe2\x02\x1e\x41rgServices\\Nlp\\V1\\GPBMetadata\xea\x02\x14\x41rgServices::Nlp::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x61rg_services/nlp/v1/nlp.proto\x12\x13\x61rg_services.nlp.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\xec\x01\n\tNlpConfig\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12\x1f\n\x0bspacy_model\x18\x02 \x01(\tR\nspacyModel\x12N\n\x10\x65mbedding_models\x18\x03 \x03(\x0b\x32#.arg_services.nlp.v1.EmbeddingModelR\x0f\x65mbeddingModels\x12R\n\x11similarity_method\x18\x04 \x01(\x0e\x32%.arg_services.nlp.v1.SimilarityMethodR\x10similarityMethod\"\xbf\x01\n\x13SimilaritiesRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12?\n\x0btext_tuples\x18\x02 \x03(\x0b\x32\x1e.arg_services.nlp.v1.TextTupleR\ntextTuples\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"k\n\x14SimilaritiesResponse\x12\"\n\x0csimilarities\x18\x01 \x03(\x01R\x0csimilarities\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"7\n\tTextTuple\x12\x14\n\x05text1\x18\x01 \x01(\tR\x05text1\x12\x14\n\x05text2\x18\x02 \x01(\tR\x05text2\"!\n\x07Strings\x12\x16\n\x06values\x18\x01 \x03(\tR\x06values\"\xc5\x03\n\rDocBinRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12\x14\n\x05texts\x18\x02 \x03(\tR\x05texts\x12\x41\n\nattributes\x18\x03 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x01R\nattributes\x88\x01\x01\x12\x43\n\renabled_pipes\x18\x04 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x00R\x0c\x65nabledPipes\x12\x45\n\x0e\x64isabled_pipes\x18\x05 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x00R\rdisabledPipes\x12N\n\x10\x65mbedding_levels\x18\x06 \x03(\x0e\x32#.arg_services.nlp.v1.EmbeddingLevelR\x0f\x65mbeddingLevels\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtrasB\x07\n\x05pipesB\r\n\x0b_attributes\"Y\n\x0e\x44ocBinResponse\x12\x16\n\x06\x64ocbin\x18\x01 \x01(\x0cR\x06\x64ocbin\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xdf\x01\n\x0eVectorsRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12\x14\n\x05texts\x18\x02 \x03(\tR\x05texts\x12N\n\x10\x65mbedding_levels\x18\x03 \x03(\x0e\x32#.arg_services.nlp.v1.EmbeddingLevelR\x0f\x65mbeddingLevels\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x81\x01\n\x0fVectorsResponse\x12=\n\x07vectors\x18\x01 \x03(\x0b\x32#.arg_services.nlp.v1.VectorResponseR\x07vectors\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xea\x01\n\x0eVectorResponse\x12\x37\n\x08\x64ocument\x18\x01 \x01(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\x08\x64ocument\x12\x33\n\x06tokens\x18\x02 \x03(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\x06tokens\x12\x39\n\tsentences\x18\x03 \x03(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\tsentences\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\" \n\x06Vector\x12\x16\n\x06vector\x18\x01 \x03(\x01R\x06vector\"\xd8\x01\n\x0e\x45mbeddingModel\x12\x41\n\nmodel_type\x18\x01 \x01(\x0e\x32\".arg_services.nlp.v1.EmbeddingTypeR\tmodelType\x12\x1d\n\nmodel_name\x18\x02 \x01(\tR\tmodelName\x12\x41\n\x0cpooling_type\x18\x03 \x01(\x0e\x32\x1c.arg_services.nlp.v1.PoolingH\x00R\x0bpoolingType\x12\x16\n\x05pmean\x18\x04 \x01(\x01H\x00R\x05pmeanB\t\n\x07pooling*\xe0\x02\n\x10SimilarityMethod\x12!\n\x1dSIMILARITY_METHOD_UNSPECIFIED\x10\x00\x12\x1c\n\x18SIMILARITY_METHOD_COSINE\x10\x01\x12%\n!SIMILARITY_METHOD_DYNAMAX_JACCARD\x10\x02\x12%\n!SIMILARITY_METHOD_MAXPOOL_JACCARD\x10\x03\x12\"\n\x1eSIMILARITY_METHOD_DYNAMAX_DICE\x10\x04\x12$\n SIMILARITY_METHOD_DYNAMAX_OTSUKA\x10\x05\x12\x19\n\x15SIMILARITY_METHOD_WMD\x10\x06\x12\x1a\n\x16SIMILARITY_METHOD_EDIT\x10\x07\x12\x1d\n\x19SIMILARITY_METHOD_JACCARD\x10\x08\x12\x1d\n\x19SIMILARITY_METHOD_ANGULAR\x10\t*\x8a\x01\n\x0e\x45mbeddingLevel\x12\x1f\n\x1b\x45MBEDDING_LEVEL_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x45MBEDDING_LEVEL_DOCUMENT\x10\x01\x12\x1a\n\x16\x45MBEDDING_LEVEL_TOKENS\x10\x02\x12\x1d\n\x19\x45MBEDDING_LEVEL_SENTENCES\x10\x03*\xc6\x01\n\x07Pooling\x12\x17\n\x13POOLING_UNSPECIFIED\x10\x00\x12\x10\n\x0cPOOLING_MEAN\x10\x01\x12\x0f\n\x0bPOOLING_MAX\x10\x02\x12\x0f\n\x0bPOOLING_MIN\x10\x03\x12\x0f\n\x0bPOOLING_SUM\x10\x04\x12\x11\n\rPOOLING_FIRST\x10\x05\x12\x10\n\x0cPOOLING_LAST\x10\x06\x12\x12\n\x0ePOOLING_MEDIAN\x10\x07\x12\x11\n\rPOOLING_GMEAN\x10\x08\x12\x11\n\rPOOLING_HMEAN\x10\t*\xd2\x01\n\rEmbeddingType\x12\x1e\n\x1a\x45MBEDDING_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x45MBEDDING_TYPE_SPACY\x10\x01\x12\x1f\n\x1b\x45MBEDDING_TYPE_TRANSFORMERS\x10\x02\x12(\n$EMBEDDING_TYPE_SENTENCE_TRANSFORMERS\x10\x03\x12!\n\x1d\x45MBEDDING_TYPE_TENSORFLOW_HUB\x10\x04\x12\x19\n\x15\x45MBEDDING_TYPE_OPENAI\x10\x05\x32\xf3\x02\n\nNlpService\x12p\n\x07Vectors\x12#.arg_services.nlp.v1.VectorsRequest\x1a$.arg_services.nlp.v1.VectorsResponse\"\x1a\x82\xd3\xe4\x93\x02\x14:\x01*\"\x0f/nlp/v1/vectors\x12\x84\x01\n\x0cSimilarities\x12(.arg_services.nlp.v1.SimilaritiesRequest\x1a).arg_services.nlp.v1.SimilaritiesResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/nlp/v1/similarities\x12l\n\x06\x44ocBin\x12\".arg_services.nlp.v1.DocBinRequest\x1a#.arg_services.nlp.v1.DocBinResponse\"\x19\x82\xd3\xe4\x93\x02\x13:\x01*\"\x0e/nlp/v1/docbinB\x8d\x01\n\x17\x63om.arg_services.nlp.v1B\x08NlpProtoP\x01\xa2\x02\x03\x41NX\xaa\x02\x12\x41rgServices.Nlp.V1\xca\x02\x12\x41rgServices\\Nlp\\V1\xe2\x02\x1e\x41rgServices\\Nlp\\V1\\GPBMetadata\xea\x02\x14\x41rgServices::Nlp::V1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.nlp.v1.nlp_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.nlp.v1.nlp_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\027com.arg_services.nlp.v1B\010NlpProtoP\001\242\002\003ANX\252\002\022ArgServices.Nlp.V1\312\002\022ArgServices\\Nlp\\V1\342\002\036ArgServices\\Nlp\\V1\\GPBMetadata\352\002\024ArgServices::Nlp::V1'
   _NLPSERVICE.methods_by_name['Vectors']._options = None
   _NLPSERVICE.methods_by_name['Vectors']._serialized_options = b'\202\323\344\223\002\024:\001*\"\017/nlp/v1/vectors'
   _NLPSERVICE.methods_by_name['Similarities']._options = None
   _NLPSERVICE.methods_by_name['Similarities']._serialized_options = b'\202\323\344\223\002\031:\001*\"\024/nlp/v1/similarities'
   _NLPSERVICE.methods_by_name['DocBin']._options = None
   _NLPSERVICE.methods_by_name['DocBin']._serialized_options = b'\202\323\344\223\002\023:\001*\"\016/nlp/v1/docbin'
-  _SIMILARITYMETHOD._serialized_start=2144
-  _SIMILARITYMETHOD._serialized_end=2496
-  _EMBEDDINGLEVEL._serialized_start=2499
-  _EMBEDDINGLEVEL._serialized_end=2637
-  _POOLING._serialized_start=2640
-  _POOLING._serialized_end=2838
-  _EMBEDDINGTYPE._serialized_start=2841
-  _EMBEDDINGTYPE._serialized_end=3024
-  _NLPCONFIG._serialized_start=115
-  _NLPCONFIG._serialized_end=351
-  _SIMILARITIESREQUEST._serialized_start=354
-  _SIMILARITIESREQUEST._serialized_end=545
-  _SIMILARITIESRESPONSE._serialized_start=547
-  _SIMILARITIESRESPONSE._serialized_end=654
-  _TEXTTUPLE._serialized_start=656
-  _TEXTTUPLE._serialized_end=711
-  _STRINGS._serialized_start=713
-  _STRINGS._serialized_end=746
-  _DOCBINREQUEST._serialized_start=749
-  _DOCBINREQUEST._serialized_end=1202
-  _DOCBINRESPONSE._serialized_start=1204
-  _DOCBINRESPONSE._serialized_end=1293
-  _VECTORSREQUEST._serialized_start=1296
-  _VECTORSREQUEST._serialized_end=1519
-  _VECTORSRESPONSE._serialized_start=1522
-  _VECTORSRESPONSE._serialized_end=1651
-  _VECTORRESPONSE._serialized_start=1654
-  _VECTORRESPONSE._serialized_end=1888
-  _VECTOR._serialized_start=1890
-  _VECTOR._serialized_end=1922
-  _EMBEDDINGMODEL._serialized_start=1925
-  _EMBEDDINGMODEL._serialized_end=2141
-  _NLPSERVICE._serialized_start=3027
-  _NLPSERVICE._serialized_end=3398
+  _globals['_SIMILARITYMETHOD']._serialized_start=2144
+  _globals['_SIMILARITYMETHOD']._serialized_end=2496
+  _globals['_EMBEDDINGLEVEL']._serialized_start=2499
+  _globals['_EMBEDDINGLEVEL']._serialized_end=2637
+  _globals['_POOLING']._serialized_start=2640
+  _globals['_POOLING']._serialized_end=2838
+  _globals['_EMBEDDINGTYPE']._serialized_start=2841
+  _globals['_EMBEDDINGTYPE']._serialized_end=3051
+  _globals['_NLPCONFIG']._serialized_start=115
+  _globals['_NLPCONFIG']._serialized_end=351
+  _globals['_SIMILARITIESREQUEST']._serialized_start=354
+  _globals['_SIMILARITIESREQUEST']._serialized_end=545
+  _globals['_SIMILARITIESRESPONSE']._serialized_start=547
+  _globals['_SIMILARITIESRESPONSE']._serialized_end=654
+  _globals['_TEXTTUPLE']._serialized_start=656
+  _globals['_TEXTTUPLE']._serialized_end=711
+  _globals['_STRINGS']._serialized_start=713
+  _globals['_STRINGS']._serialized_end=746
+  _globals['_DOCBINREQUEST']._serialized_start=749
+  _globals['_DOCBINREQUEST']._serialized_end=1202
+  _globals['_DOCBINRESPONSE']._serialized_start=1204
+  _globals['_DOCBINRESPONSE']._serialized_end=1293
+  _globals['_VECTORSREQUEST']._serialized_start=1296
+  _globals['_VECTORSREQUEST']._serialized_end=1519
+  _globals['_VECTORSRESPONSE']._serialized_start=1522
+  _globals['_VECTORSRESPONSE']._serialized_end=1651
+  _globals['_VECTORRESPONSE']._serialized_start=1654
+  _globals['_VECTORRESPONSE']._serialized_end=1888
+  _globals['_VECTOR']._serialized_start=1890
+  _globals['_VECTOR']._serialized_end=1922
+  _globals['_EMBEDDINGMODEL']._serialized_start=1925
+  _globals['_EMBEDDINGMODEL']._serialized_end=2141
+  _globals['_NLPSERVICE']._serialized_start=3054
+  _globals['_NLPSERVICE']._serialized_end=3425
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/arg_services/nlp/v1/nlp_pb2.pyi` & `arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -161,27 +161,31 @@
     """[Spacy](https://spacy.io/models)."""
     EMBEDDING_TYPE_TRANSFORMERS: _EmbeddingType.ValueType  # 2
     """[HuggingFace Transformers](https://huggingface.co/models)."""
     EMBEDDING_TYPE_SENTENCE_TRANSFORMERS: _EmbeddingType.ValueType  # 3
     """[UKPLab Sentence Transformers](https://www.sbert.net/docs/pretrained_models.html)"""
     EMBEDDING_TYPE_TENSORFLOW_HUB: _EmbeddingType.ValueType  # 4
     """Tensorflow Hub. Example: [Universal Sentence Encoder](https://tfhub.dev/google/universal-sentence-encoder/4)."""
+    EMBEDDING_TYPE_OPENAI: _EmbeddingType.ValueType  # 5
+    """[OpenAI](https://platform.openai.com/docs/guides/embeddings/use-cases)."""
 
 class EmbeddingType(_EmbeddingType, metaclass=_EmbeddingTypeEnumTypeWrapper): ...
 
 EMBEDDING_TYPE_UNSPECIFIED: EmbeddingType.ValueType  # 0
 """In the default case, no embedding is computed."""
 EMBEDDING_TYPE_SPACY: EmbeddingType.ValueType  # 1
 """[Spacy](https://spacy.io/models)."""
 EMBEDDING_TYPE_TRANSFORMERS: EmbeddingType.ValueType  # 2
 """[HuggingFace Transformers](https://huggingface.co/models)."""
 EMBEDDING_TYPE_SENTENCE_TRANSFORMERS: EmbeddingType.ValueType  # 3
 """[UKPLab Sentence Transformers](https://www.sbert.net/docs/pretrained_models.html)"""
 EMBEDDING_TYPE_TENSORFLOW_HUB: EmbeddingType.ValueType  # 4
 """Tensorflow Hub. Example: [Universal Sentence Encoder](https://tfhub.dev/google/universal-sentence-encoder/4)."""
+EMBEDDING_TYPE_OPENAI: EmbeddingType.ValueType  # 5
+"""[OpenAI](https://platform.openai.com/docs/guides/embeddings/use-cases)."""
 global___EmbeddingType = EmbeddingType
 
 @typing_extensions.final
 class NlpConfig(google.protobuf.message.Message):
     """Common message for configuring spacy."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `arg_services-1.2.3/src/arg_services/nlp/v1/nlp_pb2_grpc.py` & `arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi` & `arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/google/api/annotations_pb2.py` & `arg_services-1.3.0/src/google/api/annotations_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 from google.api import http_pb2 as google_dot_api_dot_http__pb2
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cgoogle/api/annotations.proto\x12\ngoogle.api\x1a\x15google/api/http.proto\x1a google/protobuf/descriptor.proto:K\n\x04http\x12\x1e.google.protobuf.MethodOptions\x18\xb0\xca\xbc\" \x01(\x0b\x32\x14.google.api.HttpRuleR\x04httpB\xae\x01\n\x0e\x63om.google.apiB\x10\x41nnotationsProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xa2\x02\x03GAX\xaa\x02\nGoogle.Api\xca\x02\nGoogle\\Api\xe2\x02\x16Google\\Api\\GPBMetadata\xea\x02\x0bGoogle::Apib\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.annotations_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.annotations_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(http)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\020AnnotationsProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\003GAX\252\002\nGoogle.Api\312\002\nGoogle\\Api\342\002\026Google\\Api\\GPBMetadata\352\002\013Google::Api'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/google/api/annotations_pb2.pyi` & `arg_services-1.3.0/src/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/google/api/annotations_pb2_grpc.pyi` & `arg_services-1.3.0/src/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.2.3/src/google/api/http_pb2.py` & `arg_services-1.3.0/src/google/api/http_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15google/api/http.proto\x12\ngoogle.api\"y\n\x04Http\x12*\n\x05rules\x18\x01 \x03(\x0b\x32\x14.google.api.HttpRuleR\x05rules\x12\x45\n\x1f\x66ully_decode_reserved_expansion\x18\x02 \x01(\x08R\x1c\x66ullyDecodeReservedExpansion\"\xda\x02\n\x08HttpRule\x12\x1a\n\x08selector\x18\x01 \x01(\tR\x08selector\x12\x12\n\x03get\x18\x02 \x01(\tH\x00R\x03get\x12\x12\n\x03put\x18\x03 \x01(\tH\x00R\x03put\x12\x14\n\x04post\x18\x04 \x01(\tH\x00R\x04post\x12\x18\n\x06\x64\x65lete\x18\x05 \x01(\tH\x00R\x06\x64\x65lete\x12\x16\n\x05patch\x18\x06 \x01(\tH\x00R\x05patch\x12\x37\n\x06\x63ustom\x18\x08 \x01(\x0b\x32\x1d.google.api.CustomHttpPatternH\x00R\x06\x63ustom\x12\x12\n\x04\x62ody\x18\x07 \x01(\tR\x04\x62ody\x12#\n\rresponse_body\x18\x0c \x01(\tR\x0cresponseBody\x12\x45\n\x13\x61\x64\x64itional_bindings\x18\x0b \x03(\x0b\x32\x14.google.api.HttpRuleR\x12\x61\x64\x64itionalBindingsB\t\n\x07pattern\";\n\x11\x43ustomHttpPattern\x12\x12\n\x04kind\x18\x01 \x01(\tR\x04kind\x12\x12\n\x04path\x18\x02 \x01(\tR\x04pathB\xaa\x01\n\x0e\x63om.google.apiB\tHttpProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xf8\x01\x01\xa2\x02\x03GAX\xaa\x02\nGoogle.Api\xca\x02\nGoogle\\Api\xe2\x02\x16Google\\Api\\GPBMetadata\xea\x02\x0bGoogle::Apib\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.http_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.http_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\tHttpProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\370\001\001\242\002\003GAX\252\002\nGoogle.Api\312\002\nGoogle\\Api\342\002\026Google\\Api\\GPBMetadata\352\002\013Google::Api'
-  _HTTP._serialized_start=37
-  _HTTP._serialized_end=158
-  _HTTPRULE._serialized_start=161
-  _HTTPRULE._serialized_end=507
-  _CUSTOMHTTPPATTERN._serialized_start=509
-  _CUSTOMHTTPPATTERN._serialized_end=568
+  _globals['_HTTP']._serialized_start=37
+  _globals['_HTTP']._serialized_end=158
+  _globals['_HTTPRULE']._serialized_start=161
+  _globals['_HTTPRULE']._serialized_end=507
+  _globals['_CUSTOMHTTPPATTERN']._serialized_start=509
+  _globals['_CUSTOMHTTPPATTERN']._serialized_end=568
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.2.3/src/google/api/http_pb2.pyi` & `arg_services-1.3.0/src/google/api/http_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Copyright 2015 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -231,23 +231,26 @@
     "123456")`
 
     ## Rules for HTTP mapping
 
     1. Leaf request fields (recursive expansion nested messages in the request
        message) are classified into three categories:
        - Fields referred by the path template. They are passed via the URL path.
-       - Fields referred by the [HttpRule.body][google.api.HttpRule.body]. They are passed via the HTTP
+       - Fields referred by the [HttpRule.body][google.api.HttpRule.body]. They
+       are passed via the HTTP
          request body.
        - All other fields are passed via the URL query parameters, and the
          parameter name is the field path in the request message. A repeated
          field can be represented as multiple query parameters under the same
          name.
-     2. If [HttpRule.body][google.api.HttpRule.body] is "*", there is no URL query parameter, all fields
+     2. If [HttpRule.body][google.api.HttpRule.body] is "*", there is no URL
+     query parameter, all fields
         are passed via URL path and HTTP request body.
-     3. If [HttpRule.body][google.api.HttpRule.body] is omitted, there is no HTTP request body, all
+     3. If [HttpRule.body][google.api.HttpRule.body] is omitted, there is no HTTP
+     request body, all
         fields are passed via URL path and URL query parameters.
 
     ### Path template syntax
 
         Template = "/" Segments [ Verb ] ;
         Segments = Segment { "/" Segment } ;
         Segment  = "*" | "**" | LITERAL | Variable ;
@@ -348,15 +351,16 @@
     CUSTOM_FIELD_NUMBER: builtins.int
     BODY_FIELD_NUMBER: builtins.int
     RESPONSE_BODY_FIELD_NUMBER: builtins.int
     ADDITIONAL_BINDINGS_FIELD_NUMBER: builtins.int
     selector: builtins.str
     """Selects a method to which this rule applies.
 
-    Refer to [selector][google.api.DocumentationRule.selector] for syntax details.
+    Refer to [selector][google.api.DocumentationRule.selector] for syntax
+    details.
     """
     get: builtins.str
     """Maps to HTTP GET. Used for listing and getting information about
     resources.
     """
     put: builtins.str
     """Maps to HTTP PUT. Used for replacing a resource."""
```

### Comparing `arg_services-1.2.3/src/google/api/http_pb2_grpc.pyi` & `arg_services-1.3.0/src/google/api/http_pb2_grpc.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Copyright 2015 Google LLC
+Copyright 2023 Google LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `arg_services-1.2.3/PKG-INFO` & `arg_services-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: arg-services
-Version: 1.2.3
+Version: 1.3.0
 Summary: gRPC definitions for microservice-based argumentation machines
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: grpc-stubs (>=1.24.12,<2.0.0)
-Requires-Dist: grpcio (>=1.51.1,<2.0.0)
-Requires-Dist: grpcio-reflection (>=1.51.1,<2.0.0)
-Requires-Dist: protobuf (>=4.21.12,<5.0.0)
+Requires-Dist: grpc-stubs (>=1.53.0.1,<2.0.0.0)
+Requires-Dist: grpcio (>=1.53.0,<2.0.0)
+Requires-Dist: grpcio-reflection (>=1.53.0,<2.0.0)
+Requires-Dist: protobuf (>=4.22.1,<5.0.0)
 Project-URL: Repository, https://github.com/recap-utr/arg-services-python
 Description-Content-Type: text/markdown
 
 # Argumentation Microservices
 
 This project contains Protobuf definitions for building complex argumentation machines.
 The idea is to facilitate a microservice-oriented architecture where individual parts can be swapped out easily.
```

