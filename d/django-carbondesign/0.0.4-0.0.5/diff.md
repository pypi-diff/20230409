# Comparing `tmp/django-carbondesign-0.0.4.tar.gz` & `tmp/django-carbondesign-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-carbondesign-0.0.4.tar", last modified: Thu Jun 30 10:49:08 2022, max compression
+gzip compressed data, was "django-carbondesign-0.0.5.tar", last modified: Sun Apr  9 21:54:36 2023, max compression
```

## Comparing `django-carbondesign-0.0.4.tar` & `django-carbondesign-0.0.5.tar`

### file list

```diff
@@ -1,173 +1,175 @@
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.783000 django-carbondesign-0.0.4/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1067 2022-02-11 01:28:54.000000 django-carbondesign-0.0.4/LICENSE
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1248 2022-06-30 10:40:12.783000 django-carbondesign-0.0.4/PKG-INFO
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      513 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/README.rst
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.161000 django-carbondesign-0.0.4/carbondesign/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      513 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/README.rst
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      107 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/__init__.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      223 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/apps.py
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.172000 django-carbondesign-0.0.4/carbondesign/forms-js/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1002 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/forms-js/fields.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3840 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/forms-js/forms.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1422 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/forms-js/widgets.js
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.215000 django-carbondesign-0.0.4/carbondesign/js/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      126 2021-12-15 08:31:13.000000 django-carbondesign-0.0.4/carbondesign/js/checkbox.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      269 2022-04-15 16:07:50.000000 django-carbondesign-0.0.4/carbondesign/js/content-switcher.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      138 2021-12-15 16:43:45.000000 django-carbondesign-0.0.4/carbondesign/js/data-table.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      136 2022-02-28 15:16:00.000000 django-carbondesign-0.0.4/carbondesign/js/date-picker.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      144 2022-03-05 11:11:46.000000 django-carbondesign-0.0.4/carbondesign/js/file-uploader.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      202 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/js/modal.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      142 2022-03-10 13:02:27.000000 django-carbondesign-0.0.4/carbondesign/js/notification.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      144 2022-03-01 21:03:23.000000 django-carbondesign-0.0.4/carbondesign/js/overflow-menu.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1097 2022-04-08 14:41:24.000000 django-carbondesign-0.0.4/carbondesign/js/pagination.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      220 2022-04-15 12:40:11.000000 django-carbondesign-0.0.4/carbondesign/js/tabs.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      132 2021-12-15 08:28:00.000000 django-carbondesign-0.0.4/carbondesign/js/text-input.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      834 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/js/ui-shell.js
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.135000 django-carbondesign-0.0.4/carbondesign/locale/
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.132000 django-carbondesign-0.0.4/carbondesign/locale/id/
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.226000 django-carbondesign-0.0.4/carbondesign/locale/id/LC_MESSAGES/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3382 2022-04-21 07:16:30.000000 django-carbondesign-0.0.4/carbondesign/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6385 2022-04-21 11:52:43.000000 django-carbondesign-0.0.4/carbondesign/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3093 2022-04-19 16:28:25.000000 django-carbondesign-0.0.4/carbondesign/locale/id/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6290 2022-04-15 19:42:58.000000 django-carbondesign-0.0.4/carbondesign/locale/id/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.134000 django-carbondesign-0.0.4/carbondesign/locale/jv/
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.241000 django-carbondesign-0.0.4/carbondesign/locale/jv/LC_MESSAGES/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      337 2022-04-21 07:16:30.000000 django-carbondesign-0.0.4/carbondesign/locale/jv/LC_MESSAGES/django.mo
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5492 2022-04-21 11:52:43.000000 django-carbondesign-0.0.4/carbondesign/locale/jv/LC_MESSAGES/django.po
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      337 2022-06-29 20:17:53.000000 django-carbondesign-0.0.4/carbondesign/locale/jv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5496 2022-06-29 20:17:53.000000 django-carbondesign-0.0.4/carbondesign/locale/jv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.136000 django-carbondesign-0.0.4/carbondesign/locale/su/
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.254000 django-carbondesign-0.0.4/carbondesign/locale/su/LC_MESSAGES/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      337 2022-04-21 07:16:30.000000 django-carbondesign-0.0.4/carbondesign/locale/su/LC_MESSAGES/django.mo
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5492 2022-04-21 11:52:43.000000 django-carbondesign-0.0.4/carbondesign/locale/su/LC_MESSAGES/django.po
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      337 2022-06-29 20:17:53.000000 django-carbondesign-0.0.4/carbondesign/locale/su/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5496 2022-06-29 20:17:53.000000 django-carbondesign-0.0.4/carbondesign/locale/su/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.427000 django-carbondesign-0.0.4/carbondesign/mithril-js/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2040 2022-06-29 20:44:24.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/accordion.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    14413 2022-06-30 10:36:50.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/base.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1355 2022-06-29 20:45:38.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/breadcrumb.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2775 2022-06-29 20:44:15.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/button.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1429 2022-04-09 02:41:50.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/checkbox.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4462 2022-06-29 20:44:31.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/code_snippet.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6095 2022-04-09 02:41:58.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/combo_box.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1242 2022-04-09 02:42:01.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/content_switcher.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1109 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/copy_button.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    23339 2022-06-30 10:19:52.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/data-table.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    14048 2022-04-09 02:42:15.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/date_picker.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8803 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/dropdown.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7869 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/file_uploader.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3112 2022-06-29 20:45:04.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/grid.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      767 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/hidden_input.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3379 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/inline_loading.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      806 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/link.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1124 2022-06-29 20:45:15.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/list.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8120 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/list_box.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1496 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/loading.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       68 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/messages.json
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4639 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/modal.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6964 2022-03-24 10:36:20.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/multi_select.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7245 2022-06-29 20:46:36.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/notification.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5870 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/number_input.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3050 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/overflow_menu.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7445 2022-06-30 06:11:02.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/pagination.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4422 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/pagination_nav.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4450 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/progress_indicator.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2097 2022-03-24 10:36:20.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/radio_button.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2492 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/search.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7736 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/select.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2433 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/slider.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4565 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/structured_list.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3236 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/tabs.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1425 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/tag.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2491 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/text_area.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6443 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/text_input.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3679 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/tile.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4883 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/time_picker.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8491 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/timezones.json
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2579 2022-03-16 09:09:53.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/toggle.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6344 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/toolbar.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3663 2022-06-29 20:46:17.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/tooltip.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      985 2022-06-29 20:46:06.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/uishell--action.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7835 2022-06-29 20:44:43.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/uishell--switcher.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    17704 2022-06-29 20:46:00.000000 django-carbondesign-0.0.4/carbondesign/mithril-js/uishell.js
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.488000 django-carbondesign-0.0.4/carbondesign/sass/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       58 2021-12-15 16:33:07.000000 django-carbondesign-0.0.4/carbondesign/sass/_button.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       62 2021-12-15 16:33:25.000000 django-carbondesign-0.0.4/carbondesign/sass/_checkbox.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       78 2022-04-15 15:56:55.000000 django-carbondesign-0.0.4/carbondesign/sass/_content-switcher.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       72 2021-12-15 16:32:59.000000 django-carbondesign-0.0.4/carbondesign/sass/_data-table.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      134 2022-02-28 15:17:08.000000 django-carbondesign-0.0.4/carbondesign/sass/_date-picker.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       72 2022-03-05 11:12:19.000000 django-carbondesign-0.0.4/carbondesign/sass/_file-uploader.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      105 2022-03-05 12:29:15.000000 django-carbondesign-0.0.4/carbondesign/sass/_link.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       54 2022-03-01 21:05:44.000000 django-carbondesign-0.0.4/carbondesign/sass/_menu.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      182 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/sass/_modal.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      307 2022-03-10 13:02:27.000000 django-carbondesign-0.0.4/carbondesign/sass/_notification.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       72 2022-03-01 21:02:32.000000 django-carbondesign-0.0.4/carbondesign/sass/_overflow-menu.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       54 2022-04-15 15:57:26.000000 django-carbondesign-0.0.4/carbondesign/sass/_tabs.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       64 2021-12-17 00:35:09.000000 django-carbondesign-0.0.4/carbondesign/sass/_text-area.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       66 2021-12-15 16:33:34.000000 django-carbondesign-0.0.4/carbondesign/sass/_text-input.scss
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      444 2022-04-15 11:22:43.000000 django-carbondesign-0.0.4/carbondesign/sass/_ui-shell.scss
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.140000 django-carbondesign-0.0.4/carbondesign/static/
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.543000 django-carbondesign-0.0.4/carbondesign/static/carbondesign/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   670395 2022-03-10 13:02:27.000000 django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.css
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   234814 2022-03-10 13:02:27.000000 django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.css.map
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   437817 2022-03-10 13:02:27.000000 django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.js
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   579562 2022-03-10 13:02:27.000000 django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.min.css
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   192658 2022-03-10 13:02:27.000000 django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.min.css.map
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   165492 2022-03-10 13:02:27.000000 django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.min.js
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.744000 django-carbondesign-0.0.4/carbondesign/tags/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-02-11 01:28:54.000000 django-carbondesign-0.0.4/carbondesign/tags/__init__.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3117 2022-06-29 20:34:26.000000 django-carbondesign-0.0.4/carbondesign/tags/accordion.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    28562 2022-06-30 10:21:53.000000 django-carbondesign-0.0.4/carbondesign/tags/base.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      841 2022-04-20 06:38:35.000000 django-carbondesign-0.0.4/carbondesign/tags/base_widgets.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2460 2022-06-29 20:35:08.000000 django-carbondesign-0.0.4/carbondesign/tags/breadcrumb.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3947 2022-06-29 20:35:33.000000 django-carbondesign-0.0.4/carbondesign/tags/button.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2361 2022-04-20 06:22:36.000000 django-carbondesign-0.0.4/carbondesign/tags/checkbox.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4267 2022-06-29 20:38:32.000000 django-carbondesign-0.0.4/carbondesign/tags/code_snippet.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6511 2022-04-20 06:23:29.000000 django-carbondesign-0.0.4/carbondesign/tags/combo_box.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2368 2022-06-29 20:36:22.000000 django-carbondesign-0.0.4/carbondesign/tags/content_switcher.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1255 2022-03-24 10:36:20.000000 django-carbondesign-0.0.4/carbondesign/tags/copy_button.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    23827 2022-06-30 09:56:39.000000 django-carbondesign-0.0.4/carbondesign/tags/data_table.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    11600 2022-03-24 10:36:20.000000 django-carbondesign-0.0.4/carbondesign/tags/date_picker.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7986 2022-04-20 06:26:16.000000 django-carbondesign-0.0.4/carbondesign/tags/dropdown.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7244 2022-04-20 06:26:58.000000 django-carbondesign-0.0.4/carbondesign/tags/file_uploader.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4114 2022-06-29 20:37:57.000000 django-carbondesign-0.0.4/carbondesign/tags/grid.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3200 2022-03-24 10:36:20.000000 django-carbondesign-0.0.4/carbondesign/tags/inline_loading.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1874 2022-06-29 20:37:07.000000 django-carbondesign-0.0.4/carbondesign/tags/link.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1958 2022-06-29 20:33:10.000000 django-carbondesign-0.0.4/carbondesign/tags/list_.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7160 2022-04-20 06:27:31.000000 django-carbondesign-0.0.4/carbondesign/tags/list_box.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2378 2022-03-24 10:36:20.000000 django-carbondesign-0.0.4/carbondesign/tags/loading.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5445 2022-04-07 10:29:44.000000 django-carbondesign-0.0.4/carbondesign/tags/modal.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7589 2022-04-20 06:28:43.000000 django-carbondesign-0.0.4/carbondesign/tags/multi_select.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8586 2022-06-29 20:31:41.000000 django-carbondesign-0.0.4/carbondesign/tags/notification.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5777 2022-04-20 06:29:06.000000 django-carbondesign-0.0.4/carbondesign/tags/number_input.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5179 2022-06-29 20:36:04.000000 django-carbondesign-0.0.4/carbondesign/tags/overflow_menu.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7563 2022-06-30 06:11:15.000000 django-carbondesign-0.0.4/carbondesign/tags/pagination.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8483 2022-04-07 10:29:44.000000 django-carbondesign-0.0.4/carbondesign/tags/pagination_nav.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5417 2022-04-07 10:29:44.000000 django-carbondesign-0.0.4/carbondesign/tags/progress_indicator.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2968 2022-04-20 06:29:45.000000 django-carbondesign-0.0.4/carbondesign/tags/radio_button.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3100 2022-04-20 06:30:04.000000 django-carbondesign-0.0.4/carbondesign/tags/search.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7196 2022-04-15 19:08:09.000000 django-carbondesign-0.0.4/carbondesign/tags/select.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3101 2022-04-07 10:29:44.000000 django-carbondesign-0.0.4/carbondesign/tags/slider.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5790 2022-04-07 10:29:44.000000 django-carbondesign-0.0.4/carbondesign/tags/structured_list.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4053 2022-04-07 10:29:44.000000 django-carbondesign-0.0.4/carbondesign/tags/tabs.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2025 2022-04-07 10:29:44.000000 django-carbondesign-0.0.4/carbondesign/tags/tag.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2717 2022-04-09 00:11:40.000000 django-carbondesign-0.0.4/carbondesign/tags/text_area.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6811 2022-04-09 00:15:57.000000 django-carbondesign-0.0.4/carbondesign/tags/text_input.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5895 2022-04-20 06:37:46.000000 django-carbondesign-0.0.4/carbondesign/tags/tile.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5479 2022-04-09 00:10:50.000000 django-carbondesign-0.0.4/carbondesign/tags/time_picker.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2824 2022-04-20 06:32:18.000000 django-carbondesign-0.0.4/carbondesign/tags/toggle.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8141 2022-06-29 20:34:45.000000 django-carbondesign-0.0.4/carbondesign/tags/toolbar.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6148 2022-04-20 06:33:47.000000 django-carbondesign-0.0.4/carbondesign/tags/tooltip.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    19865 2022-06-29 20:34:08.000000 django-carbondesign-0.0.4/carbondesign/tags/ui_shell.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     9223 2022-06-29 20:32:34.000000 django-carbondesign-0.0.4/carbondesign/tags/ui_shell_switcher.py
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.767000 django-carbondesign-0.0.4/carbondesign/templatetags/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-02-11 01:28:54.000000 django-carbondesign-0.0.4/carbondesign/templatetags/__init__.py
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4217 2022-04-15 14:21:37.000000 django-carbondesign-0.0.4/carbondesign/templatetags/carbondesign.py
-drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-06-30 10:40:12.781000 django-carbondesign-0.0.4/django_carbondesign.egg-info/
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1248 2022-06-30 10:40:07.000000 django-carbondesign-0.0.4/django_carbondesign.egg-info/PKG-INFO
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5435 2022-06-30 10:40:11.000000 django-carbondesign-0.0.4/django_carbondesign.egg-info/SOURCES.txt
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)        1 2022-06-30 10:40:07.000000 django-carbondesign-0.0.4/django_carbondesign.egg-info/dependency_links.txt
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       17 2022-06-30 10:40:10.000000 django-carbondesign-0.0.4/django_carbondesign.egg-info/requires.txt
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       13 2022-06-30 10:40:10.000000 django-carbondesign-0.0.4/django_carbondesign.egg-info/top_level.txt
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      114 2022-02-11 01:28:54.000000 django-carbondesign-0.0.4/pyproject.toml
--rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      798 2022-06-30 10:40:12.788000 django-carbondesign-0.0.4/setup.cfg
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:36.232824 django-carbondesign-0.0.5/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1067 2022-02-11 01:28:54.000000 django-carbondesign-0.0.5/LICENSE
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1248 2023-04-09 21:54:36.233825 django-carbondesign-0.0.5/PKG-INFO
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      513 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/README.rst
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.917825 django-carbondesign-0.0.5/carbondesign/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      513 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/README.rst
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-03 00:07:01.000000 django-carbondesign-0.0.5/carbondesign/__init__.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      223 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/apps.py
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.923824 django-carbondesign-0.0.5/carbondesign/forms-js/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1002 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/forms-js/fields.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3840 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/forms-js/forms.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1422 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/forms-js/widgets.js
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.946824 django-carbondesign-0.0.5/carbondesign/js/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      126 2021-12-15 08:31:13.000000 django-carbondesign-0.0.5/carbondesign/js/checkbox.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      269 2022-04-15 16:07:50.000000 django-carbondesign-0.0.5/carbondesign/js/content-switcher.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      138 2021-12-15 16:43:45.000000 django-carbondesign-0.0.5/carbondesign/js/data-table.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      420 2023-04-09 01:16:30.000000 django-carbondesign-0.0.5/carbondesign/js/date-picker.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      144 2022-03-05 11:11:46.000000 django-carbondesign-0.0.5/carbondesign/js/file-uploader.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      202 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/js/modal.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      142 2022-03-10 13:02:27.000000 django-carbondesign-0.0.5/carbondesign/js/notification.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      144 2022-03-01 21:03:23.000000 django-carbondesign-0.0.5/carbondesign/js/overflow-menu.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1097 2022-04-08 14:41:24.000000 django-carbondesign-0.0.5/carbondesign/js/pagination.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      220 2022-04-15 12:40:11.000000 django-carbondesign-0.0.5/carbondesign/js/tabs.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      132 2021-12-15 08:28:00.000000 django-carbondesign-0.0.5/carbondesign/js/text-input.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      834 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/js/ui-shell.js
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.899824 django-carbondesign-0.0.5/carbondesign/locale/
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.897824 django-carbondesign-0.0.5/carbondesign/locale/id/
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.955824 django-carbondesign-0.0.5/carbondesign/locale/id/LC_MESSAGES/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3251 2023-04-09 20:37:17.000000 django-carbondesign-0.0.5/carbondesign/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6319 2023-04-09 20:37:08.000000 django-carbondesign-0.0.5/carbondesign/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3221 2023-04-09 12:21:57.000000 django-carbondesign-0.0.5/carbondesign/locale/id/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6452 2023-04-09 12:21:30.000000 django-carbondesign-0.0.5/carbondesign/locale/id/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.898825 django-carbondesign-0.0.5/carbondesign/locale/jv/
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.964825 django-carbondesign-0.0.5/carbondesign/locale/jv/LC_MESSAGES/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      337 2023-04-09 20:37:17.000000 django-carbondesign-0.0.5/carbondesign/locale/jv/LC_MESSAGES/django.mo
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5346 2023-04-09 20:37:08.000000 django-carbondesign-0.0.5/carbondesign/locale/jv/LC_MESSAGES/django.po
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      337 2023-04-03 05:14:53.000000 django-carbondesign-0.0.5/carbondesign/locale/jv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5628 2023-04-02 18:57:49.000000 django-carbondesign-0.0.5/carbondesign/locale/jv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.900824 django-carbondesign-0.0.5/carbondesign/locale/su/
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.972824 django-carbondesign-0.0.5/carbondesign/locale/su/LC_MESSAGES/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      337 2023-04-09 20:37:17.000000 django-carbondesign-0.0.5/carbondesign/locale/su/LC_MESSAGES/django.mo
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5346 2023-04-09 20:37:08.000000 django-carbondesign-0.0.5/carbondesign/locale/su/LC_MESSAGES/django.po
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      337 2023-04-03 05:14:53.000000 django-carbondesign-0.0.5/carbondesign/locale/su/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5628 2023-04-02 18:57:49.000000 django-carbondesign-0.0.5/carbondesign/locale/su/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:36.065825 django-carbondesign-0.0.5/carbondesign/mithril-js/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2040 2022-06-29 20:44:24.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/accordion.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    14445 2023-04-09 12:13:01.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/base.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1355 2022-06-29 20:45:38.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/breadcrumb.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2775 2022-06-29 20:44:15.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/button.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1429 2022-04-09 02:41:50.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/checkbox.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4462 2022-06-29 20:44:31.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/code_snippet.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6095 2022-04-09 02:41:58.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/combo_box.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1242 2022-04-09 02:42:01.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/content_switcher.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1109 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/copy_button.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    23340 2022-06-30 10:44:33.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/data-table.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    15471 2023-04-08 23:17:33.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/date_picker.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8803 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/dropdown.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7869 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/file_uploader.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3112 2022-06-29 20:45:04.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/grid.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      767 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/hidden_input.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3379 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/inline_loading.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      806 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/link.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1124 2022-06-29 20:45:15.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/list.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8120 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/list_box.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1496 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/loading.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       68 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/messages.json
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4639 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/modal.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6964 2022-03-24 10:36:20.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/multi_select.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7245 2022-06-29 20:46:36.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/notification.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5870 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/number_input.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3050 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/overflow_menu.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7445 2022-06-30 06:11:02.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/pagination.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4422 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/pagination_nav.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4450 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/progress_indicator.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2097 2022-03-24 10:36:20.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/radio_button.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2492 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/search.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7704 2023-04-09 10:26:30.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/select.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2433 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/slider.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4565 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/structured_list.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3236 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/tabs.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1425 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/tag.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2491 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/text_area.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6443 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/text_input.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3679 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/tile.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8825 2023-04-09 12:15:37.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/time_picker.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2579 2022-03-16 09:09:53.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/toggle.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6344 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/toolbar.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3663 2022-06-29 20:46:17.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/tooltip.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      985 2022-06-29 20:46:06.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/uishell--action.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7835 2022-06-29 20:44:43.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/uishell--switcher.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    17704 2022-06-29 20:46:00.000000 django-carbondesign-0.0.5/carbondesign/mithril-js/uishell.js
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:36.095825 django-carbondesign-0.0.5/carbondesign/sass/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       58 2021-12-15 16:33:07.000000 django-carbondesign-0.0.5/carbondesign/sass/_button.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       62 2021-12-15 16:33:25.000000 django-carbondesign-0.0.5/carbondesign/sass/_checkbox.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       78 2022-04-15 15:56:55.000000 django-carbondesign-0.0.5/carbondesign/sass/_content-switcher.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       72 2021-12-15 16:32:59.000000 django-carbondesign-0.0.5/carbondesign/sass/_data-table.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      134 2022-02-28 15:17:08.000000 django-carbondesign-0.0.5/carbondesign/sass/_date-picker.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       72 2022-03-05 11:12:19.000000 django-carbondesign-0.0.5/carbondesign/sass/_file-uploader.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      105 2022-03-05 12:29:15.000000 django-carbondesign-0.0.5/carbondesign/sass/_link.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       54 2022-03-01 21:05:44.000000 django-carbondesign-0.0.5/carbondesign/sass/_menu.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      182 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/sass/_modal.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      307 2022-03-10 13:02:27.000000 django-carbondesign-0.0.5/carbondesign/sass/_notification.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       72 2022-03-01 21:02:32.000000 django-carbondesign-0.0.5/carbondesign/sass/_overflow-menu.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       54 2022-04-15 15:57:26.000000 django-carbondesign-0.0.5/carbondesign/sass/_tabs.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       64 2021-12-17 00:35:09.000000 django-carbondesign-0.0.5/carbondesign/sass/_text-area.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       66 2021-12-15 16:33:34.000000 django-carbondesign-0.0.5/carbondesign/sass/_text-input.scss
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      444 2022-04-15 11:22:43.000000 django-carbondesign-0.0.5/carbondesign/sass/_ui-shell.scss
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:35.902824 django-carbondesign-0.0.5/carbondesign/static/
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:36.132825 django-carbondesign-0.0.5/carbondesign/static/carbondesign/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   670395 2022-03-10 13:02:27.000000 django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.css
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   234814 2022-03-10 13:02:27.000000 django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.css.map
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   437817 2022-03-10 13:02:27.000000 django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.js
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   579562 2022-03-10 13:02:27.000000 django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.min.css
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   192658 2022-03-10 13:02:27.000000 django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.min.css.map
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)   165492 2022-03-10 13:02:27.000000 django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.min.js
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:36.213825 django-carbondesign-0.0.5/carbondesign/tags/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-02-11 01:28:54.000000 django-carbondesign-0.0.5/carbondesign/tags/__init__.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3117 2022-06-29 20:34:26.000000 django-carbondesign-0.0.5/carbondesign/tags/accordion.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    28884 2023-04-09 10:08:02.000000 django-carbondesign-0.0.5/carbondesign/tags/base.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      841 2022-04-20 06:38:35.000000 django-carbondesign-0.0.5/carbondesign/tags/base_widgets.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2460 2022-06-29 20:35:08.000000 django-carbondesign-0.0.5/carbondesign/tags/breadcrumb.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3943 2023-04-02 23:55:48.000000 django-carbondesign-0.0.5/carbondesign/tags/button.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2361 2022-04-20 06:22:36.000000 django-carbondesign-0.0.5/carbondesign/tags/checkbox.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4267 2022-06-29 20:38:32.000000 django-carbondesign-0.0.5/carbondesign/tags/code_snippet.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6511 2022-04-20 06:23:29.000000 django-carbondesign-0.0.5/carbondesign/tags/combo_box.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2368 2022-06-29 20:36:22.000000 django-carbondesign-0.0.5/carbondesign/tags/content_switcher.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1255 2022-03-24 10:36:20.000000 django-carbondesign-0.0.5/carbondesign/tags/copy_button.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    23864 2023-04-02 23:55:23.000000 django-carbondesign-0.0.5/carbondesign/tags/data_table.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    13028 2023-04-09 20:36:44.000000 django-carbondesign-0.0.5/carbondesign/tags/date_picker.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7976 2023-04-02 23:53:36.000000 django-carbondesign-0.0.5/carbondesign/tags/dropdown.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7244 2022-04-20 06:26:58.000000 django-carbondesign-0.0.5/carbondesign/tags/file_uploader.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3873 2023-04-07 22:14:22.000000 django-carbondesign-0.0.5/carbondesign/tags/grid.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3200 2022-03-24 10:36:20.000000 django-carbondesign-0.0.5/carbondesign/tags/inline_loading.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1874 2022-06-29 20:37:07.000000 django-carbondesign-0.0.5/carbondesign/tags/link.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1958 2022-06-29 20:33:10.000000 django-carbondesign-0.0.5/carbondesign/tags/list_.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7160 2022-04-20 06:27:31.000000 django-carbondesign-0.0.5/carbondesign/tags/list_box.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2378 2022-03-24 10:36:20.000000 django-carbondesign-0.0.5/carbondesign/tags/loading.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5445 2022-04-07 10:29:44.000000 django-carbondesign-0.0.5/carbondesign/tags/modal.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7583 2023-04-07 13:44:09.000000 django-carbondesign-0.0.5/carbondesign/tags/multi_select.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8586 2022-06-29 20:31:41.000000 django-carbondesign-0.0.5/carbondesign/tags/notification.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5777 2022-04-20 06:29:06.000000 django-carbondesign-0.0.5/carbondesign/tags/number_input.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5179 2022-06-29 20:36:04.000000 django-carbondesign-0.0.5/carbondesign/tags/overflow_menu.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7563 2022-06-30 06:11:15.000000 django-carbondesign-0.0.5/carbondesign/tags/pagination.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8483 2023-04-07 13:43:41.000000 django-carbondesign-0.0.5/carbondesign/tags/pagination_nav.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5417 2022-04-07 10:29:44.000000 django-carbondesign-0.0.5/carbondesign/tags/progress_indicator.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2962 2023-04-07 13:43:50.000000 django-carbondesign-0.0.5/carbondesign/tags/radio_button.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3100 2022-04-20 06:30:04.000000 django-carbondesign-0.0.5/carbondesign/tags/search.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     7164 2023-04-09 10:27:09.000000 django-carbondesign-0.0.5/carbondesign/tags/select.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     3101 2022-04-07 10:29:44.000000 django-carbondesign-0.0.5/carbondesign/tags/slider.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5790 2022-04-07 10:29:44.000000 django-carbondesign-0.0.5/carbondesign/tags/structured_list.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4053 2022-04-07 10:29:44.000000 django-carbondesign-0.0.5/carbondesign/tags/tabs.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2025 2022-04-07 10:29:44.000000 django-carbondesign-0.0.5/carbondesign/tags/tag.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2717 2022-04-09 00:11:40.000000 django-carbondesign-0.0.5/carbondesign/tags/text_area.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6811 2022-04-09 00:15:57.000000 django-carbondesign-0.0.5/carbondesign/tags/text_input.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5895 2022-04-20 06:37:46.000000 django-carbondesign-0.0.5/carbondesign/tags/tile.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8997 2023-04-09 12:29:27.000000 django-carbondesign-0.0.5/carbondesign/tags/time_picker.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2824 2022-04-20 06:32:18.000000 django-carbondesign-0.0.5/carbondesign/tags/toggle.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     8119 2023-04-07 13:43:59.000000 django-carbondesign-0.0.5/carbondesign/tags/toolbar.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     6138 2023-04-02 19:11:08.000000 django-carbondesign-0.0.5/carbondesign/tags/tooltip.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)    19888 2023-04-02 09:06:59.000000 django-carbondesign-0.0.5/carbondesign/tags/ui_shell.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     9223 2023-04-02 08:38:11.000000 django-carbondesign-0.0.5/carbondesign/tags/ui_shell_switcher.py
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:36.217825 django-carbondesign-0.0.5/carbondesign/templatetags/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2022-02-11 01:28:54.000000 django-carbondesign-0.0.5/carbondesign/templatetags/__init__.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     4217 2022-04-15 14:21:37.000000 django-carbondesign-0.0.5/carbondesign/templatetags/carbondesign.py
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:36.220825 django-carbondesign-0.0.5/carbondesign/utils/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 19:12:18.000000 django-carbondesign-0.0.5/carbondesign/utils/__init__.py
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     2389 2023-04-09 19:40:05.000000 django-carbondesign-0.0.5/carbondesign/utils/formats.py
+drwxr-xr-x   0 dozymoe  (1000000001) dozymoe  (1000000001)        0 2023-04-09 21:54:36.231824 django-carbondesign-0.0.5/django_carbondesign.egg-info/
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     1248 2023-04-09 21:54:35.000000 django-carbondesign-0.0.5/django_carbondesign.egg-info/PKG-INFO
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)     5457 2023-04-09 21:54:35.000000 django-carbondesign-0.0.5/django_carbondesign.egg-info/SOURCES.txt
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)        1 2023-04-09 21:54:35.000000 django-carbondesign-0.0.5/django_carbondesign.egg-info/dependency_links.txt
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       17 2023-04-09 21:54:35.000000 django-carbondesign-0.0.5/django_carbondesign.egg-info/requires.txt
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)       13 2023-04-09 21:54:35.000000 django-carbondesign-0.0.5/django_carbondesign.egg-info/top_level.txt
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      114 2022-02-11 01:28:54.000000 django-carbondesign-0.0.5/pyproject.toml
+-rw-r--r--   0 dozymoe  (1000000001) dozymoe  (1000000001)      798 2023-04-09 21:54:36.234825 django-carbondesign-0.0.5/setup.cfg
```

### Comparing `django-carbondesign-0.0.4/LICENSE` & `django-carbondesign-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/PKG-INFO` & `django-carbondesign-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-carbondesign
-Version: 0.0.4
+Version: 0.0.5
 Summary: Carbon Design in Django templates
 Home-page: https://github.com/dozymoe/django-carbondesign
 Author: Fahri Reza
 Author-email: i@dozy.moe
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dozymoe/django-carbondesign/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-carbondesign-0.0.4/README.rst` & `django-carbondesign-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/README.rst` & `django-carbondesign-0.0.5/carbondesign/README.rst`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/forms-js/fields.js` & `django-carbondesign-0.0.5/carbondesign/forms-js/fields.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/forms-js/forms.js` & `django-carbondesign-0.0.5/carbondesign/forms-js/forms.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/forms-js/widgets.js` & `django-carbondesign-0.0.5/carbondesign/forms-js/widgets.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/js/pagination.js` & `django-carbondesign-0.0.5/carbondesign/js/pagination.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/js/ui-shell.js` & `django-carbondesign-0.0.5/carbondesign/js/ui-shell.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/locale/id/LC_MESSAGES/django.mo` & `django-carbondesign-0.0.5/carbondesign/locale/id/LC_MESSAGES/djangojs.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,20 +7,14 @@
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-msgid "Argument {prop} for template tag is required."
-msgstr "Argumen {prop} harus diset untuk template tag."
-
-msgid "Cancel"
-msgstr "Batal"
-
 msgid "Choose an option"
 msgstr "Pilih satu"
 
 msgid "Clear all"
 msgstr "Hapus bersih"
 
 msgid "Clear all selected items"
@@ -73,17 +67,14 @@
 
 msgid "Next page"
 msgstr "Halaman berikutnya"
 
 msgid "Off"
 msgstr "Mati"
 
-msgid "On"
-msgstr "Menyala"
-
 msgid "Open menu"
 msgstr "Buka menu"
 
 msgid "Overflow"
 msgstr "Luapan"
 
 msgid "Previous page"
@@ -145,36 +136,42 @@
 
 msgid "decrease number input"
 msgstr "kurangi"
 
 msgid "increase number input"
 msgstr "tambah"
 
+msgid "items"
+msgstr "total"
+
 msgid "items selected"
 msgstr "baris dipilih"
 
 msgid "next page"
 msgstr "halaman berikutnya"
 
-msgid "of {total} pages"
-msgstr "dari {total} halaman"
+msgid "of"
+msgstr "dari"
+
+msgid "of %(total)s pages"
+msgstr "dari %(total)s halaman"
+
+msgid "on"
+msgstr "menyala"
 
 msgid "page"
 msgstr "halaman"
 
+msgid "pagination"
+msgstr "paginasi"
+
 msgid "previous page"
 msgstr "halaman sebelumnya"
 
 msgid "select number of items per page"
 msgstr "pilih jumlah baris per halaman"
 
-msgid "select page number"
-msgstr "pilih halaman"
-
 msgid "select page number to view"
-msgstr "pilih halaman untuk ditampilkan"
+msgstr "pilihan halaman untuk ditampilkan"
 
 msgid "tile"
 msgstr "ubin"
-
-msgid "{range} of {total} items"
-msgstr "{range} dari {total} baris"
```

### Comparing `django-carbondesign-0.0.4/carbondesign/locale/id/LC_MESSAGES/django.po` & `django-carbondesign-0.0.5/carbondesign/locale/id/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-16 02:28+0700\n"
+"POT-Creation-Date: 2023-04-10 03:35+0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: carbondesign/tags/base.py:209
+#: carbondesign/tags/base.py:223
 #, python-brace-format
 msgid "Argument {prop} for template tag is required."
 msgstr "Argumen {prop} harus diset untuk template tag."
 
 #: carbondesign/tags/breadcrumb.py:36
 msgid "breadcrumb"
 msgstr "remahan"
@@ -193,15 +193,15 @@
 msgid "page"
 msgstr "halaman"
 
 #: carbondesign/tags/pagination_nav.py:97
 msgid "select page number"
 msgstr "pilih halaman"
 
-#: carbondesign/tags/select.py:37
+#: carbondesign/tags/select.py:35
 msgid "Choose an option"
 msgstr "Pilih satu"
 
 #: carbondesign/tags/slider.py:42
 msgid "slider"
 msgstr ""
 
@@ -213,22 +213,14 @@
 msgid "Show password"
 msgstr "Tampilkan kata kunci"
 
 #: carbondesign/tags/tile.py:40
 msgid "tile"
 msgstr "ubin"
 
-#: carbondesign/tags/time_picker.py:26
-msgid "Select AM/PM"
-msgstr "Pilih sebelum/sesudah siang"
-
-#: carbondesign/tags/time_picker.py:27
-msgid "Select time zone"
-msgstr "Pilih zona waktu"
-
 #: carbondesign/tags/toggle.py:34
 msgid "Off"
 msgstr "Mati"
 
 #: carbondesign/tags/toggle.py:35
 msgid "On"
 msgstr "Menyala"
@@ -256,7 +248,13 @@
 #: carbondesign/tags/ui_shell.py:419
 msgid "Toggle the expansion state of the navigation"
 msgstr "Buka tutup navigasi"
 
 #: carbondesign/tags/ui_shell.py:497
 msgid "Switcher"
 msgstr "Penampil"
+
+#~ msgid "Select AM/PM"
+#~ msgstr "Pilih sebelum/sesudah siang"
+
+#~ msgid "Select time zone"
+#~ msgstr "Pilih zona waktu"
```

### Comparing `django-carbondesign-0.0.4/carbondesign/locale/id/LC_MESSAGES/djangojs.po` & `django-carbondesign-0.0.5/carbondesign/locale/id/LC_MESSAGES/djangojs.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-14 14:05+0700\n"
+"POT-Creation-Date: 2023-04-02 15:06+0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -39,15 +39,15 @@
 msgstr "Tampilkan tambahan icon"
 
 #: carbondesign/mithril-js/code_snippet.js:16
 msgid "Show less"
 msgstr "Kurangi tampilan"
 
 #: carbondesign/mithril-js/combo_box.js:12
-#: carbondesign/mithril-js/data-table.js:607
+#: carbondesign/mithril-js/data-table.js:600
 #: carbondesign/mithril-js/list_box.js:13
 #: carbondesign/mithril-js/multi_select.js:12
 #: carbondesign/mithril-js/uishell.js:17
 msgid "Open menu"
 msgstr "Buka menu"
 
 #: carbondesign/mithril-js/combo_box.js:13
@@ -63,21 +63,21 @@
 msgstr "baris dipilih"
 
 #: carbondesign/mithril-js/data-table.js:24
 #: carbondesign/mithril-js/overflow_menu.js:13
 msgid "Overflow"
 msgstr "Luapan"
 
-#: carbondesign/mithril-js/data-table.js:803
+#: carbondesign/mithril-js/data-table.js:794
 #: carbondesign/mithril-js/search.js:15 carbondesign/mithril-js/toolbar.js:34
 #: carbondesign/mithril-js/uishell--switcher.js:124
 msgid "Search"
 msgstr "Pencarian"
 
-#: carbondesign/mithril-js/data-table.js:804
+#: carbondesign/mithril-js/data-table.js:795
 #: carbondesign/mithril-js/search.js:12 carbondesign/mithril-js/toolbar.js:31
 #: carbondesign/mithril-js/uishell--switcher.js:118
 msgid "Clear search input"
 msgstr "Bersihkan pencarian"
 
 #: carbondesign/mithril-js/file_uploader.js:9
 msgid "Drag and drop files here or upload"
@@ -141,41 +141,49 @@
 msgid "increase number input"
 msgstr "tambah"
 
 #: carbondesign/mithril-js/number_input.js:13
 msgid "decrease number input"
 msgstr "kurangi"
 
-#: carbondesign/mithril-js/pagination.js:15
+#: carbondesign/mithril-js/pagination.js:19
 msgid "Items per page"
 msgstr "Baris per halaman"
 
-#: carbondesign/mithril-js/pagination.js:16
+#: carbondesign/mithril-js/pagination.js:20
 msgid "select number of items per page"
 msgstr "pilih jumlah baris per halaman"
 
-#: carbondesign/mithril-js/pagination.js:17
+#: carbondesign/mithril-js/pagination.js:21
 msgid "select page number to view"
 msgstr "pilihan halaman untuk ditampilkan"
 
-#: carbondesign/mithril-js/pagination.js:18
-msgid "Backward button"
-msgstr "Tombol mundur"
-
-#: carbondesign/mithril-js/pagination.js:19
-msgid "Forward button"
-msgstr "Tombol maju"
-
-#: carbondesign/mithril-js/pagination.js:250
-msgid "of {total} pages"
-msgstr " dari {total} halaman"
+#: carbondesign/mithril-js/pagination.js:22
+msgid "previous page"
+msgstr "halaman sebelumnya"
+
+#: carbondesign/mithril-js/pagination.js:23
+msgid "next page"
+msgstr "halaman berikutnya"
+
+#: carbondesign/mithril-js/pagination.js:255
+msgid "of"
+msgstr "dari"
+
+#: carbondesign/mithril-js/pagination.js:261
+msgid "items"
+msgstr "total"
+
+#: carbondesign/mithril-js/pagination.js:269
+msgid "of %(total)s pages"
+msgstr "dari %(total)s halaman"
 
 #: carbondesign/mithril-js/pagination_nav.js:11
 msgid "pagination"
-msgstr ""
+msgstr "paginasi"
 
 #: carbondesign/mithril-js/pagination_nav.js:12
 msgid "Previous page"
 msgstr "Halaman sebelumnya"
 
 #: carbondesign/mithril-js/pagination_nav.js:13
 msgid "Next page"
```

### Comparing `django-carbondesign-0.0.4/carbondesign/locale/jv/LC_MESSAGES/django.po` & `django-carbondesign-0.0.5/carbondesign/locale/jv/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-20 19:26+0700\n"
+"POT-Creation-Date: 2023-04-10 03:35+0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: carbondesign/tags/base.py:209
+#: carbondesign/tags/base.py:223
 #, python-brace-format
 msgid "Argument {prop} for template tag is required."
 msgstr ""
 
 #: carbondesign/tags/breadcrumb.py:36
 msgid "breadcrumb"
 msgstr ""
@@ -193,15 +193,15 @@
 msgid "page"
 msgstr ""
 
 #: carbondesign/tags/pagination_nav.py:97
 msgid "select page number"
 msgstr ""
 
-#: carbondesign/tags/select.py:37
+#: carbondesign/tags/select.py:35
 msgid "Choose an option"
 msgstr ""
 
 #: carbondesign/tags/slider.py:42
 msgid "slider"
 msgstr ""
 
@@ -213,22 +213,14 @@
 msgid "Show password"
 msgstr ""
 
 #: carbondesign/tags/tile.py:40
 msgid "tile"
 msgstr ""
 
-#: carbondesign/tags/time_picker.py:26
-msgid "Select AM/PM"
-msgstr ""
-
-#: carbondesign/tags/time_picker.py:27
-msgid "Select time zone"
-msgstr ""
-
 #: carbondesign/tags/toggle.py:34
 msgid "Off"
 msgstr ""
 
 #: carbondesign/tags/toggle.py:35
 msgid "On"
 msgstr ""
```

### Comparing `django-carbondesign-0.0.4/carbondesign/locale/jv/LC_MESSAGES/djangojs.po` & `django-carbondesign-0.0.5/carbondesign/locale/jv/LC_MESSAGES/djangojs.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-04 16:17+0700\n"
+"POT-Creation-Date: 2023-04-02 15:06+0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -39,15 +39,15 @@
 msgstr ""
 
 #: carbondesign/mithril-js/code_snippet.js:16
 msgid "Show less"
 msgstr ""
 
 #: carbondesign/mithril-js/combo_box.js:12
-#: carbondesign/mithril-js/data-table.js:607
+#: carbondesign/mithril-js/data-table.js:600
 #: carbondesign/mithril-js/list_box.js:13
 #: carbondesign/mithril-js/multi_select.js:12
 #: carbondesign/mithril-js/uishell.js:17
 msgid "Open menu"
 msgstr ""
 
 #: carbondesign/mithril-js/combo_box.js:13
@@ -63,21 +63,21 @@
 msgstr ""
 
 #: carbondesign/mithril-js/data-table.js:24
 #: carbondesign/mithril-js/overflow_menu.js:13
 msgid "Overflow"
 msgstr ""
 
-#: carbondesign/mithril-js/data-table.js:803
+#: carbondesign/mithril-js/data-table.js:794
 #: carbondesign/mithril-js/search.js:15 carbondesign/mithril-js/toolbar.js:34
 #: carbondesign/mithril-js/uishell--switcher.js:124
 msgid "Search"
 msgstr ""
 
-#: carbondesign/mithril-js/data-table.js:804
+#: carbondesign/mithril-js/data-table.js:795
 #: carbondesign/mithril-js/search.js:12 carbondesign/mithril-js/toolbar.js:31
 #: carbondesign/mithril-js/uishell--switcher.js:118
 msgid "Clear search input"
 msgstr ""
 
 #: carbondesign/mithril-js/file_uploader.js:9
 msgid "Drag and drop files here or upload"
@@ -141,36 +141,44 @@
 msgid "increase number input"
 msgstr ""
 
 #: carbondesign/mithril-js/number_input.js:13
 msgid "decrease number input"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:15
+#: carbondesign/mithril-js/pagination.js:19
 msgid "Items per page"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:16
+#: carbondesign/mithril-js/pagination.js:20
 msgid "select number of items per page"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:17
+#: carbondesign/mithril-js/pagination.js:21
 msgid "select page number to view"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:18
-msgid "Backward button"
+#: carbondesign/mithril-js/pagination.js:22
+msgid "previous page"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:19
-msgid "Forward button"
+#: carbondesign/mithril-js/pagination.js:23
+msgid "next page"
+msgstr ""
+
+#: carbondesign/mithril-js/pagination.js:255
+msgid "of"
+msgstr ""
+
+#: carbondesign/mithril-js/pagination.js:261
+msgid "items"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:250
-msgid "of {total} pages"
+#: carbondesign/mithril-js/pagination.js:269
+msgid "of %(total)s pages"
 msgstr ""
 
 #: carbondesign/mithril-js/pagination_nav.js:11
 msgid "pagination"
 msgstr ""
 
 #: carbondesign/mithril-js/pagination_nav.js:12
```

### Comparing `django-carbondesign-0.0.4/carbondesign/locale/su/LC_MESSAGES/django.po` & `django-carbondesign-0.0.5/carbondesign/locale/su/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-20 19:26+0700\n"
+"POT-Creation-Date: 2023-04-10 03:35+0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: carbondesign/tags/base.py:209
+#: carbondesign/tags/base.py:223
 #, python-brace-format
 msgid "Argument {prop} for template tag is required."
 msgstr ""
 
 #: carbondesign/tags/breadcrumb.py:36
 msgid "breadcrumb"
 msgstr ""
@@ -193,15 +193,15 @@
 msgid "page"
 msgstr ""
 
 #: carbondesign/tags/pagination_nav.py:97
 msgid "select page number"
 msgstr ""
 
-#: carbondesign/tags/select.py:37
+#: carbondesign/tags/select.py:35
 msgid "Choose an option"
 msgstr ""
 
 #: carbondesign/tags/slider.py:42
 msgid "slider"
 msgstr ""
 
@@ -213,22 +213,14 @@
 msgid "Show password"
 msgstr ""
 
 #: carbondesign/tags/tile.py:40
 msgid "tile"
 msgstr ""
 
-#: carbondesign/tags/time_picker.py:26
-msgid "Select AM/PM"
-msgstr ""
-
-#: carbondesign/tags/time_picker.py:27
-msgid "Select time zone"
-msgstr ""
-
 #: carbondesign/tags/toggle.py:34
 msgid "Off"
 msgstr ""
 
 #: carbondesign/tags/toggle.py:35
 msgid "On"
 msgstr ""
```

### Comparing `django-carbondesign-0.0.4/carbondesign/locale/su/LC_MESSAGES/djangojs.po` & `django-carbondesign-0.0.5/carbondesign/locale/su/LC_MESSAGES/djangojs.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-04 16:17+0700\n"
+"POT-Creation-Date: 2023-04-02 15:06+0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -39,15 +39,15 @@
 msgstr ""
 
 #: carbondesign/mithril-js/code_snippet.js:16
 msgid "Show less"
 msgstr ""
 
 #: carbondesign/mithril-js/combo_box.js:12
-#: carbondesign/mithril-js/data-table.js:607
+#: carbondesign/mithril-js/data-table.js:600
 #: carbondesign/mithril-js/list_box.js:13
 #: carbondesign/mithril-js/multi_select.js:12
 #: carbondesign/mithril-js/uishell.js:17
 msgid "Open menu"
 msgstr ""
 
 #: carbondesign/mithril-js/combo_box.js:13
@@ -63,21 +63,21 @@
 msgstr ""
 
 #: carbondesign/mithril-js/data-table.js:24
 #: carbondesign/mithril-js/overflow_menu.js:13
 msgid "Overflow"
 msgstr ""
 
-#: carbondesign/mithril-js/data-table.js:803
+#: carbondesign/mithril-js/data-table.js:794
 #: carbondesign/mithril-js/search.js:15 carbondesign/mithril-js/toolbar.js:34
 #: carbondesign/mithril-js/uishell--switcher.js:124
 msgid "Search"
 msgstr ""
 
-#: carbondesign/mithril-js/data-table.js:804
+#: carbondesign/mithril-js/data-table.js:795
 #: carbondesign/mithril-js/search.js:12 carbondesign/mithril-js/toolbar.js:31
 #: carbondesign/mithril-js/uishell--switcher.js:118
 msgid "Clear search input"
 msgstr ""
 
 #: carbondesign/mithril-js/file_uploader.js:9
 msgid "Drag and drop files here or upload"
@@ -141,36 +141,44 @@
 msgid "increase number input"
 msgstr ""
 
 #: carbondesign/mithril-js/number_input.js:13
 msgid "decrease number input"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:15
+#: carbondesign/mithril-js/pagination.js:19
 msgid "Items per page"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:16
+#: carbondesign/mithril-js/pagination.js:20
 msgid "select number of items per page"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:17
+#: carbondesign/mithril-js/pagination.js:21
 msgid "select page number to view"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:18
-msgid "Backward button"
+#: carbondesign/mithril-js/pagination.js:22
+msgid "previous page"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:19
-msgid "Forward button"
+#: carbondesign/mithril-js/pagination.js:23
+msgid "next page"
+msgstr ""
+
+#: carbondesign/mithril-js/pagination.js:255
+msgid "of"
+msgstr ""
+
+#: carbondesign/mithril-js/pagination.js:261
+msgid "items"
 msgstr ""
 
-#: carbondesign/mithril-js/pagination.js:250
-msgid "of {total} pages"
+#: carbondesign/mithril-js/pagination.js:269
+msgid "of %(total)s pages"
 msgstr ""
 
 #: carbondesign/mithril-js/pagination_nav.js:11
 msgid "pagination"
 msgstr ""
 
 #: carbondesign/mithril-js/pagination_nav.js:12
```

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/accordion.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/accordion.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/base.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/base.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -120,15 +120,15 @@
         }
 
         let values = {};
 
         this.before_prepare(vnode, values, context);
         this.prepare(vnode, values, context);
 
-        if (this.WANT_CHILDREN) {
+        if (this.nodelist.length) {
             values.child = m.fragment({
                     _context: Object.assign({}, context)
                 },
                 this.nodelist);
         }
 
         this.after_prepare(vnode, values, context);
@@ -398,39 +398,36 @@
                     this.bound_field.help_text)
                 //##
             );
         }
     }
 
     render_tmpl_errors(vnode, values, context) {
-        return _render_errors(this.bound_field);
+        return render_errors(this.bound_field);
     }
 }
 
-
-export function render_errors(bound_field) {
-    let errors = _render_errors(bound_field);
-    if (errors) {
-        return m('div.bx--form-requirement', errors);
+export function render_errors(bound_fields) {
+    if (!isArray(bound_fields)) {
+        bound_fields = [bound_fields];
     }
-}
-
-function _render_errors(bound_field) {
-    if (!bound_field.errors) return;
-
     let items = [];
-    for (let error of bound_field.errors) {
-        let pos = error.indexOf('\n');
-        if (pos >= 0) {
-            items.push(m('div.bx--form-requirement__title',
-                error.slice(0, pos)));
-            items.push(m('p.bx--form-requirement__supplement',
-                error.slice(pos + 1)));
-        } else {
-            items.push(m('div.bx--form-requirement__title', error));
+    for (let bound_field of bound_fields) {
+        if (!bound_field.errors) return;
+
+        for (let error of bound_field.errors) {
+            let pos = error.indexOf('\n');
+            if (pos >= 0) {
+                items.push(m('div.bx--form-requirement__title',
+                    error.slice(0, pos)));
+                items.push(m('p.bx--form-requirement__supplement',
+                    error.slice(pos + 1)));
+            } else {
+                items.push(m('div.bx--form-requirement__title', error));
+            }
         }
     }
     if (items.length) {
         return m.fragment(items);
     }
 }
```

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/breadcrumb.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/breadcrumb.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/button.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/button.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/checkbox.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/checkbox.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/code_snippet.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/code_snippet.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/combo_box.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/combo_box.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/content_switcher.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/content_switcher.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/copy_button.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/copy_button.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/data-table.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/data-table.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -498,427 +498,427 @@
         return (
             //##
             m('th', {
                     'class': `bx--table-expand ${values['class']}`,
                     'data-event': 'expandAll',
                     ...values.props,
                 },
-                m('span.bx--table-header-label')
-                //##
-            );
-        }
+                m('span.bx--table-header-label'))
+            //##
+        );
+    }
 
-        render_expand_all(vnode, values, context) {
-            return (
-                //##
-                m('th', {
-                        'class': `bx--table-expand ${values['class']}`,
-                        'data-event': 'expandAll',
-                        ...values.props,
+    render_expand_all(vnode, values, context) {
+        return (
+            //##
+            m('th', {
+                    'class': `bx--table-expand ${values['class']}`,
+                    'data-event': 'expandAll',
+                    ...values.props,
+                },
+                m('button.bx--table-expand__button', null,
+                    m('svg', {
+                            focusable: false,
+                            preserveAspectRatio: 'xMidYMid meet',
+                            xmlns: 'http://www.w3.org/2000/svg',
+                            fill: 'currentColor',
+                            'class': 'bx--table-expand__svg',
+                            width: 16,
+                            height: 16,
+                            viewBox: '0 0 16 16',
+                            'aria-hidden': true,
+                        },
+                        m('path', {
+                            d: 'M11 8L6 13 5.3 12.3 9.6 8 5.3 3.7 6 3z'
+                        }))))
+            //##
+        );
+    }
+
+    render_row(vnode, values, context) {
+        return (
+            //##
+            m('th', {
+                    scope: 'row',
+                    'class': values['class'],
+                    ...values.props,
+                },
+                values.child)
+            //##
+        );
+    }
+}
+
+
+export class Td extends Node {
+    WANT_CHILDREN = true
+    MODE = ['default', 'menu', 'menu_visible']
+    SLOTS = ['secondary']
+
+    prepare(vnode, values, context) {
+        values.txt_menu = gettext("Open menu");
+    }
+
+    render_default(vnode, values, context) {
+        return (
+            //##
+            m('td', {
+                    'class': values['class'],
+                    ...values.props,
+                },
+                [
+                    values.child,
+                    this.slot('secondary', ...arguments),
+                ])
+            //##
+        );
+    }
+
+    render_menu(vnode, values, context) {
+        return (
+            //##
+            m('td', {
+                    'class': `bx--table-column-menu ${values['class']}`,
+                    ...values.props,
+                },
+                m('div', {
+                        'data-overflow-menu': '',
+                        role: 'menu',
+                        tabindex: 0,
+                        'aria-label': `${values.label}${values.label_suffix}`,
+                        'class': 'bx--overflow-menu',
+                        title: values.txt_menu,
                     },
-                    m('button.bx--table-expand__button', null,
+                    [
                         m('svg', {
                                 focusable: false,
                                 preserveAspectRatio: 'xMidYMid meet',
                                 xmlns: 'http://www.w3.org/2000/svg',
                                 fill: 'currentColor',
-                                'class': 'bx--table-expand__svg',
+                                'class': 'bx--overflow-menu__icon',
                                 width: 16,
                                 height: 16,
                                 viewBox: '0 0 16 16',
                                 'aria-hidden': true,
                             },
-                            m('path', {
-                                d: 'M11 8L6 13 5.3 12.3 9.6 8 5.3 3.7 6 3z'
-                            }))))
-                //##
-            );
-        }
+                            [
+                                m('circle', {
+                                    cx: 8,
+                                    cy: 3,
+                                    r: 1
+                                }),
+                                m('circle', {
+                                    cx: 8,
+                                    cy: 8,
+                                    r: 1
+                                }),
+                                m('circle', {
+                                    cx: 8,
+                                    cy: 13,
+                                    r: 1
+                                }),
+                            ]),
+                        m('ul.bx--overflow-menu-options.bx--overflow-menu--flip', null,
+                            values.child),
+                    ]))
+            //##
+        );
+    }
 
-        render_row(vnode, values, context) {
-            return (
-                //##
-                m('th', {
-                        scope: 'row',
-                        'class': values['class'],
-                        ...values.props,
+    render_menu_visible(vnode, values, context) {
+        return (
+            //##
+            m('td', {
+                    'class': `bx--table-column-menu ${values['class']}`,
+                    ...values.props,
+                },
+                m('div', {
+                        'data-overflow-menu': '',
+                        role: 'menu',
+                        tabindex: 0,
+                        'aria-label': `${values.label}${values.label_suffix}`,
+                        'class': 'bx--overflow-menu',
+                        title: values.txt_menu,
                     },
-                    values.child)
-                //##
-            );
-        }
+                    [
+                        m('svg', {
+                                focusable: false,
+                                preserveAspectRatio: 'xMidYMid meet',
+                                fill: 'currentColor',
+                                xmlns: 'http://www.w3.org/2000/svg',
+                                'class': 'bx--overflow-menu__icon',
+                                width: 16,
+                                height: 16,
+                                viewBox: '0 0 16 16',
+                                'aria-hidden': true,
+                            },
+                            [
+                                m('circle', {
+                                    cx: 8,
+                                    cy: 3,
+                                    r: 1
+                                }),
+                                m('circle', {
+                                    cx: 8,
+                                    cy: 8,
+                                    r: 1
+                                }),
+                                m('circle', {
+                                    cx: 8,
+                                    cy: 13,
+                                    r: 1
+                                }),
+                            ]),
+                        m('ul.bx--overflow-menu-options.bx--overflow-menu--flip', null,
+                            values.child),
+                    ]))
+            //##
+        );
     }
 
+    render_slot_secondary(vnode, values, context) {
+        return (
+            //##
+            m('div', {
+                    'class': `bx--data-table--cell-secondary-text ${values['class']}`,
+                    ...values.props,
+                },
+                values.child)
+            //##
+        );
+    }
+}
 
-    export class Td extends Node {
-        WANT_CHILDREN = true
-        MODE = ['default', 'menu', 'menu_visible']
-        SLOTS = ['secondary']
 
-        prepare(vnode, values, context) {
-            values.txt_menu = gettext("Open menu");
-        }
+export class TdCheckbox extends FormNode {
+    NODE_PROPS = ['value']
+    REQUIRED_PROPS = ['value']
 
-        render_default(vnode, values, context) {
-            return (
-                //##
-                m('td', {
-                        'class': values['class'],
-                        ...values.props,
-                    },
-                    [
-                        values.child,
-                        this.slot('secondary', ...arguments),
-                    ])
-                //##
-            );
-        }
+    default_id(vnode) {
+        return uniqueId(this.bound_field.id_for_label + '-');
+    }
 
-        render_menu(vnode, values, context) {
-            return (
-                //##
-                m('td', {
-                        'class': `bx--table-column-menu ${values['class']}`,
-                        ...values.props,
-                    },
-                    m('div', {
-                            'data-overflow-menu': '',
-                            role: 'menu',
-                            tabindex: 0,
-                            'aria-label': `${values.label}${values.label_suffix}`,
-                            'class': 'bx--overflow-menu',
-                            title: values.txt_menu,
-                        },
-                        [
-                            m('svg', {
-                                    focusable: false,
-                                    preserveAspectRatio: 'xMidYMid meet',
-                                    xmlns: 'http://www.w3.org/2000/svg',
-                                    fill: 'currentColor',
-                                    'class': 'bx--overflow-menu__icon',
-                                    width: 16,
-                                    height: 16,
-                                    viewBox: '0 0 16 16',
-                                    'aria-hidden': true,
-                                },
-                                [
-                                    m('circle', {
-                                        cx: 8,
-                                        cy: 3,
-                                        r: 1
-                                    }),
-                                    m('circle', {
-                                        cx: 8,
-                                        cy: 8,
-                                        r: 1
-                                    }),
-                                    m('circle', {
-                                        cx: 8,
-                                        cy: 13,
-                                        r: 1
-                                    }),
-                                ]),
-                            m('ul.bx--overflow-menu-options.bx--overflow-menu--flip', null,
-                                values.child),
-                        ]))
-                //##
-            );
+    label() {
+        for (let [group, val, txt] of this.choices()) {
+            if (val === this.value) {
+                return txt;
+            }
         }
+    }
 
-        render_menu_visible(vnode, values, context) {
-            return (
-                //##
-                m('td', {
-                        'class': `bx--table-column-menu ${values['class']}`,
-                        ...values.props,
-                    },
-                    m('div', {
-                            'data-overflow-menu': '',
-                            role: 'menu',
-                            tabindex: 0,
-                            'aria-label': `${values.label}${values.label_suffix}`,
-                            'class': 'bx--overflow-menu',
-                            title: values.txt_menu,
-                        },
-                        [
-                            m('svg', {
-                                    focusable: false,
-                                    preserveAspectRatio: 'xMidYMid meet',
-                                    fill: 'currentColor',
-                                    xmlns: 'http://www.w3.org/2000/svg',
-                                    'class': 'bx--overflow-menu__icon',
-                                    width: 16,
-                                    height: 16,
-                                    viewBox: '0 0 16 16',
-                                    'aria-hidden': true,
-                                },
-                                [
-                                    m('circle', {
-                                        cx: 8,
-                                        cy: 3,
-                                        r: 1
-                                    }),
-                                    m('circle', {
-                                        cx: 8,
-                                        cy: 8,
-                                        r: 1
-                                    }),
-                                    m('circle', {
-                                        cx: 8,
-                                        cy: 13,
-                                        r: 1
-                                    }),
-                                ]),
-                            m('ul.bx--overflow-menu-options.bx--overflow-menu--flip', null,
-                                values.child),
-                        ]))
-                //##
-            );
-        }
+    before_prepare(vnode, values, context) {
+        this.value = vnode.attrs.value;
+        super.before_prepare(...arguments);
+    }
 
-        render_slot_secondary(vnode, values, context) {
-            return (
-                //##
-                m('div', {
-                        'class': `bx--data-table--cell-secondary-text ${values['class']}`,
-                        ...values.props,
-                    },
-                    values.child)
-                //##
-            );
+    prepare(vnode, values, context) {
+        if (this.bound_value && this.bound_value.indexOf(this.value) !== -1) {
+            values.props.push(['checked', '']);
         }
     }
 
+    render_default(vnode, values, context) {
+        return (
+            //##
+            m('td.bx--table-column-checkbox',
+                [
+                    m('input', {
+                        type: 'checkbox',
+                        name: this.bound_field.name,
+                        value: this.value,
+                        id: values.id,
+                        'class': `bx--checkbox ${values['class']}`,
+                        'data-event': 'select',
+                        ...values.props,
+                    }),
+                    m('label.bx--checkbox-label', {
+                        'for': values.id,
+                        'aria-label': `${values.label}${values.label_suffix}`,
+                    }),
+                ])
+            //##
+        );
+    }
 
-    export class TdCheckbox extends FormNode {
-        NODE_PROPS = ['value']
-        REQUIRED_PROPS = ['value']
+}
 
-        default_id(vnode) {
-            return uniqueId(this.bound_field.id_for_label + '-');
-        }
 
-        label() {
-            for (let [group, val, txt] of this.choices()) {
-                if (val === this.value) {
-                    return txt;
-                }
-            }
-        }
+export class TbSearch extends Node {
+    NODE_PROPS = ['id', 'expandable', 'small']
+    CLASS_AND_PROPS = ['wrapper', 'magnifier']
+    CATCH_PROPS = ['search_props']
 
-        before_prepare(vnode, values, context) {
-            this.value = vnode.attrs.value;
-            super.before_prepare(...arguments);
+    prepare(vnode, values, context) {
+        values.txt_search = gettext("Search");
+        values.txt_clear = gettext("Clear search input");
+        if (!values.label) {
+            values.label = values.txt_search;
         }
 
-        prepare(vnode, values, context) {
-            if (this.bound_value && this.bound_value.indexOf(this.value) !== -1) {
-                values.props.push(['checked', '']);
-            }
+        if (vnode.attrs.expandable) {
+            values.wrapper_class.push('bx--toolbar-search-container-expandable');
+            values.magnifier_props.push(['tabindex', 0]);
+        } else {
+            values.wrapper_class.push('bx--toolbar-search-container-persistent');
         }
 
-        render_default(vnode, values, context) {
-            return (
-                //##
-                m('td.bx--table-column-checkbox',
-                    [
-                        m('input', {
-                            type: 'checkbox',
-                            name: this.bound_field.name,
-                            value: this.value,
-                            id: values.id,
-                            'class': `bx--checkbox ${values['class']}`,
-                            'data-event': 'select',
-                            ...values.props,
-                        }),
-                        m('label.bx--checkbox-label', {
-                            'for': values.id,
-                            'aria-label': `${values.label}${values.label_suffix}`,
-                        }),
-                    ])
-                //##
-            );
+        if (vnode.attrs.small) {
+            values['class'].push('bx--search--sm');
         }
-
     }
 
-
-    export class TbSearch extends Node {
-        NODE_PROPS = ['id', 'expandable', 'small']
-        CLASS_AND_PROPS = ['wrapper', 'magnifier']
-        CATCH_PROPS = ['search_props']
-
-        prepare(vnode, values, context) {
-            values.txt_search = gettext("Search");
-            values.txt_clear = gettext("Clear search input");
-            if (!values.label) {
-                values.label = values.txt_search;
-            }
-
-            if (vnode.attrs.expandable) {
-                values.wrapper_class.push('bx--toolbar-search-container-expandable');
-                values.magnifier_props.push(['tabindex', 0]);
-            } else {
-                values.wrapper_class.push('bx--toolbar-search-container-persistent');
-            }
-
-            if (vnode.attrs.small) {
-                values['class'].push('bx--search--sm');
-            }
-        }
-
-        render_default(vnode, values, context) {
-            return (
-                //##
+    render_default(vnode, values, context) {
+        return (
+            //##
+            m('div', {
+                    'class': values.wrapper_class,
+                    ...values.wrapper_props,
+                },
                 m('div', {
-                        'class': values.wrapper_class,
-                        ...values.wrapper_props,
+                        'data-search': '',
+                        'class': `bx--search ${values['class']}`,
+                        role: 'search',
+                        ...values.props,
                     },
-                    m('div', {
-                            'data-search': '',
-                            'class': `bx--search ${values['class']}`,
+                    [
+                        m('div', {
+                                'class': `bx--search-magnifier ${values.magnifier_class}`,
+                                ...values.magnifier_props,
+                            },
+                            this.tmpl('magnifier_icon', ...arguments)),
+                        m('label.bx--label', {
+                                id: `label-${values.id}`,
+                                'for': values.id,
+                            },
+                            `${values.label}${values.label_suffix}`),
+                        m('input.bx--search-input', {
+                            type: 'text',
+                            id: values.id,
                             role: 'search',
-                            ...values.props,
-                        },
-                        [
-                            m('div', {
-                                    'class': `bx--search-magnifier ${values.magnifier_class}`,
-                                    ...values.magnifier_props,
-                                },
-                                this.tmpl('magnifier_icon', ...arguments)),
-                            m('label.bx--label', {
-                                    id: `label-${values.id}`,
-                                    'for': values.id,
-                                },
-                                `${values.label}${values.label_suffix}`),
-                            m('input.bx--search-input', {
-                                type: 'text',
-                                id: values.id,
-                                role: 'search',
-                                placeholder: values.txt_search,
-                                'aria-labelledby': `label-${values.id}`,
-                            }),
-                            m('button.bx--search-close.bx--search-close--hidden', {
-                                    title: values.txt_clear,
-                                    'aria-label': values.txt_clear,
+                            placeholder: values.txt_search,
+                            'aria-labelledby': `label-${values.id}`,
+                        }),
+                        m('button.bx--search-close.bx--search-close--hidden', {
+                                title: values.txt_clear,
+                                'aria-label': values.txt_clear,
+                            },
+                            m('svg', {
+                                    focusable: false,
+                                    preserveAspectRatio: 'xMidYMid meet',
+                                    xmlns: 'http://www.w3.org/2000/svg',
+                                    fill: 'currentColor',
+                                    width: 16,
+                                    height: 16,
+                                    viewBox: '0 0 16 16',
+                                    'aria-hidden': true,
                                 },
-                                m('svg', {
-                                        focusable: false,
-                                        preserveAspectRatio: 'xMidYMid meet',
-                                        xmlns: 'http://www.w3.org/2000/svg',
-                                        fill: 'currentColor',
-                                        width: 16,
-                                        height: 16,
-                                        viewBox: '0 0 16 16',
-                                        'aria-hidden': true,
-                                    },
-                                    m('path', {
-                                        d: 'M12 4.7L11.3 4 8 7.3 4.7 4 4 4.7 7.3 8 4 11.3 4.7 12 8 8.7 \
+                                m('path', {
+                                    d: 'M12 4.7L11.3 4 8 7.3 4.7 4 4 4.7 7.3 8 4 11.3 4.7 12 8 8.7 \
                   11.3 12 12 11.3 8.7 8z',
-                                    }))),
-                        ]))
-                //##
-            );
-        }
+                                }))),
+                    ]))
+            //##
+        );
+    }
 
-        render_tmpl_magnifier_icon(vnode, values, context) {
-            return (
-                //##
-                m('svg', {
-                        focusable: false,
-                        preserveAspectRatio: 'xMidYMid meet',
-                        style: {
-                            'will-change': 'transform'
-                        },
-                        xmlns: 'http://www.w3.org/2000/svg',
-                        width: 16,
-                        height: 16,
-                        viewBox: '0 0 16 16',
-                        'aria-hidden': true,
+    render_tmpl_magnifier_icon(vnode, values, context) {
+        return (
+            //##
+            m('svg', {
+                    focusable: false,
+                    preserveAspectRatio: 'xMidYMid meet',
+                    style: {
+                        'will-change': 'transform'
                     },
-                    m('path', {
-                        d: 'M15,14.3L10.7,10c1.9-2.3,1.6-5.8-0.7-7.7S4.2,0.7,2.3,3S0.7,\
+                    xmlns: 'http://www.w3.org/2000/svg',
+                    width: 16,
+                    height: 16,
+                    viewBox: '0 0 16 16',
+                    'aria-hidden': true,
+                },
+                m('path', {
+                    d: 'M15,14.3L10.7,10c1.9-2.3,1.6-5.8-0.7-7.7S4.2,0.7,2.3,3S0.7,\
           8.8,3,10.7c2,1.7,5,1.7,7,0l4.3,4.3L15,14.3z M2,6.5	C2,4,\
           4,2,6.5,2S11,4,11,6.5S9,11,6.5,11S2,9,2,6.5z',
-                    }))
-                //##
-            );
-        }
+                }))
+            //##
+        );
     }
+}
 
 
-    export class TableOvButton extends Node {
-        WANT_CHILDREN = true
-        NODE_PROPS = ['active']
-        CLASS_AND_PROPS = ['list']
-
-        prepare(vnode, values, context) {
-            if (vnode.attrs.active) {
-                values.props.push(['data-floating-menu-primary-focus', '']);
-            }
+export class TableOvButton extends Node {
+    WANT_CHILDREN = true
+    NODE_PROPS = ['active']
+    CLASS_AND_PROPS = ['list']
 
-            if (context.compact) {
-                values.list_class.push('bx--overflow-menu--data-table');
-            }
+    prepare(vnode, values, context) {
+        if (vnode.attrs.active) {
+            values.props.push(['data-floating-menu-primary-focus', '']);
         }
 
-        render_default(vnode, values, context) {
-            return (
-                //##
-                m('li', {
-                        'class': `bx--overflow-menu-options__option ${values.list_class}`,
-                        role: 'presentation',
-                        ...values.list_props,
-                    },
-                    m('button', {
-                            'class': `bx--overflow-menu-options__btn ${values['class']}`,
-                            role: 'menuitem',
-                            ...values.props,
-                        },
-                        m('div.bx--overflow-menu-options__option-content', null, values.child)))
-                //##
-            );
+        if (context.compact) {
+            values.list_class.push('bx--overflow-menu--data-table');
         }
     }
 
+    render_default(vnode, values, context) {
+        return (
+            //##
+            m('li', {
+                    'class': `bx--overflow-menu-options__option ${values.list_class}`,
+                    role: 'presentation',
+                    ...values.list_props,
+                },
+                m('button', {
+                        'class': `bx--overflow-menu-options__btn ${values['class']}`,
+                        role: 'menuitem',
+                        ...values.props,
+                    },
+                    m('div.bx--overflow-menu-options__option-content', null, values.child)))
+            //##
+        );
+    }
+}
 
-    export class TdOvButton extends Node {
-        WANT_CHILDREN = true
-        SLOTS = ['icon']
-        NODE_PROPS = ['icon_size']
-
-        render_default(vnode, values, context) {
-            let cleaned_child = clean_attr_value(m_tostring(values.child));
-
-            return (
-                //##
-                m('li.bx--overflow-menu-options__option.bx--table-row--menu-option',
-                    m(values.astag, {
-                            'class': `bx--overflow-menu-options__btn ${values['class']}`,
-                            title: cleaned_child,
-                            ...values.props,
-                        },
-                        m('div.bx--overflow-menu-options__option-content', null,
-                            [
-                                this.slot('icon', ...arguments),
-                                values.child,
-                            ])))
-                //##
-            );
-        }
 
-        render_slot_icon(vnode, values, context) {
-            let size = vnode.attrs.icon_size || 16;
-            return modify_svg(values.child, {
-                focusable: false,
-                preserveAspectRatio: 'xMidYMid meet',
-                fill: 'currentColor',
-                style: {
-                    width: `${size}px`,
-                    height: `${size}px`,
-                },
-                'aria-hidden': true,
-                'class': values['class'],
-                ...values.props,
-            });
-        }
-    }
+export class TdOvButton extends Node {
+    WANT_CHILDREN = true
+    SLOTS = ['icon']
+    NODE_PROPS = ['icon_size']
+
+    render_default(vnode, values, context) {
+        let cleaned_child = clean_attr_value(m_tostring(values.child));
+
+        return (
+            //##
+            m('li.bx--overflow-menu-options__option.bx--table-row--menu-option',
+                m(values.astag, {
+                        'class': `bx--overflow-menu-options__btn ${values['class']}`,
+                        title: cleaned_child,
+                        ...values.props,
+                    },
+                    m('div.bx--overflow-menu-options__option-content', null,
+                        [
+                            this.slot('icon', ...arguments),
+                            values.child,
+                        ])))
+            //##
+        );
+    }
+
+    render_slot_icon(vnode, values, context) {
+        let size = vnode.attrs.icon_size || 16;
+        return modify_svg(values.child, {
+            focusable: false,
+            preserveAspectRatio: 'xMidYMid meet',
+            fill: 'currentColor',
+            style: {
+                width: `${size}px`,
+                height: `${size}px`,
+            },
+            'aria-hidden': true,
+            'class': values['class'],
+            ...values.props,
+        });
+    }
+}
```

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/date_picker.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/date_picker.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,60 +1,105 @@
+import flatpickr from 'flatpickr';
 import {
     some
 } from 'lodash';
 import m from 'mithril/hyperscript';
 //-
 import {
     FormNode,
     FormNodes
 } from './base';
 
+const TOKEN_REGEX = {
+    D: "(\\w+)",
+    F: "(\\w+)",
+    G: "(\\d\\d|\\d)",
+    H: "(\\d\\d|\\d)",
+    J: "(\\d\\d|\\d)\\w+",
+    // ToDo: K is ignored
+    M: "(\\w+)",
+    S: "(\\d\\d|\\d)",
+    U: "(.+)",
+    W: "(\\d\\d|\\d)",
+    Y: "(\\d{4})",
+    Z: "(.+)",
+    d: "(\\d\\d|\\d)",
+    h: "(\\d\\d|\\d)",
+    i: "(\\d\\d|\\d)",
+    j: "(\\d\\d|\\d)",
+    l: "(\\w+)",
+    m: "(\\d\\d|\\d)",
+    n: "(\\d\\d|\\d)",
+    s: "(\\d\\d|\\d)",
+    u: "(.+)",
+    w: "(\\d\\d|\\d)",
+    y: "(\\d{2})",
+};
+const DEFAULT_DATE_FORMAT = 'm/d/Y';
+const DEFAULT_SHORTDATE_FORMAT = 'm/Y';
+
+function format_to_pattern(value) {
+    return value.split('').map((x) => REGEX_PATTERN[x] || x).join('');
+}
+
 export class DatePicker extends FormNode {
     MODES = ['default', 'basic', 'nolabel']
-    NODE_PROPS = ['light']
+    NODE_PROPS = ['short', 'light', 'format']
+    CLASS_AND_PROPS = ['label', 'help', 'picker']
 
     prepare(vnode, values, context) {
         if (vnode.attrs.light) {
-            values.wrapper_class.push('bx--date-picker--light');
+            values.picker_class.push('bx--date-picker--light');
+        }
+        if (vnode.attrs.short) {
+            values.picker_class.push('bx--date-picker--short');
         }
+
+        if (vnode.attrs.format) {
+            this.datefmt = vnode.attrs.format;
+        } else if (vnode.attrs.short) {
+            this.datefmt = DEFAULT_SHORTDATE_FORMAT;
+        } else {
+            this.datefmt = DEFAULT_DATE_FORMAT;
+        }
+        this.placeholder = flatpickr.formatDate(new Date(1, 1, 1, 0, 0, 0),
+            this.datefmt);
+        this.pattern = format_to_pattern(this.datefmt);
+
+        values['picker_props'].push(['data-date-picker-format', this.datefmt]);
     }
 
     prepare_element_props(vnode, props, default_props, context) {
         props['class'].push('bx--date-picker__input');
         props['data-date-picker-input'] = '';
-        props.pattern = '\\d{1,2}/\\d{1,2}/\\d{4}';
-        props.placeholder = 'mm/dd/yyyy';
+        props.pattern = this.pattern;
+        props.placeholder = this.placeholder;
 
         if (this.bound_field.errors) {
             props['data-invalid'] = '';
         }
     }
 
     render_default(vnode, values, context) {
         if (this.bound_field.errors) {
             return (
                 //##
                 m('div.bx--form-item', null,
                     m('div', {
                             'data-date-picker': '',
                             'data-date-picker-type': 'single',
-                            'class': `bx--date-picker bx--date-picker--single ${values.wrapper_class}`,
-                            ...values.wrapper_props,
+                            'class': `bx--date-picker bx--date-picker--single ${values.picker_class}`,
+                            ...values.picker_props,
                         },
                         m('div.bx--date-picker-container', null,
                             [
-                                m('label', {
-                                        'for': values.id,
-                                        'class': `bx--label ${values.label_class}`,
-                                        ...values.label_props,
-                                    },
-                                    values.label),
+                                this.tmpl('label', ...arguments),
                                 m('div.bx--date-picker-input__wrapper', null,
                                     [
-                                        values.element,
+                                        this.tmpl('element', ...arguments),
                                         m('svg', {
                                                 focusable: false,
                                                 preserveAspectRatio: 'xMidYMid meet',
                                                 xmlns: 'http://www.w3.org/2000/svg',
                                                 fill: 'currentColor',
                                                 'data-date-picker-icon': true,
                                                 'class': 'bx--date-picker__icon',
@@ -65,40 +110,36 @@
                                             },
                                             m('path', {
                                                 d: 'M26,4h-4V2h-2v2h-8V2h-2v2H6C4.9,4,4,4.9,4,6v20c0,1.1,\
                       0.9,2,2,2h20c1.1,0,2-0.9,2-2V6C28,4.9,27.1,4,26,4z M26,\
                       26H6V12h20  V26z M26,10H6V6h4v2h2V6h8v2h2V6h4V10z',
                                             })),
                                     ]),
-                                m('div.bx--form-requirement', null, values.form_errors),
+                                m('div.bx--form-requirement', null,
+                                    this.tmpl('errors', ...arguments)),
                             ])))
                 //##
             );
         }
 
         return (
             //##
             m('div.bx--form-item', null,
                 m('div', {
                         'data-date-picker': '',
                         'data-date-picker-type': 'single',
-                        'class': `bx--date-picker bx--date-picker--single ${values.wrapper_class}`,
-                        ...values.wrapper_props,
+                        'class': `bx--date-picker bx--date-picker--single ${values.picker_class}`,
+                        ...values.picker_props,
                     },
                     m('div.bx--date-picker-container', null,
                         [
-                            m('label', {
-                                    'for': values.id,
-                                    'class': `bx--label ${values.label_class}`,
-                                    ...values.label_props,
-                                },
-                                values.label),
+                            this.tmpl('label', ...arguments),
                             m('div.bx--date-picker-input__wrapper', null,
                                 [
-                                    values.element,
+                                    this.tmpl('element', ...arguments),
                                     m('svg', {
                                             focusable: false,
                                             preserveAspectRatio: 'xMidYMid meet',
                                             xmlns: 'http://www.w3.org/2000/svg',
                                             fill: 'currentColor',
                                             'data-date-picker-icon': true,
                                             'class': 'bx--date-picker__icon',
@@ -122,22 +163,22 @@
         if (this.bound_field.errors) {
             return (
                 //##
                 m('div.bx--form-item', null,
                     m('div', {
                             'data-date-picker': '',
                             'data-date-picker-type': 'single',
-                            'class': `bx--date-picker bx--date-picker--single bx--date-picker--nolabel ${values.wrapper_class}`,
-                            ...values.wrapper_props,
+                            'class': `bx--date-picker bx--date-picker--single bx--date-picker--nolabel ${values.picker_class}`,
+                            ...values.picker_props,
                         },
                         m('div.bx--date-picker-container', null,
                             [
                                 m('div.bx--date-picker-input__wrapper', null,
                                     [
-                                        value.element,
+                                        this.tmpl('element', ...arguments),
                                         m('svg', {
                                                 focusable: false,
                                                 preserveAspectRatio: 'xMidYMid meet',
                                                 xmlns: 'http://www.w3.org/2000/svg',
                                                 fill: 'currentColor',
                                                 'data-date-picker-icon': true,
                                                 'class': 'bx--date-picker__icon',
@@ -147,35 +188,36 @@
                                                 'aria-hidden': true,
                                             },
                                             m('path', {
                                                 d: 'M26,4h-4V2h-2v2h-8V2h-2v2H6C4.9,4,4,4.9,4,6v20c0,1.1,\
                       0.9,2,2,2h20c1.1,0,2-0.9,2-2V6C28,4.9,27.1,4,26,4z M26,\
                       26H6V12h20  V26z M26,10H6V6h4v2h2V6h8v2h2V6h4V10z',
                                             })),
-                                        m('div.bx--form-requirement', null, values.form_errors),
+                                        m('div.bx--form-requirement', null,
+                                            this.tmpl('errors', ...arguments)),
                                     ]),
                             ])))
                 //##
             );
         }
 
         return (
             //##
             m('div.bx--form-item', null,
                 m('div', {
                         'data-date-picker': '',
                         'data-date-picker-type': 'single',
-                        'class': `bx--date-picker bx--date-picker--single bx--date-picker--nolabel ${values.wrapper_class}`,
-                        ...values.wrapper_props,
+                        'class': `bx--date-picker bx--date-picker--single bx--date-picker--nolabel ${values.picker_class}`,
+                        ...values.picker_props,
                     },
                     m('div.bx--date-picker-container', null,
                         [
                             m('div.bx--date-picker-input__wrapper', null,
                                 [
-                                    value.element,
+                                    this.tmpl('element', ...arguments),
                                     m('svg', {
                                             focusable: false,
                                             preserveAspectRatio: 'xMidYMid meet',
                                             xmlns: 'http://www.w3.org/2000/svg',
                                             fill: 'currentColor',
                                             'data-date-picker-icon': true,
                                             'class': 'bx--date-picker__icon',
@@ -185,83 +227,82 @@
                                             'aria-hidden': true,
                                         },
                                         m('path', {
                                             d: 'M26,4h-4V2h-2v2h-8V2h-2v2H6C4.9,4,4,4.9,4,6v20c0,1.1,\
                       0.9,2,2,2h20c1.1,0,2-0.9,2-2V6C28,4.9,27.1,4,26,4z M26,\
                       26H6V12h20  V26z M26,10H6V6h4v2h2V6h8v2h2V6h4V10z',
                                         })),
-                                    m('div.bx--form-requirement', null, values.form_errors),
                                 ]),
                         ])))
             //##
         );
     }
 
     render_basic(vnode, values, context) {
         if (this.bound_field.errors) {
             return (
                 //##
                 m('div.bx--form-item', null,
                     m('div', {
-                            'class': `bx--date-picker bx--date-picker--simple ${values.wrapper_class}`,
-                            ...values.wrapper_props,
+                            'class': `bx--date-picker bx--date-picker--simple ${values.picker_class}`,
+                            ...values.picker_props,
                         },
                         m('div.bx--date-picker-container', null,
                             [
-                                m('label', {
-                                        'for': values.id,
-                                        'class': `bx--label ${values.label_class}`,
-                                        ...values.label_props,
-                                    },
-                                    values.label),
-                                values.element,
-                                m('div.bx--form-requirement', null, values.form_errors),
+                                this.tmpl('label', ...arguments),
+                                this.tmpl('element', ...arguments),
+                                m('div.bx--form-requirement', null,
+                                    this.tmpl('errors', ...arguments)),
                             ])))
                 //##
             );
         }
 
         return (
             //##
             m('div.bx--form-item', null,
                 m('div', {
-                        'class': `bx--date-picker bx--date-picker--simple bx--date-picker--short ${values.wrapper_class}`,
-                        ...values.wrapper_props,
+                        'class': `bx--date-picker bx--date-picker--simple ${values.picker_class}`,
+                        ...values.picker_props,
                     },
                     m('div.bx--date-picker-container', null,
                         [
-                            m('label', {
-                                    'for': values.id,
-                                    'class': `bx--label ${values.label_class}`,
-                                    ...values.label_props,
-                                },
-                                values.label),
-                            values.element,
+                            this.tmpl('label', ...arguments),
+                            this.tmpl('element', ...arguments),
                         ])))
             //##
         );
     }
 }
 
 
 export class RangeDatePicker extends FormNodes {
-    NODE_PROPS = ['light']
+    NODE_PROPS = ['light', 'format']
 
     prepare(vnode, values, context) {
         if (vnode.attrs.light) {
             values.wrapper_class.push('bx--date-picker--light');
         }
+
+        if (vnode.attrs.format) {
+            this.datefmt = vnode.attrs.format;
+        } else {
+            this.datefmt = DEFAULT_DATE_FORMAT;
+        }
+        this.placeholder = flatpickr.formatDate(new Date(1, 1, 1, 0, 0, 0),
+            this.datefmt);
+        this.pattern = format_to_pattern(this.datefmt);
     }
 
     prepare_element_props(vnode, field, props, default_props, context) {
         let index = this.bound_fields.indexOf(field);
 
         props['class'].push('bx--date-picker__input');
-        props.pattern = '\\d{1,2}/\\d{1,2}/\\d{4}';
-        props.placeholder = 'mm/dd/yyyy';
+        props.pattern = this.pattern;
+        props.placeholder = this.placeholder;
 
         if (index) {
             props['data-date-picker-input-to'] = '';
         } else {
             props['data-date-picker-input-from'] = '';
         }
 
@@ -275,29 +316,29 @@
         if (has_errors) {
             return (
                 //##
                 m('div.bx--form-item', null,
                     m('div', {
                             'data-date-picker': '',
                             'data-date-picker-type': 'range',
-                            'class': `bx--date-picker bx--date-picker--range ${values.wrapper_class}`,
-                            ...values.wrapper_props,
+                            'class': `bx--date-picker bx--date-picker--range ${values.picker_class}`,
+                            ...values.picker_props,
                         },
                         [
                             m('div.bx--date-picker-container', null,
                                 [
                                     m('label', {
                                             'for': values.id_0,
                                             'class': `bx--label ${values.label_class}`,
                                             ...values.label_props,
                                         },
                                         values.label_0),
                                     m('div.bx--date-picker-input__wrapper', null,
                                         [
-                                            values.element_0,
+                                            this.tmpl('element_0', ...arguments),
                                             m('svg', {
                                                     focusable: false,
                                                     preserveAspectRatio: 'xMidYMid meet',
                                                     xmlns: 'http://www.w3.org/2000/svg',
                                                     fill: 'currentColor',
                                                     'data-date-picker-icon': true,
                                                     'class': 'bx--date-picker__icon',
@@ -308,27 +349,28 @@
                                                 },
                                                 m('path', {
                                                     d: 'M26,4h-4V2h-2v2h-8V2h-2v2H6C4.9,4,4,4.9,4,6v20c0,1.1,\
                         0.9,2,2,2h20c1.1,0,2-0.9,2-2V6C28,4.9,27.1,4,26,\
                         4z M26,26H6V12h20  V26z M26,10H6V6h4v2h2V6h8v2h2V6h4V10z',
                                                 })),
                                         ]),
-                                    m('div.bx--form-requirement', null, values.form_errors_0),
+                                    m('div.bx--form-requirement', null,
+                                        this.tmpl('errors_0', ...arguments)),
                                 ]),
                             m('div.bx--date-picker-container', null,
                                 [
                                     m('label', {
                                             'for': values.id_1,
                                             'class': `bx--label ${values.label_class}`,
                                             ...values.label_props,
                                         },
                                         values.label_1),
                                     m('div.bx--date-picker-input__wrapper', null,
                                         [
-                                            values.element_1,
+                                            this.tmpl('element_1', ...arguments),
                                             m('svg', {
                                                     focusable: false,
                                                     preserveAspectRatio: 'xMidYMid meet',
                                                     xmlns: 'http://www.w3.org/2000/svg',
                                                     fill: 'currentColor',
                                                     'data-date-picker-icon': true,
                                                     'class': 'bx--date-picker__icon',
@@ -339,42 +381,43 @@
                                                 },
                                                 m('path', {
                                                     d: 'M26,4h-4V2h-2v2h-8V2h-2v2H6C4.9,4,4,4.9,4,6v20c0,1.1,\
                         0.9,2,2,2h20c1.1,0,2-0.9,2-2V6C28,4.9,27.1,4,26,4z \
                         M26,26H6V12h20  V26z M26,10H6V6h4v2h2V6h8v2h2V6h4V10z',
                                                 })),
                                         ]),
-                                    m('div.bx--form-requirement', null, values.form_errors_1),
+                                    m('div.bx--form-requirement', null,
+                                        this.tmpl('errors_1', ...arguments)),
                                 ]),
                         ]))
                 //##
             );
         }
 
         return (
             //##
             m('div.bx--form-item', null,
                 m('div', {
                         'data-date-picker': '',
                         'data-date-picker-type': 'range',
-                        'class': `bx--date-picker bx--date-picker--range ${values.wrapper_class}`,
-                        ...values.wrapper_props,
+                        'class': `bx--date-picker bx--date-picker--range ${values.picker_class}`,
+                        ...values.picker_props,
                     },
                     [
                         m('div.bx--date-picker-container', null,
                             [
                                 m('label', {
                                         'for': values.id_0,
                                         'class': `bx--label ${values.label_class}`,
                                         ...values.label_props,
                                     },
                                     values.label_0),
                                 m('div.bx--date-picker-input__wrapper', null,
                                     [
-                                        values.element_0,
+                                        this.tmpl('element_0', ...arguments),
                                         m('svg', {
                                                 focusable: false,
                                                 preserveAspectRatio: 'xMidYMid meet',
                                                 xmlns: 'http://www.w3.org/2000/svg',
                                                 fill: 'currentColor',
                                                 'data-date-picker-icon': true,
                                                 'class': 'bx--date-picker__icon',
@@ -396,15 +439,15 @@
                                         'for': values.id_1,
                                         'class': `bx--label ${values.label_class}`,
                                         ...values.label_props,
                                     },
                                     values.label_1),
                                 m('div.bx--date-picker-input__wrapper', null,
                                     [
-                                        values.element_1,
+                                        this.tmpl('element_1', ..arguments),
                                         m('svg', {
                                                 focusable: false,
                                                 preserveAspectRatio: 'xMidYMid meet',
                                                 xmlns: 'http://www.w3.org/2000/svg',
                                                 fill: 'currentColor',
                                                 'data-date-picker-icon': true,
                                                 'class': 'bx--date-picker__icon',
```

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/dropdown.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/dropdown.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/file_uploader.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/file_uploader.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/grid.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/grid.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/hidden_input.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/hidden_input.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/inline_loading.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/inline_loading.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/link.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/link.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/list.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/list.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/list_box.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/list_box.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/loading.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/loading.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/modal.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/modal.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/multi_select.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/multi_select.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/notification.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/notification.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/number_input.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/number_input.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/overflow_menu.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/overflow_menu.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/pagination.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/pagination.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/pagination_nav.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/pagination_nav.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/progress_indicator.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/progress_indicator.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/radio_button.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/radio_button.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/search.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/search.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/select.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/select.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,25 +5,23 @@
 } from './base';
 
 export class Select extends FormNode {
     MODEs = ['default', 'inline']
     NODE_PROPS = ['light']
     CLASS_AND_PROPS = ['label', 'help', 'select']
 
-    required = false
-
     prepare(vnode, values, context) {
         values.txt_choose = gettext("Choose an option");
 
         values.props.push(['id', values.id]);
         values.props.push(['name', this.bound_field.name]);
 
-        this.required = this.bound_field.field.required &&
+        required = this.bound_field.field.required &&
             this.bound_field.form.use_required_attribute;
-        if (this.required) {
+        if (required) {
             values.props.push(['required', '']);
         }
 
         if (vnode.attrs.disabled) {
             values.props.push(['disabled', '']);
             values.label_class.push('bx--label--disabled');
             values.select_class.push('bx--select--disabled');
```

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/slider.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/slider.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/structured_list.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/structured_list.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/tabs.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/tabs.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/tag.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/tag.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/text_area.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/text_area.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/text_input.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/text_input.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/tile.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/tile.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/toggle.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/toggle.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/toolbar.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/toolbar.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/tooltip.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/tooltip.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/uishell--action.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/uishell--action.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/uishell--switcher.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/uishell--switcher.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/mithril-js/uishell.js` & `django-carbondesign-0.0.5/carbondesign/mithril-js/uishell.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.css` & `django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.css`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.css.map` & `django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.css.map`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.js` & `django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.min.css` & `django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.min.css`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.min.css.map` & `django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.min.css.map`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/static/carbondesign/carbon-components.min.js` & `django-carbondesign-0.0.5/carbondesign/static/carbondesign/carbon-components.min.js`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/accordion.py` & `django-carbondesign-0.0.5/carbondesign/tags/accordion.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/base.py` & `django-carbondesign-0.0.5/carbondesign/tags/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import logging
 import re
 from typing import Sequence
 from uuid import uuid4
 #-
 from django import template
 from django.template.base import TextNode # pylint:disable=unused-import
-from django.template.base import FilterExpression, Variable
+from django.template.base import FilterExpression, NodeList, Variable
+from django.template.base import VariableDoesNotExist
 from django.utils.html import strip_tags
 from django.utils.translation import gettext as _
 from lxml import etree
 #-
 from .base_widgets import CustomCheckboxInput, CustomTextarea, CustomTextInput
 
 _logger = logging.getLogger(__name__)
@@ -22,15 +23,19 @@
 VARIABLE_IN_ARG = re.compile(r'{{([\w.:|\'"]+)}}')
 
 
 def var_eval(value, context):
     """Evaluate argument passed to our Template Tag.
     """
     if isinstance(value, (VariableInVariable, FilterExpression, Variable)):
-        return value.resolve(context)
+        try:
+            return value.resolve(context)
+        except VariableDoesNotExist:
+            _logger.error("Missing variable %s", repr(value))
+            return ''
 
     if isinstance(value, str):
         for match in VARIABLE_IN_ARG.finditer(value):
             parsed = Variable(match.group(1)).resolve(context)
             value = value.replace(match.group(0), str(parsed))
 
     return value
@@ -39,15 +44,15 @@
 def modify_svg(xml, props):
     """Modify xml attributes of an svg image.
     """
     # pylint:disable=c-extension-no-member
     root = etree.fromstring(xml)
     for attr, value in props.items():
         if attr == 'style':
-            value = ';'.join('%s:%s' % (x, y) for x, y in value.items())
+            value = ';'.join(f'{x}:{y}' for x, y in value.items())
         root.attrib[attr] = value
     return etree.tostring(root).decode()
 
 
 def clean_attr_value(value):
     """Strip html of its tags and prepare it to be used as html attribute value.
     """
@@ -68,14 +73,17 @@
         value = self.value
         for match in VARIABLE_IN_ARG.finditer(value):
             expr = FilterExpression(match.group(1), self.parser)
             parsed = expr.resolve(context)
             value = value.replace(match.group(0), parsed)
         return Variable(value).resolve(context)
 
+    def __repr__(self):
+        return f"VariableInVariable('{self.value}')"
+
 
 class IgnoreMissing(dict):
     """String formatting but the variables are optional.
     """
     def __missing__(self, key):
         """Replacement string for missing variables.
         """
@@ -185,14 +193,15 @@
             self.nodelist = args[0]
             slots = self.nodelist.get_nodes_by_type(Slot)
             for slot in slots:
                 self.nodelist.remove(slot)
             self.slots = {s.name: s for s in slots}
         else:
             self.args = args
+            self.nodelist = NodeList()
             self.slots = {}
 
         self.kwargs = kwargs
 
 
     def render(self, context):
         """Render the Template Tag as html.
@@ -215,25 +224,24 @@
                         .format(prop=prop))
 
         values = {}
 
         self.before_prepare(values, context)
         self.prepare(values, context)
 
-        if self.WANT_CHILDREN:
+        if self.nodelist:
             values['child'] = self.nodelist.render(context)
         else:
             values['child'] = ''
 
         self.after_prepare(values, context)
 
-        method = getattr(self, 'render_%s' % self.mode, None)
+        method = getattr(self, f'render_{self.mode}', None)
         if not method:
-            raise NotImplementedError("Method is missing: render_%s" %\
-                    self.mode)
+            raise NotImplementedError(f"Method is missing: render_{self.mode}")
 
         result = method(values, context) # pylint:disable=not-callable
         # Destroy local context.
         context.pop()
         return result
 
 
@@ -310,22 +318,21 @@
         """Initialize the values meant for rendering templates.
         """
         self.mode = self.kwargs.get('mode', None)
         if self.MODES:
             if not self.mode:
                 self.mode = self.MODES[0]
             elif self.mode not in self.MODES:
-                raise NotImplementedError("Mode %s is not allowed." %\
-                        self.mode)
+                raise NotImplementedError(f"Mode {self.mode} is not allowed.")
         else:
             self.mode = 'default'
 
         values['mode'] = self.mode
         if 'tag' in self.kwargs and 'astag' not in self.kwargs:
-            _logger.warning("tag NODE_PROPS is deprecated by astag")
+            _logger.warning("tag in NODE_PROPS is deprecated by astag")
             mytag = var_eval(self.kwargs['tag'], context)
         else:
             mytag = var_eval(self.kwargs.get('astag', self.DEFAULT_TAG),
                     context)
         values['astag'] = mytag
         values['props'] = self.props(context)
         values['class'] = var_eval(self.kwargs.get('class', ''), context)\
@@ -441,16 +448,18 @@
                 method = getattr(self, typ)
                 method(nam, values, context, slots)
             if slots:
                 tpl = tpl.format_map(IgnoreMissing(slots))
 
         try:
             return tpl.format_map(IgnoreMissing(values))
-        except ValueError as e:
-            raise e
+        except ValueError:
+            _logger.exception("Trying to render template:\n%s\nwith %s", tpl,
+                    values)
+            return ''
 
 
     def set_child_props(self, context, name, slot=None, **kwargs):
         """Use context to set arguments for all children Template Tags.
         """
         if slot:
             name = f'{slot}_{name}'
@@ -821,23 +830,23 @@
 
         self.prepare_element_props(attrs, attrs, context)
         attrs['class'] = ' '.join(attrs['class'])
 
         if var_eval(self.kwargs.get('hidden'), context):
             attrs.pop('type')
             props = self.join_attributes(self.prune_attributes(attrs))
-            return '<input type="hidden" {props}">'.format(props=props)
+            return f'<input type="hidden" {props}>'
         return self.render_form_control(attrs, context)
 
 
     def render_form_control(self, values, context):
         """Default to rendering input, need to be overridden by subclass.
         """
         props = self.join_attributes(self.prune_attributes(values))
-        return '<input {props}">'.format(props=props)
+        return f'<input {props}>'
 
 
     def after_prepare(self, values, context):
         """Post-process the values for rendering templates.
         """
         values['element'] = self.element(values, context)
         super().after_prepare(values, context)
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/base_widgets.py` & `django-carbondesign-0.0.5/carbondesign/tags/base_widgets.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/breadcrumb.py` & `django-carbondesign-0.0.5/carbondesign/tags/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/button.py` & `django-carbondesign-0.0.5/carbondesign/tags/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
         """
         size = self.eval(self.kwargs.get('icon_size', 16), context)
         return modify_svg(values['child'], {
             'focusable': 'false',
             'preserveAspectRatio': 'xMidYMid meet',
             'fill': 'currentColor',
             'style': {
-                'width': '%spx' % size,
-                'height': '%spx' % size,
+                'width': f'{size}px',
+                'height': f'{size}px',
             },
             'aria-hidden': 'true',
             'class': 'bx--btn__icon ' + values['class'],
         })
 
 
 class IconButton(Button):
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/checkbox.py` & `django-carbondesign-0.0.5/carbondesign/tags/checkbox.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/code_snippet.py` & `django-carbondesign-0.0.5/carbondesign/tags/code_snippet.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/combo_box.py` & `django-carbondesign-0.0.5/carbondesign/tags/combo_box.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/content_switcher.py` & `django-carbondesign-0.0.5/carbondesign/tags/content_switcher.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/copy_button.py` & `django-carbondesign-0.0.5/carbondesign/tags/copy_button.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/data_table.py` & `django-carbondesign-0.0.5/carbondesign/tags/data_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,15 +518,15 @@
     "Will raise Exception if not set."
 
     value = None
 
     def default_id(self):
         """Get Django form field html id.
         """
-        return '%s-%s' % (self.bound_field.id_for_label, uuid4().hex)
+        return '%s-%s' % (self.bound_field.id_for_label, uuid4().hex) # pylint:disable=consider-using-f-string
 
 
     def label(self):
         """Get Django form field label.
         """
         for _, val, txt in self.choices():
             if val == self.value:
@@ -706,16 +706,16 @@
         """
         size = self.eval(self.kwargs.get('icon_size', 16), context)
         return modify_svg(values['child'], {
             'focusable': 'false',
             'preserveAspectRatio': 'xMidYMid meet',
             'fill': 'currentColor',
             'style': {
-                'width': '%spx' % size,
-                'height': '%spx' % size,
+                'width': f'{size}px',
+                'height': f'{size}px',
             },
             'aria-hidden': 'true',
             'class': values['class'],
         })
 
 
 components = {
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/date_picker.py` & `django-carbondesign-0.0.5/carbondesign/tags/date_picker.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,50 +10,76 @@
 Overview
 --------
 
 Pickers are used to display past, present, or future dates or times. The kind
 of date (exact, approximate, memorable) you are requesting from the user will
 determine which picker is best to use. Each picker’s format can be customized
 depending on location or need.
+
+For available formats see:
+
+* https://flatpickr.js.org/formatting/
+* https://docs.djangoproject.com/en/dev/ref/templates/builtins/#date
+
 """ # pylint:disable=line-too-long
 # pylint:disable=too-many-lines
-
+from django.utils.formats import date_format
+#-
+from ..utils.formats import SAMPLE_DATETIME
+from ..utils.formats import dateformat_to_pattern, get_field_dateformat
 from .base import FormNode, FormNodes
 
 class DatePicker(FormNode):
     """Date Picker component.
     """
     MODES = ('default', 'basic', 'nolabel')
     "Available variants."
-    NODE_PROPS = ('short', 'light')
+    NODE_PROPS = ('short', 'light', 'format')
     "Extended Template Tag arguments."
     CLASS_AND_PROPS = ('label', 'help', 'picker')
     "Prepare xxx_class and xxx_props values."
 
+    datefmt = None
+    placeholder = None
+    pattern = None
+
     def prepare(self, values, context):
         """Prepare values for rendering the templates.
         """
         if self.eval(self.kwargs.get('light'), context):
             values['picker_class'].append('bx--date-picker--light')
 
-        if self.eval(self.kwargs.get('short'), context):
+        short = self.eval(self.kwargs.get('short'), context)
+        if short:
             values['picker_class'].append('bx--date-picker--short')
 
+        datefmt = self.eval(self.kwargs.get('format'), context)
+        if not datefmt and self.bound_field:
+            datefmt = get_field_dateformat(self.bound_field)
+
+        if datefmt:
+            self.datefmt = datefmt
+        elif short:
+            self.datefmt = 'm/Y'
+        else:
+            # This is the default of Carbon Design datepicker
+            self.datefmt = 'm/d/Y'
+        self.placeholder = date_format(SAMPLE_DATETIME, self.datefmt)
+        self.pattern = dateformat_to_pattern(self.datefmt)
+
+        values['picker_props'].append(('data-date-picker-format', self.datefmt))
+
 
     def prepare_element_props(self, props, context):
         """Prepare html attributes for rendering the form element.
         """
         props['class'].append('bx--date-picker__input')
         props['data-date-picker-input'] = ''
-        if self.eval(self.kwargs.get('short'), context):
-            props['pattern'] = r'\d{1,2}/\d{4,4}'
-            props['placeholder'] = 'mm/yyyy'
-        else:
-            props['pattern'] = r'\d{1,2}/\d{1,2}/\d{4,4}'
-            props['placeholder'] = 'mm/dd/yyyy'
+        props['pattern'] = self.pattern
+        props['placeholder'] = self.placeholder
 
         if self.bound_field.errors:
             props['data-invalid'] = ''
 
 
     def render_default(self, values, context):
         """Output html of the component.
@@ -193,34 +219,52 @@
 """
         return self.format(template, values, context)
 
 
 class RangeDatePicker(FormNodes):
     """Date Picker component with range inputs.
     """
-    NODE_PROPS = ('light',)
+    NODE_PROPS = ('light', 'format')
     "Extended Template Tag arguments."
     CLASS_AND_PROPS = ('label', 'help', 'picker')
     "Prepare xxx_class and xxx_props values."
 
+    datefmt = None
+    placeholder = None
+    pattern = None
+
     def prepare(self, values, context):
         """Prepare values for rendering the templates.
         """
         if self.eval(self.kwargs.get('light'), context):
             values['picker_class'].append('bx--date-picker--light')
 
+        datefmt = self.eval(self.kwargs.get('format'), context)
+        if not datefmt and self.bound_fields:
+            datefmt = get_field_dateformat(self.bound_fields[0])
+
+        if datefmt:
+            self.datefmt = datefmt
+        else:
+            # This is the default of Carbon Design datepicker
+            self.datefmt = 'm/d/Y'
+        self.placeholder = date_format(SAMPLE_DATETIME, self.datefmt)
+        self.pattern = dateformat_to_pattern(self.datefmt)
+
+        values['picker_props'].append(('data-date-picker-format', self.datefmt))
+
 
     def prepare_element_props(self, props, context, bound_field):
         """Prepare html attributes for rendering the form element.
         """
         index = self.bound_fields.index(bound_field)
 
         props['class'].append('bx--date-picker__input')
-        props['pattern'] = r'\d{1,2}/\d{1,2}/\d{4,4}'
-        props['placeholder'] = 'mm/dd/yyyy'
+        props['pattern'] = self.pattern
+        props['placeholder'] = self.placeholder
 
         if index:
             props['data-date-picker-input-to'] = ''
         else:
             props['data-date-picker-input-from'] = ''
 
         if bound_field.errors:
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/dropdown.py` & `django-carbondesign-0.0.5/carbondesign/tags/dropdown.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,16 +200,16 @@
             'focusable': 'false',
             'preserveAspectRatio': 'xMidYMid meet',
             'fill': 'currentColor',
             'class': 'bx--list-box__menu-item__selected-icon ' +\
                 values['class'],
             'style': {
                 'will-change': 'transform',
-                'width': '%spx' % 16,
-                'height': '%spx' % 16,
+                'width': '16px',
+                'height': '16px',
             },
             'aria-hidden': 'true',
         })
 
 
 components = {
     'Dropdown': Dropdown,
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/file_uploader.py` & `django-carbondesign-0.0.5/carbondesign/tags/file_uploader.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/grid.py` & `django-carbondesign-0.0.5/carbondesign/tags/grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """Prepare values for rendering the templates.
         """
         if self.eval(self.kwargs.get('full_width'), context):
             values['class'].append('bx--grid--full-width')
 
         gap = self.eval(self.kwargs.get('gap'), context)
         if gap in self.GAP_SIZES:
-            values['class'].append('bx--grid--%s' % gap)
+            values['class'].append(f'bx--grid--{gap}')
 
 
     def render_default(self, values, context):
         """Output html of the component.
         """
         template = '<{astag} class="bx--grid {class}" {props}>{child}</{astag}>'
         return self.format(template, values)
@@ -64,60 +64,52 @@
 
 
 class Column(Node):
     """Grid columns.
     """
     WANT_CHILDREN = True
     "Template Tag needs closing end tag."
-    MODES = ('default', 'inner')
-    "Available variants."
     COL_SIZES = ('sm', 'md', 'lg', 'xlg', 'max')
     "Column sizes."
-    NODE_PROPS = (*COL_SIZES, *['offset_%s' % x for x in COL_SIZES])
+    NODE_PROPS = (*COL_SIZES, *[f'offset_{x}' for x in COL_SIZES])
     "Extended Template Tag arguments."
 
+    has_size = False
+
     def prepare(self, values, context):
         """Prepare values for rendering the templates.
         """
-        if self.mode != 'inner':
-            values['class'].append('bx--col')
-
-        has_size = False
         for size in self.COL_SIZES:
             width = self.eval(self.kwargs.get(size), context)
             if width:
-                has_size = True
-                values['class'].append('bx--col-%s-%s' % (size, width))
+                self.has_size = True
+                values['class'].append(f'bx--col-{size}-{width}')
 
-            width = self.eval(self.kwargs.get('offset_%s' % size), context)
+            width = self.eval(self.kwargs.get(f'offset_{size}'), context)
             if width:
-                values['class'].append('bx--offset-%s-%s' % (size, width))
-        if not has_size:
-            values['class'].append('bx--col--auto')
+                values['class'].append(f'bx--offset-{size}-{width}')
+        if not self.has_size:
+            values['class'].append('bx--col bx--col--auto')
 
 
     def render_default(self, values, context):
         """Output html of the component.
         """
-        template = '<{astag} class="{class}" {props}>{child}</{astag}>'
-        return self.format(template, values)
-
-
-    def render_inner(self, values, context):
-        """Output html of the component.
-        """
-        template = """
+        if self.has_size:
+            template = """
 <{astag} class="{class}" {props}>
   <div class="outside">
     <div class="inside">
       {child}
     </div>
   </div>
 </{astag}>
 """
+        else:
+            template = '<{astag} class="{class}" {props}>{child}</{astag}>'
         return self.format(template, values)
 
 
 class AspectRatio(Node):
     """Grid aspect ratio.
     """
     WANT_CHILDREN = True
@@ -126,15 +118,15 @@
     "Extended Template Tag arguments."
 
     def prepare(self, values, context):
         """Prepare values for rendering the templates.
         """
         ratio = self.eval(self.kwargs.get('ratio'), context)
         if ratio:
-            values['class'].append('bx--aspect-ratio--%s' % ratio)
+            values['class'].append(f'bx--aspect-ratio--{ratio}')
 
 
     def render_default(self, values, context):
         """Output html of the component.
         """
         template = """
 <{astag} class="bx--aspect-ratio {class}" {props}>
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/inline_loading.py` & `django-carbondesign-0.0.5/carbondesign/tags/inline_loading.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/link.py` & `django-carbondesign-0.0.5/carbondesign/tags/link.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/list_.py` & `django-carbondesign-0.0.5/carbondesign/tags/list_.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/list_box.py` & `django-carbondesign-0.0.5/carbondesign/tags/list_box.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/loading.py` & `django-carbondesign-0.0.5/carbondesign/tags/loading.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/modal.py` & `django-carbondesign-0.0.5/carbondesign/tags/modal.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/multi_select.py` & `django-carbondesign-0.0.5/carbondesign/tags/multi_select.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     </div>
   </div>
 </div>
 """
         items = []
         for ii, (_, val, txt) in enumerate(self.choices()):
             options = {
-                'id': '%s-%s' % (values['id'], ii + 1),
+                'id': f"{values['id']}-{ii + 1}",
                 'value': val,
                 'child': txt,
                 'name': self.bound_field.name,
             }
             props = []
             if val in self.bound_value:
                 props.append('checked')
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/notification.py` & `django-carbondesign-0.0.5/carbondesign/tags/notification.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/number_input.py` & `django-carbondesign-0.0.5/carbondesign/tags/number_input.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/overflow_menu.py` & `django-carbondesign-0.0.5/carbondesign/tags/overflow_menu.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/pagination.py` & `django-carbondesign-0.0.5/carbondesign/tags/pagination.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/pagination_nav.py` & `django-carbondesign-0.0.5/carbondesign/tags/pagination_nav.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/progress_indicator.py` & `django-carbondesign-0.0.5/carbondesign/tags/progress_indicator.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/radio_button.py` & `django-carbondesign-0.0.5/carbondesign/tags/radio_button.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         excludes = self.eval(self.kwargs.get('exclude', []), context)
         if isinstance(excludes, str):
             excludes = [x.strip() for x in excludes.split(';')]
 
         items = []
         for ii, (_, val, txt) in enumerate(self.choices()):
             options = {
-                'id': '%s-%s' % (values['id'], ii + 1),
+                'id': f"{values['id']}-{ii + 1}",
                 'value': val,
                 'child': txt,
                 'name': self.bound_field.name,
                 'class': values['class'],
             }
             props = []
             if val == selected:
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/search.py` & `django-carbondesign-0.0.5/carbondesign/tags/search.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/select.py` & `django-carbondesign-0.0.5/carbondesign/tags/select.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,25 @@
     MODES = ('default', 'inline')
     "Available variants."
     NODE_PROPS = ('light', 'with_empty')
     "Extended Template Tag arguments."
     CLASS_AND_PROPS = ('label', 'help', 'select')
     "Prepare xxx_class and xxx_props values."
 
-    required = False
-
     def prepare(self, values, context):
         """Prepare values for rendering the templates.
         """
         values['txt_choose'] = _("Choose an option")
 
         values['props'].append(('id', values['id']))
         values['props'].append(('name', self.bound_field.name))
 
-        self.required = self.bound_field.field.required and\
+        required = self.bound_field.field.required and\
                 self.bound_field.form.use_required_attribute
-        if self.required:
+        if required:
             values['props'].append(('required', True))
 
         if self.eval(self.kwargs.get('disabled'), context):
             values['props'].append(('disabled', True))
             values['label_class'].append('bx--label--disabled')
             values['select_class'].append('bx--select--disabled')
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/slider.py` & `django-carbondesign-0.0.5/carbondesign/tags/slider.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/structured_list.py` & `django-carbondesign-0.0.5/carbondesign/tags/structured_list.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/tabs.py` & `django-carbondesign-0.0.5/carbondesign/tags/tabs.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/tag.py` & `django-carbondesign-0.0.5/carbondesign/tags/tag.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/text_area.py` & `django-carbondesign-0.0.5/carbondesign/tags/text_area.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/text_input.py` & `django-carbondesign-0.0.5/carbondesign/tags/text_input.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/tile.py` & `django-carbondesign-0.0.5/carbondesign/tags/tile.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/time_picker.py` & `django-carbondesign-0.0.5/carbondesign/tags/tooltip.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,182 +1,206 @@
 """
-Time Picker
-===========
+Tooltip
+=======
 
-See: https://the-carbon-components.netlify.app/?nav=time-picker
+See: https://www.carbondesignsystem.com/components/tooltip/usage/
 
+Tooltips display additional information upon click, hover, or focus. The
+information should be contextual, useful, and nonessential.
+
+Overview
+--------
+
+A tooltip is a message box that is displayed when a user hovers over, clicks
+or gives focus to a UI element such as an icon, a highlighted word, or a button.
 """ # pylint:disable=line-too-long
 # pylint:disable=too-many-lines
 
-from django.utils.translation import gettext as _
-import pytz
-#-
-from .base import FormNode
+from .base import Node, modify_svg
 
-class TimePicker(FormNode):
-    """Time Picker component.
+class BaseTooltip(Node):
+    """Base tooltip.
     """
-    NODE_PROPS = ('light', 'zones')
+    WANT_CHILDREN = True
+    "Template Tag needs closing end tag."
+    NODE_PROPS = ('id', 'align', 'position')
     "Extended Template Tag arguments."
-    CLASS_AND_PROPS = ('label', 'select')
-    "Prepare xxx_class and xxx_props values."
+    POSSIBLE_ALIGN = ('start', 'center', 'end')
+    "Documentation only."
+    POSSIBLE_POSITION = ('top', 'right', 'bottom', 'left')
+    "Documentation only."
 
     def prepare(self, values, context):
         """Prepare values for rendering the templates.
         """
-        values['txt_select_ampm'] = _("Select AM/PM")
-        values['txt_select_zone'] = _("Select time zone")
+        align = self.eval(self.kwargs.get('align'), context)
+        if align and align in self.POSSIBLE_ALIGN:
+            values['class'].append(f'bx--tooltip--align-{align}')
+
+        position = self.eval(self.kwargs.get('position'), context)
+        if position and position in self.POSSIBLE_POSITION:
+            values['class'].append(f'bx--tooltip--{position}')
+
+
+    def render_slot_icon(self, values, context):
+        """Render html of the slot.
+        """
+        return modify_svg(values['child'], {
+            'focusable': 'false',
+            'preserveAspectRatio': 'xMidYMid meet',
+            'fill': 'currentColor',
+            'style': {
+                'width': '16px',
+                'height': '16px',
+            },
+            'aria-hidden': 'true',
+        })
 
-        if self.eval(self.kwargs.get('disabled'), context):
-            values['label_class'].append('bx--label--disabled')
-            values['select_props'].append(('disabled', True))
-
-        if self.eval(self.kwargs.get('light'), context):
-            values['class'].append('bx--time-picker--light')
-            values['select_class'].append('bx--select--light')
 
+class Interactive(BaseTooltip):
+    """Tooltip component.
+    """
+    SLOTS = ('icon', 'footer', 'heading')
+    "Named children."
+    MODES = ('interactive', 'nolabel')
+    "Available variants."
+    REQUIRED_PROPS = ('label',)
+    "Will raise Exception if not set."
+    CLASS_AND_PROPS = ('label', 'content')
+    "Prepare xxx_class and xxx_props values."
 
-    def prepare_element_props(self, props, context):
-        """Prepare html attributes for rendering the form element.
+    def prepare(self, values, context):
+        """Prepare values for rendering the templates.
         """
-        props['class'].append('bx--text-input')
-        props['class'].append('bx--time-picker__input-field')
-        props['pattern'] = r'(1[012]|[1-9]):[0-5][0-9](\\s)?'
-        props['placeholder'] = 'hh:mm'
-        props['maxlength'] = "5"
-
-        if self.eval(self.kwargs.get('light'), context):
-            props['class'].append('bx--text-input--light')
+        if 'heading' in self.slots:
+            values['content_props'].append(
+                    ('aria-labelledby', 'heading-' + self._id))
+        elif self.mode == 'nolabel':
+            values['content_props'].append(('aria-label',
+                    values['label'] + values['label_suffix']))
+        else:
+            values['content_props'].append(
+                    ('aria-labelledby', 'label-' + self._id))
 
 
-    def render_default(self, values, context):
+    def render_interactive(self, values, context):
         """Output html of the component.
         """
-        light = self.eval(self.kwargs.get('light'), context)
-        if self.bound_field.errors:
-            if light:
-                template = """
-<div class="bx--form-item">
-  <div class="bx--time-picker {class}" data-invalid>
-    <div class="bx--time-picker__input">
-      {tmpl_label}
-      {tmpl_element}
-    </div>
-    {tmpl_select_ampm}
-    {tmpl_select_zone}
-  </div>
-  <div class="bx--form-requirement">
-    {tmpl_errors}
-  </div>
-  {tmpl_help}
-</div>
-"""
-            else:
-                template = """
-<div class="bx--form-item">
-  {tmpl_label}
-  <div class="bx--time-picker {class}" data-invalid>
-    <div class="bx--time-picker__input">{tmpl_element}</div>
-    {tmpl_select_ampm}
-    {tmpl_select_zone}
-  </div>
-  <div class="bx--form-requirement">
-    {tmpl_errors}
-  </div>
-  {tmpl_help}
-</div>
-"""
-        elif light and self.eval(self.kwargs.get('disabled'), context):
-            template = """
-<div class="bx--form-item">
-  <div class="bx--time-picker {class}">
-    <div class="bx--time-picker__input">
-      {tmpl_label}
-      {tmpl_element}
-    </div>
-    {tmpl_select_ampm}
-    {tmpl_select_zone}
+        template = """
+<div id="label-{id}" class="bx--tooltip__label">
+  {label}{label_suffix}
+  <button aria-expanded="false" aria-labelledby="label-{id}"
+      data-tooltip-trigger data-tooltip-target="#{id}"
+      class="bx--tooltip__trigger {class}" aria-controls="{id}" {props}>
+    {slot_icon}
+  </button>
+</div>
+<div id="{id}" aria-hidden="true" data-floating-menu-direction="bottom"
+    class="bx--tooltip">
+  <span class="bx--tooltip__caret"></span>
+  <div class="bx--tooltip__content {content_class}" tabindex="-1" role="dialog"
+      aria-describedby="body-{id}" {content_props}>
+    {slot_heading}
+    <p id="body-{id}">{child}</p>
+    {slot_footer}
   </div>
-  {tmpl_help}
+  <span tabindex="0"></span>
 </div>
 """
-        else:
-            template = """
-<div class="bx--form-item">
-  {tmpl_label}
-  <div class="bx--time-picker {class}">
-    <div class="bx--time-picker__input">{tmpl_element}</div>
-    {tmpl_select_ampm}
-    {tmpl_select_zone}
+        return self.format(template, values, context)
+
+
+    def render_nolabel(self, values, context):
+        """Output html of the component.
+        """
+        template = """
+<div id="label-{id}" class="bx--tooltip__label">
+  {label}{label_suffix}
+  <div tabindex="0" aria-expanded="false" aria-labelledby="label-{id}"
+      data-tooltip-trigger data-tooltip-target="#{id}"
+      role="button" class="bx--tooltip__trigger {class}" aria-controls="{id}" {props}>
+    {slot_icon}
+  </div>
+</div>
+<div id="{id}" aria-hidden="true" data-floating-menu-direction="bottom"
+    class="bx--tooltip">
+  <span class="bx--tooltip__caret"></span>
+  <div class="bx--tooltip__content {content_class}" tabindex="-1" role="dialog"
+      aria-describedby="body-{id}" {content_props}>
+    {slot_heading}
+    <p id="body-{id}">{child}</p>
+    {slot_footer}
   </div>
-  {tmpl_help}
+  <span tabindex="0"></span>
 </div>
 """
         return self.format(template, values, context)
 
 
-    def render_tmpl_select_ampm(self, values, context):
-        """Dynamically render a part of the component's template.
+    def render_slot_heading(self, values, context):
+        """Render html of the slot.
         """
         template = """
-<div class="bx--time-picker__select bx--select {select_class}">
-  <label for="select-ampm-{id}" class="bx--label bx--visually-hidden">
-    {txt_select_ampm}
-  </label>
-  <select id="select-ampm-{id}" class="bx--select-input" {select_props}>
-    <option class="bx--select-option" value="AM">AM</option>
-    <option class="bx--select-option" value="PM">PM</option>
-  </select>
-  <svg focusable="false" preserveAspectRatio="xMidYMid meet"
-      xmlns="http://www.w3.org/2000/svg" fill="currentColor"
-      class="bx--select__arrow" width="16" height="16" viewBox="0 0 16 16"
-      aria-hidden="true">
-    <path d="M8 11L3 6 3.7 5.3 8 9.6 12.3 5.3 13 6z"></path>
-  </svg>
+<h4 id="heading-{id}" class="bx--tooltip__heading {class}" {props}>{child}</h4>
+"""
+        return self.format(template, values)
+
+
+    def render_slot_footer(self, values, context):
+        """Render html of the slot.
+        """
+        template = """
+<div class="bx--tooltip__footer {class}" {props}>
+  {child}
 </div>
 """
         return self.format(template, values)
 
 
-    def render_tmpl_select_zone(self, values, context):
-        """Dynamically render a part of the component's template.
+class Definition(BaseTooltip):
+    """Tooltip component.
+    """
+    REQUIRED_PROPS = ('label',)
+    "Will raise Exception if not set."
+
+    def render_default(self, values, context):
+        """Output html of the component.
         """
         template = """
-<div class="bx--time-picker__select bx--select {select_class}">
-  <label for="select-zone-{id}" class="bx--label bx--visually-hidden">
-    {txt_select_zone}
-  </label>
-  <select id="select-zone-{id}" class="bx--select-input" {select_props}>
-    {tmpl_timezones}
-  </select>
-  <svg focusable="false" preserveAspectRatio="xMidYMid meet"
-      xmlns="http://www.w3.org/2000/svg" fill="currentColor"
-      class="bx--select__arrow" width="16" height="16" viewBox="0 0 16 16"
-      aria-hidden="true">
-    <path d="M8 11L3 6 3.7 5.3 8 9.6 12.3 5.3 13 6z"></path>
-  </svg>
+<div class="bx--tooltip--definition bx--tooltip--a11y" data-tooltip-definition>
+  <button aria-describedby="{id}"
+      class="bx--tooltip__trigger bx--tooltip--a11y bx--tooltip__trigger--definition {class}"
+      {props}>
+    {label}{label_suffix}
+  </button>
+  <div class="bx--assistive-text" id="{id}" role="tooltip">
+    {child}
+  </div>
 </div>
 """
-        return self.format(template, values, context)
+        return self.format(template, values)
 
 
-    def render_tmpl_timezones(self, values, context):
-        """Dynamically render a part of the component's template.
+class Icon(BaseTooltip):
+    """Tooltip component.
+    """
+    SLOTS = ('icon',)
+    "Named children."
+
+    def render_default(self, values, context):
+        """Output html of the component.
         """
         template = """
-<option class="bx--select-option" value="{value}">{label}</option>
+<button class="bx--tooltip__trigger bx--tooltip--a11y {class}"
+    data-tooltip-icon {props}>
+  <span class="bx--assistive-text">{child}</span>
+  {slot_icon}
+</button>
 """
-        timezones = self.eval(self.kwargs.get('zones',
-                pytz.common_timezones), context)
-        items = []
-        for zone in timezones:
-            if isinstance(zone, str):
-                value = label = zone
-            else:
-                value, label = zone
-            items.append(template.format(value=value, label=label))
-        return '\n'.join(items)
+        return self.format(template, values, context)
 
 
 components = {
-    'TimePicker': TimePicker,
+    'InteractiveTooltip': Interactive,
+    'DefinitionTooltip': Definition,
+    'IconTooltip': Icon,
 }
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/toggle.py` & `django-carbondesign-0.0.5/carbondesign/tags/toggle.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/toolbar.py` & `django-carbondesign-0.0.5/carbondesign/tags/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,16 @@
 
         return modify_svg(values['child'], {
             'focusable': 'false',
             'preserveAspectRatio': 'xMidYMid meet',
             'fill': 'currentColor',
             'class': ' '.join(classname),
             'style': {
-                'width': '%spx' % 16,
-                'height': '%spx' % 16,
+                'width': '16px',
+                'height': '16px',
             },
             'aria-hidden': 'true',
         })
 
 
 class ToolbarItemMultiSelect(FormNode):
     """Toolbar multi select item component.
@@ -150,15 +150,15 @@
 """
         items = []
 
         items.append(self.format(template_header, values))
 
         for ii, (_, val, txt) in enumerate(self.choices()):
             options = {
-                'id': '%s-%s' % (values['id'], ii),
+                'id': f"{values['id']}-{ii}",
                 'index': ii,
                 'value': val,
                 'child': txt,
                 'name': self.bound_field.name,
             }
             props = []
             if ii == 0:
@@ -209,15 +209,15 @@
     {child}
   </label>
 </li>
 """
         items = []
         for ii, (_, val, txt) in enumerate(self.choices()):
             options = {
-                'id': '%s-%s' % (values['id'], ii),
+                'id': f"{values['id']}-{ii}",
                 'index': ii,
                 'value': val,
                 'child': txt,
                 'name': self.bound_field.name,
             }
             props = []
             if ii == 0:
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/ui_shell.py` & `django-carbondesign-0.0.5/carbondesign/tags/ui_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         values['txt_skip_menu'] = _("Skip to main content")
         values['txt_open_menu'] = _("Open menu")
         values['txt_close_menu'] = _("Close menu")
 
         values['href'] = self.eval(self.kwargs.get('href', '#'), context)
 
         if 'label_prefix' in self.kwargs:
-            values['long_label'] = '%s %s' % (
+            values['long_label'] = '%s %s' % ( # pylint:disable=consider-using-f-string
                     self.eval(self.kwargs.get('label_prefix'), context),
                     values['label'])
         else:
             values['long_label'] = values['label']
 
 
     def render_default(self, values, context):
@@ -381,16 +381,16 @@
         """
         size = self.eval(self.kwargs.get('icon_size', 20), context)
         values['child'] = modify_svg(values['child'], {
             'focusable': 'false',
             'preserveAspectRatio': 'xMidYMid meet',
             'fill': 'currentColor',
             'style': {
-                'width': '%spx' % size,
-                'height': '%spx' % size,
+                'width': f'{size}px',
+                'height': f'{size}px',
             },
             'aria-hidden': 'true',
         })
 
         template = """
 <div class="bx--navigation-icon {class}" {props}>
   {child}
@@ -461,16 +461,16 @@
     def render_slot_title_icon(self, values, context):
         """Render html of the slot.
         """
         values['child'] = modify_svg(values['child'], {
             'preserveAspectRatio': 'xMidYMid meet',
             'fill': 'currentColor',
             'style': {
-                'width': '%spx' % 20,
-                'height': '%spx' % 20,
+                'width': '20px',
+                'height': '20px',
             },
             'aria-hidden': 'true',
         })
         template = """
 <div class="bx--side-nav__icon {class}">
   {child}
 </div>
@@ -640,16 +640,16 @@
         """Render html of the slot.
         """
         size = self.eval(self.kwargs.get('icon_size', 20), context)
         values['child'] = modify_svg(values['child'], {
             'preserveAspectRatio': 'xMidYMid meet',
             'fill': 'currentColor',
             'style': {
-                'width': '%spx' % size,
-                'height': '%spx' % size,
+                'width': f'{size}px',
+                'height': f'{size}px',
             },
             'aria-hidden': 'true',
         })
         template = """
 <div class="bx--side-nav__icon {class}" {props}>
   {child}
 </div>
```

### Comparing `django-carbondesign-0.0.4/carbondesign/tags/ui_shell_switcher.py` & `django-carbondesign-0.0.5/carbondesign/tags/ui_shell_switcher.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/carbondesign/templatetags/carbondesign.py` & `django-carbondesign-0.0.5/carbondesign/templatetags/carbondesign.py`

 * *Files identical despite different names*

### Comparing `django-carbondesign-0.0.4/django_carbondesign.egg-info/PKG-INFO` & `django-carbondesign-0.0.5/django_carbondesign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-carbondesign
-Version: 0.0.4
+Version: 0.0.5
 Summary: Carbon Design in Django templates
 Home-page: https://github.com/dozymoe/django-carbondesign
 Author: Fahri Reza
 Author-email: i@dozy.moe
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dozymoe/django-carbondesign/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-carbondesign-0.0.4/django_carbondesign.egg-info/SOURCES.txt` & `django-carbondesign-0.0.5/django_carbondesign.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 carbondesign/mithril-js/structured_list.js
 carbondesign/mithril-js/tabs.js
 carbondesign/mithril-js/tag.js
 carbondesign/mithril-js/text_area.js
 carbondesign/mithril-js/text_input.js
 carbondesign/mithril-js/tile.js
 carbondesign/mithril-js/time_picker.js
-carbondesign/mithril-js/timezones.json
 carbondesign/mithril-js/toggle.js
 carbondesign/mithril-js/toolbar.js
 carbondesign/mithril-js/tooltip.js
 carbondesign/mithril-js/uishell--action.js
 carbondesign/mithril-js/uishell--switcher.js
 carbondesign/mithril-js/uishell.js
 carbondesign/sass/_button.scss
@@ -143,12 +142,14 @@
 carbondesign/tags/toggle.py
 carbondesign/tags/toolbar.py
 carbondesign/tags/tooltip.py
 carbondesign/tags/ui_shell.py
 carbondesign/tags/ui_shell_switcher.py
 carbondesign/templatetags/__init__.py
 carbondesign/templatetags/carbondesign.py
+carbondesign/utils/__init__.py
+carbondesign/utils/formats.py
 django_carbondesign.egg-info/PKG-INFO
 django_carbondesign.egg-info/SOURCES.txt
 django_carbondesign.egg-info/dependency_links.txt
 django_carbondesign.egg-info/requires.txt
 django_carbondesign.egg-info/top_level.txt
```

### Comparing `django-carbondesign-0.0.4/setup.cfg` & `django-carbondesign-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-carbondesign
-version = 0.0.4
+version = 0.0.5
 description = Carbon Design in Django templates
 long_description = file: README.rst
 url = https://github.com/dozymoe/django-carbondesign
 author = Fahri Reza
 author_email = i@dozy.moe
 license = MIT
 project_urls =
```

