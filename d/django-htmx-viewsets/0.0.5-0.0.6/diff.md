# Comparing `tmp/django-htmx-viewsets-0.0.5.tar.gz` & `tmp/django-htmx-viewsets-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-viewsets-0.0.5.tar", last modified: Sat Apr  8 21:38:57 2023, max compression
+gzip compressed data, was "django-htmx-viewsets-0.0.6.tar", last modified: Sun Apr  9 08:37:49 2023, max compression
```

## Comparing `django-htmx-viewsets-0.0.5.tar` & `django-htmx-viewsets-0.0.6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 21:38:51.000000 django-htmx-viewsets-0.0.5/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-08 21:38:57.000000 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-08 21:38:57.000000 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:38:57.000000 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-08 21:38:57.000000 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 21:38:57.000000 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.949133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 21:38:51.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.949133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/bootstrap/5.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    60404 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.949133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/datatables/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    87108 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.949133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/css/
--rw-r--r--   0 runner    (1001) docker     (123)   102025 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/htmx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/htmx/1.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/jquery/3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/select2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/select2/4.1.0-rc.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/full.html
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/modal/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/partial.html
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templatetags/htmx_viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 08:37:39.000000 django-htmx-viewsets-0.0.6/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.196925 django-htmx-viewsets-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-09 08:37:49.000000 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-09 08:37:49.000000 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:37:49.000000 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-09 08:37:49.000000 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-09 08:37:49.000000 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.204925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 08:37:39.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.196925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.204925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    60404 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.196925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.204925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    87108 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.196925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.204925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   102025 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.208925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/htmx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.208925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/htmx/1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.208925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/jquery/3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.208925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/4.1.0-rc.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.208925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/full.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/modal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/partial.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templatetags/htmx_viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/viewsets.py
```

### Comparing `django-htmx-viewsets-0.0.5/LICENSE` & `django-htmx-viewsets-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/PKG-INFO` & `django-htmx-viewsets-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-viewsets
-Version: 0.0.5
+Version: 0.0.6
 Summary: Viewsets for Django using HTMX, Chartjs and DataTables
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -24,62 +24,73 @@
 Provides-Extra: test
 Provides-Extra: build
 License-File: LICENSE
 
 [![Django CI](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml)
 [![codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/main/graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-htmx-viewsets)
 [![Maintainability](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/maintainability)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/test_coverage)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/test_coverage)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
+
 django-htmx-viewsets
 ========================
 Viewsets for Django using HTMX and DataTables
 
+
 Built with
 ------------------------
 + [htmx](https://htmx.org/)
 + [chart.js](https://www.chartjs.org/)
 + [jQuery](https://jquery.com/)
 + [Bootstrap 5](https://getbootstrap.com/docs/5.0/getting-started/introduction/)
 + [Datatables](https://datatables.net/)
 + [Select2](https://select2.org/)
 + [Font Awesome](https://fontawesome.com/)
 
+
 Description
 ------------------------
 When working with Django REST framework you will stumble upon so called ViewSets.
 They allow you to combine a set of related Views without repeating.
 This aproach has no counterpart in Django itself.
 
 Therefore I created this package.
 
+
 Features
-========================
+------------------------
 + Create a viewset with one line
 + Dynamic loading of DetailView, UpdateView, CreateView and DeleteView
 + Urls are auto created
 + Queryset group by, filter and exclude by all possible date and time transform lookups
 + Auto create mixed chart with AJAX loading
 + Auto create table with AJAX loading
 + Customizable architecture[^1]
 
 [^1]: Things may change while in early state (<1.0.0)
 
 
+Screenshot
+------------------------
+![django-htmx-viewsets_screenshot1](https://raw.githubusercontent.com/snake-soft/django-htmx-viewsets/master/docs/screenshot1.png)
+
 Quick-Start
 ========================
 
 Installation
 ------------------------
+
 ```
 pip install django-htmx-viewset
 ```
 
 views.py
 ------------------------
+
 Create a ModelViewset by passing the model
 ```python
 MainViewSet = modelviewset_factory(model=Main)
 ```
 or a queryset
 ```python
 MainViewSet = modelviewset_factory(queryset=Main.objects.all())
@@ -92,29 +103,39 @@
 ```python
 app_name = 'test_db'
 urlpatterns = [
     path('main/', include(MainViewSet.urls)),
 ]
 ```
 
+
+Middleware
+------------------------
+
+```python
+MIDDLEWARE += ['django_htmx.middleware.HtmxMiddleware', "debug_toolbar.middleware.DebugToolbarMiddleware",]
+```
+
+
 Template
 ------------------------
 Project contains a full template.
 If you want to use your own template, you can overwrite the template (htmx_viewsets/full.html) or pass the full_template_name as kwarg to modelviewset_factory.
 The template should contain the following tags and blocks:
 
 ```html
 {% load htmx_viewsets %}
 <html>
   <head>
     {% htmx_viewsets_static_all %}
   </head>
   <body>
-    {% block main %}{% endblock main %}
-    {% htmx_viewsets_fixed_content %}
+    <div class="container">
+      {% block main %}{% endblock main %}
+      {% htmx_viewsets_fixed_content %}
+    </div>
   </body>
 </html>
 ```
 htmx_viewsets_static_all can be splitted by using htmx_viewsets_static_js and htmx_viewsets_static_css.
 
 htmx_viewsets_fixed_content can be splitted by using htmx_viewsets_modal and htmx_viewsets_messages.
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-htmx-viewsets Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: django-htmx-viewsets Version: 0.0.6 Summary:
 Viewsets for Django using HTMX, Chartjs and DataTables Author: Snake-Soft
 Author-email: info@snake-soft.com License: GPL3 Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Web Environment Classifier: Framework ::
 Django Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django
 :: 3.1 Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Unix Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -13,40 +13,46 @@
 Provides-Extra: build License-File: LICENSE [![Django CI](https://github.com/
 snake-soft/django-htmx-viewsets/actions/workflows/django.yml/badge.svg)](https:
 //github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml) [!
 [codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/main/
 graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-
 htmx-viewsets) [![Maintainability](https://api.codeclimate.com/v1/badges/
 bf8a8ff519a38147e922/maintainability)](https://codeclimate.com/github/snake-
-soft/django-htmx-viewsets/maintainability) [![License: GPL v3](https://
-img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
-3.0) django-htmx-viewsets ======================== Viewsets for Django using
-HTMX and DataTables Built with ------------------------ + [htmx](https://
-htmx.org/) + [chart.js](https://www.chartjs.org/) + [jQuery](https://
-jquery.com/) + [Bootstrap 5](https://getbootstrap.com/docs/5.0/getting-started/
-introduction/) + [Datatables](https://datatables.net/) + [Select2](https://
-select2.org/) + [Font Awesome](https://fontawesome.com/) Description ----------
--------------- When working with Django REST framework you will stumble upon so
-called ViewSets. They allow you to combine a set of related Views without
-repeating. This aproach has no counterpart in Django itself. Therefore I
-created this package. Features ======================== + Create a viewset with
-one line + Dynamic loading of DetailView, UpdateView, CreateView and DeleteView
-+ Urls are auto created + Queryset group by, filter and exclude by all possible
-date and time transform lookups + Auto create mixed chart with AJAX loading +
-Auto create table with AJAX loading + Customizable architecture[^1] [^1]:
-Things may change while in early state (<1.0.0) Quick-Start
-======================== Installation ------------------------ ``` pip install
-django-htmx-viewset ``` views.py ------------------------ Create a ModelViewset
-by passing the model ```python MainViewSet = modelviewset_factory(model=Main)
-``` or a queryset ```python MainViewSet = modelviewset_factory
-(queryset=Main.objects.all()) ``` urls.py ------------------------ ```python
-app_name = 'test_db' urlpatterns = [ path('main/', include(MainViewSet.urls)),
-] ``` Template ------------------------ Project contains a full template. If
-you want to use your own template, you can overwrite the template
-(htmx_viewsets/full.html) or pass the full_template_name as kwarg to
-modelviewset_factory. The template should contain the following tags and
-blocks: ```html {% load htmx_viewsets %}
+soft/django-htmx-viewsets/maintainability) [![Test Coverage](https://
+api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/test_coverage)](https://
+codeclimate.com/github/snake-soft/django-htmx-viewsets/test_coverage) [!
+[License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https:/
+/www.gnu.org/licenses/gpl-3.0) django-htmx-viewsets ========================
+Viewsets for Django using HTMX and DataTables Built with ----------------------
+-- + [htmx](https://htmx.org/) + [chart.js](https://www.chartjs.org/) +
+[jQuery](https://jquery.com/) + [Bootstrap 5](https://getbootstrap.com/docs/
+5.0/getting-started/introduction/) + [Datatables](https://datatables.net/) +
+[Select2](https://select2.org/) + [Font Awesome](https://fontawesome.com/
+) Description ------------------------ When working with Django REST framework
+you will stumble upon so called ViewSets. They allow you to combine a set of
+related Views without repeating. This aproach has no counterpart in Django
+itself. Therefore I created this package. Features ------------------------ +
+Create a viewset with one line + Dynamic loading of DetailView, UpdateView,
+CreateView and DeleteView + Urls are auto created + Queryset group by, filter
+and exclude by all possible date and time transform lookups + Auto create mixed
+chart with AJAX loading + Auto create table with AJAX loading + Customizable
+architecture[^1] [^1]: Things may change while in early state (<1.0.0)
+Screenshot ------------------------ ![django-htmx-viewsets_screenshot1](https:/
+/raw.githubusercontent.com/snake-soft/django-htmx-viewsets/master/docs/
+screenshot1.png) Quick-Start ======================== Installation ------------
+------------ ``` pip install django-htmx-viewset ``` views.py -----------------
+------- Create a ModelViewset by passing the model ```python MainViewSet =
+modelviewset_factory(model=Main) ``` or a queryset ```python MainViewSet =
+modelviewset_factory(queryset=Main.objects.all()) ``` urls.py -----------------
+------- ```python app_name = 'test_db' urlpatterns = [ path('main/', include
+(MainViewSet.urls)), ] ``` Middleware ------------------------ ```python
+MIDDLEWARE += ['django_htmx.middleware.HtmxMiddleware',
+"debug_toolbar.middleware.DebugToolbarMiddleware",] ``` Template --------------
+---------- Project contains a full template. If you want to use your own
+template, you can overwrite the template (htmx_viewsets/full.html) or pass the
+full_template_name as kwarg to modelviewset_factory. The template should
+contain the following tags and blocks: ```html {% load htmx_viewsets %}
 {% htmx_viewsets_static_all %}
 {% block main %}{% endblock main %} {% htmx_viewsets_fixed_content %}
 ``` htmx_viewsets_static_all can be splitted by using htmx_viewsets_static_js
 and htmx_viewsets_static_css. htmx_viewsets_fixed_content can be splitted by
 using htmx_viewsets_modal and htmx_viewsets_messages.
```

### Comparing `django-htmx-viewsets-0.0.5/README.md` & `django-htmx-viewsets-0.0.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,69 @@
 [![Django CI](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml)
 [![codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/main/graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-htmx-viewsets)
 [![Maintainability](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/maintainability)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/test_coverage)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/test_coverage)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
+
 django-htmx-viewsets
 ========================
 Viewsets for Django using HTMX and DataTables
 
+
 Built with
 ------------------------
 + [htmx](https://htmx.org/)
 + [chart.js](https://www.chartjs.org/)
 + [jQuery](https://jquery.com/)
 + [Bootstrap 5](https://getbootstrap.com/docs/5.0/getting-started/introduction/)
 + [Datatables](https://datatables.net/)
 + [Select2](https://select2.org/)
 + [Font Awesome](https://fontawesome.com/)
 
+
 Description
 ------------------------
 When working with Django REST framework you will stumble upon so called ViewSets.
 They allow you to combine a set of related Views without repeating.
 This aproach has no counterpart in Django itself.
 
 Therefore I created this package.
 
+
 Features
-========================
+------------------------
 + Create a viewset with one line
 + Dynamic loading of DetailView, UpdateView, CreateView and DeleteView
 + Urls are auto created
 + Queryset group by, filter and exclude by all possible date and time transform lookups
 + Auto create mixed chart with AJAX loading
 + Auto create table with AJAX loading
 + Customizable architecture[^1]
 
 [^1]: Things may change while in early state (<1.0.0)
 
 
+Screenshot
+------------------------
+![django-htmx-viewsets_screenshot1](https://raw.githubusercontent.com/snake-soft/django-htmx-viewsets/master/docs/screenshot1.png)
+
 Quick-Start
 ========================
 
 Installation
 ------------------------
+
 ```
 pip install django-htmx-viewset
 ```
 
 views.py
 ------------------------
+
 Create a ModelViewset by passing the model
 ```python
 MainViewSet = modelviewset_factory(model=Main)
 ```
 or a queryset
 ```python
 MainViewSet = modelviewset_factory(queryset=Main.objects.all())
@@ -65,29 +76,39 @@
 ```python
 app_name = 'test_db'
 urlpatterns = [
     path('main/', include(MainViewSet.urls)),
 ]
 ```
 
+
+Middleware
+------------------------
+
+```python
+MIDDLEWARE += ['django_htmx.middleware.HtmxMiddleware', "debug_toolbar.middleware.DebugToolbarMiddleware",]
+```
+
+
 Template
 ------------------------
 Project contains a full template.
 If you want to use your own template, you can overwrite the template (htmx_viewsets/full.html) or pass the full_template_name as kwarg to modelviewset_factory.
 The template should contain the following tags and blocks:
 
 ```html
 {% load htmx_viewsets %}
 <html>
   <head>
     {% htmx_viewsets_static_all %}
   </head>
   <body>
-    {% block main %}{% endblock main %}
-    {% htmx_viewsets_fixed_content %}
+    <div class="container">
+      {% block main %}{% endblock main %}
+      {% htmx_viewsets_fixed_content %}
+    </div>
   </body>
 </html>
 ```
 htmx_viewsets_static_all can be splitted by using htmx_viewsets_static_js and htmx_viewsets_static_css.
 
 htmx_viewsets_fixed_content can be splitted by using htmx_viewsets_modal and htmx_viewsets_messages.
-
```

#### html2text {}

```diff
@@ -1,39 +1,45 @@
 [![Django CI](https://github.com/snake-soft/django-htmx-viewsets/actions/
 workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-htmx-
 viewsets/actions/workflows/django.yml) [![codecov](https://codecov.io/gh/snake-
 soft/django-htmx-viewsets/branch/main/graph/badge.svg?token=Tyfji4Pe6Q)](https:
 //codecov.io/gh/snake-soft/django-htmx-viewsets) [![Maintainability](https://
 api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/maintainability)](https://
-codeclimate.com/github/snake-soft/django-htmx-viewsets/maintainability) [!
-[License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https:/
-/www.gnu.org/licenses/gpl-3.0) django-htmx-viewsets ========================
-Viewsets for Django using HTMX and DataTables Built with ----------------------
--- + [htmx](https://htmx.org/) + [chart.js](https://www.chartjs.org/) +
-[jQuery](https://jquery.com/) + [Bootstrap 5](https://getbootstrap.com/docs/
-5.0/getting-started/introduction/) + [Datatables](https://datatables.net/) +
-[Select2](https://select2.org/) + [Font Awesome](https://fontawesome.com/
-) Description ------------------------ When working with Django REST framework
-you will stumble upon so called ViewSets. They allow you to combine a set of
-related Views without repeating. This aproach has no counterpart in Django
-itself. Therefore I created this package. Features ======================== +
-Create a viewset with one line + Dynamic loading of DetailView, UpdateView,
-CreateView and DeleteView + Urls are auto created + Queryset group by, filter
-and exclude by all possible date and time transform lookups + Auto create mixed
-chart with AJAX loading + Auto create table with AJAX loading + Customizable
-architecture[^1] [^1]: Things may change while in early state (<1.0.0) Quick-
-Start ======================== Installation ------------------------ ``` pip
-install django-htmx-viewset ``` views.py ------------------------ Create a
-ModelViewset by passing the model ```python MainViewSet = modelviewset_factory
-(model=Main) ``` or a queryset ```python MainViewSet = modelviewset_factory
-(queryset=Main.objects.all()) ``` urls.py ------------------------ ```python
-app_name = 'test_db' urlpatterns = [ path('main/', include(MainViewSet.urls)),
-] ``` Template ------------------------ Project contains a full template. If
-you want to use your own template, you can overwrite the template
-(htmx_viewsets/full.html) or pass the full_template_name as kwarg to
-modelviewset_factory. The template should contain the following tags and
-blocks: ```html {% load htmx_viewsets %}
+codeclimate.com/github/snake-soft/django-htmx-viewsets/maintainability) [![Test
+Coverage](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/
+test_coverage)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/
+test_coverage) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-
+blue.svg)](https://www.gnu.org/licenses/gpl-3.0) django-htmx-viewsets
+======================== Viewsets for Django using HTMX and DataTables Built
+with ------------------------ + [htmx](https://htmx.org/) + [chart.js](https://
+www.chartjs.org/) + [jQuery](https://jquery.com/) + [Bootstrap 5](https://
+getbootstrap.com/docs/5.0/getting-started/introduction/) + [Datatables](https:/
+/datatables.net/) + [Select2](https://select2.org/) + [Font Awesome](https://
+fontawesome.com/) Description ------------------------ When working with Django
+REST framework you will stumble upon so called ViewSets. They allow you to
+combine a set of related Views without repeating. This aproach has no
+counterpart in Django itself. Therefore I created this package. Features ------
+------------------ + Create a viewset with one line + Dynamic loading of
+DetailView, UpdateView, CreateView and DeleteView + Urls are auto created +
+Queryset group by, filter and exclude by all possible date and time transform
+lookups + Auto create mixed chart with AJAX loading + Auto create table with
+AJAX loading + Customizable architecture[^1] [^1]: Things may change while in
+early state (<1.0.0) Screenshot ------------------------ ![django-htmx-
+viewsets_screenshot1](https://raw.githubusercontent.com/snake-soft/django-htmx-
+viewsets/master/docs/screenshot1.png) Quick-Start ========================
+Installation ------------------------ ``` pip install django-htmx-viewset ```
+views.py ------------------------ Create a ModelViewset by passing the model
+```python MainViewSet = modelviewset_factory(model=Main) ``` or a queryset
+```python MainViewSet = modelviewset_factory(queryset=Main.objects.all()) ```
+urls.py ------------------------ ```python app_name = 'test_db' urlpatterns =
+[ path('main/', include(MainViewSet.urls)), ] ``` Middleware ------------------
+------ ```python MIDDLEWARE += ['django_htmx.middleware.HtmxMiddleware',
+"debug_toolbar.middleware.DebugToolbarMiddleware",] ``` Template --------------
+---------- Project contains a full template. If you want to use your own
+template, you can overwrite the template (htmx_viewsets/full.html) or pass the
+full_template_name as kwarg to modelviewset_factory. The template should
+contain the following tags and blocks: ```html {% load htmx_viewsets %}
 {% htmx_viewsets_static_all %}
 {% block main %}{% endblock main %} {% htmx_viewsets_fixed_content %}
 ``` htmx_viewsets_static_all can be splitted by using htmx_viewsets_static_js
 and htmx_viewsets_static_css. htmx_viewsets_fixed_content can be splitted by
 using htmx_viewsets_modal and htmx_viewsets_messages.
```

### Comparing `django-htmx-viewsets-0.0.5/setup.py` & `django-htmx-viewsets-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/PKG-INFO` & `django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-viewsets
-Version: 0.0.5
+Version: 0.0.6
 Summary: Viewsets for Django using HTMX, Chartjs and DataTables
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -24,62 +24,73 @@
 Provides-Extra: test
 Provides-Extra: build
 License-File: LICENSE
 
 [![Django CI](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml)
 [![codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/main/graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-htmx-viewsets)
 [![Maintainability](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/maintainability)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/test_coverage)](https://codeclimate.com/github/snake-soft/django-htmx-viewsets/test_coverage)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
+
 django-htmx-viewsets
 ========================
 Viewsets for Django using HTMX and DataTables
 
+
 Built with
 ------------------------
 + [htmx](https://htmx.org/)
 + [chart.js](https://www.chartjs.org/)
 + [jQuery](https://jquery.com/)
 + [Bootstrap 5](https://getbootstrap.com/docs/5.0/getting-started/introduction/)
 + [Datatables](https://datatables.net/)
 + [Select2](https://select2.org/)
 + [Font Awesome](https://fontawesome.com/)
 
+
 Description
 ------------------------
 When working with Django REST framework you will stumble upon so called ViewSets.
 They allow you to combine a set of related Views without repeating.
 This aproach has no counterpart in Django itself.
 
 Therefore I created this package.
 
+
 Features
-========================
+------------------------
 + Create a viewset with one line
 + Dynamic loading of DetailView, UpdateView, CreateView and DeleteView
 + Urls are auto created
 + Queryset group by, filter and exclude by all possible date and time transform lookups
 + Auto create mixed chart with AJAX loading
 + Auto create table with AJAX loading
 + Customizable architecture[^1]
 
 [^1]: Things may change while in early state (<1.0.0)
 
 
+Screenshot
+------------------------
+![django-htmx-viewsets_screenshot1](https://raw.githubusercontent.com/snake-soft/django-htmx-viewsets/master/docs/screenshot1.png)
+
 Quick-Start
 ========================
 
 Installation
 ------------------------
+
 ```
 pip install django-htmx-viewset
 ```
 
 views.py
 ------------------------
+
 Create a ModelViewset by passing the model
 ```python
 MainViewSet = modelviewset_factory(model=Main)
 ```
 or a queryset
 ```python
 MainViewSet = modelviewset_factory(queryset=Main.objects.all())
@@ -92,29 +103,39 @@
 ```python
 app_name = 'test_db'
 urlpatterns = [
     path('main/', include(MainViewSet.urls)),
 ]
 ```
 
+
+Middleware
+------------------------
+
+```python
+MIDDLEWARE += ['django_htmx.middleware.HtmxMiddleware', "debug_toolbar.middleware.DebugToolbarMiddleware",]
+```
+
+
 Template
 ------------------------
 Project contains a full template.
 If you want to use your own template, you can overwrite the template (htmx_viewsets/full.html) or pass the full_template_name as kwarg to modelviewset_factory.
 The template should contain the following tags and blocks:
 
 ```html
 {% load htmx_viewsets %}
 <html>
   <head>
     {% htmx_viewsets_static_all %}
   </head>
   <body>
-    {% block main %}{% endblock main %}
-    {% htmx_viewsets_fixed_content %}
+    <div class="container">
+      {% block main %}{% endblock main %}
+      {% htmx_viewsets_fixed_content %}
+    </div>
   </body>
 </html>
 ```
 htmx_viewsets_static_all can be splitted by using htmx_viewsets_static_js and htmx_viewsets_static_css.
 
 htmx_viewsets_fixed_content can be splitted by using htmx_viewsets_modal and htmx_viewsets_messages.
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-htmx-viewsets Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: django-htmx-viewsets Version: 0.0.6 Summary:
 Viewsets for Django using HTMX, Chartjs and DataTables Author: Snake-Soft
 Author-email: info@snake-soft.com License: GPL3 Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Web Environment Classifier: Framework ::
 Django Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django
 :: 3.1 Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Unix Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -13,40 +13,46 @@
 Provides-Extra: build License-File: LICENSE [![Django CI](https://github.com/
 snake-soft/django-htmx-viewsets/actions/workflows/django.yml/badge.svg)](https:
 //github.com/snake-soft/django-htmx-viewsets/actions/workflows/django.yml) [!
 [codecov](https://codecov.io/gh/snake-soft/django-htmx-viewsets/branch/main/
 graph/badge.svg?token=Tyfji4Pe6Q)](https://codecov.io/gh/snake-soft/django-
 htmx-viewsets) [![Maintainability](https://api.codeclimate.com/v1/badges/
 bf8a8ff519a38147e922/maintainability)](https://codeclimate.com/github/snake-
-soft/django-htmx-viewsets/maintainability) [![License: GPL v3](https://
-img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
-3.0) django-htmx-viewsets ======================== Viewsets for Django using
-HTMX and DataTables Built with ------------------------ + [htmx](https://
-htmx.org/) + [chart.js](https://www.chartjs.org/) + [jQuery](https://
-jquery.com/) + [Bootstrap 5](https://getbootstrap.com/docs/5.0/getting-started/
-introduction/) + [Datatables](https://datatables.net/) + [Select2](https://
-select2.org/) + [Font Awesome](https://fontawesome.com/) Description ----------
--------------- When working with Django REST framework you will stumble upon so
-called ViewSets. They allow you to combine a set of related Views without
-repeating. This aproach has no counterpart in Django itself. Therefore I
-created this package. Features ======================== + Create a viewset with
-one line + Dynamic loading of DetailView, UpdateView, CreateView and DeleteView
-+ Urls are auto created + Queryset group by, filter and exclude by all possible
-date and time transform lookups + Auto create mixed chart with AJAX loading +
-Auto create table with AJAX loading + Customizable architecture[^1] [^1]:
-Things may change while in early state (<1.0.0) Quick-Start
-======================== Installation ------------------------ ``` pip install
-django-htmx-viewset ``` views.py ------------------------ Create a ModelViewset
-by passing the model ```python MainViewSet = modelviewset_factory(model=Main)
-``` or a queryset ```python MainViewSet = modelviewset_factory
-(queryset=Main.objects.all()) ``` urls.py ------------------------ ```python
-app_name = 'test_db' urlpatterns = [ path('main/', include(MainViewSet.urls)),
-] ``` Template ------------------------ Project contains a full template. If
-you want to use your own template, you can overwrite the template
-(htmx_viewsets/full.html) or pass the full_template_name as kwarg to
-modelviewset_factory. The template should contain the following tags and
-blocks: ```html {% load htmx_viewsets %}
+soft/django-htmx-viewsets/maintainability) [![Test Coverage](https://
+api.codeclimate.com/v1/badges/bf8a8ff519a38147e922/test_coverage)](https://
+codeclimate.com/github/snake-soft/django-htmx-viewsets/test_coverage) [!
+[License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https:/
+/www.gnu.org/licenses/gpl-3.0) django-htmx-viewsets ========================
+Viewsets for Django using HTMX and DataTables Built with ----------------------
+-- + [htmx](https://htmx.org/) + [chart.js](https://www.chartjs.org/) +
+[jQuery](https://jquery.com/) + [Bootstrap 5](https://getbootstrap.com/docs/
+5.0/getting-started/introduction/) + [Datatables](https://datatables.net/) +
+[Select2](https://select2.org/) + [Font Awesome](https://fontawesome.com/
+) Description ------------------------ When working with Django REST framework
+you will stumble upon so called ViewSets. They allow you to combine a set of
+related Views without repeating. This aproach has no counterpart in Django
+itself. Therefore I created this package. Features ------------------------ +
+Create a viewset with one line + Dynamic loading of DetailView, UpdateView,
+CreateView and DeleteView + Urls are auto created + Queryset group by, filter
+and exclude by all possible date and time transform lookups + Auto create mixed
+chart with AJAX loading + Auto create table with AJAX loading + Customizable
+architecture[^1] [^1]: Things may change while in early state (<1.0.0)
+Screenshot ------------------------ ![django-htmx-viewsets_screenshot1](https:/
+/raw.githubusercontent.com/snake-soft/django-htmx-viewsets/master/docs/
+screenshot1.png) Quick-Start ======================== Installation ------------
+------------ ``` pip install django-htmx-viewset ``` views.py -----------------
+------- Create a ModelViewset by passing the model ```python MainViewSet =
+modelviewset_factory(model=Main) ``` or a queryset ```python MainViewSet =
+modelviewset_factory(queryset=Main.objects.all()) ``` urls.py -----------------
+------- ```python app_name = 'test_db' urlpatterns = [ path('main/', include
+(MainViewSet.urls)), ] ``` Middleware ------------------------ ```python
+MIDDLEWARE += ['django_htmx.middleware.HtmxMiddleware',
+"debug_toolbar.middleware.DebugToolbarMiddleware",] ``` Template --------------
+---------- Project contains a full template. If you want to use your own
+template, you can overwrite the template (htmx_viewsets/full.html) or pass the
+full_template_name as kwarg to modelviewset_factory. The template should
+contain the following tags and blocks: ```html {% load htmx_viewsets %}
 {% htmx_viewsets_static_all %}
 {% block main %}{% endblock main %} {% htmx_viewsets_fixed_content %}
 ``` htmx_viewsets_static_all can be splitted by using htmx_viewsets_static_js
 and htmx_viewsets_static_css. htmx_viewsets_fixed_content can be splitted by
 using htmx_viewsets_modal and htmx_viewsets_messages.
```

### Comparing `django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/SOURCES.txt` & `django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/chart.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/chart.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/color.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/color.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/fields.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/fields.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/forms.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/forms.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/action.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/action.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/cell.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/cell.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/column.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/column.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/row.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/row.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/table.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/table.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/delete.html` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/delete.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/form.html` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/form.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/list.html` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/list.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 {% extends './dispatch.html' %}
 
 {% block htmx_main %}
-<div class="container-fluid">
-  <div class="row mt-3">
-    <div class="col-12">
-      <h2>{{ verbose_name_plural }}</h2>
-    </div>
-    <form method="POST" action="{{ request.path }}?{{ request.GET.urlencode }}">{% csrf_token %}
-      {% if enabled_filter_form.enabled_lookups %}
-        <div class="row mt-3">
+<div class="row mt-3">
+  <div class="col-12">
+    <h2>{{ verbose_name_plural }}</h2>
+  </div>
+  <form method="POST" action="{{ request.path }}?{{ request.GET.urlencode }}">{% csrf_token %}
+    {% if enabled_filter_form.enabled_lookups %}
+      <div class="row mt-3">
+        <div class="col-auto">
+          <span class="badge badge-light text-bg-light">
+            Filter entfernen:
+          </span>
+        </div>
+        {% for lookup in enabled_filter_form.enabled_lookups %}
           <div class="col-auto">
-            <span class="badge badge-light text-bg-light">
-              Filter entfernen:
-            </span>
+            <button type="submit" class="btn btn-{{ lookup.bg_class }} btn-sm p-0" name="delete_method_lookup" value="{{ lookup.key }}={{ lookup.value }}">
+              <span class="badge">
+                {{ lookup.name }}={{ lookup.value }}
+              </span>
+            </button>
           </div>
-          {% for lookup in enabled_filter_form.enabled_lookups %}
-            <div class="col-auto">
-              <button type="submit" class="btn btn-{{ lookup.bg_class }} btn-sm p-0" name="delete_method_lookup" value="{{ lookup.key }}={{ lookup.value }}">
-                <span class="badge">
-                  {{ lookup.name }}={{ lookup.value }}
-                </span>
-              </button>
-            </div>
-          {% endfor %}
-          <div class="row">
-            <div class="col-12">
-              <hr>
-            </div>
+        {% endfor %}
+        <div class="row">
+          <div class="col-12">
+            <hr>
           </div>
         </div>
-      {% endif %}
-    </form>
-    <div class="row">
-      <div class="col-12">
-        <button class="btn btn-link text-decoration-none" type="button" data-bs-toggle="collapse" data-bs-target="#add-filter-form" aria-expanded="false" aria-controls="add-filter-form">
-          &#43; Filter hinzufügen
-        </button>
-        <div>
-          <div class="collapse" id="add-filter-form">
-            <div class="card card-body w-100">
-              <form id="add-filter-argument-form" method="POST" action="{{ request.path }}?{{ request.GET.urlencode }}">{% csrf_token %}
-                <table>
-                  {{ add_filter_form.as_table }}
-                  <tr>
-                    <td>
-                    </td>
-                    <td>
-                      <button class="btn btn-primary" type="submit">Filter hinzufügen</button>
-                      <button class="btn btn-secondary" type="reset">Zurücksetzen</button>
-                    </td>
-                  </tr>
-                </table>
-              </form>
-            </div>
+      </div>
+    {% endif %}
+  </form>
+  <div class="row">
+    <div class="col-12">
+      <button class="btn btn-link text-decoration-none" type="button" data-bs-toggle="collapse" data-bs-target="#add-filter-form" aria-expanded="false" aria-controls="add-filter-form">
+        &#43; Filter hinzufügen
+      </button>
+      <div>
+        <div class="collapse" id="add-filter-form">
+          <div class="card card-body w-100">
+            <form id="add-filter-argument-form" method="POST" action="{{ request.path }}?{{ request.GET.urlencode }}">{% csrf_token %}
+              <table>
+                {{ add_filter_form.as_table }}
+                <tr>
+                  <td>
+                  </td>
+                  <td>
+                    <button class="btn btn-primary" type="submit">Filter hinzufügen</button>
+                    <button class="btn btn-secondary" type="reset">Zurücksetzen</button>
+                  </td>
+                </tr>
+              </table>
+            </form>
           </div>
         </div>
       </div>
     </div>
   </div>
-  {% if chart %}
-  <div class="row">
-    <div class="col-12">
-      <hr>
-    </div>
-    <form id="group-by-form" method=GET action="{{ request.path }}?{{ request.GET.urlencode }}">
-      <div class="col-12">
-        <table>
-          {{ group_by_form.as_table }}
-        </table>
-      </div>
-    </form>
+</div>
+{% if chart %}
+<div class="row">
+  <div class="col-12">
+    <hr>
   </div>
-    <div class="row">
-      <div class="col-12">
-        {% include './chart.html' %}
-      </div>
+  <form id="group-by-form" method=GET action="{{ request.path }}?{{ request.GET.urlencode }}">
+    <div class="col-12">
+      <table>
+        {{ group_by_form.as_table }}
+      </table>
     </div>
+  </form>
+</div>
+  <div class="row">
     <div class="col-12">
-      <hr>
+      {% include './chart.html' %}
     </div>
-  {% endif %}
-  <div class="row mt-3">
-    <div class="col-12 table-responsive">
+  </div>
+  <div class="col-12">
+    <hr>
+  </div>
+{% endif %}
+<div class="row mt-3">
+  <div class="col-12">
+    <div class="table-responsive">
       {% include table %}{{ table_id }}
     </div>
   </div>
 </div>
 <script>
     htmx.onLoad(function() {
       $('.modal-close-button').on('click', function () {
```

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/modal.html` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/modal.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/partial.html` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/partial.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/table.html` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/table.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templatetags/htmx_viewsets.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templatetags/htmx_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/views.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/views.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.5/src/htmx_viewsets/viewsets.py` & `django-htmx-viewsets-0.0.6/src/htmx_viewsets/viewsets.py`

 * *Files identical despite different names*

