# Comparing `tmp/afex-audit-trail-0.1.1.tar.gz` & `tmp/afex-audit-trail-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-audit-trail-0.1.1.tar", last modified: Wed Apr  5 17:12:36 2023, max compression
+gzip compressed data, was "afex-audit-trail-0.1.2.tar", last modified: Sun Apr  9 17:17:54 2023, max compression
```

## Comparing `afex-audit-trail-0.1.1.tar` & `afex-audit-trail-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 17:12:36.037380 afex-audit-trail-0.1.1/
--rw-rw-rw-   0        0        0     1061 2023-04-04 12:20:36.000000 afex-audit-trail-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6661 2023-04-05 17:12:36.037380 afex-audit-trail-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-05 17:12:36.018506 afex-audit-trail-0.1.1/afex_audit_trail.egg-info/
--rw-rw-rw-   0        0        0     6661 2023-04-05 17:12:35.000000 afex-audit-trail-0.1.1/afex_audit_trail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      681 2023-04-05 17:12:35.000000 afex-audit-trail-0.1.1/afex_audit_trail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 17:12:35.000000 afex-audit-trail-0.1.1/afex_audit_trail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-05 17:12:35.000000 afex-audit-trail-0.1.1/afex_audit_trail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-05 17:12:35.000000 afex-audit-trail-0.1.1/afex_audit_trail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 17:12:36.021013 afex-audit-trail-0.1.1/audit_trails/
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.1/audit_trails/__init__.py
--rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.1/audit_trails/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-05 17:12:36.037380 afex-audit-trail-0.1.1/audit_trails/api/
--rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.1.1/audit_trails/api/__init__.py
--rw-rw-rw-   0        0        0      708 2023-04-05 12:51:50.000000 afex-audit-trail-0.1.1/audit_trails/api/serializers.py
--rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.1.1/audit_trails/api/urls.py
--rw-rw-rw-   0        0        0     3096 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.1/audit_trails/api/views.py
--rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.1/audit_trails/apps.py
--rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.1.1/audit_trails/logger.py
--rw-rw-rw-   0        0        0     3164 2023-04-05 10:39:42.000000 afex-audit-trail-0.1.1/audit_trails/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-05 17:12:36.037380 afex-audit-trail-0.1.1/audit_trails/migrations/
--rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.1.1/audit_trails/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.1/audit_trails/migrations/__init__.py
--rw-rw-rw-   0        0        0     3438 2023-04-04 08:39:29.000000 afex-audit-trail-0.1.1/audit_trails/models.py
--rw-rw-rw-   0        0        0     1072 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.1/audit_trails/signals.py
--rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.1/audit_trails/tests.py
--rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.1/audit_trails/urls.py
--rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.1/audit_trails/views.py
--rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      987 2023-04-05 17:12:36.037380 afex-audit-trail-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:17:54.477253 afex-audit-trail-0.1.2/
+-rw-rw-rw-   0        0        0     1061 2023-04-04 12:20:36.000000 afex-audit-trail-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6661 2023-04-09 17:17:54.477253 afex-audit-trail-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-09 17:17:54.272490 afex-audit-trail-0.1.2/afex_audit_trail.egg-info/
+-rw-rw-rw-   0        0        0     6661 2023-04-09 17:17:52.000000 afex-audit-trail-0.1.2/afex_audit_trail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2023-04-09 17:17:52.000000 afex-audit-trail-0.1.2/afex_audit_trail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 17:17:52.000000 afex-audit-trail-0.1.2/afex_audit_trail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-04-09 17:17:52.000000 afex-audit-trail-0.1.2/afex_audit_trail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-09 17:17:52.000000 afex-audit-trail-0.1.2/afex_audit_trail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 17:17:54.413844 afex-audit-trail-0.1.2/audit_trails/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.2/audit_trails/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.2/audit_trails/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:17:54.445355 afex-audit-trail-0.1.2/audit_trails/api/
+-rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.1.2/audit_trails/api/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.1.2/audit_trails/api/serializers.py
+-rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.1.2/audit_trails/api/urls.py
+-rw-rw-rw-   0        0        0     3096 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.2/audit_trails/api/views.py
+-rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.2/audit_trails/apps.py
+-rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.1.2/audit_trails/logger.py
+-rw-rw-rw-   0        0        0     3164 2023-04-05 10:39:42.000000 afex-audit-trail-0.1.2/audit_trails/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:17:54.477253 afex-audit-trail-0.1.2/audit_trails/migrations/
+-rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.1.2/audit_trails/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.2/audit_trails/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3438 2023-04-04 08:39:29.000000 afex-audit-trail-0.1.2/audit_trails/models.py
+-rw-rw-rw-   0        0        0     1072 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.2/audit_trails/signals.py
+-rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.2/audit_trails/tests.py
+-rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.2/audit_trails/urls.py
+-rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.2/audit_trails/views.py
+-rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      987 2023-04-09 17:17:54.477253 afex-audit-trail-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.1.2/setup.py
```

### Comparing `afex-audit-trail-0.1.1/LICENSE` & `afex-audit-trail-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/PKG-INFO` & `afex-audit-trail-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
```

### Comparing `afex-audit-trail-0.1.1/afex_audit_trail.egg-info/PKG-INFO` & `afex-audit-trail-0.1.2/afex_audit_trail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
```

### Comparing `afex-audit-trail-0.1.1/afex_audit_trail.egg-info/SOURCES.txt` & `afex-audit-trail-0.1.2/afex_audit_trail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/audit_trails/api/urls.py` & `afex-audit-trail-0.1.2/audit_trails/api/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/audit_trails/api/views.py` & `afex-audit-trail-0.1.2/audit_trails/api/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/audit_trails/logger.py` & `afex-audit-trail-0.1.2/audit_trails/logger.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/audit_trails/middleware.py` & `afex-audit-trail-0.1.2/audit_trails/middleware.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/audit_trails/migrations/0001_initial.py` & `afex-audit-trail-0.1.2/audit_trails/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/audit_trails/models.py` & `afex-audit-trail-0.1.2/audit_trails/models.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/audit_trails/signals.py` & `afex-audit-trail-0.1.2/audit_trails/signals.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/audit_trails/urls.py` & `afex-audit-trail-0.1.2/audit_trails/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/audit_trails/views.py` & `afex-audit-trail-0.1.2/audit_trails/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.1/setup.cfg` & `afex-audit-trail-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6665 782d 6175 6469 742d 7472   = afex-audit-tr
 00000020: 6169 6c0d 0a76 6572 7369 6f6e 203d 2030  ail..version = 0
-00000030: 2e31 2e31 0d0a 6465 7363 7269 7074 696f  .1.1..descriptio
+00000030: 2e31 2e32 0d0a 6465 7363 7269 7074 696f  .1.2..descriptio
 00000040: 6e20 3d20 4120 446a 616e 676f 2061 7070  n = A Django app
 00000050: 2074 6f20 6372 6561 7465 2073 6572 7665   to create serve
 00000060: 7220 6c6f 6773 2061 6e64 2075 7365 7273  r logs and users
 00000070: 2720 6e6f 7469 6669 6361 7469 6f6e 2e0d  ' notification..
 00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000090: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
 000000a0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
```

