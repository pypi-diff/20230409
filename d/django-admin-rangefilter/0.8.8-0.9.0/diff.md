# Comparing `tmp/django-admin-rangefilter-0.8.8.tar.gz` & `tmp/django-admin-rangefilter-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-rangefilter-0.8.8.tar", last modified: Fri Sep  2 14:23:31 2022, max compression
+gzip compressed data, was "django-admin-rangefilter-0.9.0.tar", last modified: Sun Sep 25 07:08:38 2022, max compression
```

## Comparing `django-admin-rangefilter-0.8.8.tar` & `django-admin-rangefilter-0.9.0.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.743061 django-admin-rangefilter-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)     6579 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (121)     1082 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (121)      287 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3499 2022-09-02 14:23:31.743061 django-admin-rangefilter-0.8.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     2257 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/django_admin_rangefilter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3499 2022-09-02 14:23:31.000000 django-admin-rangefilter-0.8.8/django_admin_rangefilter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-09-02 14:23:31.000000 django-admin-rangefilter-0.8.8/django_admin_rangefilter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 14:23:31.000000 django-admin-rangefilter-0.8.8/django_admin_rangefilter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 14:23:31.000000 django-admin-rangefilter-0.8.8/django_admin_rangefilter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-02 14:23:31.000000 django-admin-rangefilter-0.8.8/django_admin_rangefilter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9309 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/cs_CZ/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/cs_CZ/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/en_US/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/en_US/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/en_US/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.739061 django-admin-rangefilter-0.8.8/rangefilter/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.743061 django-admin-rangefilter-0.8.8/rangefilter/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.743061 django-admin-rangefilter-0.8.8/rangefilter/static/rangefilter/
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/static/rangefilter/iife.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/rangefilter/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.743061 django-admin-rangefilter-0.8.8/rangefilter/templates/rangefilter/
--rw-r--r--   0 runner    (1001) docker     (121)     5631 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/templates/rangefilter/date_filter.html
--rw-r--r--   0 runner    (1001) docker     (121)     3212 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/templates/rangefilter/date_filter_1_8.html
--rw-r--r--   0 runner    (1001) docker     (121)     5193 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/templates/rangefilter/date_filter_csp.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.743061 django-admin-rangefilter-0.8.8/rangefilter/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/rangefilter/templatetags/rangefilter_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-02 14:23:31.743061 django-admin-rangefilter-0.8.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.735061 django-admin-rangefilter-0.8.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:31.743061 django-admin-rangefilter-0.8.8/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 14:23:24.000000 django-admin-rangefilter-0.8.8/tests/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.679417 django-admin-rangefilter-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     6743 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1082 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (121)      287 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-09-25 07:08:38.679417 django-admin-rangefilter-0.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2342 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/django_admin_rangefilter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-09-25 07:08:38.000000 django-admin-rangefilter-0.9.0/django_admin_rangefilter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-09-25 07:08:38.000000 django-admin-rangefilter-0.9.0/django_admin_rangefilter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 07:08:38.000000 django-admin-rangefilter-0.9.0/django_admin_rangefilter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 07:08:38.000000 django-admin-rangefilter-0.9.0/django_admin_rangefilter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-25 07:08:38.000000 django-admin-rangefilter-0.9.0/django_admin_rangefilter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13306 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.667417 django-admin-rangefilter-0.9.0/rangefilter/locale/cs_CZ/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/cs_CZ/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.667417 django-admin-rangefilter-0.9.0/rangefilter/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.667417 django-admin-rangefilter-0.9.0/rangefilter/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/en_US/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/en_US/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/en_US/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      888 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.675418 django-admin-rangefilter-0.9.0/rangefilter/static/rangefilter/
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/static/rangefilter/iife.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/rangefilter/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.679417 django-admin-rangefilter-0.9.0/rangefilter/templates/rangefilter/
+-rw-r--r--   0 runner    (1001) docker     (121)     5631 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/templates/rangefilter/date_filter.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3212 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/templates/rangefilter/date_filter_1_8.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5193 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/templates/rangefilter/date_filter_csp.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2472 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/templates/rangefilter/numeric_filter.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.679417 django-admin-rangefilter-0.9.0/rangefilter/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/rangefilter/templatetags/rangefilter_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-25 07:08:38.679417 django-admin-rangefilter-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.671418 django-admin-rangefilter-0.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:38.679417 django-admin-rangefilter-0.9.0/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 07:08:35.000000 django-admin-rangefilter-0.9.0/tests/migrations/__init__.py
```

### Comparing `django-admin-rangefilter-0.8.8/CHANGELOG.md` & `django-admin-rangefilter-0.9.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ## [Unreleased]
 
+## [0.9.0] - 2022-09-25
+### Added
+- Add filter for integer and float #85
+
 ## [0.8.8] - 2022-09-01
 ### Fix
 - Fix using settings.USE_TZ = False on django4.0+ #85
 
 ## [0.8.7] - 2022-08-13
 ### Added
 - Use admin CSS vars for colors (thx @mharju)
@@ -163,15 +167,16 @@
 - Compatibility Django 2.0
 
 ## [0.3.4] - 2018-03-17
 ### Changed
 - Add get_timezone
 - Drop support Django < 1.8
 
-[Unreleased]: https://github.com/silentsokolov/django-admin-rangefilter/compare/v0.8.8...HEAD
+[Unreleased]: https://github.com/silentsokolov/django-admin-rangefilter/compare/0.9.0...HEAD
+[0.9.0]: https://github.com/silentsokolov/django-admin-rangefilter/compare/v0.8.8...v0.9.0
 [0.8.8]: https://github.com/silentsokolov/django-admin-rangefilter/compare/v0.8.7...v0.8.8
 [0.8.7]: https://github.com/silentsokolov/django-admin-rangefilter/compare/v0.8.6...v0.8.7
 [0.8.6]: https://github.com/silentsokolov/django-admin-rangefilter/compare/v0.8.5...v0.8.6
 [0.8.5]: https://github.com/silentsokolov/django-admin-rangefilter/compare/v0.8.4...v0.8.5
 [0.8.4]: https://github.com/silentsokolov/django-admin-rangefilter/compare/v0.8.3...v0.8.4
 [0.8.3]: https://github.com/silentsokolov/django-admin-rangefilter/compare/v0.8.2...v0.8.3
 [0.8.2]: https://github.com/silentsokolov/django-admin-rangefilter/compare/v0.8.1...v0.8.2
```

### Comparing `django-admin-rangefilter-0.8.8/LICENSE` & `django-admin-rangefilter-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-rangefilter-0.8.8/PKG-INFO` & `django-admin-rangefilter-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-rangefilter
-Version: 0.8.8
+Version: 0.9.0
 Summary: django-admin-rangefilter app, add the filter by a custom date range on the admin UI.
 Home-page: https://github.com/silentsokolov/django-admin-rangefilter
 Author: Dmitriy Sokolov
 Author-email: silentsokolov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,15 +33,15 @@
 
 .. image:: https://codecov.io/gh/silentsokolov/django-admin-rangefilter/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/silentsokolov/django-admin-rangefilter
 
 django-admin-rangefilter
 ========================
 
-A Django app that adds a filter by date range to the admin UI.
+A Django app that adds a filter by date range and numeric range to the admin UI.
 
 .. image:: https://raw.githubusercontent.com/silentsokolov/django-admin-rangefilter/master/docs/images/screenshot.png
 
 
 Requirements
 ------------
 
@@ -77,23 +77,24 @@
 
 In admin
 ~~~~~~~~
 
 .. code:: python
 
     from django.contrib import admin
-    from rangefilter.filters import DateRangeFilter, DateTimeRangeFilter
+    from rangefilter.filters import DateRangeFilter, DateTimeRangeFilter, NumericRangeFilter
 
     from .models import Post
 
 
     @admin.register(Post)
     class PostAdmin(admin.ModelAdmin):
         list_filter = (
             ('created_at', DateRangeFilter), ('updated_at', DateTimeRangeFilter),
+            ('num_value', NumericRangeFilter),
         )
         
         # If you would like to add a default range filter
         # method pattern "get_rangefilter_{field_name}_default"
         def get_rangefilter_created_at_default(self, request):
             return (datetime.date.today, datetime.date.today)
```

### Comparing `django-admin-rangefilter-0.8.8/README.rst` & `django-admin-rangefilter-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 .. image:: https://codecov.io/gh/silentsokolov/django-admin-rangefilter/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/silentsokolov/django-admin-rangefilter
 
 django-admin-rangefilter
 ========================
 
-A Django app that adds a filter by date range to the admin UI.
+A Django app that adds a filter by date range and numeric range to the admin UI.
 
 .. image:: https://raw.githubusercontent.com/silentsokolov/django-admin-rangefilter/master/docs/images/screenshot.png
 
 
 Requirements
 ------------
 
@@ -47,23 +47,24 @@
 
 In admin
 ~~~~~~~~
 
 .. code:: python
 
     from django.contrib import admin
-    from rangefilter.filters import DateRangeFilter, DateTimeRangeFilter
+    from rangefilter.filters import DateRangeFilter, DateTimeRangeFilter, NumericRangeFilter
 
     from .models import Post
 
 
     @admin.register(Post)
     class PostAdmin(admin.ModelAdmin):
         list_filter = (
             ('created_at', DateRangeFilter), ('updated_at', DateTimeRangeFilter),
+            ('num_value', NumericRangeFilter),
         )
         
         # If you would like to add a default range filter
         # method pattern "get_rangefilter_{field_name}_default"
         def get_rangefilter_created_at_default(self, request):
             return (datetime.date.today, datetime.date.today)
```

### Comparing `django-admin-rangefilter-0.8.8/django_admin_rangefilter.egg-info/PKG-INFO` & `django-admin-rangefilter-0.9.0/django_admin_rangefilter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-rangefilter
-Version: 0.8.8
+Version: 0.9.0
 Summary: django-admin-rangefilter app, add the filter by a custom date range on the admin UI.
 Home-page: https://github.com/silentsokolov/django-admin-rangefilter
 Author: Dmitriy Sokolov
 Author-email: silentsokolov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,15 +33,15 @@
 
 .. image:: https://codecov.io/gh/silentsokolov/django-admin-rangefilter/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/silentsokolov/django-admin-rangefilter
 
 django-admin-rangefilter
 ========================
 
-A Django app that adds a filter by date range to the admin UI.
+A Django app that adds a filter by date range and numeric range to the admin UI.
 
 .. image:: https://raw.githubusercontent.com/silentsokolov/django-admin-rangefilter/master/docs/images/screenshot.png
 
 
 Requirements
 ------------
 
@@ -77,23 +77,24 @@
 
 In admin
 ~~~~~~~~
 
 .. code:: python
 
     from django.contrib import admin
-    from rangefilter.filters import DateRangeFilter, DateTimeRangeFilter
+    from rangefilter.filters import DateRangeFilter, DateTimeRangeFilter, NumericRangeFilter
 
     from .models import Post
 
 
     @admin.register(Post)
     class PostAdmin(admin.ModelAdmin):
         list_filter = (
             ('created_at', DateRangeFilter), ('updated_at', DateTimeRangeFilter),
+            ('num_value', NumericRangeFilter),
         )
         
         # If you would like to add a default range filter
         # method pattern "get_rangefilter_{field_name}_default"
         def get_rangefilter_created_at_default(self, request):
             return (datetime.date.today, datetime.date.today)
```

### Comparing `django-admin-rangefilter-0.8.8/django_admin_rangefilter.egg-info/SOURCES.txt` & `django-admin-rangefilter-0.9.0/django_admin_rangefilter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,11 +51,12 @@
 rangefilter/locale/zh_CN/LC_MESSAGES/django.po
 rangefilter/locale/zh_Hans/LC_MESSAGES/django.mo
 rangefilter/locale/zh_Hans/LC_MESSAGES/django.po
 rangefilter/static/rangefilter/iife.js
 rangefilter/templates/rangefilter/date_filter.html
 rangefilter/templates/rangefilter/date_filter_1_8.html
 rangefilter/templates/rangefilter/date_filter_csp.html
+rangefilter/templates/rangefilter/numeric_filter.html
 rangefilter/templatetags/__init__.py
 rangefilter/templatetags/rangefilter_compat.py
 tests/migrations/0001_initial.py
 tests/migrations/__init__.py
```

### Comparing `django-admin-rangefilter-0.8.8/pyproject.toml` & `django-admin-rangefilter-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/filters.py` & `django-admin-rangefilter-0.9.0/rangefilter/filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -273,7 +273,123 @@
             )
         if date_value_lte:
             query_params["{0}__lte".format(self.field_path)] = self.make_dt_aware(
                 date_value_lte, self.get_timezone(request)
             )
 
         return query_params
+
+
+class NumericRangeFilter(admin.filters.FieldListFilter):
+    def __init__(self, field, request, params, model, model_admin, field_path):
+        self.lookup_kwarg_gte = "{0}__range__gte".format(field_path)
+        self.lookup_kwarg_lte = "{0}__range__lte".format(field_path)
+
+        self.default_gte, self.default_lte = self._get_default_values(
+            request, model_admin, field_path
+        )
+
+        super(NumericRangeFilter, self).__init__(
+            field, request, params, model, model_admin, field_path
+        )
+        self.request = request
+        self.model_admin = model_admin
+        self.form = self.get_form(request)
+
+        custom_title = self._get_custom_title(request, model_admin, field_path)
+        if custom_title:
+            self.title = custom_title
+
+    def get_template(self):
+        return "rangefilter/numeric_filter.html"
+
+    template = property(get_template)
+
+    def expected_parameters(self):
+        return self._get_expected_fields()
+
+    def _get_expected_fields(self):
+        return [self.lookup_kwarg_gte, self.lookup_kwarg_lte]
+
+    @staticmethod
+    def _get_custom_title(request, model_admin, field_path):
+        title_method_name = "get_rangefilter_{0}_title".format(field_path)
+        title_method = getattr(model_admin, title_method_name, None)
+
+        if not callable(title_method):
+            return None
+
+        return title_method(request, field_path)
+
+    @staticmethod
+    def _get_default_values(request, model_admin, field_path):
+        default_method_name = "get_rangefilter_{0}_default".format(field_path)
+        default_method = getattr(model_admin, default_method_name, None)
+
+        if not callable(default_method):
+            return None, None
+
+        return default_method(request)
+
+    def get_form(self, _request):
+        form_class = self._get_form_class()
+        return form_class(self.used_parameters or None)
+
+    def _get_form_class(self):
+        fields = self._get_form_fields()
+
+        form_class = type(str("NumericRangeFilter"), (forms.BaseForm,), {"base_fields": fields})
+
+        return form_class
+
+    def _get_form_fields(self):
+        return OrderedDict(
+            (
+                (
+                    self.lookup_kwarg_gte,
+                    forms.FloatField(
+                        label="",
+                        widget=forms.NumberInput(attrs={"placeholder": _("From")}),
+                        required=False,
+                        localize=True,
+                        initial=self.default_lte,
+                    ),
+                ),
+                (
+                    self.lookup_kwarg_lte,
+                    forms.FloatField(
+                        label="",
+                        widget=forms.NumberInput(attrs={"placeholder": _("To")}),
+                        localize=True,
+                        required=False,
+                        initial=self.default_lte,
+                    ),
+                ),
+            )
+        )
+
+    def queryset(self, request, queryset):
+        if self.form.is_valid():
+            validated_data = dict(self.form.cleaned_data.items())
+            if validated_data:
+                return queryset.filter(**self._make_query_filter(request, validated_data))
+        return queryset
+
+    def _make_query_filter(self, _request, validated_data):
+        query_params = {}
+        value_gte = validated_data.get(self.lookup_kwarg_gte, None)
+        value_lte = validated_data.get(self.lookup_kwarg_lte, None)
+
+        if value_gte:
+            query_params["{0}__gte".format(self.field_path)] = value_gte
+        if value_lte:
+            query_params["{0}__lte".format(self.field_path)] = value_lte
+
+        return query_params
+
+    def choices(self, changelist):
+        yield {
+            "system_name": force_str(
+                slugify(self.title) if slugify(self.title) else id(self.title)
+            ),
+            "query_string": changelist.get_query_string({}, remove=self._get_expected_fields()),
+        }
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/cs_CZ/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,21 +9,27 @@
 "Language: cs_CZ\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
+msgid "From"
+msgstr "Od"
+
 msgid "From date"
 msgstr "Od data"
 
 msgid "Range Filter"
 msgstr "Filtr rozsahu"
 
 msgid "Reset"
 msgstr "Resetovat"
 
 msgid "Search"
 msgstr "Vyhledat"
 
+msgid "To"
+msgstr "Do"
+
 msgid "To date"
 msgstr "Do data"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/da/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/da/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,21 +8,27 @@
 "teams/95736/da/)\n"
 "Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+msgid "From"
+msgstr "Fra"
+
 msgid "From date"
 msgstr "Fra dato"
 
 msgid "Range Filter"
 msgstr "Datofilter"
 
 msgid "Reset"
 msgstr "Nulstil"
 
 msgid "Search"
 msgstr "Søg"
 
+msgid "To"
+msgstr "Til"
+
 msgid "To date"
 msgstr "Til dato"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/da/LC_MESSAGES/django.po` & `django-admin-rangefilter-0.9.0/rangefilter/locale/da/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -7,41 +7,51 @@
 # Dmitriy Sokolov <silentsokolov@gmail.com>, 2020
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-20 16:01+0300\n"
+"POT-Creation-Date: 2022-09-25 09:48+0300\n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
 "Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2020\n"
 "Language-Team: Danish (https://www.transifex.com/django-admin-rangefilter/"
 "teams/95736/da/)\n"
 "Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: apps.py:18
+#: apps.py:16
 msgid "Range Filter"
 msgstr "Datofilter"
 
-#: filter.py:171 filter.py:222
+#: filters.py:210 filters.py:246
 msgid "From date"
 msgstr "Fra dato"
 
-#: filter.py:178 filter.py:229
+#: filters.py:220 filters.py:256
 msgid "To date"
 msgstr "Til dato"
 
-#: templates/rangefilter/date_filter.html:135
-#: templates/rangefilter/date_filter_1_8.html:89
-#: templates/rangefilter/date_filter_csp.html:137
-msgid "Search"
-msgstr "Søg"
+#: filters.py:351
+msgid "From"
+msgstr "Fra"
+
+#: filters.py:361
+msgid "To"
+msgstr "Til"
 
-#: templates/rangefilter/date_filter.html:136
+#: templates/rangefilter/date_filter.html:139
 #: templates/rangefilter/date_filter_1_8.html:90
 #: templates/rangefilter/date_filter_csp.html:138
+#: templates/rangefilter/numeric_filter.html:55
+msgid "Search"
+msgstr "Søg"
+
+#: templates/rangefilter/date_filter.html:140
+#: templates/rangefilter/date_filter_1_8.html:91
+#: templates/rangefilter/date_filter_csp.html:139
+#: templates/rangefilter/numeric_filter.html:56
 msgid "Reset"
 msgstr "Nulstil"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/de/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/de/LC_MESSAGES/django.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,21 +8,27 @@
 "teams/95736/de/)\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+msgid "From"
+msgstr "Von"
+
 msgid "From date"
 msgstr "Von"
 
 msgid "Range Filter"
 msgstr "Bereichsfilter"
 
 msgid "Reset"
 msgstr "Zurücksetzen"
 
 msgid "Search"
 msgstr "Suchen"
 
+msgid "To"
+msgstr "Bis"
+
 msgid "To date"
 msgstr "Bis"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/de/LC_MESSAGES/django.po` & `django-admin-rangefilter-0.9.0/rangefilter/locale/ru/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-# Translators:
-# Fabien Schwob <trad@x-phuture.com>, 2019
-#
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-20 16:01+0300\n"
+"POT-Creation-Date: 2022-09-25 09:48+0300\n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Fabien Schwob <trad@x-phuture.com>, 2019\n"
-"Language-Team: German (https://www.transifex.com/django-admin-rangefilter/"
-"teams/95736/de/)\n"
-"Language: de\n"
+"Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2019\n"
+"Language-Team: Russian (https://www.transifex.com/django-admin-rangefilter/"
+"teams/95736/ru/)\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
+"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
+"%100>=11 && n%100<=14)? 2 : 3);\n"
 
-#: apps.py:18
+#: apps.py:16
 msgid "Range Filter"
-msgstr "Bereichsfilter"
+msgstr "Фильтр диапазона"
 
-#: filter.py:171 filter.py:222
+#: filters.py:210 filters.py:246
 msgid "From date"
-msgstr "Von"
+msgstr "С даты"
 
-#: filter.py:178 filter.py:229
+#: filters.py:220 filters.py:256
 msgid "To date"
-msgstr "Bis"
+msgstr "По дату"
 
-#: templates/rangefilter/date_filter.html:135
-#: templates/rangefilter/date_filter_1_8.html:89
-#: templates/rangefilter/date_filter_csp.html:137
-msgid "Search"
-msgstr "Suchen"
+#: filters.py:351
+msgid "From"
+msgstr "С"
+
+#: filters.py:361
+msgid "To"
+msgstr "До"
 
-#: templates/rangefilter/date_filter.html:136
+#: templates/rangefilter/date_filter.html:139
 #: templates/rangefilter/date_filter_1_8.html:90
 #: templates/rangefilter/date_filter_csp.html:138
+#: templates/rangefilter/numeric_filter.html:55
+msgid "Search"
+msgstr "Поиск"
+
+#: templates/rangefilter/date_filter.html:140
+#: templates/rangefilter/date_filter_1_8.html:91
+#: templates/rangefilter/date_filter_csp.html:139
+#: templates/rangefilter/numeric_filter.html:56
 msgid "Reset"
-msgstr "Zurücksetzen"
+msgstr "Сбросить"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/el/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/es/LC_MESSAGES/django.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,34 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Dimitris Karagiannis <mitch.karajohn@gmail.com>, 2021\n"
-"Language-Team: Greek (https://www.transifex.com/django-admin-rangefilter/"
-"teams/95736/el/)\n"
-"Language: el\n"
+"Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2019\n"
+"Language-Team: Spanish (https://www.transifex.com/django-admin-rangefilter/"
+"teams/95736/es/)\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+msgid "From"
+msgstr "Desde"
+
 msgid "From date"
-msgstr "Από"
+msgstr "Desde"
 
 msgid "Range Filter"
-msgstr "Φίλτρο εύρους"
+msgstr "Filtro de Rango"
 
 msgid "Reset"
-msgstr "Επαναφορά"
+msgstr "Reiniciar"
 
 msgid "Search"
-msgstr "Αναζήτηση"
+msgstr "Buscar"
+
+msgid "To"
+msgstr "Hasta"
 
 msgid "To date"
-msgstr "Εως"
+msgstr "Hasta"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/el/LC_MESSAGES/django.po` & `django-admin-rangefilter-0.9.0/rangefilter/locale/pl/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,59 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 # Translators:
-# Dimitris Karagiannis <mitch.karajohn@gmail.com>, 2021
+# sqlmiles <sqlmiles@gmail.com>, 2020
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-20 16:01+0300\n"
+"POT-Creation-Date: 2022-09-25 09:48+0300\n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Dimitris Karagiannis <mitch.karajohn@gmail.com>, 2021\n"
-"Language-Team: Greek (https://www.transifex.com/django-admin-rangefilter/"
-"teams/95736/el/)\n"
-"Language: el\n"
+"Last-Translator: sqlmiles <sqlmiles@gmail.com>, 2020\n"
+"Language-Team: Polish (https://www.transifex.com/django-admin-rangefilter/"
+"teams/95736/pl/)\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n"
+"%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n"
+"%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
-#: apps.py:18
+#: apps.py:16
 msgid "Range Filter"
-msgstr "Φίλτρο εύρους"
+msgstr "Filtr zakresu dat"
 
-#: filter.py:171 filter.py:222
+#: filters.py:210 filters.py:246
 msgid "From date"
-msgstr "Από"
+msgstr "Od"
 
-#: filter.py:178 filter.py:229
+#: filters.py:220 filters.py:256
 msgid "To date"
-msgstr "Εως"
+msgstr "Do"
 
-#: templates/rangefilter/date_filter.html:135
-#: templates/rangefilter/date_filter_1_8.html:89
-#: templates/rangefilter/date_filter_csp.html:137
-msgid "Search"
-msgstr "Αναζήτηση"
+#: filters.py:351
+msgid "From"
+msgstr "Od"
+
+#: filters.py:361
+msgid "To"
+msgstr "Do"
 
-#: templates/rangefilter/date_filter.html:136
+#: templates/rangefilter/date_filter.html:139
 #: templates/rangefilter/date_filter_1_8.html:90
 #: templates/rangefilter/date_filter_csp.html:138
+#: templates/rangefilter/numeric_filter.html:55
+msgid "Search"
+msgstr "Szukaj"
+
+#: templates/rangefilter/date_filter.html:140
+#: templates/rangefilter/date_filter_1_8.html:91
+#: templates/rangefilter/date_filter_csp.html:139
+#: templates/rangefilter/numeric_filter.html:56
 msgid "Reset"
-msgstr "Επαναφορά"
+msgstr "Resetuj"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/en_US/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/en_US/LC_MESSAGES/django.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -6,21 +6,27 @@
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
+msgid "From"
+msgstr "From"
+
 msgid "From date"
 msgstr "From date"
 
 msgid "Range Filter"
 msgstr "Range Filter"
 
 msgid "Reset"
 msgstr "Reset"
 
 msgid "Search"
 msgstr "Search"
 
+msgid "To"
+msgstr "To"
+
 msgid "To date"
 msgstr "To date"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/en_US/LC_MESSAGES/django.po` & `django-admin-rangefilter-0.9.0/rangefilter/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+# Translators:
+# Jian Dai <daijian1@qq.com>, 2020
+#
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-20 16:01+0300\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2022-09-25 09:48+0300\n"
+"PO-Revision-Date: 2019-01-31 09:16+0000\n"
+"Last-Translator: Jian Dai <daijian1@qq.com>, 2020\n"
+"Language-Team: Chinese (China) (https://www.transifex.com/django-admin-"
+"rangefilter/teams/95736/zh_CN/)\n"
+"Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: apps.py:18
+#: apps.py:16
 msgid "Range Filter"
-msgstr "Range Filter"
+msgstr "区间过滤器"
 
-#: filter.py:171 filter.py:222
+#: filters.py:210 filters.py:246
 msgid "From date"
-msgstr "From date"
+msgstr "从"
 
-#: filter.py:178 filter.py:229
+#: filters.py:220 filters.py:256
 msgid "To date"
-msgstr "To date"
+msgstr "到"
 
-#: templates/rangefilter/date_filter.html:135
-#: templates/rangefilter/date_filter_1_8.html:89
-#: templates/rangefilter/date_filter_csp.html:137
-msgid "Search"
-msgstr "Search"
+#: filters.py:351
+msgid "From"
+msgstr "从"
+
+#: filters.py:361
+msgid "To"
+msgstr "到"
 
-#: templates/rangefilter/date_filter.html:136
+#: templates/rangefilter/date_filter.html:139
 #: templates/rangefilter/date_filter_1_8.html:90
 #: templates/rangefilter/date_filter_csp.html:138
+#: templates/rangefilter/numeric_filter.html:55
+msgid "Search"
+msgstr "搜索"
+
+#: templates/rangefilter/date_filter.html:140
+#: templates/rangefilter/date_filter_1_8.html:91
+#: templates/rangefilter/date_filter_csp.html:139
+#: templates/rangefilter/numeric_filter.html:56
 msgid "Reset"
-msgstr "Reset"
+msgstr "重置"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/es/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/ja/LC_MESSAGES/django.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,28 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2019\n"
-"Language-Team: Spanish (https://www.transifex.com/django-admin-rangefilter/"
-"teams/95736/es/)\n"
-"Language: es\n"
+"Last-Translator: syachi <syachi-reg@brownmush.net>, 2020\n"
+"Language-Team: Japanese (https://www.transifex.com/django-admin-rangefilter/"
+"teams/95736/ja/)\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "From date"
-msgstr "Desde"
+msgstr "開始"
 
 msgid "Range Filter"
-msgstr "Filtro de Rango"
+msgstr "範囲フィルター"
 
 msgid "Reset"
-msgstr "Reiniciar"
+msgstr "リセット"
 
 msgid "Search"
-msgstr "Buscar"
+msgstr "検索"
 
 msgid "To date"
-msgstr "Hasta"
+msgstr "終了"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/es/LC_MESSAGES/django.po` & `django-admin-rangefilter-0.9.0/rangefilter/locale/el/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+# Translators:
+# Dimitris Karagiannis <mitch.karajohn@gmail.com>, 2021
+#
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-20 16:01+0300\n"
+"POT-Creation-Date: 2022-09-25 09:48+0300\n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2019\n"
-"Language-Team: Spanish (https://www.transifex.com/django-admin-rangefilter/"
-"teams/95736/es/)\n"
-"Language: es\n"
+"Last-Translator: Dimitris Karagiannis <mitch.karajohn@gmail.com>, 2021\n"
+"Language-Team: Greek (https://www.transifex.com/django-admin-rangefilter/"
+"teams/95736/el/)\n"
+"Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: apps.py:18
+#: apps.py:16
 msgid "Range Filter"
-msgstr "Filtro de Rango"
+msgstr "Φίλτρο εύρους"
 
-#: filter.py:171 filter.py:222
+#: filters.py:210 filters.py:246
 msgid "From date"
-msgstr "Desde"
+msgstr "Από"
 
-#: filter.py:178 filter.py:229
+#: filters.py:220 filters.py:256
 msgid "To date"
-msgstr "Hasta"
+msgstr "Εως"
 
-#: templates/rangefilter/date_filter.html:135
-#: templates/rangefilter/date_filter_1_8.html:89
-#: templates/rangefilter/date_filter_csp.html:137
-msgid "Search"
-msgstr "Buscar"
+#: filters.py:351
+msgid "From"
+msgstr "Από"
+
+#: filters.py:361
+msgid "To"
+msgstr "Εως"
 
-#: templates/rangefilter/date_filter.html:136
+#: templates/rangefilter/date_filter.html:139
 #: templates/rangefilter/date_filter_1_8.html:90
 #: templates/rangefilter/date_filter_csp.html:138
+#: templates/rangefilter/numeric_filter.html:55
+msgid "Search"
+msgstr "Αναζήτηση"
+
+#: templates/rangefilter/date_filter.html:140
+#: templates/rangefilter/date_filter_1_8.html:91
+#: templates/rangefilter/date_filter_csp.html:139
+#: templates/rangefilter/numeric_filter.html:56
 msgid "Reset"
-msgstr "Reiniciar"
+msgstr "Επαναφορά"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/es_AR/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,34 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2019\n"
-"Language-Team: Spanish (Argentina) (https://www.transifex.com/django-admin-"
-"rangefilter/teams/95736/es_AR/)\n"
-"Language: es_AR\n"
+"Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2020\n"
+"Language-Team: Portuguese (Portugal) (https://www.transifex.com/django-admin-"
+"rangefilter/teams/95736/pt_PT/)\n"
+"Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+msgid "From"
+msgstr "Inicial"
+
 msgid "From date"
-msgstr "Desde"
+msgstr "Data inicial"
 
 msgid "Range Filter"
-msgstr "Seleccionar Rango"
+msgstr "Range Filter"
 
 msgid "Reset"
-msgstr "Quitar filtros"
+msgstr "Limpar"
 
 msgid "Search"
-msgstr "Aplicar filtros"
+msgstr "Pesquisar"
+
+msgid "To"
+msgstr "Final"
 
 msgid "To date"
-msgstr "Hasta"
+msgstr "Data final"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/es_AR/LC_MESSAGES/django.po` & `django-admin-rangefilter-0.9.0/rangefilter/locale/ja/LC_MESSAGES/django.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+# Translators:
+# syachi <syachi-reg@brownmush.net>, 2020
+#
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-20 16:01+0300\n"
+"POT-Creation-Date: 2022-09-25 09:48+0300\n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2019\n"
-"Language-Team: Spanish (Argentina) (https://www.transifex.com/django-admin-"
-"rangefilter/teams/95736/es_AR/)\n"
-"Language: es_AR\n"
+"Last-Translator: syachi <syachi-reg@brownmush.net>, 2020\n"
+"Language-Team: Japanese (https://www.transifex.com/django-admin-rangefilter/"
+"teams/95736/ja/)\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: apps.py:18
+#: apps.py:16
 msgid "Range Filter"
-msgstr "Seleccionar Rango"
+msgstr "範囲フィルター"
 
-#: filter.py:171 filter.py:222
+#: filters.py:210 filters.py:246
 msgid "From date"
-msgstr "Desde"
+msgstr "開始"
 
-#: filter.py:178 filter.py:229
+#: filters.py:220 filters.py:256
 msgid "To date"
-msgstr "Hasta"
+msgstr "終了"
 
-#: templates/rangefilter/date_filter.html:135
-#: templates/rangefilter/date_filter_1_8.html:89
-#: templates/rangefilter/date_filter_csp.html:137
-msgid "Search"
-msgstr "Aplicar filtros"
+#: filters.py:351
+msgid "From"
+msgstr ""
 
-#: templates/rangefilter/date_filter.html:136
+#: filters.py:361
+msgid "To"
+msgstr ""
+
+#: templates/rangefilter/date_filter.html:139
 #: templates/rangefilter/date_filter_1_8.html:90
 #: templates/rangefilter/date_filter_csp.html:138
+#: templates/rangefilter/numeric_filter.html:55
+msgid "Search"
+msgstr "検索"
+
+#: templates/rangefilter/date_filter.html:140
+#: templates/rangefilter/date_filter_1_8.html:91
+#: templates/rangefilter/date_filter_csp.html:139
+#: templates/rangefilter/numeric_filter.html:56
 msgid "Reset"
-msgstr "Quitar filtros"
+msgstr "リセット"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/fa/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/fa/LC_MESSAGES/django.po` & `django-admin-rangefilter-0.9.0/rangefilter/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <shahmohammadiemes@gmail.com>, YEAR.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+# Translators:
+# Jian Dai <daijian1@qq.com>, 2020
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-12 23:54+0430\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Mahdi Shahmohammadi <shahmohammadiemes@gmail.com>\n"
-"Language-Team: Iran \n"
-"Language: \n"
+"POT-Creation-Date: 2022-09-25 09:48+0300\n"
+"PO-Revision-Date: 2019-01-31 09:16+0000\n"
+"Last-Translator: Jian Dai <daijian1@qq.com>, 2020\n"
+"Language-Team: Chinese (China) (https://www.transifex.com/django-admin-"
+"rangefilter/teams/95736/zh_CN/)\n"
+"Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: apps.py:16
 msgid "Range Filter"
-msgstr "محدوده فیلتر"
+msgstr "区间过滤器"
 
 #: filters.py:210 filters.py:246
 msgid "From date"
-msgstr "از روز"
+msgstr "从"
 
 #: filters.py:220 filters.py:256
 msgid "To date"
-msgstr "تا روز"
+msgstr "到"
+
+#: filters.py:351
+msgid "From"
+msgstr "从"
+
+#: filters.py:361
+msgid "To"
+msgstr "到"
 
 #: templates/rangefilter/date_filter.html:139
 #: templates/rangefilter/date_filter_1_8.html:90
 #: templates/rangefilter/date_filter_csp.html:138
+#: templates/rangefilter/numeric_filter.html:55
 msgid "Search"
-msgstr "جست و جو"
+msgstr "搜索"
 
 #: templates/rangefilter/date_filter.html:140
 #: templates/rangefilter/date_filter_1_8.html:91
 #: templates/rangefilter/date_filter_csp.html:139
+#: templates/rangefilter/numeric_filter.html:56
 msgid "Reset"
-msgstr "بازنشانی"
+msgstr "重置"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/fr/LC_MESSAGES/django.po` & `django-admin-rangefilter-0.9.0/rangefilter/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 # Translators:
-# Fabien Schwob <trad@x-phuture.com>, 2019
+# Michal S <Michal.Semenka@gmail.com>, 2019
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-20 16:01+0300\n"
+"POT-Creation-Date: 2022-09-25 09:48+0300\n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Fabien Schwob <trad@x-phuture.com>, 2019\n"
-"Language-Team: French (https://www.transifex.com/django-admin-rangefilter/"
-"teams/95736/fr/)\n"
-"Language: fr\n"
+"Last-Translator: Michal S <Michal.Semenka@gmail.com>, 2019\n"
+"Language-Team: Czech (Czech Republic) (https://www.transifex.com/django-"
+"admin-rangefilter/teams/95736/cs_CZ/)\n"
+"Language: cs_CZ\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
-#: apps.py:18
+#: apps.py:16
 msgid "Range Filter"
-msgstr "Filtre par tranche"
+msgstr "Filtr rozsahu"
 
-#: filter.py:171 filter.py:222
+#: filters.py:210 filters.py:246
 msgid "From date"
-msgstr "Depuis la date"
+msgstr "Od data"
 
-#: filter.py:178 filter.py:229
+#: filters.py:220 filters.py:256
 msgid "To date"
-msgstr "Jusqu'à la date"
+msgstr "Do data"
 
-#: templates/rangefilter/date_filter.html:135
-#: templates/rangefilter/date_filter_1_8.html:89
-#: templates/rangefilter/date_filter_csp.html:137
-msgid "Search"
-msgstr "Chercher"
+#: filters.py:351
+msgid "From"
+msgstr "Od"
+
+#: filters.py:361
+msgid "To"
+msgstr "Do"
 
-#: templates/rangefilter/date_filter.html:136
+#: templates/rangefilter/date_filter.html:139
 #: templates/rangefilter/date_filter_1_8.html:90
 #: templates/rangefilter/date_filter_csp.html:138
+#: templates/rangefilter/numeric_filter.html:55
+msgid "Search"
+msgstr "Vyhledat"
+
+#: templates/rangefilter/date_filter.html:140
+#: templates/rangefilter/date_filter_1_8.html:91
+#: templates/rangefilter/date_filter_csp.html:139
+#: templates/rangefilter/numeric_filter.html:56
 msgid "Reset"
-msgstr "Réinitialiser"
+msgstr "Resetovat"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/it/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/it/LC_MESSAGES/django.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,21 +8,27 @@
 "teams/95736/it/)\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+msgid "From"
+msgstr "Da"
+
 msgid "From date"
 msgstr "Da"
 
 msgid "Range Filter"
 msgstr "Filtra per intervallo"
 
 msgid "Reset"
 msgstr "Reimposta"
 
 msgid "Search"
 msgstr "Cerca"
 
+msgid "To"
+msgstr "A"
+
 msgid "To date"
 msgstr "A"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/ja/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,34 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: syachi <syachi-reg@brownmush.net>, 2020\n"
-"Language-Team: Japanese (https://www.transifex.com/django-admin-rangefilter/"
-"teams/95736/ja/)\n"
-"Language: ja\n"
+"Last-Translator: Jian Dai <daijian1@qq.com>, 2020\n"
+"Language-Team: Chinese (China) (https://www.transifex.com/django-admin-"
+"rangefilter/teams/95736/zh_CN/)\n"
+"Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
+msgid "From"
+msgstr "从"
+
 msgid "From date"
-msgstr "開始"
+msgstr "从"
 
 msgid "Range Filter"
-msgstr "範囲フィルター"
+msgstr "区间过滤器"
 
 msgid "Reset"
-msgstr "リセット"
+msgstr "重置"
 
 msgid "Search"
-msgstr "検索"
+msgstr "搜索"
+
+msgid "To"
+msgstr "到"
 
 msgid "To date"
-msgstr "終了"
+msgstr "到"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/pl/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/ru/LC_MESSAGES/django.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,30 +1,36 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: sqlmiles <sqlmiles@gmail.com>, 2020\n"
-"Language-Team: Polish (https://www.transifex.com/django-admin-rangefilter/"
-"teams/95736/pl/)\n"
-"Language: pl\n"
+"Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2019\n"
+"Language-Team: Russian (https://www.transifex.com/django-admin-rangefilter/"
+"teams/95736/ru/)\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
-"(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
-"n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+
+msgid "From"
+msgstr "С"
 
 msgid "From date"
-msgstr "Od"
+msgstr "С даты"
 
 msgid "Range Filter"
-msgstr "Filtr zakresu dat"
+msgstr "Фильтр диапазона"
 
 msgid "Reset"
-msgstr "Resetuj"
+msgstr "Сбросить"
 
 msgid "Search"
-msgstr "Szukaj"
+msgstr "Поиск"
+
+msgid "To"
+msgstr "До"
 
 msgid "To date"
-msgstr "Do"
+msgstr "По дату"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/pt_PT/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,34 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2020\n"
-"Language-Team: Portuguese (Portugal) (https://www.transifex.com/django-admin-"
-"rangefilter/teams/95736/pt_PT/)\n"
-"Language: pt_PT\n"
+"Last-Translator: Jian Dai <daijian1@qq.com>, 2020\n"
+"Language-Team: Chinese (China) (https://www.transifex.com/django-admin-"
+"rangefilter/teams/95736/zh_CN/)\n"
+"Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+msgid "From"
+msgstr "从"
 
 msgid "From date"
-msgstr "Data inicial"
+msgstr "从"
 
 msgid "Range Filter"
-msgstr "Range Filter"
+msgstr "区间过滤器"
 
 msgid "Reset"
-msgstr "Limpar"
+msgstr "重置"
 
 msgid "Search"
-msgstr "Pesquisar"
+msgstr "搜索"
+
+msgid "To"
+msgstr "到"
 
 msgid "To date"
-msgstr "Data final"
+msgstr "到"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/uk/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/uk/LC_MESSAGES/django.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -11,21 +11,27 @@
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
+msgid "From"
+msgstr "З"
+
 msgid "From date"
 msgstr "З дати"
 
 msgid "Range Filter"
 msgstr "Фільтр діапазону"
 
 msgid "Reset"
 msgstr "Скинути"
 
 msgid "Search"
 msgstr "Пошук"
 
+msgid "To"
+msgstr "По"
+
 msgid "To date"
 msgstr "По дату"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/uk/LC_MESSAGES/django.po` & `django-admin-rangefilter-0.9.0/rangefilter/locale/uk/LC_MESSAGES/django.po`

 * *Files 26% similar despite different names*

```diff
@@ -7,44 +7,54 @@
 # vadshu <vadik@shustikov.kiev.ua>, 2019
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-20 16:01+0300\n"
+"POT-Creation-Date: 2022-09-25 09:48+0300\n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
 "Last-Translator: vadshu <vadik@shustikov.kiev.ua>, 2019\n"
 "Language-Team: Ukrainian (https://www.transifex.com/django-admin-rangefilter/"
 "teams/95736/uk/)\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
-#: apps.py:18
+#: apps.py:16
 msgid "Range Filter"
 msgstr "Фільтр діапазону"
 
-#: filter.py:171 filter.py:222
+#: filters.py:210 filters.py:246
 msgid "From date"
 msgstr "З дати"
 
-#: filter.py:178 filter.py:229
+#: filters.py:220 filters.py:256
 msgid "To date"
 msgstr "По дату"
 
-#: templates/rangefilter/date_filter.html:135
-#: templates/rangefilter/date_filter_1_8.html:89
-#: templates/rangefilter/date_filter_csp.html:137
-msgid "Search"
-msgstr "Пошук"
+#: filters.py:351
+msgid "From"
+msgstr "З"
+
+#: filters.py:361
+msgid "To"
+msgstr "По"
 
-#: templates/rangefilter/date_filter.html:136
+#: templates/rangefilter/date_filter.html:139
 #: templates/rangefilter/date_filter_1_8.html:90
 #: templates/rangefilter/date_filter_csp.html:138
+#: templates/rangefilter/numeric_filter.html:55
+msgid "Search"
+msgstr "Пошук"
+
+#: templates/rangefilter/date_filter.html:140
+#: templates/rangefilter/date_filter_1_8.html:91
+#: templates/rangefilter/date_filter_csp.html:139
+#: templates/rangefilter/numeric_filter.html:56
 msgid "Reset"
 msgstr "Скинути"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/zh_CN/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,34 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Jian Dai <daijian1@qq.com>, 2020\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/django-admin-"
-"rangefilter/teams/95736/zh_CN/)\n"
-"Language: zh_CN\n"
+"Last-Translator: Rui Mineiro <mineiro.rui@gmail.com>, 2020\n"
+"Language-Team: Portuguese (Brazil) (https://www.transifex.com/django-admin-"
+"rangefilter/teams/95736/pt_BR/)\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+
+msgid "From"
+msgstr "Inicial"
 
 msgid "From date"
-msgstr "从"
+msgstr "Data inicial"
 
 msgid "Range Filter"
-msgstr "区间过滤器"
+msgstr "Range Filter"
 
 msgid "Reset"
-msgstr "重置"
+msgstr "Limpar"
 
 msgid "Search"
-msgstr "搜索"
+msgstr "Pesquisar"
+
+msgid "To"
+msgstr "Final"
 
 msgid "To date"
-msgstr "到"
+msgstr "Data final"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-admin-rangefilter-0.9.0/rangefilter/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,34 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2019-01-31 09:16+0000\n"
-"Last-Translator: Jian Dai <daijian1@qq.com>, 2020\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/django-admin-"
-"rangefilter/teams/95736/zh_CN/)\n"
-"Language: zh_CN\n"
+"Last-Translator: Dmitriy Sokolov <silentsokolov@gmail.com>, 2019\n"
+"Language-Team: Spanish (Argentina) (https://www.transifex.com/django-admin-"
+"rangefilter/teams/95736/es_AR/)\n"
+"Language: es_AR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+msgid "From"
+msgstr "Desde"
 
 msgid "From date"
-msgstr "从"
+msgstr "Desde"
 
 msgid "Range Filter"
-msgstr "区间过滤器"
+msgstr "Seleccionar Rango"
 
 msgid "Reset"
-msgstr "重置"
+msgstr "Quitar filtros"
 
 msgid "Search"
-msgstr "搜索"
+msgstr "Aplicar filtros"
+
+msgid "To"
+msgstr "Hasta"
 
 msgid "To date"
-msgstr "到"
+msgstr "Hasta"
```

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/static/rangefilter/iife.js` & `django-admin-rangefilter-0.9.0/rangefilter/static/rangefilter/iife.js`

 * *Files identical despite different names*

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/templates/rangefilter/date_filter.html` & `django-admin-rangefilter-0.9.0/rangefilter/templates/rangefilter/date_filter.html`

 * *Files identical despite different names*

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/templates/rangefilter/date_filter_1_8.html` & `django-admin-rangefilter-0.9.0/rangefilter/templates/rangefilter/date_filter_1_8.html`

 * *Files identical despite different names*

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/templates/rangefilter/date_filter_csp.html` & `django-admin-rangefilter-0.9.0/rangefilter/templates/rangefilter/date_filter_csp.html`

 * *Files identical despite different names*

### Comparing `django-admin-rangefilter-0.8.8/rangefilter/templatetags/rangefilter_compat.py` & `django-admin-rangefilter-0.9.0/rangefilter/templatetags/rangefilter_compat.py`

 * *Files identical despite different names*

### Comparing `django-admin-rangefilter-0.8.8/setup.py` & `django-admin-rangefilter-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-admin-rangefilter-0.8.8/tests/migrations/0001_initial.py` & `django-admin-rangefilter-0.9.0/tests/migrations/0001_initial.py`

 * *Files 23% similar despite different names*

```diff
@@ -42,8 +42,26 @@
                 ),
                 ("created_at", models.DateTimeField()),
             ],
             options={
                 "ordering": ("created_at",),
             },
         ),
+        migrations.CreateModel(
+            name="RangeModelFloat",
+            fields=[
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("float_value", models.FloatField()),
+            ],
+            options={
+                "ordering": ("float_value",),
+            },
+        ),
     ]
```

