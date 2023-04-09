# Comparing `tmp/zibanu-django-1.2.0a3.tar.gz` & `tmp/zibanu-django-1.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-1.2.0a3.tar", last modified: Sun Apr  9 00:05:17 2023, max compression
+gzip compressed data, was "zibanu-django-1.2.0a4.tar", last modified: Sun Apr  9 00:12:54 2023, max compression
```

## Comparing `zibanu-django-1.2.0a3.tar` & `zibanu-django-1.2.0a4.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.041174 zibanu-django-1.2.0a3/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0a3/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      207 2023-03-31 15:51:33.000000 zibanu-django-1.2.0a3/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-04-09 00:05:17.041174 zibanu-django-1.2.0a3/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      158 2023-01-18 12:15:22.000000 zibanu-django-1.2.0a3/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      849 2023-04-09 00:04:23.000000 zibanu-django-1.2.0a3/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-04-09 00:05:17.042173 zibanu-django-1.2.0a3/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.026174 zibanu-django-1.2.0a3/zibanu/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0a3/zibanu/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.027174 zibanu-django-1.2.0a3/zibanu/django/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0a3/zibanu/django/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.027174 zibanu-django-1.2.0a3/zibanu/django/auth/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-1.2.0a3/zibanu/django/auth/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.028174 zibanu-django-1.2.0a3/zibanu/django/auth/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-1.2.0a3/zibanu/django/auth/api/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3430 2023-04-09 00:00:29.000000 zibanu-django-1.2.0a3/zibanu/django/auth/api/serializers.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1647 2023-04-08 23:45:31.000000 zibanu-django-1.2.0a3/zibanu/django/auth/apps.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      637 2023-04-08 12:38:36.000000 zibanu-django-1.2.0a3/zibanu/django/auth/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.028174 zibanu-django-1.2.0a3/zibanu/django/db/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0a3/zibanu/django/db/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.028174 zibanu-django-1.2.0a3/zibanu/django/db/backends/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a3/zibanu/django/db/backends/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.029174 zibanu-django-1.2.0a3/zibanu/django/db/backends/oracle/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a3/zibanu/django/db/backends/oracle/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0a3/zibanu/django/db/backends/oracle/base.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.029174 zibanu-django-1.2.0a3/zibanu/django/db/models/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0a3/zibanu/django/db/models/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0a3/zibanu/django/db/models/dated_model.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0a3/zibanu/django/db/models/manager.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0a3/zibanu/django/db/models/model.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.021174 zibanu-django-1.2.0a3/zibanu/django/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.021174 zibanu-django-1.2.0a3/zibanu/django/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.030174 zibanu-django-1.2.0a3/zibanu/django/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3609 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.030174 zibanu-django-1.2.0a3/zibanu/django/logging/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0a3/zibanu/django/logging/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/logging/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.031174 zibanu-django-1.2.0a3/zibanu/django/logging/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0a3/zibanu/django/logging/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.031174 zibanu-django-1.2.0a3/zibanu/django/logging/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/logging/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/logging/lib/events/on_change_password.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/logging/lib/events/on_login.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/logging/lib/events/on_send_mail.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.031174 zibanu-django-1.2.0a3/zibanu/django/logging/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0a3/zibanu/django/logging/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      453 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/logging/lib/signals.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.022174 zibanu-django-1.2.0a3/zibanu/django/logging/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.022174 zibanu-django-1.2.0a3/zibanu/django/logging/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.032174 zibanu-django-1.2.0a3/zibanu/django/logging/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.032174 zibanu-django-1.2.0a3/zibanu/django/logging/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0a3/zibanu/django/logging/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/logging/migrations/0002_maillog.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0a3/zibanu/django/logging/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/logging/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.033174 zibanu-django-1.2.0a3/zibanu/django/repository/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-03 02:16:47.000000 zibanu-django-1.2.0a3/zibanu/django/repository/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.033174 zibanu-django-1.2.0a3/zibanu/django/repository/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:42:37.000000 zibanu-django-1.2.0a3/zibanu/django/repository/api/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      958 2023-02-03 02:43:10.000000 zibanu-django-1.2.0a3/zibanu/django/repository/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.033174 zibanu-django-1.2.0a3/zibanu/django/repository/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a3/zibanu/django/repository/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.033174 zibanu-django-1.2.0a3/zibanu/django/repository/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      566 2023-02-04 20:47:18.000000 zibanu-django-1.2.0a3/zibanu/django/repository/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      740 2023-02-04 21:36:16.000000 zibanu-django-1.2.0a3/zibanu/django/repository/lib/managers/document.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.033174 zibanu-django-1.2.0a3/zibanu/django/repository/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      593 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a3/zibanu/django/repository/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     6973 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/repository/lib/utils/document_generator.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.023174 zibanu-django-1.2.0a3/zibanu/django/repository/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.023174 zibanu-django-1.2.0a3/zibanu/django/repository/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.034174 zibanu-django-1.2.0a3/zibanu/django/repository/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-02-09 14:40:51.000000 zibanu-django-1.2.0a3/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2664 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/repository/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.034174 zibanu-django-1.2.0a3/zibanu/django/repository/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1372 2023-02-03 02:43:34.000000 zibanu-django-1.2.0a3/zibanu/django/repository/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      427 2023-02-08 14:23:11.000000 zibanu-django-1.2.0a3/zibanu/django/repository/migrations/0002_document_description.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-02-03 02:23:41.000000 zibanu-django-1.2.0a3/zibanu/django/repository/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1575 2023-02-08 14:23:06.000000 zibanu-django-1.2.0a3/zibanu/django/repository/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.034174 zibanu-django-1.2.0a3/zibanu/django/rest_framework/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.035174 zibanu-django-1.2.0a3/zibanu/django/rest_framework/exceptions/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/exceptions/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1967 2022-12-14 09:17:28.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/exceptions/api_exception.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.035174 zibanu-django-1.2.0a3/zibanu/django/rest_framework/fields/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/fields/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/fields/current_user_default.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.035174 zibanu-django-1.2.0a3/zibanu/django/rest_framework/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/serializers/fields.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/serializers/model_serializer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.036174 zibanu-django-1.2.0a3/zibanu/django/rest_framework/viewsets/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/viewsets/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    10439 2023-03-31 16:50:03.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/viewsets/model_viewset.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a3/zibanu/django/rest_framework/viewsets/viewset.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.036174 zibanu-django-1.2.0a3/zibanu/django/template/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0a3/zibanu/django/template/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0a3/zibanu/django/template/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.037174 zibanu-django-1.2.0a3/zibanu/django/template/context_processors/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a3/zibanu/django/template/context_processors/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a3/zibanu/django/template/context_processors/full_static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0a3/zibanu/django/template/context_processors/site.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.025174 zibanu-django-1.2.0a3/zibanu/django/template/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.025174 zibanu-django-1.2.0a3/zibanu/django/template/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.037174 zibanu-django-1.2.0a3/zibanu/django/template/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0a3/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/template/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.038174 zibanu-django-1.2.0a3/zibanu/django/template/templatetags/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0a3/zibanu/django/template/templatetags/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0a3/zibanu/django/template/templatetags/static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0a3/zibanu/django/template/templatetags/string_concat.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0a3/zibanu/django/template/templatetags/subtotal_dict.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0a3/zibanu/django/template/templatetags/sum_dict.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.040174 zibanu-django-1.2.0a3/zibanu/django/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3059 2023-03-14 20:09:11.000000 zibanu-django-1.2.0a3/zibanu/django/utils/code_generator.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0a3/zibanu/django/utils/date_time.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a3/zibanu/django/utils/error_messages.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4325 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/utils/mail.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a3/zibanu/django/utils/request_utils.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1251 2022-12-14 09:24:38.000000 zibanu-django-1.2.0a3/zibanu/django/utils/user.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a3/zibanu/django/utils/validate_cache_code.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:05:17.041174 zibanu-django-1.2.0a3/zibanu_django.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-04-09 00:05:17.000000 zibanu-django-1.2.0a3/zibanu_django.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3621 2023-04-09 00:05:17.000000 zibanu-django-1.2.0a3/zibanu_django.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-04-09 00:05:17.000000 zibanu-django-1.2.0a3/zibanu_django.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       32 2023-04-09 00:05:17.000000 zibanu-django-1.2.0a3/zibanu_django.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-04-09 00:05:17.000000 zibanu-django-1.2.0a3/zibanu_django.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.433503 zibanu-django-1.2.0a4/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0a4/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      207 2023-03-31 15:51:33.000000 zibanu-django-1.2.0a4/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-04-09 00:12:54.433503 zibanu-django-1.2.0a4/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      158 2023-01-18 12:15:22.000000 zibanu-django-1.2.0a4/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      849 2023-04-09 00:11:04.000000 zibanu-django-1.2.0a4/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-04-09 00:12:54.433503 zibanu-django-1.2.0a4/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.417503 zibanu-django-1.2.0a4/zibanu/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0a4/zibanu/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.417503 zibanu-django-1.2.0a4/zibanu/django/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0a4/zibanu/django/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.418503 zibanu-django-1.2.0a4/zibanu/django/auth/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-1.2.0a4/zibanu/django/auth/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.418503 zibanu-django-1.2.0a4/zibanu/django/auth/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-1.2.0a4/zibanu/django/auth/api/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3471 2023-04-09 00:10:08.000000 zibanu-django-1.2.0a4/zibanu/django/auth/api/serializers.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1647 2023-04-08 23:45:31.000000 zibanu-django-1.2.0a4/zibanu/django/auth/apps.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      637 2023-04-08 12:38:36.000000 zibanu-django-1.2.0a4/zibanu/django/auth/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.418503 zibanu-django-1.2.0a4/zibanu/django/db/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0a4/zibanu/django/db/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.419504 zibanu-django-1.2.0a4/zibanu/django/db/backends/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a4/zibanu/django/db/backends/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.419504 zibanu-django-1.2.0a4/zibanu/django/db/backends/oracle/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a4/zibanu/django/db/backends/oracle/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0a4/zibanu/django/db/backends/oracle/base.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.420503 zibanu-django-1.2.0a4/zibanu/django/db/models/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0a4/zibanu/django/db/models/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0a4/zibanu/django/db/models/dated_model.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0a4/zibanu/django/db/models/manager.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0a4/zibanu/django/db/models/model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.414504 zibanu-django-1.2.0a4/zibanu/django/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.414504 zibanu-django-1.2.0a4/zibanu/django/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.420503 zibanu-django-1.2.0a4/zibanu/django/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3609 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.420503 zibanu-django-1.2.0a4/zibanu/django/logging/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0a4/zibanu/django/logging/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.421503 zibanu-django-1.2.0a4/zibanu/django/logging/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.421503 zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_change_password.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_login.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_send_mail.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.421503 zibanu-django-1.2.0a4/zibanu/django/logging/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      453 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/signals.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.414504 zibanu-django-1.2.0a4/zibanu/django/logging/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.414504 zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.422503 zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.422503 zibanu-django-1.2.0a4/zibanu/django/logging/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0a4/zibanu/django/logging/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/migrations/0002_maillog.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0a4/zibanu/django/logging/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.423503 zibanu-django-1.2.0a4/zibanu/django/repository/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-03 02:16:47.000000 zibanu-django-1.2.0a4/zibanu/django/repository/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.423503 zibanu-django-1.2.0a4/zibanu/django/repository/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:42:37.000000 zibanu-django-1.2.0a4/zibanu/django/repository/api/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      958 2023-02-03 02:43:10.000000 zibanu-django-1.2.0a4/zibanu/django/repository/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.423503 zibanu-django-1.2.0a4/zibanu/django/repository/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a4/zibanu/django/repository/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.423503 zibanu-django-1.2.0a4/zibanu/django/repository/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      566 2023-02-04 20:47:18.000000 zibanu-django-1.2.0a4/zibanu/django/repository/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      740 2023-02-04 21:36:16.000000 zibanu-django-1.2.0a4/zibanu/django/repository/lib/managers/document.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.424503 zibanu-django-1.2.0a4/zibanu/django/repository/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      593 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a4/zibanu/django/repository/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     6973 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/repository/lib/utils/document_generator.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.415504 zibanu-django-1.2.0a4/zibanu/django/repository/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.415504 zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.424503 zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-02-09 14:40:51.000000 zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2664 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.425503 zibanu-django-1.2.0a4/zibanu/django/repository/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1372 2023-02-03 02:43:34.000000 zibanu-django-1.2.0a4/zibanu/django/repository/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      427 2023-02-08 14:23:11.000000 zibanu-django-1.2.0a4/zibanu/django/repository/migrations/0002_document_description.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-02-03 02:23:41.000000 zibanu-django-1.2.0a4/zibanu/django/repository/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1575 2023-02-08 14:23:06.000000 zibanu-django-1.2.0a4/zibanu/django/repository/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.425503 zibanu-django-1.2.0a4/zibanu/django/rest_framework/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.425503 zibanu-django-1.2.0a4/zibanu/django/rest_framework/exceptions/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/exceptions/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1967 2022-12-14 09:17:28.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/exceptions/api_exception.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.425503 zibanu-django-1.2.0a4/zibanu/django/rest_framework/fields/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/fields/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/fields/current_user_default.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.426503 zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/fields.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/model_serializer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.426503 zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    10439 2023-03-31 16:50:03.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/model_viewset.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/viewset.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.427503 zibanu-django-1.2.0a4/zibanu/django/template/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0a4/zibanu/django/template/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0a4/zibanu/django/template/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.427503 zibanu-django-1.2.0a4/zibanu/django/template/context_processors/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a4/zibanu/django/template/context_processors/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a4/zibanu/django/template/context_processors/full_static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0a4/zibanu/django/template/context_processors/site.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.416504 zibanu-django-1.2.0a4/zibanu/django/template/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.416504 zibanu-django-1.2.0a4/zibanu/django/template/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.427503 zibanu-django-1.2.0a4/zibanu/django/template/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0a4/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/template/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.428503 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/string_concat.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/subtotal_dict.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/sum_dict.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.432503 zibanu-django-1.2.0a4/zibanu/django/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3059 2023-03-14 20:09:11.000000 zibanu-django-1.2.0a4/zibanu/django/utils/code_generator.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0a4/zibanu/django/utils/date_time.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a4/zibanu/django/utils/error_messages.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4325 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/utils/mail.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/utils/request_utils.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1251 2022-12-14 09:24:38.000000 zibanu-django-1.2.0a4/zibanu/django/utils/user.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a4/zibanu/django/utils/validate_cache_code.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.432503 zibanu-django-1.2.0a4/zibanu_django.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-04-09 00:12:54.000000 zibanu-django-1.2.0a4/zibanu_django.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3621 2023-04-09 00:12:54.000000 zibanu-django-1.2.0a4/zibanu_django.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-04-09 00:12:54.000000 zibanu-django-1.2.0a4/zibanu_django.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       32 2023-04-09 00:12:54.000000 zibanu-django-1.2.0a4/zibanu_django.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-04-09 00:12:54.000000 zibanu-django-1.2.0a4/zibanu_django.egg-info/top_level.txt
```

### Comparing `zibanu-django-1.2.0a3/LICENSE` & `zibanu-django-1.2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/PKG-INFO` & `zibanu-django-1.2.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0a3
+Version: 1.2.0a4
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.2.0a3/pyproject.toml` & `zibanu-django-1.2.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "zibanu-django"
-version = "1.2.0-alpha.3"
+version = "1.2.0-alpha.4"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "Zibanu library for django projects"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `zibanu-django-1.2.0a3/zibanu/__init__.py` & `zibanu-django-1.2.0a4/zibanu/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/apps.py` & `zibanu-django-1.2.0a4/zibanu/django/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/auth/api/serializers.py` & `zibanu-django-1.2.0a4/zibanu/django/auth/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,17 @@
             lst_user_roles.append("guest")
         # Include User Permissions
         if b_include_permissions:
             for user_permission in user.permissions.all():
                 lst_user_permissions.append(user_permission.codename)
 
         token["user"] = dict(full_name=user.get_full_name(), email=user.email, username=user.username,
-                             is_staff=user.is_staff, is_superuser=user.is_superuser, last_login=user.last_login,
-                             roles=lst_user_roles.copy(), permissiones=lst_user_permissions.copy())
+                             is_staff=user.is_staff, is_superuser=user.is_superuser,
+                             last_login=user.last_login.isoformat(), roles=lst_user_roles.copy(),
+                             permissiones=lst_user_permissions.copy())
 
         # Include User Permissions
         if b_include_permissions:
             for user_permission in user.permissions.all():
                 lst_user_permissions.append(user_permission.codename)
             token["permissions"] = lst_user_permissions
         return token
```

### Comparing `zibanu-django-1.2.0a3/zibanu/django/auth/apps.py` & `zibanu-django-1.2.0a4/zibanu/django/auth/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/auth/urls.py` & `zibanu-django-1.2.0a4/zibanu/django/auth/urls.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/db/backends/oracle/base.py` & `zibanu-django-1.2.0a4/zibanu/django/db/backends/oracle/base.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/db/models/__init__.py` & `zibanu-django-1.2.0a4/zibanu/django/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/db/models/dated_model.py` & `zibanu-django-1.2.0a4/zibanu/django/db/models/dated_model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/db/models/manager.py` & `zibanu-django-1.2.0a4/zibanu/django/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/db/models/model.py` & `zibanu-django-1.2.0a4/zibanu/django/db/models/model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a4/zibanu/django/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a4/zibanu/django/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/logging/apps.py` & `zibanu-django-1.2.0a4/zibanu/django/logging/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/logging/lib/events/__init__.py` & `zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/logging/lib/events/on_change_password.py` & `zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_change_password.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/logging/lib/events/on_login.py` & `zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_login.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/logging/lib/events/on_send_mail.py` & `zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_send_mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/logging/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/logging/migrations/0001_initial.py` & `zibanu-django-1.2.0a4/zibanu/django/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/logging/migrations/0002_maillog.py` & `zibanu-django-1.2.0a4/zibanu/django/logging/migrations/0002_maillog.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/logging/models.py` & `zibanu-django-1.2.0a4/zibanu/django/logging/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/repository/apps.py` & `zibanu-django-1.2.0a4/zibanu/django/repository/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/repository/lib/managers/__init__.py` & `zibanu-django-1.2.0a4/zibanu/django/repository/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/repository/lib/managers/document.py` & `zibanu-django-1.2.0a4/zibanu/django/repository/lib/managers/document.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/repository/lib/utils/__init__.py` & `zibanu-django-1.2.0a4/zibanu/django/repository/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/repository/lib/utils/document_generator.py` & `zibanu-django-1.2.0a4/zibanu/django/repository/lib/utils/document_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/repository/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/repository/migrations/0001_initial.py` & `zibanu-django-1.2.0a4/zibanu/django/repository/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/repository/models.py` & `zibanu-django-1.2.0a4/zibanu/django/repository/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/rest_framework/exceptions/__init__.py` & `zibanu-django-1.2.0a4/zibanu/django/rest_framework/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/rest_framework/exceptions/api_exception.py` & `zibanu-django-1.2.0a4/zibanu/django/rest_framework/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/rest_framework/fields/__init__.py` & `zibanu-django-1.2.0a4/zibanu/django/rest_framework/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/rest_framework/fields/current_user_default.py` & `zibanu-django-1.2.0a4/zibanu/django/rest_framework/fields/current_user_default.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/rest_framework/serializers/__init__.py` & `zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/rest_framework/serializers/fields.py` & `zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/rest_framework/serializers/model_serializer.py` & `zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/model_serializer.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/rest_framework/viewsets/__init__.py` & `zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/rest_framework/viewsets/model_viewset.py` & `zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/model_viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/rest_framework/viewsets/viewset.py` & `zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/template/apps.py` & `zibanu-django-1.2.0a4/zibanu/django/template/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/template/context_processors/__init__.py` & `zibanu-django-1.2.0a4/zibanu/django/template/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/template/context_processors/full_static_uri.py` & `zibanu-django-1.2.0a4/zibanu/django/template/context_processors/full_static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/template/context_processors/site.py` & `zibanu-django-1.2.0a4/zibanu/django/template/context_processors/site.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/template/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a4/zibanu/django/template/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/template/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a4/zibanu/django/template/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/template/templatetags/static_uri.py` & `zibanu-django-1.2.0a4/zibanu/django/template/templatetags/static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/template/templatetags/string_concat.py` & `zibanu-django-1.2.0a4/zibanu/django/template/templatetags/string_concat.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/template/templatetags/subtotal_dict.py` & `zibanu-django-1.2.0a4/zibanu/django/template/templatetags/subtotal_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/template/templatetags/sum_dict.py` & `zibanu-django-1.2.0a4/zibanu/django/template/templatetags/sum_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/utils/__init__.py` & `zibanu-django-1.2.0a4/zibanu/django/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/utils/code_generator.py` & `zibanu-django-1.2.0a4/zibanu/django/utils/code_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/utils/date_time.py` & `zibanu-django-1.2.0a4/zibanu/django/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/utils/error_messages.py` & `zibanu-django-1.2.0a4/zibanu/django/utils/error_messages.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/utils/mail.py` & `zibanu-django-1.2.0a4/zibanu/django/utils/mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/utils/request_utils.py` & `zibanu-django-1.2.0a4/zibanu/django/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/utils/user.py` & `zibanu-django-1.2.0a4/zibanu/django/utils/user.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu/django/utils/validate_cache_code.py` & `zibanu-django-1.2.0a4/zibanu/django/utils/validate_cache_code.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a3/zibanu_django.egg-info/PKG-INFO` & `zibanu-django-1.2.0a4/zibanu_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0a3
+Version: 1.2.0a4
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.2.0a3/zibanu_django.egg-info/SOURCES.txt` & `zibanu-django-1.2.0a4/zibanu_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

