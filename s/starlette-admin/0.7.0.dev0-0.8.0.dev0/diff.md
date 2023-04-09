# Comparing `tmp/starlette_admin-0.7.0.dev0.tar.gz` & `tmp/starlette_admin-0.8.0.dev0.tar.gz`

## Comparing `starlette_admin-0.7.0.dev0.tar` & `starlette_admin-0.8.0.dev0.tar`

### file list

```diff
@@ -1,120 +1,122 @@
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/__init__.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/_types.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/actions.py
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/auth.py
--rw-r--r--   0        0        0    21930 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/base.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/exceptions.py
--rw-r--r--   0        0        0    40036 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/fields.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/helpers.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/i18n.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/py.typed
--rw-r--r--   0        0        0    25018 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/mongoengine/__init__.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/mongoengine/admin.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/mongoengine/exceptions.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/mongoengine/fields.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/mongoengine/helpers.py
--rw-r--r--   0        0        0     9798 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/mongoengine/view.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/odmantic/__init__.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/odmantic/admin.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/odmantic/exceptions.py
--rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/odmantic/helpers.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/odmantic/middleware.py
--rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/odmantic/view.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/__init__.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/admin.py
--rw-r--r--   0        0        0     9336 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/converters.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/exceptions.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/fields.py
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/helpers.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/middleware.py
--rw-r--r--   0        0        0    16081 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/view.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqlmodel/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqlmodel/admin.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqlmodel/view.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/css/dt.checkboxes.css
--rw-r--r--   0        0        0    38335 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/css/dt.min.css
--rw-r--r--   0        0        0    16167 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/css/flatpickr.min.css
--rw-r--r--   0        0        0   100783 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/css/fontawesome.min.css
--rw-r--r--   0        0        0    35418 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/css/jsoneditor.min.css
--rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/css/select2.min.css
--rw-r--r--   0        0        0   498576 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/css/tabler.min.css
--rw-r--r--   0        0        0    31482 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/css/img/jsoneditor-icons.svg
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/i18n/dt/README.md
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/i18n/dt/en.json
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/i18n/dt/fr.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/i18n/flatpickr/fr.js
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/i18n/momentjs/fr.js
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/displays.js
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/form.js
--rw-r--r--   0        0        0    16174 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/list.js
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/render.js
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/utils.js
--rw-r--r--   0        0        0    13295 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/dt.checkboxes.js
--rw-r--r--   0        0        0   354520 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/dt.min.js
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/dt.searchHighlight.js
--rw-r--r--   0        0        0    50680 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/flatpickr.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/jquery.min.js
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/js.cookie.min.js
--rw-r--r--   0        0        0   890454 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/jsoneditor.min.js
--rw-r--r--   0        0        0    59517 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/moment.min.js
--rw-r--r--   0        0        0   970347 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/pdfmake.min.js
--rw-r--r--   0        0        0    73164 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/select2.min.js
--rw-r--r--   0        0        0   146912 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/tabler.min.js
--rw-r--r--   0        0        0   870285 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/vfs_fonts.js
--rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/base.html
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/create.html
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/detail.html
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/edit.html
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/error.html
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/index.html
--rw-r--r--   0        0        0    14329 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/layout.html
--rw-r--r--   0        0        0     9127 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/list.html
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/login.html
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/_empty.html
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/_null.html
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/boolean.html
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/collection.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/email.html
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/file.html
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/image.html
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/json.html
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/list.html
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/relation.html
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/text.html
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/tinymce.html
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/url.html
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/_delete.html
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/_error.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/_label.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/boolean.html
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/collection.html
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/enum.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/file.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/image.html
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/input.html
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/json.html
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/list.html
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/relation.html
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/tags.html
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/textarea.html
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/macros/views.html
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/modals/actions.html
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/modals/delete.html
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/modals/error.html
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/templates/modals/loading.html
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.mo
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.po
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.mo
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/utils/__init__.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/utils/countries.py
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/starlette_admin/utils/timezones.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/LICENSE
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/README.md
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 starlette_admin-0.7.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/__init__.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/_types.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/actions.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/auth.py
+-rw-r--r--   0        0        0    21467 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/base.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/exceptions.py
+-rw-r--r--   0        0        0    40038 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/fields.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/helpers.py
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/i18n.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/py.typed
+-rw-r--r--   0        0        0    27613 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/mongoengine/__init__.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/mongoengine/admin.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/mongoengine/exceptions.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/mongoengine/fields.py
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/mongoengine/helpers.py
+-rw-r--r--   0        0        0     9780 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/mongoengine/view.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/odmantic/__init__.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/odmantic/admin.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/odmantic/exceptions.py
+-rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/odmantic/helpers.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/odmantic/middleware.py
+-rw-r--r--   0        0        0    10604 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/odmantic/view.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/__init__.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/admin.py
+-rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/converters.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/exceptions.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/fields.py
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/helpers.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/middleware.py
+-rw-r--r--   0        0        0    16081 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/ext/__init__.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/ext/pydantic.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqlmodel/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqlmodel/admin.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqlmodel/view.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/css/dt.checkboxes.css
+-rw-r--r--   0        0        0    38335 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/css/dt.min.css
+-rw-r--r--   0        0        0    16167 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/css/flatpickr.min.css
+-rw-r--r--   0        0        0   100783 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/css/fontawesome.min.css
+-rw-r--r--   0        0        0    35418 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/css/jsoneditor.min.css
+-rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/css/select2.min.css
+-rw-r--r--   0        0        0   498576 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/css/tabler.min.css
+-rw-r--r--   0        0        0    31482 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/css/img/jsoneditor-icons.svg
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/i18n/dt/README.md
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/i18n/dt/en.json
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/i18n/dt/fr.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/i18n/flatpickr/fr.js
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/i18n/momentjs/fr.js
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/displays.js
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/form.js
+-rw-r--r--   0        0        0    16174 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/list.js
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/render.js
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/utils.js
+-rw-r--r--   0        0        0    13295 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/dt.checkboxes.js
+-rw-r--r--   0        0        0   354520 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/dt.min.js
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/dt.searchHighlight.js
+-rw-r--r--   0        0        0    50680 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/flatpickr.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/jquery.min.js
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/js.cookie.min.js
+-rw-r--r--   0        0        0   890454 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/jsoneditor.min.js
+-rw-r--r--   0        0        0    59517 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/moment.min.js
+-rw-r--r--   0        0        0   970347 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/pdfmake.min.js
+-rw-r--r--   0        0        0    73164 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/select2.min.js
+-rw-r--r--   0        0        0   146912 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/tabler.min.js
+-rw-r--r--   0        0        0   870285 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/vfs_fonts.js
+-rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/base.html
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/create.html
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/detail.html
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/edit.html
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/error.html
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/index.html
+-rw-r--r--   0        0        0    14329 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/layout.html
+-rw-r--r--   0        0        0     9127 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/list.html
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/login.html
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/_empty.html
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/_null.html
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/boolean.html
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/collection.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/email.html
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/file.html
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/image.html
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/json.html
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/list.html
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/relation.html
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/text.html
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/tinymce.html
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/url.html
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/_delete.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/_error.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/_label.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/boolean.html
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/collection.html
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/enum.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/file.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/image.html
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/input.html
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/json.html
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/list.html
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/relation.html
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/tags.html
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/textarea.html
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/macros/views.html
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/modals/actions.html
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/modals/delete.html
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/modals/error.html
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/templates/modals/loading.html
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.mo
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.po
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.mo
+-rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/utils/__init__.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/utils/countries.py
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/starlette_admin/utils/timezones.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/LICENSE
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/README.md
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 starlette_admin-0.8.0.dev0/PKG-INFO
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/__init__.py` & `starlette_admin-0.8.0.dev0/starlette_admin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0.dev0"
+__version__ = "0.8.0.dev0"
 
 from ._types import ExportType, RequestAction
 from .actions import action
 from .base import BaseAdmin
 from .fields import (
     ArrowField,
     BaseField,
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/_types.py` & `starlette_admin-0.8.0.dev0/starlette_admin/_types.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/actions.py` & `starlette_admin-0.8.0.dev0/starlette_admin/actions.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/auth.py` & `starlette_admin-0.8.0.dev0/starlette_admin/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,9 +158,8 @@
             return RedirectResponse(
                 "{url}?{query_params}".format(
                     url=request.url_for(request.app.state.ROUTE_NAME + ":login"),
                     query_params=urlencode({"next": str(request.url)}),
                 ),
                 status_code=HTTP_303_SEE_OTHER,
             )
-        else:
-            return await call_next(request)
+        return await call_next(request)
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/base.py` & `starlette_admin-0.8.0.dev0/starlette_admin/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,18 +92,15 @@
         self.init_auth()
         self.init_routes()
 
     def add_view(self, view: Union[Type[BaseView], BaseView]) -> None:
         """
         Add View to the Admin interface.
         """
-        if isinstance(view, BaseView):
-            view_instance = view
-        else:
-            view_instance = view()
+        view_instance = view if isinstance(view, BaseView) else view()
         self._views.append(view_instance)
         self.setup_view(view_instance)
 
     def custom_render_js(self, request: Request) -> Optional[str]:
         """
         Override this function to provide a link to custom js to override the
         global `render` object in javascript which is use to render fields in
@@ -291,15 +288,15 @@
         if not model.is_accessible(request):
             return JSONResponse(None, status_code=HTTP_403_FORBIDDEN)
         skip = int(request.query_params.get("skip") or "0")
         limit = int(request.query_params.get("limit") or "100")
         order_by = request.query_params.getlist("order_by")
         where = request.query_params.get("where")
         pks = request.query_params.getlist("pks")
-        select2 = "select2" in request.query_params.keys()
+        select2 = "select2" in request.query_params
         if len(pks) > 0:
             items = await model.find_by_pks(request, pks)
             total = len(items)
         else:
             if where is not None:
                 try:
                     where = json.loads(where)
@@ -347,41 +344,40 @@
 
     async def _render_login(self, request: Request) -> Response:
         if request.method == "GET":
             return self.templates.TemplateResponse(
                 "login.html",
                 {"request": request, "_is_login_path": True},
             )
-        else:
-            form = await request.form()
-            try:
-                assert self.auth_provider is not None
-                return await self.auth_provider.login(
-                    form.get("username"),  # type: ignore
-                    form.get("password"),  # type: ignore
-                    form.get("remember_me") == "on",
-                    request,
-                    RedirectResponse(
-                        request.query_params.get("next")
-                        or request.url_for(self.route_name + ":index"),
-                        status_code=HTTP_303_SEE_OTHER,
-                    ),
-                )
-            except FormValidationError as errors:
-                return self.templates.TemplateResponse(
-                    "login.html",
-                    {"request": request, "form_errors": errors, "_is_login_path": True},
-                    status_code=HTTP_422_UNPROCESSABLE_ENTITY,
-                )
-            except LoginFailed as error:
-                return self.templates.TemplateResponse(
-                    "login.html",
-                    {"request": request, "error": error.msg, "_is_login_path": True},
-                    status_code=HTTP_400_BAD_REQUEST,
-                )
+        form = await request.form()
+        try:
+            assert self.auth_provider is not None
+            return await self.auth_provider.login(
+                form.get("username"),  # type: ignore
+                form.get("password"),  # type: ignore
+                form.get("remember_me") == "on",
+                request,
+                RedirectResponse(
+                    request.query_params.get("next")
+                    or request.url_for(self.route_name + ":index"),
+                    status_code=HTTP_303_SEE_OTHER,
+                ),
+            )
+        except FormValidationError as errors:
+            return self.templates.TemplateResponse(
+                "login.html",
+                {"request": request, "form_errors": errors, "_is_login_path": True},
+                status_code=HTTP_422_UNPROCESSABLE_ENTITY,
+            )
+        except LoginFailed as error:
+            return self.templates.TemplateResponse(
+                "login.html",
+                {"request": request, "error": error.msg, "_is_login_path": True},
+                status_code=HTTP_400_BAD_REQUEST,
+            )
 
     async def _render_logout(self, request: Request) -> Response:
         assert self.auth_provider is not None
         return await self.auth_provider.logout(
             request,
             RedirectResponse(
                 request.url_for(self.route_name + ":index"),
@@ -429,41 +425,38 @@
         if not model.is_accessible(request) or not model.can_create(request):
             raise HTTPException(HTTP_403_FORBIDDEN)
         if request.method == "GET":
             return self.templates.TemplateResponse(
                 model.create_template,
                 {"request": request, "model": model},
             )
-        else:
-            form = await request.form()
-            dict_obj = await self.form_to_dict(
-                request, form, model, RequestAction.CREATE
+        form = await request.form()
+        dict_obj = await self.form_to_dict(request, form, model, RequestAction.CREATE)
+        try:
+            obj = await model.create(request, dict_obj)
+        except FormValidationError as exc:
+            return self.templates.TemplateResponse(
+                model.create_template,
+                {
+                    "request": request,
+                    "model": model,
+                    "errors": exc.errors,
+                    "obj": dict_obj,
+                },
+                status_code=HTTP_422_UNPROCESSABLE_ENTITY,
             )
-            try:
-                obj = await model.create(request, dict_obj)
-            except FormValidationError as exc:
-                return self.templates.TemplateResponse(
-                    model.create_template,
-                    {
-                        "request": request,
-                        "model": model,
-                        "errors": exc.errors,
-                        "obj": dict_obj,
-                    },
-                    status_code=HTTP_422_UNPROCESSABLE_ENTITY,
-                )
-            pk = getattr(obj, model.pk_attr)  # type: ignore
-            url = request.url_for(self.route_name + ":list", identity=model.identity)
-            if form.get("_continue_editing", None) is not None:
-                url = request.url_for(
-                    self.route_name + ":edit", identity=model.identity, pk=pk
-                )
-            elif form.get("_add_another", None) is not None:
-                url = request.url
-            return RedirectResponse(url, status_code=HTTP_303_SEE_OTHER)
+        pk = getattr(obj, model.pk_attr)  # type: ignore
+        url = request.url_for(self.route_name + ":list", identity=model.identity)
+        if form.get("_continue_editing", None) is not None:
+            url = request.url_for(
+                self.route_name + ":edit", identity=model.identity, pk=pk
+            )
+        elif form.get("_add_another", None) is not None:
+            url = request.url
+        return RedirectResponse(url, status_code=HTTP_303_SEE_OTHER)
 
     async def _render_edit(self, request: Request) -> Response:
         identity = request.path_params.get("identity")
         model = self._find_model_from_identity(identity)
         if not model.is_accessible(request) or not model.can_edit(request):
             raise HTTPException(HTTP_403_FORBIDDEN)
         pk = request.path_params.get("pk")
@@ -476,41 +469,38 @@
                 {
                     "request": request,
                     "model": model,
                     "raw_obj": obj,
                     "obj": await model.serialize(obj, request, RequestAction.EDIT),
                 },
             )
-        else:
-            form = await request.form()
-            dict_obj = await self.form_to_dict(request, form, model, RequestAction.EDIT)
-            try:
-                obj = await model.edit(request, pk, dict_obj)
-            except FormValidationError as exc:
-                return self.templates.TemplateResponse(
-                    model.edit_template,
-                    {
-                        "request": request,
-                        "model": model,
-                        "errors": exc.errors,
-                        "obj": dict_obj,
-                    },
-                    status_code=HTTP_422_UNPROCESSABLE_ENTITY,
-                )
-            pk = getattr(obj, model.pk_attr)  # type: ignore
-            url = request.url_for(self.route_name + ":list", identity=model.identity)
-            if form.get("_continue_editing", None) is not None:
-                url = request.url_for(
-                    self.route_name + ":edit", identity=model.identity, pk=pk
-                )
-            elif form.get("_add_another", None) is not None:
-                url = request.url_for(
-                    self.route_name + ":create", identity=model.identity
-                )
-            return RedirectResponse(url, status_code=HTTP_303_SEE_OTHER)
+        form = await request.form()
+        dict_obj = await self.form_to_dict(request, form, model, RequestAction.EDIT)
+        try:
+            obj = await model.edit(request, pk, dict_obj)
+        except FormValidationError as exc:
+            return self.templates.TemplateResponse(
+                model.edit_template,
+                {
+                    "request": request,
+                    "model": model,
+                    "errors": exc.errors,
+                    "obj": dict_obj,
+                },
+                status_code=HTTP_422_UNPROCESSABLE_ENTITY,
+            )
+        pk = getattr(obj, model.pk_attr)  # type: ignore
+        url = request.url_for(self.route_name + ":list", identity=model.identity)
+        if form.get("_continue_editing", None) is not None:
+            url = request.url_for(
+                self.route_name + ":edit", identity=model.identity, pk=pk
+            )
+        elif form.get("_add_another", None) is not None:
+            url = request.url_for(self.route_name + ":create", identity=model.identity)
+        return RedirectResponse(url, status_code=HTTP_303_SEE_OTHER)
 
     async def _render_error(
         self,
         request: Request,
         exc: Exception = HTTPException(status_code=HTTP_500_INTERNAL_SERVER_ERROR),
     ) -> Response:
         assert isinstance(exc, HTTPException)
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/exceptions.py` & `starlette_admin-0.8.0.dev0/starlette_admin/exceptions.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/fields.py` & `starlette_admin-0.8.0.dev0/starlette_admin/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -913,21 +913,19 @@
             files = form_data.getlist(self.id)
             return [f for f in files if not is_empty_file(f.file)], should_be_deleted  # type: ignore
         file = form_data.get(self.id)
         return (None if (file and is_empty_file(file.file)) else file), should_be_deleted  # type: ignore
 
     def _isvalid_value(self, value: Any) -> bool:
         return value is not None and all(
-            [
-                (
-                    hasattr(v, "url")
-                    or (isinstance(v, dict) and v.get("url", None) is not None)
-                )
-                for v in (value if self.multiple else [value])
-            ]
+            (
+                hasattr(v, "url")
+                or (isinstance(v, dict) and v.get("url", None) is not None)
+            )
+            for v in (value if self.multiple else [value])
         )
 
     def input_params(self) -> str:
         return html_params(
             {
                 "accept": self.accept,
                 "disabled": self.disabled,
@@ -1071,16 +1069,18 @@
     ) -> None:
         self.name = name
         self.fields = fields
         self.required = required
         super().__post_init__()
         self._propagate_id()
 
-    def _extract_fields(
-        self, action: RequestAction = RequestAction.LIST
+    def get_fields_list(
+        self,
+        request: Request,
+        action: RequestAction = RequestAction.LIST,
     ) -> Sequence[BaseField]:
         return extract_fields(self.fields, action)
 
     def _propagate_id(self) -> None:
         """Will update fields id by adding his id as prefix (ex: category.name)"""
         for field in self.fields:
             field.id = self.id + ("." if self.id else "") + field.name
@@ -1194,19 +1194,19 @@
         """
         Return list of all indices.  For example, if field id is `foo` and
         form_data contains following keys ['foo.0.bar', 'foo.1.baz'], then the indices are [0,1].
         Note that some numbers can be skipped. For example, you may have [0,1,3,8]
         as indices.
         """
         indices = set()
-        for k in form_data:
-            if k.startswith(self.id):
-                k = k[len(self.id) + 1 :].split(".", maxsplit=1)[0]
-                if k.isdigit():
-                    indices.add(int(k))
+        for name in form_data:
+            if name.startswith(self.id):
+                idx = name[len(self.id) + 1 :].split(".", maxsplit=1)[0]
+                if idx.isdigit():
+                    indices.add(int(idx))
         return sorted(indices)
 
     def _field_at(self, idx: Optional[int] = None) -> BaseField:
         if idx is not None:
             self.field.id = self.id + "." + str(idx)
         else:
             """To generate template string to be used in javascript"""
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/helpers.py` & `starlette_admin-0.8.0.dev0/starlette_admin/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,24 +60,25 @@
 
 def html_params(kwargs: Dict[str, Any]) -> str:
     """Converts a dictionary of HTML attribute name-value pairs into a string of HTML parameters."""
     params = []
     for k, v in kwargs.items():
         if v is None or v is False:
             continue
-        elif v is True:
+        if v is True:
             params.append(k)
         else:
             params.append('{}="{}"'.format(str(k).replace("_", "-"), escape(v)))
     return " ".join(params)
 
 
 def extract_fields(
     fields: Sequence["BaseField"], action: RequestAction = RequestAction.LIST
 ) -> Sequence["BaseField"]:
+    """Extract fields based on the requested action and exclude flags."""
     arr = []
     for field in fields:
         if (
             (action == RequestAction.LIST and field.exclude_from_list)
             or (action == RequestAction.DETAIL and field.exclude_from_detail)
             or (action == RequestAction.CREATE and field.exclude_from_create)
             or (action == RequestAction.EDIT and field.exclude_from_edit)
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/i18n.py` & `starlette_admin-0.8.0.dev0/starlette_admin/i18n.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "current_locale", default=DEFAULT_LOCALE
     )
     _current_translation: ContextVar[NullTranslations] = ContextVar(
         "current_translation", default=translations[DEFAULT_LOCALE]
     )
 
     def set_locale(locale: str) -> None:
-        _current_locale.set(locale if locale in translations.keys() else DEFAULT_LOCALE)
+        _current_locale.set(locale if locale in translations else DEFAULT_LOCALE)
         _current_translation.set(translations[get_locale()])
 
     def get_locale() -> str:
         return _current_locale.get()
 
     def gettext(message: str) -> str:
         return _current_translation.get().ugettext(message)
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/views.py` & `starlette_admin-0.8.0.dev0/starlette_admin/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,18 +87,18 @@
         self.icon = icon
         self.always_open = always_open
         self.views: List[BaseView] = [
             (v if isinstance(v, BaseView) else v()) for v in views
         ]
 
     def is_active(self, request: Request) -> bool:
-        return any([v.is_active(request) for v in self.views])
+        return any(v.is_active(request) for v in self.views)
 
     def is_accessible(self, request: Request) -> bool:
-        return any([v.is_accessible(request) for v in self.views])
+        return any(v.is_accessible(request) for v in self.views)
 
 
 class Link(BaseView):
     """
     Add arbitrary hyperlinks to the menu
 
     Example:
@@ -362,15 +362,15 @@
         limit: int = 100,
         where: Union[Dict[str, Any], str, None] = None,
         order_by: Optional[List[str]] = None,
     ) -> Sequence[Any]:
         """
         Find all items
         Parameters:
-            request: Starlette Request
+            request: The request being processed
             where: Can be dict for complex query
                 ```json
                  {"and":[{"id": {"gt": 5}},{"name": {"startsWith": "ban"}}]}
                 ```
                 or plain text for full search
             skip: should return values start from position skip+1
             limit: number of maximum items to return
@@ -383,71 +383,71 @@
         self,
         request: Request,
         where: Union[Dict[str, Any], str, None] = None,
     ) -> int:
         """
         Count items
         Parameters:
-            request: Starlette Request
+            request: The request being processed
             where: Can be dict for complex query
                 ```json
                  {"and":[{"id": {"gt": 5}},{"name": {"startsWith": "ban"}}]}
                 ```
                 or plain text for full search
         """
         raise NotImplementedError()
 
     @abstractmethod
     async def delete(self, request: Request, pks: List[Any]) -> Optional[int]:
         """
         Bulk delete items
         Parameters:
-            request: Starlette Request
+            request: The request being processed
             pks: List of primary keys
         """
         raise NotImplementedError()
 
     @abstractmethod
     async def find_by_pk(self, request: Request, pk: Any) -> Any:
         """
         Find one item
         Parameters:
-            request: Starlette Request
+            request: The request being processed
             pk: Primary key
         """
         raise NotImplementedError()
 
     @abstractmethod
     async def find_by_pks(self, request: Request, pks: List[Any]) -> Sequence[Any]:
         """
         Find many items
         Parameters:
-            request: Starlette Request
+            request: The request being processed
             pks: List of Primary key
         """
         raise NotImplementedError()
 
     @abstractmethod
     async def create(self, request: Request, data: Dict) -> Any:
         """
         Create item
         Parameters:
-            request: Starlette Request
+            request: The request being processed
             data: Dict values contained converted form data
         Returns:
             Any: Created Item
         """
         raise NotImplementedError()
 
     @abstractmethod
     async def edit(self, request: Request, pk: Any, data: Dict[str, Any]) -> Any:
         """
         Edit item
         Parameters:
-            request: Starlette Request
+            request: The request being processed
             pk: Primary key
             data: Dict values contained converted form data
         Returns:
             Any: Edited Item
         """
         raise NotImplementedError()
 
@@ -478,15 +478,15 @@
 
         Parameters:
             value: attribute of item returned by `find_all` or `find_by_pk`
             field: Starlette Admin field for this attribute
             action: Specify where the data will be used. Possible values are
                 `VIEW` for detail page, `EDIT` for editing page and `API`
                 for listing page and select2 data.
-            request: Starlette Request
+            request: The request being processed
         """
         if value is None:
             return await field.serialize_none_value(request, action)
         return await field.serialize_value(request, value, action)
 
     async def serialize(
         self,
@@ -547,61 +547,121 @@
         )
         obj_serialized["_edit_url"] = str(
             request.url_for(route_name + ":edit", identity=self.identity, pk=pk)
         )
         return obj_serialized
 
     async def repr(self, obj: Any, request: Request) -> str:
-        """
-        Override this function to customize item representation in
-        relationships columns
-        """
-        return str(getattr(obj, self.pk_attr))  # type: ignore
+        """Return a string representation of the given object that can be displayed in the admin interface.
+
+        If the object has a custom representation method `__admin_repr__`, it is used to generate the string. Otherwise,
+        the value of the object's primary key attribute is used.
+
+        Args:
+            obj: The object to represent.
+            request: The request being processed
+
+        Example:
+            For example, the following implementation for a `User` model will display
+            the user's full name instead of their primary key in the admin interface:
+
+            ```python
+            class User:
+                id: int
+                first_name: str
+                last_name: str
+
+                def __admin_repr__(self, request: Request):
+                    return f"{self.last_name} {self.first_name}"
+            ```
+        """
+        repr_method = getattr(
+            obj,
+            "__admin_repr__",
+            lambda request: str(getattr(obj, self.pk_attr)),  # type: ignore[arg-type]
+        )
+        if inspect.iscoroutinefunction(repr_method):
+            return await repr_method(request)
+        return repr_method(request)
 
     async def select2_result(self, obj: Any, request: Request) -> str:
-        """
-        Override this function to customize the way that search results are rendered.
+        """Returns an HTML-formatted string that represents the search results for a Select2 search box.
+
+        By default, this method returns a string that contains all the object's attributes in a list except
+        relation and file attributes.
+
+        If the object has a custom representation method `__admin_select2_repr__`, it is used to generate the
+        HTML-formatted string.
+
         !!! note
-            The returned value should be html. You can use `<span>mytext</span>`
-            when you want to return string value
+            The returned value should be valid HTML.
+
         !!! danger
             Escape your database value to avoid Cross-Site Scripting (XSS) attack.
             You can use Jinja2 Template render with `autoescape=True`.
             For more information [click here](https://owasp.org/www-community/attacks/xss/)
 
         Parameters:
-            obj: item returned by `find_all` or `find_by_pk`
-            request: Starlette Request
+            obj: The object returned by the `find_all` or `find_by_pk` method.
+            request: The request being processed
+
+        Example:
+            Here is an example implementation for a `User` model
+            that includes the user's name and photo:
+
+            ```python
+            class User:
+                id: int
+                name: str
+                photo_url: str
+
+                def __admin_select2_repr__(self, request: Request) -> str:
+                    return f'<div><img src="{escape(photo_url)}"><span>{escape(self.name)}</span></div>'
+            ```
 
         """
         template_str = (
             "<span>{%for col in fields %}{%if obj[col]%}<strong>{{col}}:"
             " </strong>{{obj[col]}} {%endif%}{%endfor%}</span>"
         )
         fields = [
             field.name
             for field in self.fields
-            if not isinstance(field, (RelationField, FileField))
+            if (
+                not isinstance(field, (RelationField, FileField))
+                and not field.exclude_from_detail
+            )
         ]
-        return Template(template_str, autoescape=True).render(obj=obj, fields=fields)
+        html_repr_method = getattr(
+            obj,
+            "__admin_select2_repr__",
+            lambda request: Template(template_str, autoescape=True).render(
+                obj=obj, fields=fields
+            ),
+        )
+        if inspect.iscoroutinefunction(html_repr_method):
+            return await html_repr_method(request)
+        return html_repr_method(request)
 
     async def select2_selection(self, obj: Any, request: Request) -> str:
         """
-        Override this function to customize the way that selections are rendered.
+        Returns the HTML representation of an item selected by a user in a Select2 component.
+        By default, it simply calls `select2_result()`.
+
         !!! note
-            The returned value should be html. You can use `<span>mytext</span>`
-            when you want to return string value
+            The returned value should be valid HTML.
+
         !!! danger
             Escape your database value to avoid Cross-Site Scripting (XSS) attack.
             You can use Jinja2 Template render with `autoescape=True`.
             For more information [click here](https://owasp.org/www-community/attacks/xss/)
 
         Parameters:
             obj: item returned by `find_all` or `find_by_pk`
-            request: Starlette Request
+            request: The request being processed
 
         """
         return await self.select2_result(obj, request)
 
     def _length_menu(self) -> Any:
         return [
             self.page_size_options,
@@ -610,17 +670,27 @@
 
     def _search_columns_selector(self) -> List[str]:
         return ["%s:name" % name for name in self.searchable_fields]  # type: ignore
 
     def _export_columns_selector(self) -> List[str]:
         return ["%s:name" % name for name in self.export_fields]  # type: ignore
 
-    def _extract_fields(
-        self, action: RequestAction = RequestAction.LIST
+    def get_fields_list(
+        self,
+        request: Request,
+        action: RequestAction = RequestAction.LIST,
     ) -> Sequence[BaseField]:
+        """Return a list of field instances to display in the specified view action.
+        This function excludes fields with corresponding exclude flags, which are
+        determined by the `exclude_fields_from_*` attributes.
+
+        Parameters:
+             request: The request being processed.
+             action: The type of action being performed on the view.
+        """
         return extract_fields(self.fields, action)
 
     def _additional_css_links(
         self, request: Request, action: RequestAction
     ) -> Sequence[str]:
         links = []
         for field in self.fields:
@@ -662,15 +732,15 @@
                 (it, False) if isinstance(it, str) else it
                 for it in self.fields_default_sort  # type: ignore[union-attr]
             ),
             "exportTypes": self.export_types,
             "columnVisibility": self.column_visibility,
             "searchBuilder": self.search_builder,
             "responsiveTable": self.responsive_table,
-            "fields": [f.dict() for f in self._extract_fields()],
+            "fields": [f.dict() for f in self.get_fields_list(request)],
             "actions": await self.get_all_actions(request),
             "pk": self.pk_attr,
             "locale": locale,
             "apiUrl": request.url_for(
                 f"{request.app.state.ROUTE_NAME}:api", identity=self.identity
             ),
             "actionUrl": request.url_for(
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/mongoengine/admin.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/mongoengine/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/mongoengine/fields.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/mongoengine/fields.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/mongoengine/helpers.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/mongoengine/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 from typing import Any, Callable, Dict, List, Optional, Sequence, Type
 
 import mongoengine.fields as me
 import starlette_admin.fields as sa
 from mongoengine import EmbeddedDocument
 from mongoengine.base.fields import BaseField as MongoBaseField
-from mongoengine.queryset import Q as BaseQ
+from mongoengine.queryset import Q as BaseQ  # noqa: N811
 from mongoengine.queryset import QNode
 from starlette_admin.contrib.mongoengine.exceptions import NotSupportedField
 from starlette_admin.contrib.mongoengine.fields import FileField, ImageField
 from starlette_admin.helpers import slugify_class_name
 
 mongoengine_to_admin_map = {
     me.ObjectIdField: sa.StringField,
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/mongoengine/view.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/mongoengine/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,16 +218,15 @@
     async def _build_query(
         self, request: Request, where: Union[Dict[str, Any], str, None] = None
     ) -> QNode:
         if where is None:
             return Q.empty()
         if isinstance(where, dict):
             return resolve_deep_query(where, self.document)
-        else:
-            return await self.build_full_text_search_query(request, where)
+        return await self.build_full_text_search_query(request, where)
 
     async def build_full_text_search_query(self, request: Request, term: str) -> QNode:
         queries = []
         for field in self.fields:
             if (
                 field.searchable
                 and field.name != "id"
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/odmantic/admin.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/odmantic/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/odmantic/helpers.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/odmantic/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     admin_field: t.Optional[BaseField] = None
     _origin = get_origin(annotation)
     if _origin is t.Union:  # type: ignore
         """Support for Optional"""
         return convert_odm_field_to_admin_field(
             field, field_name, get_args(annotation)[0]
         )
-    elif _origin in annotation_map:
+    if _origin in annotation_map:
         admin_field = annotation_map.get(_origin)(field_name)  # type: ignore
     elif _origin in (list, set) and not isinstance(field, ODMEmbeddedGeneric):
         child_field = convert_odm_field_to_admin_field(
             field, field_name, get_args(annotation)[0]
         )
         if isinstance(child_field, EnumField):
             child_field.multiple = True
@@ -101,15 +101,15 @@
         return HasOne(field_name, identity=slugify_class_name(field.model.__name__))
     elif hasattr(annotation, "__mro__"):
         types = inspect.getmro(annotation)
         for _type in types:
             if issubclass(_type, Enum):
                 admin_field = EnumField(field_name, enum=_type)
                 break
-            elif annotation_map.get(_type) is not None:
+            if annotation_map.get(_type) is not None:
                 admin_field = annotation_map.get(_type)(field_name)  # type: ignore
                 break
     if admin_field is None:
         raise NotSupportedAnnotation(f"{annotation} is not supported")
     admin_field.required = field.is_required_in_doc() and not field.primary_field  # type: ignore
     return admin_field
 
@@ -188,15 +188,15 @@
 def _check_value(v: t.Any, proxy: t.Optional[FieldProxy]) -> t.Any:
     """
     The purpose of this function is to detect datetime string, or ObjectId
     and convert them into the appropriate python type.
     """
     if isinstance(v, str) and pyd.datetime_parse.datetime_re.match(v):
         return datetime.datetime.fromisoformat(v)
-    elif proxy is not None and +proxy == "_id" and bson.ObjectId.is_valid(v):
+    if proxy is not None and +proxy == "_id" and bson.ObjectId.is_valid(v):
         return bson.ObjectId(v)
     return v
 
 
 def resolve_deep_query(
     where: t.Dict[str, t.Any],
     model: t.Type[Model],
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/odmantic/middleware.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/odmantic/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/odmantic/view.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/odmantic/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,16 +221,15 @@
     async def _build_query(
         self, request: Request, where: Union[Dict[str, Any], str, None] = None
     ) -> Any:
         if where is None:
             return {}
         if isinstance(where, dict):
             return resolve_deep_query(where, self.model)
-        else:
-            return await self.build_full_text_search_query(request, where)
+        return await self.build_full_text_search_query(request, where)
 
     async def _build_order_clauses(self, order_list: List[str]) -> Any:
         clauses = []
         for value in order_list:
             key, order = value.strip().split(maxsplit=1)
             clause = resolve_proxy(self.model, key)
             if clause is not None:
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/admin.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,19 +82,18 @@
         file = StorageManager.get_file(f"{storage}/{file_id}")
         if file.object.driver.name == "Local Storage":
             """If file is stored in local storage, just return a
             FileResponse with the fill full path."""
             return FileResponse(
                 file.get_cdn_url(), media_type=file.content_type, filename=file.filename  # type: ignore
             )
-        elif file.get_cdn_url() is not None:  # pragma: no cover
+        if file.get_cdn_url() is not None:  # pragma: no cover
             """If file has public url, redirect to this url"""
             return RedirectResponse(file.get_cdn_url())  # type: ignore
-        else:
-            """Otherwise, return a streaming response"""
-            return StreamingResponse(
-                file.object.as_stream(),
-                media_type=file.content_type,
-                headers={"Content-Disposition": f"attachment;filename={file.filename}"},
-            )
+        """Otherwise, return a streaming response"""
+        return StreamingResponse(
+            file.object.as_stream(),
+            media_type=file.content_type,
+            headers={"Content-Disposition": f"attachment;filename={file.filename}"},
+        )
     except ObjectDoesNotExistError:
         return JSONResponse({"detail": "Not found"}, status_code=404)
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/converters.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,18 +71,15 @@
     # Search by name
     for col_type in types:
         if col_type.__name__ in converters:
             return converters[col_type.__name__]
 
         # Support for custom types which inherit TypeDecorator
         if hasattr(col_type, "impl"):
-            if callable(col_type.impl):
-                impl = col_type.impl
-            else:
-                impl = col_type.impl.__class__
+            impl = col_type.impl if callable(col_type.impl) else col_type.impl.__class__
             return _search_converter_for_col_type(impl)
     return None  # pragma: no cover
 
 
 def field_common(column: Column) -> Dict[str, Any]:
     extra_args: Dict[str, Any] = {
         "help_text": column.comment,
@@ -129,20 +126,20 @@
 
 @converts("Boolean", "BIT")  # includes UnicodeText
 def conv_boolean(name: str, column: Column) -> BaseField:
     return BooleanField(name, **field_common(column))
 
 
 @converts("DateTime")
-def conv_dateTime(name: str, column: Column) -> BaseField:
+def conv_datetime(name: str, column: Column) -> BaseField:
     return DateTimeField(name, **field_common(column))
 
 
 @converts("Date")
-def conv_Date(name: str, column: Column) -> BaseField:
+def conv_date(name: str, column: Column) -> BaseField:
     return DateField(name, **field_common(column))
 
 
 @converts("Time")
 def conv_time(name: str, column: Column) -> BaseField:
     return TimeField(name, **field_common(column))
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/fields.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 def _serialize_sqlalchemy_file_library(
     request: Request, value: Any, action: RequestAction, is_multiple: bool
 ) -> Optional[Union[List[Dict[str, Any]], Dict[str, Any]]]:
     from sqlalchemy_file import File
 
     if isinstance(value, File) or (
-        isinstance(value, list) and all([isinstance(f, File) for f in value])
+        isinstance(value, list) and all(isinstance(f, File) for f in value)
     ):
         data = []
         for item in value if isinstance(value, list) else [value]:
             path = item["path"]
             if (
                 action == RequestAction.LIST
                 and getattr(item, "thumbnail", None) is not None
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/helpers.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,15 @@
         attr_key, order = value.strip().split(maxsplit=1)
         attr = getattr(model, attr_key, None)
         if attr is not None:
             clauses.append(attr.desc() if order.lower() == "desc" else attr)
     return clauses
 
 
-def normalize_fields(  # noqa: C901
-    fields: Sequence[Any], mapper: Mapper
-) -> List[BaseField]:
+def normalize_fields(fields: Sequence[Any], mapper: Mapper) -> List[BaseField]:
     """
     Look and convert all InstrumentedAttribute or str in fields into the
     right field (starlette_admin.BaseField)
     """
     converted_fields = []
     for field in fields:
         if isinstance(field, BaseField):
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/middleware.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqla/view.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqla/view.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/contrib/sqlmodel/view.py` & `starlette_admin-0.8.0.dev0/starlette_admin/contrib/sqlmodel/view.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/css/dt.checkboxes.css` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/css/dt.checkboxes.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/css/dt.min.css` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/css/dt.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/css/flatpickr.min.css` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/css/flatpickr.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/css/fontawesome.min.css` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/css/jsoneditor.min.css` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/css/jsoneditor.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/css/select2.min.css` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/css/tabler.min.css` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/css/img/jsoneditor-icons.svg` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/css/img/jsoneditor-icons.svg`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/i18n/dt/en.json` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/i18n/dt/en.json`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/i18n/dt/fr.json` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/i18n/dt/fr.json`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/i18n/flatpickr/fr.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/i18n/flatpickr/fr.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/i18n/momentjs/fr.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/i18n/momentjs/fr.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/form.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/form.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/list.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/list.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/render.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/render.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/utils.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/utils.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/dt.checkboxes.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/dt.checkboxes.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/dt.min.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/dt.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/dt.searchHighlight.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/dt.searchHighlight.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/flatpickr.min.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/flatpickr.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/jquery.min.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/jquery.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/js.cookie.min.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/js.cookie.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/jsoneditor.min.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/jsoneditor.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/moment.min.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/moment.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/pdfmake.min.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/pdfmake.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/select2.min.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/select2.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/tabler.min.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/tabler.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/js/vendor/vfs_fonts.js` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/js/vendor/vfs_fonts.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.ttf` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.woff2` & `starlette_admin-0.8.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/base.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/base.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/create.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/create.html`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,17 @@
                             <div class="container-fluid">
                                 <div class="d-flex justify-content-between align-items-center">
                                     <h3 class="card-title">{{ _("New %(name)s", name=model.name ) }}</h3>
                                 </div>
                             </div>
                         </div>
                         <div class="card-body border-bottom py-3">
-                            {% for field in model._extract_fields('CREATE') %}
+                            {% for field in model.get_fields_list(request, 'CREATE' | ra) %}
                                 <div class="mb-3">
-                                    {% with action='CREATE', data=(None if not obj else obj[field.name]), error=errors.get(field.name, None) if errors else None %}
+                                    {% with action=('CREATE'| ra), data=(None if not obj else obj[field.name]), error=errors.get(field.name, None) if errors else None %}
                                         {% include field.label_template %}
                                         {% include field.form_template %}
                                     {% endwith %}
                                 </div>
                             {% endfor %}
                         </div>
                         <div class="card-footer text-black">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 {% extends "layout.html" %} {% block header %}
 ****** {{ model.label }} ******
    1. {{__("Admin")_}}
    2. {{_model.label_}}
    3. {{ _("Create") }}
 {% endblock %} {% block content %}
 **** {{ _("New %(name)s", name=model.name ) }} ****
-{% for field in model._extract_fields('CREATE') %}
-{% with action='CREATE', data=(None if not obj else obj[field.name]),
+{% for field in model.get_fields_list(request, 'CREATE' | ra) %}
+{% with action=('CREATE'| ra), data=(None if not obj else obj[field.name]),
 error=errors.get(field.name, None) if errors else None %} {% include
 field.label_template %} {% include field.form_template %} {% endwith %}
 {% endfor %}
 {{__("Cancel")_}} {{ _("Save and add another") }} {{ _("Save and continue
 editing") }} {{ _("Save") }}
 {% endblock %} {% block head_css %} {% for link in model._additional_css_links
 (request, "CREATE" | ra) %}
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/detail.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/detail.html`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                                 <thead>
                                 <tr>
                                     <th>{{ _("Attribute") }}</th>
                                     <th>{{ _("Value") }}</th>
                                 </tr>
                                 </thead>
                                 <tbody>
-                                {% for field in model._extract_fields('DETAIL') %}
+                                {% for field in model.get_fields_list(request, 'DETAIL' | ra) %}
                                     <tr>
                                         <td data-label="Attribute">
                                             <div>
                                                 <strong>{{ field.label }}</strong>
                                             </div>
                                         </td>
                                         <td data-label="Value">
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/edit.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/edit.html`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,17 @@
                             <div class="container-fluid">
                                 <div class="d-flex justify-content-between align-items-center">
                                     <h3 class="card-title">{{ _("Edit %(name)s", name=model.name ) }}</h3>
                                 </div>
                             </div>
                         </div>
                         <div class="card-body border-bottom py-3">
-                            {% for field in model._extract_fields('EDIT') %}
+                            {% for field in model.get_fields_list(request, 'EDIT' | ra) %}
                                 <div class="mb-3">
-                                    {% with action='EDIT',data=obj[field.name], error=errors.get(field.name, None) if errors else None %}
+                                    {% with action=('EDIT' | ra),data=obj[field.name], error=errors.get(field.name, None) if errors else None %}
                                         {% include field.label_template %}
                                         {% include field.form_template %}
                                     {% endwith %}
                                 </div>
                             {% endfor %}
                         </div>
                         <div class="card-footer text-black">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 {% extends "layout.html" %} {% block header %}
 ****** {{ model.label }} ******
    1. {{__("Admin")_}}
    2. {{_model.label_}}
    3. {{ _("Edit") }}
 {% endblock %} {% block content %}
 **** {{ _("Edit %(name)s", name=model.name ) }} ****
-{% for field in model._extract_fields('EDIT') %}
-{% with action='EDIT',data=obj[field.name], error=errors.get(field.name, None)
-if errors else None %} {% include field.label_template %} {% include
+{% for field in model.get_fields_list(request, 'EDIT' | ra) %}
+{% with action=('EDIT' | ra),data=obj[field.name], error=errors.get(field.name,
+None) if errors else None %} {% include field.label_template %} {% include
 field.form_template %} {% endwith %}
 {% endfor %}
 {{__("Cancel")_}} {{ _("Save and add another") }} {{ _("Save and continue
 editing") }} {{ _("Save") }}
 {% endblock %} {% block head_css %} {% for link in model._additional_css_links
 (request, "EDIT" | ra) %}
  {% endfor %}
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/error.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/error.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/layout.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/layout.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/list.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/list.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/login.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/login.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/displays/collection.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/displays/collection.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <dl>
-    {% for field in field._extract_fields('DETAIL') %}
+    {% for field in field.get_fields_list(request, 'DETAIL' | ra) %}
         <dt>{{ field.label }}:</dt>
         <dd>
             {% with data=(data[field.name] if data else None) %}
                 {% if data == None %}
                     {% include "displays/_null.html" %}
                 {% elif (data | is_iter) and (data |length) ==0 %}
                     {% include "displays/_empty.html" %}
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/_delete.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/_delete.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/collection.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/collection.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <fieldset class="form-fieldset">
-    {% for field in field._extract_fields(action) %}
+    {% for field in field.get_fields_list(request, action) %}
         <div class="form-group row mb-3">
             <label class="col-3 col-form-label {% if field.required %}required{% endif %}"
                    for="{{ field.id }}">{{ field.label }}</label>
             <div class="col">
                 {% set item_data= (data[field.name] if data else None) %}
                 {% with data=item_data, error=error.get(field.name, None) if error else None %}
                     {% include field.form_template %}
```

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/enum.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/enum.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/file.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/file.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/image.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/image.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/list.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/list.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/relation.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/relation.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/forms/tags.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/forms/tags.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/macros/views.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/macros/views.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/modals/actions.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/modals/actions.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/modals/delete.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/modals/delete.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/modals/error.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/modals/error.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/templates/modals/loading.html` & `starlette_admin-0.8.0.dev0/starlette_admin/templates/modals/loading.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.mo` & `starlette_admin-0.8.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.mo`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.po` & `starlette_admin-0.8.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.po`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.mo` & `starlette_admin-0.8.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.mo`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.po` & `starlette_admin-0.8.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.po`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/utils/countries.py` & `starlette_admin-0.8.0.dev0/starlette_admin/utils/countries.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/starlette_admin/utils/timezones.py` & `starlette_admin-0.8.0.dev0/starlette_admin/utils/timezones.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/LICENSE` & `starlette_admin-0.8.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/README.md` & `starlette_admin-0.8.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.7.0.dev0/pyproject.toml` & `starlette_admin-0.8.0.dev0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 [project.optional-dependencies]
 i18n = [
     "babel >=2.12.1"
 ]
 test = [
     "pytest >=7.2.0, <7.3.0",
     "pytest-asyncio >=0.20.2, <0.22.0",
-    "mypy ==1.1.1",
-    "ruff ==0.0.259",
-    "black ==23.1.0",
+    "mypy ==1.2.0",
+    "ruff ==0.0.261",
+    "black ==23.3.0",
     "httpx >=0.23.3, <0.24.0",
     "coverage >=7.0.0, <7.3.0",
     "SQLAlchemy-Utils >=0.40.0, <0.41.0",
     "arrow >=1.2.3, <1.3.0",
     "colour >=0.1.5, <0.2.0",
     "phonenumbers >=8.13.3, <8.14.0",
     "passlib >=1.7.4, <1.8.0",
@@ -64,22 +64,22 @@
     "psycopg2-binary >=2.9.5, <3.0.0",
     "aiosqlite >=0.17.0, <0.19.0",
     "asyncpg >=0.27.0, <0.28.0",
     "aiomysql >=0.1.1, <0.2.0",
     "mongoengine >=0.25.0, <0.28.0",
     "odmantic >=0.9.0,<0.10.0",
     "tinydb >=4.7.0, <4.8.0",
-    "Pillow >=9.4.0, <9.5.0",
+    "Pillow >=9.4.0, <9.6.0",
     "itsdangerous >=2.1.2, <2.2.0",
     "pydantic[email] >=1.10.2, <2.0.0",
 ]
 doc = [
     "mkdocs >=1.4.2, <2.0.0",
     "mkdocs-material >=9.0.0, <10.0.0",
-    "mkdocstrings[python] >=0.19.0, <0.21.0",
+    "mkdocstrings[python] >=0.19.0, <0.22.0",
     "mkdocs-static-i18n >=0.53.0, <0.57.0"
 ]
 dev = [
     "pre-commit >=2.20.0, <4.0.0",
     "uvicorn >=0.20.0, <0.22.0",
 ]
 
@@ -159,32 +159,48 @@
 [tool.coverage.run]
 parallel = true
 concurrency = ["thread", "greenlet"]
 source = ["starlette_admin", "tests"]
 
 [tool.ruff]
 select = [
+    "B", # flake8-bugbear
+    "C4", # flake8-comprehensions
+    "C90", # mccabe
     "E", # pycodestyle errors
-    "W", # pycodestyle warnings
+    "ERA", # eradicate
     "F", # pyflakes
     "I", # isort
-    "C", # flake8-comprehensions
-    "B", # flake8-bugbear
+    "INT", # flake8-gettext
+    "N", # pep8-naming
+    "PIE", # flake8-pie,
+    "PLC", # pylint - convention
+    "PLE", # pylint - error
+    "PLW", # pylint - warning
+    "Q", # flake8-quotes
+    "RET", # flake8-return,
+    "RUF", # Ruff-specific rules
+    "SIM", # flake8-simplify
+    "UP", # pyupgrade
+    "W", # pycodestyle warnings
 ]
 ignore = [
-    "E501", # line too long, handled by black
     "B008", # Do not perform function call `_` in argument defaults, neccessary for lazy_gettext
     "B905", # `zip()` without an explicit `strict=` parameter
+    "E501", # line too long, handled by black
+    "N818", # Exception {name} should be named with an Error suffix
 ]
+target-version = "py37"
 
 [tool.ruff.isort]
 known-third-party = ["starlette_admin"]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
+"examples/**" = ["N805", "N999"]
 
 [tool.mypy]
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
 disallow_untyped_decorators = true
 no_implicit_optional = true
```

### Comparing `starlette_admin-0.7.0.dev0/PKG-INFO` & `starlette_admin-0.8.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-admin
-Version: 0.7.0.dev0
+Version: 0.8.0.dev0
 Summary: Fast, beautiful and extensible administrative interface framework for Starlette/FastApi applications
 Project-URL: Homepage, https://github.com/jowilf/starlette-admin
 Project-URL: Documentation, https://jowilf.github.io/starlette-admin
 Project-URL: Repository, https://github.com/jowilf/starlette-admin
 Project-URL: Changelog, https://jowilf.github.io/starlette-admin/changelog/
 Author-email: Jocelin Hounon <hounonj@gmail.com>
 License-Expression: MIT
@@ -30,41 +30,41 @@
 Provides-Extra: dev
 Requires-Dist: pre-commit<4.0.0,>=2.20.0; extra == 'dev'
 Requires-Dist: uvicorn<0.22.0,>=0.20.0; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mkdocs-material<10.0.0,>=9.0.0; extra == 'doc'
 Requires-Dist: mkdocs-static-i18n<0.57.0,>=0.53.0; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.4.2; extra == 'doc'
-Requires-Dist: mkdocstrings[python]<0.21.0,>=0.19.0; extra == 'doc'
+Requires-Dist: mkdocstrings[python]<0.22.0,>=0.19.0; extra == 'doc'
 Provides-Extra: i18n
 Requires-Dist: babel>=2.12.1; extra == 'i18n'
 Provides-Extra: test
 Requires-Dist: aiomysql<0.2.0,>=0.1.1; extra == 'test'
 Requires-Dist: aiosqlite<0.19.0,>=0.17.0; extra == 'test'
 Requires-Dist: arrow<1.3.0,>=1.2.3; extra == 'test'
 Requires-Dist: asyncpg<0.28.0,>=0.27.0; extra == 'test'
 Requires-Dist: backports-zoneinfo; python_version < '3.9' and extra == 'test'
-Requires-Dist: black==23.1.0; extra == 'test'
+Requires-Dist: black==23.3.0; extra == 'test'
 Requires-Dist: colour<0.2.0,>=0.1.5; extra == 'test'
 Requires-Dist: coverage<7.3.0,>=7.0.0; extra == 'test'
 Requires-Dist: fasteners==0.18; extra == 'test'
 Requires-Dist: httpx<0.24.0,>=0.23.3; extra == 'test'
 Requires-Dist: itsdangerous<2.2.0,>=2.1.2; extra == 'test'
 Requires-Dist: mongoengine<0.28.0,>=0.25.0; extra == 'test'
-Requires-Dist: mypy==1.1.1; extra == 'test'
+Requires-Dist: mypy==1.2.0; extra == 'test'
 Requires-Dist: odmantic<0.10.0,>=0.9.0; extra == 'test'
 Requires-Dist: passlib<1.8.0,>=1.7.4; extra == 'test'
 Requires-Dist: phonenumbers<8.14.0,>=8.13.3; extra == 'test'
-Requires-Dist: pillow<9.5.0,>=9.4.0; extra == 'test'
+Requires-Dist: pillow<9.6.0,>=9.4.0; extra == 'test'
 Requires-Dist: psycopg2-binary<3.0.0,>=2.9.5; extra == 'test'
 Requires-Dist: pydantic[email]<2.0.0,>=1.10.2; extra == 'test'
 Requires-Dist: pymysql[rsa]<1.1.0,>=1.0.2; extra == 'test'
 Requires-Dist: pytest-asyncio<0.22.0,>=0.20.2; extra == 'test'
 Requires-Dist: pytest<7.3.0,>=7.2.0; extra == 'test'
-Requires-Dist: ruff==0.0.259; extra == 'test'
+Requires-Dist: ruff==0.0.261; extra == 'test'
 Requires-Dist: sqlalchemy-file<0.5.0,>=0.4.0; extra == 'test'
 Requires-Dist: sqlalchemy-utils<0.41.0,>=0.40.0; extra == 'test'
 Requires-Dist: tinydb<4.8.0,>=4.7.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # starlette-admin
```

