# Comparing `tmp/django-mp-tags-0.2.tar.gz` & `tmp/django-mp-tags-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-mp-tags-0.2.tar", last modified: Fri Dec 11 17:38:58 2020, max compression
+gzip compressed data, was "django-mp-tags-1.0.0.tar", last modified: Sun Apr  9 17:54:26 2023, max compression
```

## Comparing `django-mp-tags-0.2.tar` & `django-mp-tags-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/
--rw-r--r--   0 dev       (1000) dev       (1000)      101 2020-03-14 11:05:31.000000 django-mp-tags-0.2/README.md
--rw-r--r--   0 dev       (1000) dev       (1000)      746 2019-06-06 08:10:41.000000 django-mp-tags-0.2/LICENSE
--rw-r--r--   0 dev       (1000) dev       (1000)      137 2020-03-14 11:05:31.000000 django-mp-tags-0.2/MANIFEST.in
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/django_mp_tags.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2020-12-11 17:38:58.000000 django-mp-tags-0.2/django_mp_tags.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)      628 2020-12-11 17:38:58.000000 django-mp-tags-0.2/django_mp_tags.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        5 2020-12-11 17:38:58.000000 django-mp-tags-0.2/django_mp_tags.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)      312 2020-12-11 17:38:58.000000 django-mp-tags-0.2/django_mp_tags.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)      530 2020-12-11 17:33:44.000000 django-mp-tags-0.2/setup.py
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2020-12-11 17:36:33.000000 django-mp-tags-0.2/requirements.txt
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/tags/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/tags/templates/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/tags/templates/tags/
--rw-rw-r--   0 dev       (1000) dev       (1000)      648 2020-06-18 20:24:01.000000 django-mp-tags-0.2/tags/templates/tags/add_tag_groups_action.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      627 2020-12-11 17:01:36.000000 django-mp-tags-0.2/tags/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      217 2020-12-11 17:23:27.000000 django-mp-tags-0.2/tags/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2431 2020-12-11 17:14:51.000000 django-mp-tags-0.2/tags/models.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      953 2020-06-18 20:24:01.000000 django-mp-tags-0.2/tags/actions.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      125 2020-06-18 20:24:01.000000 django-mp-tags-0.2/tags/translation.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/tags/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/tags/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/tags/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1420 2020-06-18 20:24:01.000000 django-mp-tags-0.2/tags/locale/uk/LC_MESSAGES/django.po
--rw-rw-r--   0 dev       (1000) dev       (1000)      944 2020-06-18 20:24:01.000000 django-mp-tags-0.2/tags/locale/uk/LC_MESSAGES/django.mo
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/tags/locale/ru/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/tags/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1495 2020-06-18 20:24:01.000000 django-mp-tags-0.2/tags/locale/ru/LC_MESSAGES/django.po
--rw-rw-r--   0 dev       (1000) dev       (1000)     1016 2020-06-18 20:24:01.000000 django-mp-tags-0.2/tags/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)      573 2020-06-18 20:24:01.000000 django-mp-tags-0.2/tags/forms.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2020-12-11 17:38:58.000000 django-mp-tags-0.2/tags/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1555 2020-06-18 20:24:01.000000 django-mp-tags-0.2/tags/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      811 2020-12-11 17:36:33.000000 django-mp-tags-0.2/tags/migrations/0002_translation_fields.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2020-06-18 20:24:01.000000 django-mp-tags-0.2/tags/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      170 2020-12-11 17:19:38.000000 django-mp-tags-0.2/tags/settings.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      312 2020-12-11 17:38:58.000000 django-mp-tags-0.2/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)       79 2020-12-11 17:38:58.000000 django-mp-tags-0.2/setup.cfg
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      746 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)      137 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      299 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      101 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/django_mp_tags.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      299 2023-04-09 17:54:26.000000 django-mp-tags-1.0.0/django_mp_tags.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      611 2023-04-09 17:54:26.000000 django-mp-tags-1.0.0/django_mp_tags.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-04-09 17:54:26.000000 django-mp-tags-1.0.0/django_mp_tags.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        5 2023-04-09 17:54:26.000000 django-mp-tags-1.0.0/django_mp_tags.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-04-09 17:54:26.807988 django-mp-tags-1.0.0/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      427 2023-04-09 17:54:00.000000 django-mp-tags-1.0.0/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/tags/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      216 2023-04-09 17:51:55.000000 django-mp-tags-1.0.0/tags/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      952 2023-04-09 17:51:55.000000 django-mp-tags-1.0.0/tags/actions.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      626 2023-04-09 17:51:55.000000 django-mp-tags-1.0.0/tags/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      572 2023-04-09 17:51:55.000000 django-mp-tags-1.0.0/tags/forms.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/tags/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/tags/locale/ru/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/tags/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1016 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/tags/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1495 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/tags/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/tags/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/tags/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      944 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/tags/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1420 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/tags/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/tags/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1555 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/tags/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      811 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/tags/migrations/0002_translation_fields.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/tags/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2430 2023-04-09 17:51:55.000000 django-mp-tags-1.0.0/tags/models.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      170 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/tags/settings.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/tags/templates/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-09 17:54:26.803988 django-mp-tags-1.0.0/tags/templates/tags/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      648 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/tags/templates/tags/add_tag_groups_action.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      125 2023-04-09 17:51:27.000000 django-mp-tags-1.0.0/tags/translation.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-mp-tags-0.2/LICENSE` & `django-mp-tags-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mp-tags-0.2/django_mp_tags.egg-info/SOURCES.txt` & `django-mp-tags-1.0.0/django_mp_tags.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-requirements.txt
 setup.cfg
 setup.py
 django_mp_tags.egg-info/PKG-INFO
 django_mp_tags.egg-info/SOURCES.txt
 django_mp_tags.egg-info/dependency_links.txt
 django_mp_tags.egg-info/top_level.txt
 tags/__init__.py
```

### Comparing `django-mp-tags-0.2/tags/templates/tags/add_tag_groups_action.html` & `django-mp-tags-1.0.0/tags/templates/tags/add_tag_groups_action.html`

 * *Files identical despite different names*

### Comparing `django-mp-tags-0.2/tags/admin.py` & `django-mp-tags-1.0.0/tags/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from django.contrib import admin
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from tags.models import TagGroup, Tag
 from tags.forms import TagInline
 
 
 @admin.register(Tag)
 class TagAdmin(admin.ModelAdmin):
```

### Comparing `django-mp-tags-0.2/tags/models.py` & `django-mp-tags-1.0.0/tags/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from modeltranslation.utils import get_translation_fields
 
 from model_search import model_search
 
 
 class TagManager(models.Manager):
```

### Comparing `django-mp-tags-0.2/tags/actions.py` & `django-mp-tags-1.0.0/tags/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from django.contrib import admin
 from django.shortcuts import render, redirect
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from tags.forms import AddTagGroupsForm
 
 
 def add_tag_groups(modeladmin, request, queryset):
 
     data = request.POST
```

### Comparing `django-mp-tags-0.2/tags/locale/uk/LC_MESSAGES/django.po` & `django-mp-tags-1.0.0/tags/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-tags-0.2/tags/locale/uk/LC_MESSAGES/django.mo` & `django-mp-tags-1.0.0/tags/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-tags-0.2/tags/locale/ru/LC_MESSAGES/django.po` & `django-mp-tags-1.0.0/tags/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-tags-0.2/tags/locale/ru/LC_MESSAGES/django.mo` & `django-mp-tags-1.0.0/tags/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-tags-0.2/tags/forms.py` & `django-mp-tags-1.0.0/tags/forms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from django import forms
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.contrib.admin.widgets import FilteredSelectMultiple
 
 from modeltranslation.admin import TranslationStackedInline
 
 from tags.models import Tag, TagGroup
```

### Comparing `django-mp-tags-0.2/tags/migrations/0001_initial.py` & `django-mp-tags-1.0.0/tags/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mp-tags-0.2/tags/migrations/0002_translation_fields.py` & `django-mp-tags-1.0.0/tags/migrations/0002_translation_fields.py`

 * *Files identical despite different names*

