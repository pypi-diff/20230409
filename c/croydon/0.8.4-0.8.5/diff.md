# Comparing `tmp/croydon-0.8.4.tar.gz` & `tmp/croydon-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croydon-0.8.4.tar", last modified: Wed Apr  5 20:07:51 2023, max compression
+gzip compressed data, was "croydon-0.8.5.tar", last modified: Sun Apr  9 09:55:49 2023, max compression
```

## Comparing `croydon-0.8.4.tar` & `croydon-0.8.5.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.907530 croydon-0.8.4/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-04-05 20:07:45.000000 croydon-0.8.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-04-05 20:07:45.000000 croydon-0.8.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      269 2023-04-05 20:07:51.906530 croydon-0.8.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.887528 croydon-0.8.4/croydon/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/baseapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.890529 croydon-0.8.4/croydon/cache/
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/cache/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/cache/abc.py
--rw-rw-rw-   0 root         (0) root         (0)     3227 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/cache/memcached.py
--rw-rw-rw-   0 root         (0) root         (0)      450 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/cache/no_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/cache/simple.py
--rw-rw-rw-   0 root         (0) root         (0)     2282 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.891529 croydon-0.8.4/croydon/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/commands/init.py
--rw-rw-rw-   0 root         (0) root         (0)     2308 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/config.py
--rw-rw-rw-   0 root         (0) root         (0)     5628 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/context.py
--rw-rw-rw-   0 root         (0) root         (0)    10824 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/db.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.893529 croydon-0.8.4/croydon/models/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8871 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/models/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/models/counter.py
--rw-rw-rw-   0 root         (0) root         (0)    11546 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/models/index.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/models/meta_model.py
--rw-rw-rw-   0 root         (0) root         (0)     8872 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/models/storable_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3727 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/models/submodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.895529 croydon-0.8.4/croydon/taskq/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/taskq/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/taskq/base_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     3130 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/taskq/mongo_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/taskq/task.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/taskq/types.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/taskq/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.897529 croydon-0.8.4/croydon/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.898529 croydon-0.8.4/croydon/templates/app/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.900529 croydon-0.8.4/croydon/templates/app/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/commands/dev.py
--rw-rw-rw-   0 root         (0) root         (0)     1240 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/commands/index.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/commands/prod.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/commands/shell.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/commands/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.900529 croydon-0.8.4/croydon/templates/app/controllers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/controllers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.900529 croydon-0.8.4/croydon/templates/app/controllers/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/controllers/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.901529 croydon-0.8.4/croydon/templates/app/controllers/api/v1/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/controllers/api/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/controllers/api/v1/account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.902529 croydon-0.8.4/croydon/templates/app/controllers/api/v1/response_types/
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/controllers/api/v1/response_types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/controllers/api/v1/response_types/account.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/extractors.py
--rw-rw-rw-   0 root         (0) root         (0)     1138 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.903529 croydon-0.8.4/croydon/templates/app/models/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      693 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/models/session.py
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/models/token.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.904529 croydon-0.8.4/croydon/templates/app/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/tasks/ping_task.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/app/tasks/worker.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/crcmd.py
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/development.toml
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/production.toml
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/staging.toml
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/templates/testing.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.906530 croydon-0.8.4/croydon/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/tests/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/tests/mongo_mock_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/tests/test_base_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4801 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/tests/test_storable_model.py
--rw-rw-rw-   0 root         (0) root         (0)     5546 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/tests/test_submodel.py
--rw-rw-rw-   0 root         (0) root         (0)     6072 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/tests/test_validators.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/types.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-04-05 20:07:45.000000 croydon-0.8.4/croydon/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:07:51.889528 croydon-0.8.4/croydon.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2023-04-05 20:07:51.000000 croydon-0.8.4/croydon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2282 2023-04-05 20:07:51.000000 croydon-0.8.4/croydon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 20:07:51.000000 croydon-0.8.4/croydon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-05 20:07:51.000000 croydon-0.8.4/croydon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-05 20:07:51.000000 croydon-0.8.4/croydon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-05 20:07:51.000000 croydon-0.8.4/croydon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 20:07:51.907530 croydon-0.8.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-05 20:07:45.000000 croydon-0.8.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.422119 croydon-0.8.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-04-09 09:55:42.000000 croydon-0.8.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-04-09 09:55:43.000000 croydon-0.8.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-09 09:55:49.422119 croydon-0.8.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.403118 croydon-0.8.5/croydon/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/baseapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.406118 croydon-0.8.5/croydon/cache/
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/cache/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/cache/abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3227 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/cache/memcached.py
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/cache/no_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/cache/simple.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.407118 croydon-0.8.5/croydon/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/commands/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5628 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    10824 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/db.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.409118 croydon-0.8.5/croydon/models/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8871 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/models/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/models/counter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11546 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/models/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/models/meta_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8869 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/models/storable_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3727 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/models/submodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.411118 croydon-0.8.5/croydon/taskq/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/taskq/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/taskq/base_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3130 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/taskq/mongo_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/taskq/task.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/taskq/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/taskq/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.413118 croydon-0.8.5/croydon/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.413118 croydon-0.8.5/croydon/templates/app/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.415119 croydon-0.8.5/croydon/templates/app/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/commands/dev.py
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/commands/index.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/commands/prod.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/commands/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/commands/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.416119 croydon-0.8.5/croydon/templates/app/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/controllers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.416119 croydon-0.8.5/croydon/templates/app/controllers/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/controllers/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.416119 croydon-0.8.5/croydon/templates/app/controllers/api/v1/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/controllers/api/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/controllers/api/v1/account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.417119 croydon-0.8.5/croydon/templates/app/controllers/api/v1/response_types/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/controllers/api/v1/response_types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/controllers/api/v1/response_types/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/extractors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.419119 croydon-0.8.5/croydon/templates/app/models/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      693 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/models/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/models/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.419119 croydon-0.8.5/croydon/templates/app/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/tasks/ping_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/app/tasks/worker.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/crcmd.py
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/development.toml
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/production.toml
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/staging.toml
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/templates/testing.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.422119 croydon-0.8.5/croydon/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/tests/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/tests/mongo_mock_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/tests/test_base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5080 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/tests/test_storable_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/tests/test_submodel.py
+-rw-rw-rw-   0 root         (0) root         (0)     6072 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/tests/test_validators.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-04-09 09:55:43.000000 croydon-0.8.5/croydon/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:55:49.405118 croydon-0.8.5/croydon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-09 09:55:49.000000 croydon-0.8.5/croydon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2282 2023-04-09 09:55:49.000000 croydon-0.8.5/croydon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 09:55:49.000000 croydon-0.8.5/croydon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-09 09:55:49.000000 croydon-0.8.5/croydon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-09 09:55:49.000000 croydon-0.8.5/croydon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 09:55:49.000000 croydon-0.8.5/croydon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 09:55:49.422119 croydon-0.8.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-09 09:55:43.000000 croydon-0.8.5/setup.py
```

### Comparing `croydon-0.8.4/LICENSE` & `croydon-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/baseapp.py` & `croydon-0.8.5/croydon/baseapp.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/cache/memcached.py` & `croydon-0.8.5/croydon/cache/memcached.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/cache/simple.py` & `croydon-0.8.5/croydon/cache/simple.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/command.py` & `croydon-0.8.5/croydon/command.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/commands/init.py` & `croydon-0.8.5/croydon/commands/init.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/config.py` & `croydon-0.8.5/croydon/config.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/context.py` & `croydon-0.8.5/croydon/context.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/db.py` & `croydon-0.8.5/croydon/db.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/decorators.py` & `croydon-0.8.5/croydon/decorators.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/errors.py` & `croydon-0.8.5/croydon/errors.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/models/base_model.py` & `croydon-0.8.5/croydon/models/base_model.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/models/counter.py` & `croydon-0.8.5/croydon/models/counter.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/models/fields.py` & `croydon-0.8.5/croydon/models/fields.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/models/index.py` & `croydon-0.8.5/croydon/models/index.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/models/meta_model.py` & `croydon-0.8.5/croydon/models/meta_model.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/models/storable_model.py` & `croydon-0.8.5/croydon/models/storable_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,27 +131,26 @@
         )
 
     @classmethod
     async def get(cls: Type[TModel],
                   expression: str | ObjectId | None,
                   raise_if_none: Optional[Exception] = None) -> Optional[TModel]:
         if expression is None:
+            if raise_if_none:
+                raise raise_if_none
             return None
 
         rexp = resolve_id(expression)
         if isinstance(rexp, ObjectId):
             query = {"_id": rexp}
         else:
             query = {cls.KEY_FIELD: str(rexp)}
         res = await cls.find_one(query)
         if res is None and raise_if_none is not None:
-            if isinstance(raise_if_none, Exception):
-                raise raise_if_none
-            else:
-                raise NotFound(f"{cls.__name__} not found")
+            raise raise_if_none
         return res
 
     @classmethod
     async def count(cls, query: Optional[Dict[str, Any]] = None) -> int:
         if query is None:
             query = {}
         return await cls._db().count_docs(cls.collection, query)
@@ -175,14 +174,16 @@
         await cls._db().update_query(cls.collection, cls._preprocess_query(query), attrs)
 
     @classmethod
     async def cache_get(cls: Type[TModel],
                         expression: str | None,
                         raise_if_none: Optional[Exception] = None) -> Optional[TModel]:
         if expression is None:
+            if raise_if_none:
+                raise raise_if_none
             return None
         cache_key = f"{cls.collection}.{expression}"
         getter = partial(cls.get, expression, raise_if_none)
         return await cls._cache_get(cache_key, getter)
 
     @classmethod
     async def _cache_get(cls: Type[TModel],
```

### Comparing `croydon-0.8.4/croydon/models/submodel.py` & `croydon-0.8.5/croydon/models/submodel.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/taskq/base_queue.py` & `croydon-0.8.5/croydon/taskq/base_queue.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/taskq/mongo_queue.py` & `croydon-0.8.5/croydon/taskq/mongo_queue.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/taskq/task.py` & `croydon-0.8.5/croydon/taskq/task.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/taskq/types.py` & `croydon-0.8.5/croydon/taskq/types.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/commands/dev.py` & `croydon-0.8.5/croydon/templates/app/commands/dev.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/commands/index.py` & `croydon-0.8.5/croydon/templates/app/commands/index.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/commands/prod.py` & `croydon-0.8.5/croydon/templates/app/commands/prod.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/commands/shell.py` & `croydon-0.8.5/croydon/templates/app/commands/shell.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/controllers/api/v1/account.py` & `croydon-0.8.5/croydon/templates/app/controllers/api/v1/account.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/controllers/api/v1/response_types/account.py` & `croydon-0.8.5/croydon/templates/app/controllers/api/v1/response_types/account.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/extractors.py` & `croydon-0.8.5/croydon/templates/app/extractors.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/middleware.py` & `croydon-0.8.5/croydon/templates/app/middleware.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/models/session.py` & `croydon-0.8.5/croydon/templates/app/models/session.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/models/token.py` & `croydon-0.8.5/croydon/templates/app/models/token.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/app/models/user.py` & `croydon-0.8.5/croydon/templates/app/models/user.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/development.toml` & `croydon-0.8.5/croydon/templates/development.toml`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/production.toml` & `croydon-0.8.5/croydon/templates/production.toml`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/staging.toml` & `croydon-0.8.5/croydon/templates/staging.toml`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/templates/testing.toml` & `croydon-0.8.5/croydon/templates/testing.toml`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/tests/mongo_mock_test.py` & `croydon-0.8.5/croydon/tests/mongo_mock_test.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/tests/test_base_model.py` & `croydon-0.8.5/croydon/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/tests/test_storable_model.py` & `croydon-0.8.5/croydon/tests/test_storable_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -134,7 +134,13 @@
         # check normal method usage
         deps = await master.deps().all()
         self.assertEqual(len(deps), 10)
 
         # check deps are accessible via API
         dct = await master.to_dict_ext(fields=["id", "name", "deps"])
         self.assertEqual(len(dct["deps"]), 10)
+
+    async def test_find_by_none_raises(self):
+        with self.assertRaises(ValueError):
+            _ = await TestModel.get(None, ValueError("value error"))
+        with self.assertRaises(ValueError):
+            _ = await TestModel.cache_get(None, ValueError("value error"))
```

### Comparing `croydon-0.8.4/croydon/tests/test_submodel.py` & `croydon-0.8.5/croydon/tests/test_submodel.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/tests/test_validators.py` & `croydon-0.8.5/croydon/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/types.py` & `croydon-0.8.5/croydon/types.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon/util.py` & `croydon-0.8.5/croydon/util.py`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/croydon.egg-info/SOURCES.txt` & `croydon-0.8.5/croydon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `croydon-0.8.4/setup.py` & `croydon-0.8.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="croydon",
-    version="0.8.4",
+    version="0.8.5",
     description="a micro webframework based on fastapi and motor",
     url="https://gitlab.com/viert/croydon",
     author="Pavel Vorobyov",
     author_email="aquavitale@yandex.ru",
     license="MIT",
     packages=[pkg for pkg in find_packages() if pkg.startswith("croydon")],
     include_package_data=True,
```

