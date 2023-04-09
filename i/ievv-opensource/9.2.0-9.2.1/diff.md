# Comparing `tmp/ievv_opensource-9.2.0.tar.gz` & `tmp/ievv_opensource-9.2.1.tar.gz`

## Comparing `ievv_opensource-9.2.0.tar` & `ievv_opensource-9.2.1.tar`

### file list

```diff
@@ -1,249 +1,249 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/__init__.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/__init__.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/admin.py
--rw-r--r--   0        0        0    21232 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/batchregistry.py
--rw-r--r--   0        0        0    12943 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/models.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/rq_tasks.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/test_models.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/migrations/0001_initial.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/migrations/0002_auto_20160413_0154.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_customsql/__init__.py
--rw-r--r--   0        0        0    15485 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_customsql/customsql_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_customsql/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_customsql/management/commands/__init__.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_customsql/management/commands/ievvtasks_customsql.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_customsql/tests/__init__.py
--rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_customsql/tests/test_customsql_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_db/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_db/postgres/__init__.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_db/postgres/collate_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/__init__.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/admin.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/email_backend.py
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/management/commands/__init__.py
--rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/management/commands/ievv_developemail_send_testmail.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/migrations/__init__.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/templates/ievv_developemail/admin/as-html.django.html
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/templates/ievv_developemail/admin/as-plain.django.html
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/templates/ievv_developemail/admin/as-raw.django.html
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/templates/ievv_developemail/admin/base.django.html
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/templates/ievv_developemail/cradmin_email/html_message.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/tests/__init__.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/tests/test_develop_email_backend.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_djangoadmin/__init__.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_djangoadmin/ievv_djangoadmin_mixins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_djangoadmin/models.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_djangoadmin/templates/ievv_djangoadmin/ievv_djangoadmin_mixins/read_only_change_form.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/__init__.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/active_i18n_url_translation.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/base_url.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/i18n_url_settings.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/models.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/views.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/handlers/__init__.py
--rw-r--r--   0        0        0    25171 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/handlers/abstract_handler.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/handlers/django_session_handler.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/handlers/urlpath_prefix_handler.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/i18n_url_utils/__init__.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/i18n_url_utils/get_handler.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/i18n_url_utils/handler_shortcuts.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/i18n_url_utils/i18n_urlpatterns.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/templatetags/__init__.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/templatetags/ievv_i18n_url_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/__init__.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/test_base_url.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/models.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/urls.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/views.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/test_handlers/test_abstract_handler.py
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/test_handlers/test_urlpath_prefix_handler.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/__init__.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/admin.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/models.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/management/commands/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/management/commands/ievv_opensource_logging_items_delete_older_than_last_100.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/migrations/0001_initial.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/migrations/0002_auto_20191106_1310.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/migrations/0003_auto_20191123_1147.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/migrations/0004_auto_20191124_1953.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/migrations/0005_auto_20201112_1107.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/tests/__init__.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/tests/test_management_scripts.py
--rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_logging/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_model_mommy_extras/__init__.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_model_mommy_extras/apps.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_model_mommy_extras/postgres_field_generators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_restframework_helpers/__init__.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_restframework_helpers/full_clean_model_serializer.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_restframework_helpers/serializer_fields.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/__init__.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/admin.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/apps.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/models.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/phone_number_handler.py
--rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/sms_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/backends/__init__.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/backends/debug_dbstore.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/backends/debugprint.py
--rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/backends/pswin.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/backends/pswin_debug_dbstore.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/migrations/0001_initial.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/migrations/0002_debugsmsmessage_send_as.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/__init__.py
--rw-r--r--   0        0        0     9050 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_phone_number_handler.py
--rw-r--r--   0        0        0     6643 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_sms_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_backends/__init__.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_backends/test_abstract_sms_backend.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_backends/test_debug_dbstore.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_backends/test_pswin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/__init__.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/admin.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/models.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/tests/__init__.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/tests/test_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/base_command.py
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/models.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/open_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/management/commands/__init__.py
--rw-r--r--   0        0        0     6399 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_buildstatic.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_buildstatic_npmfreeze.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_generate_django_secret_key.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/tests/__init__.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/tests/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_compilemessages.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_devrun.py
--rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_docs.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_dump_db_as_sql.py
--rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_make_source_dist.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_makemessages.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_recreate_devdb.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_set_all_passwords_to_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_compilemessages.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_docs.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_dump_db_as_json.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_makemessages.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_set_all_passwords_to_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_production/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_production/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_production/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/ievvtasks_production/management/commands/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/__init__.py
--rw-r--r--   0        0        0    12294 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/choices_with_meta.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/class_registry_singleton.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/datetime_format.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/datetimeutils.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/i18n_noop.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievv_colorize.py
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievv_json.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievv_staticfiles_autogzip.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/lazy_static.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/lazy_string.py
--rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/logmixin.py
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/model_field_choices.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/progress_print_iterator.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/run_sh_command.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/secret_key.py
--rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/semantic_versioning_prompt.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/shellcommandmixin.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/singleton.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/text_utils.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/timer.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/validate_redirect_url.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/validation_error_util.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/virtualenvutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/desktopnotifications/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/desktopnotifications/base.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/desktopnotifications/desktopnotificationapi.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/desktopnotifications/linuxnotification.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/desktopnotifications/mocknotification.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/desktopnotifications/osxnotification.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/__init__.py
--rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/autosetup_esdoc.py
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/autosetup_jsdoc.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/bowerinstall.py
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/browserify_babelbuild.py
--rw-r--r--   0        0        0     8457 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/browserify_jsbuild.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/browserify_reactjsbuild.py
--rw-r--r--   0        0        0    12695 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/coffeebuild.py
--rw-r--r--   0        0        0    20507 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/config.py
--rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/cssbuildbaseplugin.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/filepath.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/gzip_compress_mixin.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/lessbuild.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/mediacopy.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/nodemodulescopy.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/npminstall.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/npmrun.py
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/npmrun_jsbuild.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/options_mixin.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/pluginbase.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/run_jstests.py
--rw-r--r--   0        0        0    10115 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/sassbuild.py
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/single_media_copy.py
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/typescriptbuild.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/utils.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/watcher.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/docbuilders/__init__.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/docbuilders/base.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/docbuilders/npm_docbuilder.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/installers/__init__.py
--rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/installers/abstract_npm_installer.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/installers/base.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/installers/npm.py
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/installers/yarn.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/__init__.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/config.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/__init__.py
--rw-r--r--   0        0        0     7750 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/base.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/celery_worker.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/dbdev_runserver.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/django_runserver.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/ievv_buildstatic.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/redis_server.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/rq_worker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/testhelpers/__init__.py
--rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/testhelpers/testmigrations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/tests/__init__.py
--rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_choices_with_meta.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_ievv_json.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_textutils.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_validate_redirect_url.py
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_validation_error_util.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_virtualenvutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_text/__init__.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_text/test_ievv_slugify.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/text/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/ievv_opensource/utils/text/ievv_slugify.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/.gitignore
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/LICENSE
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/README.md
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/pyproject.toml
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 ievv_opensource-9.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/__init__.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/__init__.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/admin.py
+-rw-r--r--   0        0        0    21232 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/batchregistry.py
+-rw-r--r--   0        0        0    12943 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/models.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/rq_tasks.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/test_models.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/migrations/0001_initial.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/migrations/0002_auto_20160413_0154.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_customsql/__init__.py
+-rw-r--r--   0        0        0    15485 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_customsql/customsql_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_customsql/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_customsql/management/commands/__init__.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_customsql/management/commands/ievvtasks_customsql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_customsql/tests/__init__.py
+-rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_customsql/tests/test_customsql_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_db/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_db/postgres/__init__.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_db/postgres/collate_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/__init__.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/admin.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/email_backend.py
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/management/commands/__init__.py
+-rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/management/commands/ievv_developemail_send_testmail.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/migrations/__init__.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/templates/ievv_developemail/admin/as-html.django.html
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/templates/ievv_developemail/admin/as-plain.django.html
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/templates/ievv_developemail/admin/as-raw.django.html
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/templates/ievv_developemail/admin/base.django.html
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/templates/ievv_developemail/cradmin_email/html_message.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/tests/__init__.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/tests/test_develop_email_backend.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_djangoadmin/__init__.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_djangoadmin/ievv_djangoadmin_mixins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_djangoadmin/models.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_djangoadmin/templates/ievv_djangoadmin/ievv_djangoadmin_mixins/read_only_change_form.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/__init__.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/active_i18n_url_translation.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/base_url.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/i18n_url_settings.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/models.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/views.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/handlers/__init__.py
+-rw-r--r--   0        0        0    25171 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/handlers/abstract_handler.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/handlers/django_session_handler.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/handlers/urlpath_prefix_handler.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/i18n_url_utils/__init__.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/i18n_url_utils/get_handler.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/i18n_url_utils/handler_shortcuts.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/i18n_url_utils/i18n_urlpatterns.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/templatetags/__init__.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/templatetags/ievv_i18n_url_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/__init__.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/test_base_url.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/models.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/urls.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/views.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/test_handlers/test_abstract_handler.py
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/test_handlers/test_urlpath_prefix_handler.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/__init__.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/admin.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/models.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/management/commands/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/management/commands/ievv_opensource_logging_items_delete_older_than_last_100.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/migrations/0002_auto_20191106_1310.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/migrations/0003_auto_20191123_1147.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/migrations/0004_auto_20191124_1953.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/migrations/0005_auto_20201112_1107.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/tests/__init__.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/tests/test_management_scripts.py
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_logging/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_model_mommy_extras/__init__.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_model_mommy_extras/apps.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_model_mommy_extras/postgres_field_generators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_restframework_helpers/__init__.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_restframework_helpers/full_clean_model_serializer.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_restframework_helpers/serializer_fields.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/__init__.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/admin.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/apps.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/models.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/phone_number_handler.py
+-rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/sms_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/backends/__init__.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/backends/debug_dbstore.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/backends/debugprint.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/backends/pswin.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/backends/pswin_debug_dbstore.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/migrations/0001_initial.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/migrations/0002_debugsmsmessage_send_as.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/__init__.py
+-rw-r--r--   0        0        0     9050 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_phone_number_handler.py
+-rw-r--r--   0        0        0     6643 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_sms_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_backends/__init__.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_backends/test_abstract_sms_backend.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_backends/test_debug_dbstore.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_backends/test_pswin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/__init__.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/admin.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/models.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/tests/__init__.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/tests/test_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/base_command.py
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/models.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/open_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/management/commands/__init__.py
+-rw-r--r--   0        0        0     6399 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_buildstatic.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_buildstatic_npmfreeze.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_generate_django_secret_key.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/tests/__init__.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_compilemessages.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_devrun.py
+-rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_docs.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_dump_db_as_sql.py
+-rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_make_source_dist.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_makemessages.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_recreate_devdb.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_set_all_passwords_to_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_compilemessages.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_docs.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_dump_db_as_json.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_makemessages.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_set_all_passwords_to_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_production/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_production/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_production/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/ievvtasks_production/management/commands/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/__init__.py
+-rw-r--r--   0        0        0    12294 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/choices_with_meta.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/class_registry_singleton.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/datetime_format.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/datetimeutils.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/i18n_noop.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievv_colorize.py
+-rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievv_json.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievv_staticfiles_autogzip.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/lazy_static.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/lazy_string.py
+-rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/logmixin.py
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/model_field_choices.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/progress_print_iterator.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/run_sh_command.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/secret_key.py
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/semantic_versioning_prompt.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/shellcommandmixin.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/singleton.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/text_utils.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/timer.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/validate_redirect_url.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/validation_error_util.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/virtualenvutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/desktopnotifications/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/desktopnotifications/base.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/desktopnotifications/desktopnotificationapi.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/desktopnotifications/linuxnotification.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/desktopnotifications/mocknotification.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/desktopnotifications/osxnotification.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/__init__.py
+-rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/autosetup_esdoc.py
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/autosetup_jsdoc.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/bowerinstall.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/browserify_babelbuild.py
+-rw-r--r--   0        0        0     8457 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/browserify_jsbuild.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/browserify_reactjsbuild.py
+-rw-r--r--   0        0        0    12695 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/coffeebuild.py
+-rw-r--r--   0        0        0    20507 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/config.py
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/cssbuildbaseplugin.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/filepath.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/gzip_compress_mixin.py
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/lessbuild.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/mediacopy.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/nodemodulescopy.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/npminstall.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/npmrun.py
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/npmrun_jsbuild.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/options_mixin.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/pluginbase.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/run_jstests.py
+-rw-r--r--   0        0        0    10115 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/sassbuild.py
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/single_media_copy.py
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/typescriptbuild.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/utils.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/watcher.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/docbuilders/__init__.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/docbuilders/base.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/docbuilders/npm_docbuilder.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/installers/__init__.py
+-rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/installers/abstract_npm_installer.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/installers/base.py
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/installers/npm.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/installers/yarn.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/config.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/__init__.py
+-rw-r--r--   0        0        0     7750 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/base.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/celery_worker.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/dbdev_runserver.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/django_runserver.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/ievv_buildstatic.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/redis_server.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/rq_worker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/testhelpers/__init__.py
+-rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/testhelpers/testmigrations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/tests/__init__.py
+-rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_choices_with_meta.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_ievv_json.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_textutils.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_validate_redirect_url.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_validation_error_util.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_virtualenvutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_text/__init__.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_text/test_ievv_slugify.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/text/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/ievv_opensource/utils/text/ievv_slugify.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/.gitignore
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/LICENSE
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/README.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 ievv_opensource-9.2.1/PKG-INFO
```

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/admin.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/admin.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/batchregistry.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/batchregistry.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/models.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/models.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/rq_tasks.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/rq_tasks.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/test_models.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/test_models.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_batchframework/migrations/0001_initial.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_batchframework/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_customsql/customsql_registry.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_customsql/customsql_registry.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_customsql/management/commands/ievvtasks_customsql.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_customsql/management/commands/ievvtasks_customsql.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_customsql/tests/test_customsql_registry.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_customsql/tests/test_customsql_registry.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_db/postgres/collate_utils.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_db/postgres/collate_utils.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/admin.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/admin.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/email_backend.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/email_backend.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/models.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/models.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/management/commands/ievv_developemail_send_testmail.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/management/commands/ievv_developemail_send_testmail.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/migrations/0001_initial.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/templates/ievv_developemail/admin/base.django.html` & `ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/templates/ievv_developemail/admin/base.django.html`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_developemail/tests/test_develop_email_backend.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_developemail/tests/test_develop_email_backend.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_djangoadmin/ievv_djangoadmin_mixins.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_djangoadmin/ievv_djangoadmin_mixins.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/active_i18n_url_translation.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/active_i18n_url_translation.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/base_url.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/base_url.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/i18n_url_settings.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/i18n_url_settings.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/middleware.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/middleware.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/handlers/abstract_handler.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/handlers/abstract_handler.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/handlers/django_session_handler.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/handlers/django_session_handler.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/handlers/urlpath_prefix_handler.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/handlers/urlpath_prefix_handler.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/i18n_url_utils/get_handler.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/i18n_url_utils/get_handler.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/i18n_url_utils/handler_shortcuts.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/i18n_url_utils/handler_shortcuts.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/i18n_url_utils/i18n_urlpatterns.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/i18n_url_utils/i18n_urlpatterns.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/templatetags/ievv_i18n_url_tags.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/templatetags/ievv_i18n_url_tags.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/test_base_url.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/test_base_url.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/urls.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/urls.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/de/LC_MESSAGES/django.mo` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/de/LC_MESSAGES/django.po` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/en/LC_MESSAGES/django.po` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/nb/LC_MESSAGES/django.mo` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/nb/LC_MESSAGES/django.po` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/ievv_i18n_url_testapp/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/test_handlers/test_abstract_handler.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/test_handlers/test_abstract_handler.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_i18n_url/tests/test_handlers/test_urlpath_prefix_handler.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_i18n_url/tests/test_handlers/test_urlpath_prefix_handler.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/README.md` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/README.md`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/admin.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/admin.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/models.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/models.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/utils.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/utils.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/management/commands/ievv_opensource_logging_items_delete_older_than_last_100.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/management/commands/ievv_opensource_logging_items_delete_older_than_last_100.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/migrations/0001_initial.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/migrations/0002_auto_20191106_1310.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/migrations/0002_auto_20191106_1310.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/migrations/0003_auto_20191123_1147.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/migrations/0003_auto_20191123_1147.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/migrations/0004_auto_20191124_1953.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/migrations/0004_auto_20191124_1953.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/tests/test_management_scripts.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/tests/test_management_scripts.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_logging/tests/test_utils.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_logging/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_model_mommy_extras/postgres_field_generators.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_model_mommy_extras/postgres_field_generators.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_restframework_helpers/full_clean_model_serializer.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_restframework_helpers/full_clean_model_serializer.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_restframework_helpers/serializer_fields.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_restframework_helpers/serializer_fields.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/admin.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/admin.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/apps.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/apps.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/phone_number_handler.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/phone_number_handler.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/sms_registry.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/sms_registry.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/backends/debug_dbstore.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/backends/debug_dbstore.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/backends/debugprint.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/backends/debugprint.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/backends/pswin.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/backends/pswin.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/backends/pswin_debug_dbstore.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/backends/pswin_debug_dbstore.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/migrations/0001_initial.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_phone_number_handler.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_phone_number_handler.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_sms_registry.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_sms_registry.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_backends/test_abstract_sms_backend.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_backends/test_abstract_sms_backend.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_backends/test_debug_dbstore.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_backends/test_debug_dbstore.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_sms/tests/test_backends/test_pswin.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_sms/tests/test_backends/test_pswin.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/admin.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/admin.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/models.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/models.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/migrations/0001_initial.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievv_tagframework/tests/test_models.py` & `ievv_opensource-9.2.1/ievv_opensource/ievv_tagframework/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/base_command.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/base_command.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/cli.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/cli.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_buildstatic.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_buildstatic.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_buildstatic_npmfreeze.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_buildstatic_npmfreeze.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_generate_django_secret_key.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/management/commands/ievvtasks_generate_django_secret_key.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_common/tests/test_cli.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_common/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_compilemessages.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_compilemessages.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_devrun.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_devrun.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_docs.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_docs.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_dump_db_as_sql.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_dump_db_as_sql.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_make_source_dist.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_make_source_dist.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_makemessages.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_makemessages.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_recreate_devdb.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/management/commands/ievvtasks_recreate_devdb.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_compilemessages.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_compilemessages.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_docs.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_docs.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_dump_db_as_json.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_dump_db_as_json.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_makemessages.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_makemessages.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_set_all_passwords_to_test.py` & `ievv_opensource-9.2.1/ievv_opensource/ievvtasks_development/tests/test_ievvtasks_set_all_passwords_to_test.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/choices_with_meta.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/choices_with_meta.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/class_registry_singleton.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/class_registry_singleton.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/datetime_format.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/datetime_format.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/datetimeutils.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/datetimeutils.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievv_colorize.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievv_colorize.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievv_json.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievv_json.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievv_staticfiles_autogzip.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievv_staticfiles_autogzip.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/logmixin.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/logmixin.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/model_field_choices.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/model_field_choices.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/progress_print_iterator.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/progress_print_iterator.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/run_sh_command.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/run_sh_command.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,25 +2,31 @@
 import shlex
 import shutil
 import subprocess
 import sys
 import typing
 
 
-def _parse_command_kwargs(**kwargs):
+def _parse_command_kwargs(_kwargs_equals_encode=False, **kwargs):
     args = []
     for key, value in kwargs.items():
         if len(key) == 1:
             argkey = f'-{key}'
         else:
             argkey = f'--{key.replace("_", "-")}'
         if value not in (False, None):
-            args.append(argkey)
-            if value != True:
-                args.append(f'{value}')
+            if _kwargs_equals_encode and argkey.startswith('--'):
+                if value == True:
+                    args.append(argkey)
+                else:
+                    args.append(f'{argkey}={value}')
+            else:
+                args.append(argkey)
+                if value != True:
+                    args.append(f'{value}')
     return args
 
 
 def _default_out_handler(line):
     print(line, flush=True)
 
 
@@ -49,28 +55,29 @@
         executable: str,
         args: typing.Optional[list] = None,
         kwargs: typing.Optional[dict] = None,
         env: typing.Optional[dict] = None,
         cwd: typing.Optional[str] = None,
         output_handler = _default_out_handler,
         failure_output_checker = None,
-        background:bool = False):
+        background:bool = False,
+        kwargs_equals_encode:bool = False):
     """
     Run executable.
 
     This is made to make transitioning from https://amoffat.github.io/sh/ easier,
     so the kwargs are fairly compatible.
     """
     failure_output_checker = failure_output_checker or _default_failure_output_checker
     args = args or []
     kwargs = kwargs or {}
     full_args = [
         shutil.which(executable),
         *args,
-        *_parse_command_kwargs(**kwargs)
+        *_parse_command_kwargs(**kwargs, _kwargs_equals_encode=kwargs_equals_encode)
     ]
     popen_kwargs = {
         'args': full_args,
         'shell': False,
         'env': env,
         'cwd': cwd
     }
```

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/semantic_versioning_prompt.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/semantic_versioning_prompt.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/shellcommandmixin.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/shellcommandmixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         if _cwd:
             output.insert(0, '[CWD={}]'.format(_cwd))
 
         return ' '.join(output)
 
     def run_shell_command(self, executable, args=None, kwargs=None, _cwd=None,
                           _out=None, _err=None, _env=None, _failure_output_checker=None,
-                          _background=False):
+                          _background=False, _kwargs_equals_encode=False):
         """
         Run a shell command.
 
         Parameters:
             executable: The name or path of the executable.
             args: List of arguments for the ``sh.Command`` object.
             kwargs: Dict of keyword arguments for the ``sh.Command`` object.
@@ -96,15 +96,16 @@
                 executable=executable,
                 args=args,
                 kwargs=kwargs,
                 cwd=_cwd,
                 env=_env,
                 output_handler=_out,
                 failure_output_checker=_failure_output_checker,
-                background=_background)
+                background=_background,
+                kwargs_equals_encode=_kwargs_equals_encode)
         except run_sh_command.RunExecutableError as e:
             # We do not need to show any more errors here - they
             # have already been printed by the _out and _err handlers.
             if self.fatal_shell_command_errors:
                 raise ShellCommandFatalError(str(e))
             else:
                 raise ShellCommandError(str(e))
```

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/singleton.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/timer.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/validate_redirect_url.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/validate_redirect_url.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/validation_error_util.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/validation_error_util.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/virtualenvutils.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/virtualenvutils.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/desktopnotifications/desktopnotificationapi.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/desktopnotifications/desktopnotificationapi.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/__init__.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/__init__.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/autosetup_esdoc.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/autosetup_esdoc.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/autosetup_jsdoc.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/autosetup_jsdoc.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/bowerinstall.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/bowerinstall.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/browserify_babelbuild.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/browserify_babelbuild.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/browserify_jsbuild.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/browserify_jsbuild.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/browserify_reactjsbuild.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/browserify_reactjsbuild.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/coffeebuild.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/coffeebuild.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/config.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/config.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/cssbuildbaseplugin.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/cssbuildbaseplugin.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/filepath.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/filepath.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/gzip_compress_mixin.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/gzip_compress_mixin.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/lessbuild.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/lessbuild.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,15 +111,16 @@
             self.get_logger().info('Using --include-path={}'.format(less_include_paths))
         try:
             self.run_shell_command(executable,
                                    args=[
                                        self.get_sourcefile_path(),
                                        self.get_destinationfile_path()
                                    ],
-                                   kwargs=kwargs)
+                                   kwargs=kwargs,
+                                   _kwargs_equals_encode=True)
         except ShellCommandError:
             self.get_logger().command_error('LESS build FAILED!')
         else:
             self.get_logger().command_success('LESS build successful :)')
 
     def get_watch_folders(self):
         """
```

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/mediacopy.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/mediacopy.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/nodemodulescopy.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/nodemodulescopy.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/npminstall.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/npminstall.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/npmrun.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/npmrun.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/npmrun_jsbuild.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/npmrun_jsbuild.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/pluginbase.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/pluginbase.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/run_jstests.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/run_jstests.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/sassbuild.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/sassbuild.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/single_media_copy.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/single_media_copy.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/typescriptbuild.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/typescriptbuild.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/utils.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/utils.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/watcher.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/watcher.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/docbuilders/base.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/docbuilders/base.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/docbuilders/npm_docbuilder.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/docbuilders/npm_docbuilder.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/installers/abstract_npm_installer.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/installers/abstract_npm_installer.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/installers/base.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/installers/base.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/installers/npm.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/installers/npm.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvbuildstatic/installers/yarn.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvbuildstatic/installers/yarn.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/config.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/config.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/base.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/base.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/celery_worker.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/celery_worker.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/dbdev_runserver.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/dbdev_runserver.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/django_runserver.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/django_runserver.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/ievv_buildstatic.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/ievv_buildstatic.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/redis_server.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/redis_server.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/ievvdevrun/runnables/rq_worker.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/ievvdevrun/runnables/rq_worker.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/testhelpers/testmigrations.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/testhelpers/testmigrations.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_choices_with_meta.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_choices_with_meta.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_ievv_json.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_ievv_json.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_textutils.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_textutils.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_validate_redirect_url.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_validate_redirect_url.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_validation_error_util.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_validation_error_util.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_virtualenvutils.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_virtualenvutils.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/tests/test_text/test_ievv_slugify.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/tests/test_text/test_ievv_slugify.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/ievv_opensource/utils/text/ievv_slugify.py` & `ievv_opensource-9.2.1/ievv_opensource/utils/text/ievv_slugify.py`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/.gitignore` & `ievv_opensource-9.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/LICENSE` & `ievv_opensource-9.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ievv_opensource-9.2.0/README.md` & `ievv_opensource-9.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -111,52 +111,24 @@
 
 ### NOTE (release):
 - `cz bump` automatically updates CHANGELOG.md, updates version file(s), commits the change and tags the release commit.
 - If you are unsure about what `cz bump` will do, run it with `--dry-run`. You can use
   options to force a specific version instead of the one it automatically selects
   from the git log if needed, BUT if this is needed, it is a sign that someone has messed
   up with their conventional commits.
-- When you push, the Azure devops pipeline will take care of the rest. It will see the
-  ``bump: version ...`` commit, and release the python package to the artifact registry.
 - ``cz bump`` only works if conventional commits (see section about that above) is used.
 - ``cz bump`` can take a specific version etc, but it automatically select the correct version
   if conventional commits has been used correctly. See https://commitizen-tools.github.io/commitizen/.
 - If you need to add more to CHANGELOG.md (migration guide, etc), you can just edit
   CHANGELOG.md after the release, and commit the change with a `docs: some useful message`
   commit.
 - The ``cz`` command comes from ``commitizen`` (install documented above).
 
 ### What if the release fails?
 See _How to revert a bump_ in the [commitizen FAQ](https://commitizen-tools.github.io/commitizen/faq/#how-to-revert-a-bump).
 
-### Skipping tests on release
-Why?:
-- You may need to just get a release out even if a test or 2 is breaking. This may be
-  tests that is just not that important, but be very careful making this choice.
-- You may have just run all the tests, and just added a bit more docs or something
-  before the release.
-
-To release without running tests, you first need to find the current and next version.
-So run:
-```
-$ cz bump --dry-run
-```
-and take a look at the first few lines of the output. You can normally
-just copy the first line of the output (``bump: version ...``)
-into the command below...
-
-
-Now you can release with a custom message like this:
-```
-$ cz bump --bump-message "bump: version <CURRENT-VERSION> → <NEXT-VERSION> [skip tests]"
-$ git push && git push --tags
-```
-_NOTE:_ The important part here is that the message starts with ``bump: version``, and contains ``[skip tests]``.
-The prefix is required to trigger the release stages of the CI/CD pipeline, and the ``[skip tests]``
-flag tells the pipeline to skip the tests.
-
 ### Release to pypi:
 ```
 $ hatch build -t sdist
 $ hatch publish
 $ rm dist/*              # optional cleanup
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ievv_opensource-9.2.0/pyproject.toml` & `ievv_opensource-9.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -63,23 +63,23 @@
 [project.scripts]
 ievv = "ievv_opensource.ievvtasks_common.cli:cli"
 
 [tool.hatch.version]
 path = "ievv_opensource/__init__.py"
 
 [tool.hatch.build]
-include = [
+packages = [
     "/ievv_opensource"
 ]
 exclude = [
     "/ievv_opensource/demo",
     "node_modules"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "9.2.0"
+version = "9.2.1"
 version_files = [
     "ievv_opensource/__init__.py:__version__"
 ]
 tag_format = "$version"
 update_changelog_on_bump = true
```

### Comparing `ievv_opensource-9.2.0/PKG-INFO` & `ievv_opensource-9.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ievv-opensource
-Version: 9.2.0
+Version: 9.2.1
 Summary: The opensource modules from the commercial IEVV Django framework.
 Author: Tor Johansen, Magne Westlie
 Author-email: Espen Angell Kristiansen <post@appresso.no>
 License: Copyright (c) 2015, Appresso AS
         All rights reserved. 
         
         Redistribution and use in source and binary forms, with or without 
@@ -184,52 +184,24 @@
 
 ### NOTE (release):
 - `cz bump` automatically updates CHANGELOG.md, updates version file(s), commits the change and tags the release commit.
 - If you are unsure about what `cz bump` will do, run it with `--dry-run`. You can use
   options to force a specific version instead of the one it automatically selects
   from the git log if needed, BUT if this is needed, it is a sign that someone has messed
   up with their conventional commits.
-- When you push, the Azure devops pipeline will take care of the rest. It will see the
-  ``bump: version ...`` commit, and release the python package to the artifact registry.
 - ``cz bump`` only works if conventional commits (see section about that above) is used.
 - ``cz bump`` can take a specific version etc, but it automatically select the correct version
   if conventional commits has been used correctly. See https://commitizen-tools.github.io/commitizen/.
 - If you need to add more to CHANGELOG.md (migration guide, etc), you can just edit
   CHANGELOG.md after the release, and commit the change with a `docs: some useful message`
   commit.
 - The ``cz`` command comes from ``commitizen`` (install documented above).
 
 ### What if the release fails?
 See _How to revert a bump_ in the [commitizen FAQ](https://commitizen-tools.github.io/commitizen/faq/#how-to-revert-a-bump).
 
-### Skipping tests on release
-Why?:
-- You may need to just get a release out even if a test or 2 is breaking. This may be
-  tests that is just not that important, but be very careful making this choice.
-- You may have just run all the tests, and just added a bit more docs or something
-  before the release.
-
-To release without running tests, you first need to find the current and next version.
-So run:
-```
-$ cz bump --dry-run
-```
-and take a look at the first few lines of the output. You can normally
-just copy the first line of the output (``bump: version ...``)
-into the command below...
-
-
-Now you can release with a custom message like this:
-```
-$ cz bump --bump-message "bump: version <CURRENT-VERSION> → <NEXT-VERSION> [skip tests]"
-$ git push && git push --tags
-```
-_NOTE:_ The important part here is that the message starts with ``bump: version``, and contains ``[skip tests]``.
-The prefix is required to trigger the release stages of the CI/CD pipeline, and the ``[skip tests]``
-flag tells the pipeline to skip the tests.
-
 ### Release to pypi:
 ```
 $ hatch build -t sdist
 $ hatch publish
 $ rm dist/*              # optional cleanup
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

