# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-5.3.0rc1.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-6.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-cncf-kubernetes-5.3.0rc1.tar", last modified: Sun Apr  2 05:47:20 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-cncf-kubernetes-6.0.0rc1.tar", last modified: Sun Apr  9 13:48:22 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1.tar` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1174 2023-04-02 05:47:18.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    31898 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    30344 2023-04-02 05:47:18.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6151 2023-03-16 20:46:35.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     4274 2023-04-02 05:47:18.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23391 2023-03-15 08:58:48.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    37484 2023-03-12 11:08:42.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-03-15 08:58:48.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3343 2023-03-27 08:32:49.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1072 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    10454 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22378 2023-03-10 19:31:58.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2404 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)    31898 2023-04-02 05:47:19.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-02 05:47:19.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:19.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-02 05:47:19.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:19.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-02 05:47:19.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:47:19.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1976 2023-04-02 05:47:20.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1522 2023-04-02 05:47:18.000000 apache-airflow-providers-cncf-kubernetes-5.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-04-09 13:48:20.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    32291 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    30737 2023-04-09 13:48:20.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6151 2023-03-16 20:46:35.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     4323 2023-04-09 13:48:20.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23857 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    37598 2023-04-08 17:35:35.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2023-03-15 08:58:48.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3343 2023-03-27 08:32:49.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    10454 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21693 2023-04-08 17:35:35.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    32291 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-04-09 13:48:19.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/LICENSE` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/MANIFEST.in`

 * *Files 11% similar despite different names*

```diff
@@ -25,10 +25,9 @@
 
 
 include airflow/providers/cncf/kubernetes/*.jinja2
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.txt
-include README.md
+include CHANGELOG.rst
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 5.3.0rc1
+Version: 6.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/5.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``5.3.0rc1``
+Release: ``6.0.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/5.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -112,14 +112,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.0.0
+.....
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+Use ``kubernetes_default`` connection by default in the ``KubernetesPodOperator``.
+
+* ``Use default connection id for KubernetesPodOperator (#28848)``
+
+Features
+~~~~~~~~
+
+* ``Allow to set limits for XCOM container (#28125)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Add mechanism to suspend providers (#30422)``
+
 5.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``enhance spark_k8s_operator (#29977)``
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/README.rst` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``5.3.0rc1``
+Release: ``6.0.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/5.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,14 +79,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.0.0
+.....
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+Use ``kubernetes_default`` connection by default in the ``KubernetesPodOperator``.
+
+* ``Use default connection id for KubernetesPodOperator (#28848)``
+
+Features
+~~~~~~~~
+
+* ``Allow to set limits for XCOM container (#28125)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Add mechanism to suspend providers (#30422)``
+
 5.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``enhance spark_k8s_operator (#29977)``
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cncf-kubernetes",
         "name": "Kubernetes",
         "description": "`Kubernetes <https://kubernetes.io/>`__\n",
+        "suspended": False,
         "versions": [
+            "6.0.0",
             "5.3.0",
             "5.2.2",
             "5.2.1",
             "5.2.0",
             "5.1.1",
             "5.1.0",
             "5.0.0",
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import contextlib
+import json
 import tempfile
 import warnings
 from typing import TYPE_CHECKING, Any, Generator
 
 from asgiref.sync import sync_to_async
 from kubernetes import client, config, watch
 from kubernetes.client.models import V1Pod
@@ -97,14 +98,17 @@
             "namespace": StringField(lazy_gettext("Namespace"), widget=BS3TextFieldWidget()),
             "cluster_context": StringField(lazy_gettext("Cluster context"), widget=BS3TextFieldWidget()),
             "disable_verify_ssl": BooleanField(lazy_gettext("Disable SSL")),
             "disable_tcp_keepalive": BooleanField(lazy_gettext("Disable TCP keepalive")),
             "xcom_sidecar_container_image": StringField(
                 lazy_gettext("XCom sidecar image"), widget=BS3TextFieldWidget()
             ),
+            "xcom_sidecar_container_resources": StringField(
+                lazy_gettext("XCom sidecar resources (JSON format)"), widget=BS3TextFieldWidget()
+            ),
         }
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
         """Returns custom field behaviour"""
         return {
             "hidden_fields": ["host", "schema", "login", "password", "port", "extra"],
@@ -362,14 +366,21 @@
             return self._get_field("namespace")
         return None
 
     def get_xcom_sidecar_container_image(self):
         """Returns the xcom sidecar image that defined in the connection"""
         return self._get_field("xcom_sidecar_container_image")
 
+    def get_xcom_sidecar_container_resources(self):
+        """Returns the xcom sidecar resources that defined in the connection"""
+        field = self._get_field("xcom_sidecar_container_resources")
+        if not field:
+            return None
+        return json.loads(field)
+
     def get_pod_log_stream(
         self,
         pod_name: str,
         container: str | None = "",
         namespace: str | None = None,
     ) -> tuple[watch.Watch, Generator[str, None, None]]:
         """
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         "volume_mounts",
     )
     template_fields_renderers = {"env_vars": "py"}
 
     def __init__(
         self,
         *,
-        kubernetes_conn_id: str | None = None,  # 'kubernetes_default',
+        kubernetes_conn_id: str | None = KubernetesHook.default_conn_name,
         namespace: str | None = None,
         image: str | None = None,
         name: str | None = None,
         random_name_suffix: bool = True,
         cmds: list[str] | None = None,
         arguments: list[str] | None = None,
         ports: list[k8s.V1ContainerPort] | None = None,
@@ -806,15 +806,17 @@
 
         for secret in self.secrets:
             self.log.debug("Adding secret to task %s", self.task_id)
             pod = secret.attach_to_pod(pod)
         if self.do_xcom_push:
             self.log.debug("Adding xcom sidecar to task %s", self.task_id)
             pod = xcom_sidecar.add_xcom_sidecar(
-                pod, sidecar_container_image=self.hook.get_xcom_sidecar_container_image()
+                pod,
+                sidecar_container_image=self.hook.get_xcom_sidecar_container_image(),
+                sidecar_container_resources=self.hook.get_xcom_sidecar_container_resources(),
             )
 
         labels = self._get_ti_pod_labels(context)
         self.log.info("Building pod %s with labels: %s", pod.metadata.name, labels)
 
         # Merge Pod Identifying labels with labels passed to operator
         pod.metadata.labels.update(labels)
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 from kubernetes.stream import stream as kubernetes_stream
 from pendulum import DateTime
 from pendulum.parsing.exceptions import ParserError
 from urllib3.exceptions import HTTPError as BaseHTTPError
 from urllib3.response import HTTPResponse
 
 from airflow.exceptions import AirflowException
-from airflow.kubernetes.kube_client import get_kube_client
 from airflow.kubernetes.pod_generator import PodDefaults
 from airflow.utils.log.logging_mixin import LoggingMixin
 from airflow.utils.timezone import utcnow
 
 if TYPE_CHECKING:
     from kubernetes.client.models.core_v1_event_list import CoreV1EventList
 
@@ -215,36 +214,23 @@
     """
     Helper class for creating, monitoring, and otherwise interacting with Kubernetes pods
     for use with the KubernetesPodOperator
     """
 
     def __init__(
         self,
-        kube_client: client.CoreV1Api = None,
-        in_cluster: bool = True,
-        cluster_context: str | None = None,
+        kube_client: client.CoreV1Api,
     ):
         """
         Creates the launcher.
 
         :param kube_client: kubernetes client
-        :param in_cluster: whether we are in cluster
-        :param cluster_context: context of the cluster
         """
         super().__init__()
-        if kube_client:
-            self._client = kube_client
-        else:
-            self._client = get_kube_client(in_cluster=in_cluster, cluster_context=cluster_context)
-            warnings.warn(
-                "`kube_client` not supplied to PodManager. "
-                "This will be a required argument in a future release. "
-                "Please use KubernetesHook to create the client before calling.",
-                DeprecationWarning,
-            )
+        self._client = kube_client
         self._watch = watch.Watch()
 
     def run_pod_async(self, pod: V1Pod, **kwargs) -> V1Pod:
         """Runs POD asynchronously"""
         sanitized_pod = self._client.api_client.sanitize_for_serialization(pod)
         json_pod = json.dumps(sanitized_pod, indent=2)
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,24 +38,32 @@
         name=SIDECAR_CONTAINER_NAME,
         command=["sh", "-c", XCOM_CMD],
         image="alpine",
         volume_mounts=[VOLUME_MOUNT],
         resources=k8s.V1ResourceRequirements(
             requests={
                 "cpu": "1m",
-            }
+                "memory": "10Mi",
+            },
         ),
     )
 
 
-def add_xcom_sidecar(pod: k8s.V1Pod, *, sidecar_container_image=None) -> k8s.V1Pod:
+def add_xcom_sidecar(
+    pod: k8s.V1Pod,
+    *,
+    sidecar_container_image: str | None = None,
+    sidecar_container_resources: k8s.V1ResourceRequirements | dict | None = None,
+) -> k8s.V1Pod:
     """Adds sidecar"""
     pod_cp = copy.deepcopy(pod)
     pod_cp.spec.volumes = pod.spec.volumes or []
     pod_cp.spec.volumes.insert(0, PodDefaults.VOLUME)
     pod_cp.spec.containers[0].volume_mounts = pod_cp.spec.containers[0].volume_mounts or []
     pod_cp.spec.containers[0].volume_mounts.insert(0, PodDefaults.VOLUME_MOUNT)
     sidecar = copy.deepcopy(PodDefaults.SIDECAR_CONTAINER)
     sidecar.image = sidecar_container_image or PodDefaults.SIDECAR_CONTAINER.image
+    if sidecar_container_resources:
+        sidecar.resources = sidecar_container_resources
     pod_cp.spec.containers.append(sidecar)
 
     return pod_cp
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 5.3.0rc1
+Version: 6.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/5.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``5.3.0rc1``
+Release: ``6.0.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/5.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -112,14 +112,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.0.0
+.....
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+Use ``kubernetes_default`` connection by default in the ``KubernetesPodOperator``.
+
+* ``Use default connection id for KubernetesPodOperator (#28848)``
+
+Features
+~~~~~~~~
+
+* ``Allow to set limits for XCOM container (#28125)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Add mechanism to suspend providers (#30422)``
+
 5.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``enhance spark_k8s_operator (#29977)``
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/5.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-cncf-kubernetes-5.3.0rc1/setup.py` & `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-cncf-kubernetes package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.3.0"
+version = "6.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-cncf-kubernetes setup."""
     setup(
         version=version,
         extras_require={},
         packages=find_namespace_packages(
-            include=["airflow.providers.cncf.kubernetes", "airflow.providers.cncf.kubernetes.*"]
+            include=[
+                "airflow.providers.cncf.kubernetes",
+                "airflow.providers.cncf.kubernetes.*",
+                "airflow.providers.cncf.kubernetes_vendor",
+                "airflow.providers.cncf.kubernetes_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

