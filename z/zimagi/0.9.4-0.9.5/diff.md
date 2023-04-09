# Comparing `tmp/zimagi-0.9.4.tar.gz` & `tmp/zimagi-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimagi-0.9.4.tar", last modified: Sat Aug 20 05:36:53 2022, max compression
+gzip compressed data, was "zimagi-0.9.5.tar", last modified: Mon Aug 29 05:01:53 2022, max compression
```

## Comparing `zimagi-0.9.4.tar` & `zimagi-0.9.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-20 05:36:53.148763 zimagi-0.9.4/
--rw-r--r--   0 root         (0) root         (0)      403 2022-08-20 05:36:53.148763 zimagi-0.9.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-20 05:36:47.000000 zimagi-0.9.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-20 05:36:53.148763 zimagi-0.9.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1174 2022-08-20 05:36:47.000000 zimagi-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 05:01:53.039044 zimagi-0.9.5/
+-rw-r--r--   0 root         (0) root         (0)      403 2022-08-29 05:01:53.039044 zimagi-0.9.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-29 05:01:46.000000 zimagi-0.9.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-29 05:01:53.039044 zimagi-0.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1174 2022-08-29 05:01:46.000000 zimagi-0.9.5/setup.py
```

### Comparing `zimagi-0.9.4/setup.py` & `zimagi-0.9.5/setup.py`

 * *Files identical despite different names*

