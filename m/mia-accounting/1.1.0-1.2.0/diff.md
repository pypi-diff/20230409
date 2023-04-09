# Comparing `tmp/mia-accounting-1.1.0.tar.gz` & `tmp/mia-accounting-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.1.0.tar", last modified: Sat Apr  8 16:49:29 2023, max compression
+gzip compressed data, was "mia-accounting-1.2.0.tar", last modified: Sun Apr  9 04:17:12 2023, max compression
```

## Comparing `mia-accounting-1.1.0.tar` & `mia-accounting-1.2.0.tar`

### file list

```diff
@@ -1,303 +1,303 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.602893 mia-accounting-1.1.0/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.1.0/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.1.0/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     7024 2023-04-08 16:49:29.602893 mia-accounting-1.1.0/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     6225 2023-04-06 02:00:23.000000 mia-accounting-1.1.0/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.482895 mia-accounting-1.1.0/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.1.0/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.1.0/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.482895 mia-accounting-1.1.0/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.482895 mia-accounting-1.1.0/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.1.0/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.482895 mia-accounting-1.1.0/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.1.0/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-08 16:40:32.000000 mia-accounting-1.1.0/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-08 16:40:32.000000 mia-accounting-1.1.0/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1186 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-08 16:40:32.000000 mia-accounting-1.1.0/docs/source/accounting.unmatched_offset.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-08 16:40:32.000000 mia-accounting-1.1.0/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-08 16:46:46.000000 mia-accounting-1.1.0/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.1.0/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.1.0/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.1.0/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3969 2023-04-06 02:00:11.000000 mia-accounting-1.1.0/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.1.0/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-08 16:46:46.000000 mia-accounting-1.1.0/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-08 16:49:29.602893 mia-accounting-1.1.0/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     2981 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1254 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     5589 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.1.0/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7424 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1296 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2018 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1813 2023-04-06 08:06:37.000000 mia-accounting-1.1.0/src/accounting/base_account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1365 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3286 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6616 2023-04-06 08:06:37.000000 mia-accounting-1.1.0/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.1.0/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.1.0/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.1.0/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3345 2023-04-07 07:30:13.000000 mia-accounting-1.1.0/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.490895 mia-accounting-1.1.0/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.1.0/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.1.0/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.490895 mia-accounting-1.1.0/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9480 2023-04-04 23:58:41.000000 mia-accounting-1.1.0/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.1.0/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.490895 mia-accounting-1.1.0/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.1.0/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.490895 mia-accounting-1.1.0/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.1.0/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.1.0/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.490895 mia-accounting-1.1.0/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.494895 mia-accounting-1.1.0/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.1.0/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.1.0/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.1.0/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8362 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.1.0/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.1.0/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.494895 mia-accounting-1.1.0/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.1.0/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4569 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    10748 2023-04-08 10:12:56.000000 mia-accounting-1.1.0/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.494895 mia-accounting-1.1.0/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.494895 mia-accounting-1.1.0/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.1.0/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3036 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/unapplied.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/templates/accounting/unmatched-offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/unmatched-offset/dashboard.html
--rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/unmatched-offset/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 16:22:08.000000 mia-accounting-1.1.0/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.1.0/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15685 2023-04-08 16:37:13.000000 mia-accounting-1.1.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52091 2023-04-08 16:37:13.000000 mia-accounting-1.1.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15685 2023-04-08 16:37:13.000000 mia-accounting-1.1.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52091 2023-04-08 16:39:46.000000 mia-accounting-1.1.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/unmatched_offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/unmatched_offset/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/unmatched_offset/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/unmatched_offset/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.510894 mia-accounting-1.1.0/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.1.0/src/accounting/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.510894 mia-accounting-1.1.0/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     7024 2023-04-08 16:49:29.000000 mia-accounting-1.1.0/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11343 2023-04-08 16:49:29.000000 mia-accounting-1.1.0/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-08 16:49:29.000000 mia-accounting-1.1.0/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-08 16:49:29.000000 mia-accounting-1.1.0/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-08 16:49:29.000000 mia-accounting-1.1.0/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.514894 mia-accounting-1.1.0/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    35927 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     5034 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)    27074 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    16847 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   106499 2023-04-04 23:59:18.000000 mia-accounting-1.1.0/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    33566 2023-04-08 16:39:46.000000 mia-accounting-1.1.0/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    34728 2023-04-08 16:39:46.000000 mia-accounting-1.1.0/tests/test_offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)    16853 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/tests/test_option.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.514894 mia-accounting-1.1.0/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4143 2023-04-04 23:16:14.000000 mia-accounting-1.1.0/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2861 2023-04-04 09:28:44.000000 mia-accounting-1.1.0/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.1.0/tests/test_site/locale.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.514894 mia-accounting-1.1.0/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.1.0/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.514894 mia-accounting-1.1.0/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6015 2023-04-05 18:00:22.000000 mia-accounting-1.1.0/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)      812 2023-04-04 10:04:53.000000 mia-accounting-1.1.0/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1419 2023-04-04 10:04:53.000000 mia-accounting-1.1.0/tests/test_site/templates/login.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.514894 mia-accounting-1.1.0/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.1.0/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     1307 2023-04-05 18:34:06.000000 mia-accounting-1.1.0/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.578893 mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:34:39.000000 mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.602893 mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:55:17.000000 mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)     3792 2023-04-04 09:21:33.000000 mia-accounting-1.1.0/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/tests/testlib_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    13639 2023-04-08 16:39:46.000000 mia-accounting-1.1.0/tests/testlib_offset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.844457 mia-accounting-1.2.0/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.2.0/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.2.0/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     7024 2023-04-09 04:17:12.844457 mia-accounting-1.2.0/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     6225 2023-04-06 02:00:23.000000 mia-accounting-1.2.0/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.808458 mia-accounting-1.2.0/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.2.0/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.2.0/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.812458 mia-accounting-1.2.0/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.812458 mia-accounting-1.2.0/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.2.0/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.812458 mia-accounting-1.2.0/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.2.0/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-08 16:40:31.000000 mia-accounting-1.2.0/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-08 16:40:31.000000 mia-accounting-1.2.0/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-08 16:40:31.000000 mia-accounting-1.2.0/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-08 16:40:31.000000 mia-accounting-1.2.0/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-08 16:40:31.000000 mia-accounting-1.2.0/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-08 16:40:31.000000 mia-accounting-1.2.0/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-08 16:40:31.000000 mia-accounting-1.2.0/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-08 16:40:31.000000 mia-accounting-1.2.0/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-08 16:40:32.000000 mia-accounting-1.2.0/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-08 16:40:31.000000 mia-accounting-1.2.0/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-08 16:40:32.000000 mia-accounting-1.2.0/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1186 2023-04-08 16:40:31.000000 mia-accounting-1.2.0/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-08 16:40:32.000000 mia-accounting-1.2.0/docs/source/accounting.unmatched_offset.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-08 16:40:32.000000 mia-accounting-1.2.0/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-09 04:15:59.000000 mia-accounting-1.2.0/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.2.0/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.2.0/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.2.0/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3969 2023-04-06 02:00:11.000000 mia-accounting-1.2.0/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.2.0/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-09 04:15:59.000000 mia-accounting-1.2.0/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-09 04:17:12.844457 mia-accounting-1.2.0/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.808458 mia-accounting-1.2.0/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.812458 mia-accounting-1.2.0/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     2981 2023-04-08 10:12:57.000000 mia-accounting-1.2.0/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.812458 mia-accounting-1.2.0/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1254 2023-04-04 09:21:36.000000 mia-accounting-1.2.0/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5589 2023-04-08 10:12:57.000000 mia-accounting-1.2.0/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.2.0/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.2.0/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.816458 mia-accounting-1.2.0/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1296 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2018 2023-04-04 09:21:36.000000 mia-accounting-1.2.0/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.2.0/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.2.0/src/accounting/base_account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.816458 mia-accounting-1.2.0/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1365 2023-04-04 09:21:36.000000 mia-accounting-1.2.0/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3286 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.2.0/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.2.0/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.816458 mia-accounting-1.2.0/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.2.0/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.2.0/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.2.0/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.816458 mia-accounting-1.2.0/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3345 2023-04-07 07:30:13.000000 mia-accounting-1.2.0/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.816458 mia-accounting-1.2.0/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.2.0/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.2.0/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.2.0/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.2.0/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.2.0/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.816458 mia-accounting-1.2.0/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.2.0/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.2.0/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.2.0/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.2.0/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.2.0/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.2.0/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.820458 mia-accounting-1.2.0/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.2.0/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.2.0/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.820458 mia-accounting-1.2.0/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.2.0/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.2.0/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.820458 mia-accounting-1.2.0/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.2.0/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.2.0/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.2.0/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.2.0/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.820458 mia-accounting-1.2.0/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.2.0/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.2.0/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.2.0/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.2.0/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.2.0/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8362 2023-04-04 09:21:37.000000 mia-accounting-1.2.0/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.2.0/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.2.0/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.2.0/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.2.0/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.824458 mia-accounting-1.2.0/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.2.0/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.2.0/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.2.0/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.2.0/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.2.0/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.2.0/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4477 2023-04-09 02:08:22.000000 mia-accounting-1.2.0/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    10434 2023-04-09 02:08:22.000000 mia-accounting-1.2.0/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.804458 mia-accounting-1.2.0/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.824458 mia-accounting-1.2.0/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.2.0/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.824458 mia-accounting-1.2.0/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.2.0/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.2.0/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.2.0/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.804458 mia-accounting-1.2.0/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.824458 mia-accounting-1.2.0/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.824458 mia-accounting-1.2.0/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.824458 mia-accounting-1.2.0/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.824458 mia-accounting-1.2.0/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.824458 mia-accounting-1.2.0/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.824458 mia-accounting-1.2.0/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.828457 mia-accounting-1.2.0/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3036 2023-04-08 16:39:45.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.828457 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.828457 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.828457 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.828457 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.828457 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.828457 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.828457 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.828457 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.832457 mia-accounting-1.2.0/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.832457 mia-accounting-1.2.0/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.832457 mia-accounting-1.2.0/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.832457 mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/report/unapplied.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.832457 mia-accounting-1.2.0/src/accounting/templates/accounting/unmatched-offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/unmatched-offset/dashboard.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.2.0/src/accounting/templates/accounting/unmatched-offset/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.832457 mia-accounting-1.2.0/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 17:41:05.000000 mia-accounting-1.2.0/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.2.0/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.808458 mia-accounting-1.2.0/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.836457 mia-accounting-1.2.0/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.2.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.2.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.808458 mia-accounting-1.2.0/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.836457 mia-accounting-1.2.0/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.2.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.2.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.836457 mia-accounting-1.2.0/src/accounting/unmatched_offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.2.0/src/accounting/unmatched_offset/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.2.0/src/accounting/unmatched_offset/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.2.0/src/accounting/unmatched_offset/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.836457 mia-accounting-1.2.0/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.2.0/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.2.0/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.2.0/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.2.0/src/accounting/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.2.0/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.2.0/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.2.0/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.2.0/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.2.0/src/accounting/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.2.0/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.840457 mia-accounting-1.2.0/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     7024 2023-04-09 04:17:12.000000 mia-accounting-1.2.0/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11342 2023-04-09 04:17:12.000000 mia-accounting-1.2.0/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-09 04:17:12.000000 mia-accounting-1.2.0/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-09 04:17:12.000000 mia-accounting-1.2.0/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-09 04:17:12.000000 mia-accounting-1.2.0/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.840457 mia-accounting-1.2.0/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-04 09:21:35.000000 mia-accounting-1.2.0/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-04 09:21:32.000000 mia-accounting-1.2.0/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    35900 2023-04-09 03:46:55.000000 mia-accounting-1.2.0/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5034 2023-04-04 09:21:36.000000 mia-accounting-1.2.0/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)    27047 2023-04-09 03:46:55.000000 mia-accounting-1.2.0/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16820 2023-04-09 03:46:55.000000 mia-accounting-1.2.0/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   106505 2023-04-09 03:46:55.000000 mia-accounting-1.2.0/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    39089 2023-04-09 03:46:55.000000 mia-accounting-1.2.0/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16738 2023-04-09 02:42:18.000000 mia-accounting-1.2.0/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16219 2023-04-09 04:09:27.000000 mia-accounting-1.2.0/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.840457 mia-accounting-1.2.0/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4143 2023-04-04 23:16:14.000000 mia-accounting-1.2.0/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2861 2023-04-04 09:28:44.000000 mia-accounting-1.2.0/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.2.0/tests/test_site/locale.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.840457 mia-accounting-1.2.0/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.2.0/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.840457 mia-accounting-1.2.0/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6015 2023-04-05 18:00:22.000000 mia-accounting-1.2.0/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)      812 2023-04-04 10:04:53.000000 mia-accounting-1.2.0/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1419 2023-04-04 10:04:53.000000 mia-accounting-1.2.0/tests/test_site/templates/login.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.840457 mia-accounting-1.2.0/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.2.0/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     1307 2023-04-05 18:34:06.000000 mia-accounting-1.2.0/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.808458 mia-accounting-1.2.0/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.844457 mia-accounting-1.2.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.2.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:34:39.000000 mia-accounting-1.2.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.808458 mia-accounting-1.2.0/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 04:17:12.844457 mia-accounting-1.2.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.2.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:55:17.000000 mia-accounting-1.2.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    29050 2023-04-09 03:46:55.000000 mia-accounting-1.2.0/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.2.0/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14493 2023-04-09 03:46:55.000000 mia-accounting-1.2.0/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-09 03:46:55.000000 mia-accounting-1.2.0/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.1.0/LICENSE` & `mia-accounting-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/MANIFEST.in` & `mia-accounting-1.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/PKG-INFO` & `mia-accounting-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
```

### Comparing `mia-accounting-1.1.0/README.rst` & `mia-accounting-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/Makefile` & `mia-accounting-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/make.bat` & `mia-accounting-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.account.rst` & `mia-accounting-1.2.0/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.base_account.rst` & `mia-accounting-1.2.0/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.currency.rst` & `mia-accounting-1.2.0/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.2.0/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.2.0/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.2.0/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.option.rst` & `mia-accounting-1.2.0/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.report.period.rst` & `mia-accounting-1.2.0/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.report.reports.rst` & `mia-accounting-1.2.0/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.report.rst` & `mia-accounting-1.2.0/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.report.utils.rst` & `mia-accounting-1.2.0/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.rst` & `mia-accounting-1.2.0/docs/source/accounting.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.unmatched_offset.rst` & `mia-accounting-1.2.0/docs/source/accounting.unmatched_offset.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/accounting.utils.rst` & `mia-accounting-1.2.0/docs/source/accounting.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/conf.py` & `mia-accounting-1.2.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Mia! Accounting'
 copyright = '2023, imacat'
 author = 'imacat'
-release = '1.1.0'
+release = '1.2.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `mia-accounting-1.1.0/docs/source/examples.rst` & `mia-accounting-1.2.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/history.rst` & `mia-accounting-1.2.0/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/docs/source/intro.rst` & `mia-accounting-1.2.0/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/pyproject.toml` & `mia-accounting-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [project]
 name = "mia-accounting"
-version = "1.1.0"
+version = "1.2.0"
 description = "A Flask accounting module."
 readme = "README.rst"
 requires-python = ">=3.11"
 authors = [
     {name = "imacat", email = "imacat@mail.imacat.idv.tw"},
 ]
 keywords = ["mia", "accounting", "flask"]
```

### Comparing `mia-accounting-1.1.0/src/accounting/__init__.py` & `mia-accounting-1.2.0/src/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/account/__init__.py` & `mia-accounting-1.2.0/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/account/commands.py` & `mia-accounting-1.2.0/src/accounting/account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/account/converters.py` & `mia-accounting-1.2.0/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/account/forms.py` & `mia-accounting-1.2.0/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/account/queries.py` & `mia-accounting-1.2.0/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/account/views.py` & `mia-accounting-1.2.0/src/accounting/account/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     accounts: list[BaseAccount] = get_account_query()
     pagination: Pagination = Pagination[BaseAccount](accounts)
     return render_template("accounting/account/list.html",
                            list=pagination.list, pagination=pagination)
 
 
-@bp.get("/create", endpoint="create")
+@bp.get("create", endpoint="create")
 @has_permission(can_edit)
 def show_add_account_form() -> str:
     """Shows the form to add an account.
 
     :return: The form to add an account.
     """
     if "form" in session:
@@ -66,15 +66,15 @@
         form.validate()
     else:
         form = AccountForm()
     return render_template("accounting/account/create.html",
                            form=form)
 
 
-@bp.post("/store", endpoint="store")
+@bp.post("store", endpoint="store")
 @has_permission(can_edit)
 def add_account() -> redirect:
     """Adds an account.
 
     :return: The redirection to the account detail on success, or the account
         creation form on error.
     """
@@ -87,26 +87,26 @@
     form.populate_obj(account)
     db.session.add(account)
     db.session.commit()
     flash(s(lazy_gettext("The account is added successfully")), "success")
     return redirect(inherit_next(__get_detail_uri(account)))
 
 
-@bp.get("/<account:account>", endpoint="detail")
+@bp.get("<account:account>", endpoint="detail")
 @has_permission(can_view)
 def show_account_detail(account: Account) -> str:
     """Shows the account detail.
 
     :param account: The account.
     :return: The detail.
     """
     return render_template("accounting/account/detail.html", obj=account)
 
 
-@bp.get("/<account:account>/edit", endpoint="edit")
+@bp.get("<account:account>/edit", endpoint="edit")
 @has_permission(can_edit)
 def show_account_edit_form(account: Account) -> str:
     """Shows the form to edit an account.
 
     :param account: The account.
     :return: The form to edit the account.
     """
@@ -117,15 +117,15 @@
         form.validate()
     else:
         form = AccountForm(obj=account)
     return render_template("accounting/account/edit.html",
                            account=account, form=form)
 
 
-@bp.post("/<account:account>/update", endpoint="update")
+@bp.post("<account:account>/update", endpoint="update")
 @has_permission(can_edit)
 def update_account(account: Account) -> redirect:
     """Updates an account.
 
     :param account: The account.
     :return: The redirection to the account detail on success, or the account
         edit form on error.
@@ -144,15 +144,15 @@
     account.updated_by_id = get_current_user_pk()
     account.updated_at = sa.func.now()
     db.session.commit()
     flash(s(lazy_gettext("The account is updated successfully.")), "success")
     return redirect(inherit_next(__get_detail_uri(account)))
 
 
-@bp.post("/<account:account>/delete", endpoint="delete")
+@bp.post("<account:account>/delete", endpoint="delete")
 @has_permission(can_edit)
 def delete_account(account: Account) -> redirect:
     """Deletes an account.
 
     :param account: The account.
     :return: The redirection to the account list on success, or the account
         detail on error.
@@ -163,26 +163,26 @@
     account.delete()
     sort_accounts_in(account.base_code, account.id)
     db.session.commit()
     flash(s(lazy_gettext("The account is deleted successfully.")), "success")
     return redirect(or_next(__get_list_uri()))
 
 
-@bp.get("/bases/<baseAccount:base>", endpoint="order")
+@bp.get("bases/<baseAccount:base>", endpoint="order")
 @has_permission(can_view)
 def show_account_order(base: BaseAccount) -> str:
     """Shows the order of the accounts under a same base account.
 
     :param base: The base account.
     :return: The order of the accounts under the base account.
     """
     return render_template("accounting/account/order.html", base=base)
 
 
-@bp.post("/bases/<baseAccount:base>", endpoint="sort")
+@bp.post("bases/<baseAccount:base>", endpoint="sort")
 @has_permission(can_edit)
 def sort_accounts(base: BaseAccount) -> redirect:
     """Reorders the accounts under a base account.
 
     :param base: The base account.
     :return: The redirection to the incoming account or the account list.  The
         reordering operation does not fail.
```

### Comparing `mia-accounting-1.1.0/src/accounting/base_account/__init__.py` & `mia-accounting-1.2.0/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/base_account/commands.py` & `mia-accounting-1.2.0/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/base_account/converters.py` & `mia-accounting-1.2.0/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/base_account/queries.py` & `mia-accounting-1.2.0/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/base_account/views.py` & `mia-accounting-1.2.0/src/accounting/base_account/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """
     accounts: list[BaseAccount] = get_base_account_query()
     pagination: Pagination = Pagination[BaseAccount](accounts)
     return render_template("accounting/base-account/list.html",
                            list=pagination.list, pagination=pagination)
 
 
-@bp.get("/<baseAccount:account>", endpoint="detail")
+@bp.get("<baseAccount:account>", endpoint="detail")
 @has_permission(can_view)
 def show_account_detail(account: BaseAccount) -> str:
     """Shows the account detail.
 
     :param account: The account.
     :return: The detail.
     """
```

### Comparing `mia-accounting-1.1.0/src/accounting/currency/__init__.py` & `mia-accounting-1.2.0/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/currency/commands.py` & `mia-accounting-1.2.0/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/currency/converters.py` & `mia-accounting-1.2.0/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/currency/forms.py` & `mia-accounting-1.2.0/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/currency/queries.py` & `mia-accounting-1.2.0/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/currency/views.py` & `mia-accounting-1.2.0/src/accounting/currency/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
     currencies: list[Currency] = get_currency_query()
     pagination: Pagination = Pagination[Currency](currencies)
     return render_template("accounting/currency/list.html",
                            list=pagination.list, pagination=pagination)
 
 
-@bp.get("/create", endpoint="create")
+@bp.get("create", endpoint="create")
 @has_permission(can_edit)
 def show_add_currency_form() -> str:
     """Shows the form to add a currency.
 
     :return: The form to add a currency.
     """
     if "form" in session:
@@ -68,15 +68,15 @@
         form.validate()
     else:
         form = CurrencyForm()
     return render_template("accounting/currency/create.html",
                            form=form)
 
 
-@bp.post("/store", endpoint="store")
+@bp.post("store", endpoint="store")
 @has_permission(can_edit)
 def add_currency() -> redirect:
     """Adds a currency.
 
     :return: The redirection to the currency detail on success, or the currency
         creation form on error.
     """
@@ -89,26 +89,26 @@
     form.populate_obj(currency)
     db.session.add(currency)
     db.session.commit()
     flash(s(lazy_gettext("The currency is added successfully.")), "success")
     return redirect(inherit_next(__get_detail_uri(currency)))
 
 
-@bp.get("/<currency:currency>", endpoint="detail")
+@bp.get("<currency:currency>", endpoint="detail")
 @has_permission(can_view)
 def show_currency_detail(currency: Currency) -> str:
     """Shows the currency detail.
 
     :param currency: The currency.
     :return: The detail.
     """
     return render_template("accounting/currency/detail.html", obj=currency)
 
 
-@bp.get("/<currency:currency>/edit", endpoint="edit")
+@bp.get("<currency:currency>/edit", endpoint="edit")
 @has_permission(can_edit)
 def show_currency_edit_form(currency: Currency) -> str:
     """Shows the form to edit a currency.
 
     :param currency: The currency.
     :return: The form to edit the currency.
     """
@@ -119,15 +119,15 @@
         form.validate()
     else:
         form = CurrencyForm(obj=currency)
     return render_template("accounting/currency/edit.html",
                            currency=currency, form=form)
 
 
-@bp.post("/<currency:currency>/update", endpoint="update")
+@bp.post("<currency:currency>/update", endpoint="update")
 @has_permission(can_edit)
 def update_currency(currency: Currency) -> redirect:
     """Updates a currency.
 
     :param currency: The currency.
     :return: The redirection to the currency detail on success, or the currency
         edit form on error.
@@ -147,15 +147,15 @@
     currency.updated_by_id = get_current_user_pk()
     currency.updated_at = sa.func.now()
     db.session.commit()
     flash(s(lazy_gettext("The currency is updated successfully.")), "success")
     return redirect(inherit_next(__get_detail_uri(currency)))
 
 
-@bp.post("/<currency:currency>/delete", endpoint="delete")
+@bp.post("<currency:currency>/delete", endpoint="delete")
 @has_permission(can_edit)
 def delete_currency(currency: Currency) -> redirect:
     """Deletes a currency.
 
     :param currency: The currency.
     :return: The redirection to the currency list on success, or the currency
         detail on error.
@@ -165,15 +165,15 @@
         return redirect(inherit_next(__get_detail_uri(currency)))
     currency.delete()
     db.session.commit()
     flash(s(lazy_gettext("The currency is deleted successfully.")), "success")
     return redirect(or_next(url_for("accounting.currency.list")))
 
 
-@api_bp.get("/exists-code", endpoint="exists")
+@api_bp.get("exists-code", endpoint="exists")
 @has_permission(can_edit)
 def exists_code() -> dict[str, bool]:
     """Validates whether a currency code exists.
 
     :return: Whether the currency code exists.
     """
     return {"exists": db.session.get(Currency, request.args["q"]) is not None}
```

### Comparing `mia-accounting-1.1.0/src/accounting/data/base_accounts.csv` & `mia-accounting-1.2.0/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/forms.py` & `mia-accounting-1.2.0/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/converters.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/forms/line_item.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/utils/description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/journal_entry/views.py` & `mia-accounting-1.2.0/src/accounting/journal_entry/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 bp.add_app_template_filter(with_type, "accounting_journal_entry_with_type")
 bp.add_app_template_filter(to_transfer, "accounting_journal_entry_to_transfer")
 bp.add_app_template_filter(format_amount_input,
                            "accounting_journal_entry_format_amount_input")
 bp.add_app_template_filter(text2html, "accounting_journal_entry_text2html")
 
 
-@bp.get("/create/<journalEntryType:journal_entry_type>", endpoint="create")
+@bp.get("create/<journalEntryType:journal_entry_type>", endpoint="create")
 @has_permission(can_edit)
 def show_add_journal_entry_form(journal_entry_type: JournalEntryType) -> str:
     """Shows the form to add a journal entry.
 
     :param journal_entry_type: The journal entry type.
     :return: The form to add a journal entry.
     """
@@ -67,15 +67,15 @@
         form.validate()
     else:
         form = journal_entry_op.form()
         form.date.data = date.today()
     return journal_entry_op.render_create_template(form)
 
 
-@bp.post("/store/<journalEntryType:journal_entry_type>", endpoint="store")
+@bp.post("store/<journalEntryType:journal_entry_type>", endpoint="store")
 @has_permission(can_edit)
 def add_journal_entry(journal_entry_type: JournalEntryType) -> redirect:
     """Adds a journal entry.
 
     :param journal_entry_type: The journal entry type.
     :return: The redirection to the journal entry detail on success, or the
         journal entry creation form on error.
@@ -94,28 +94,28 @@
     db.session.add(journal_entry)
     db.session.commit()
     flash(s(lazy_gettext("The journal entry is added successfully.")),
           "success")
     return redirect(inherit_next(__get_detail_uri(journal_entry)))
 
 
-@bp.get("/<journalEntry:journal_entry>", endpoint="detail")
+@bp.get("<journalEntry:journal_entry>", endpoint="detail")
 @has_permission(can_view)
 def show_journal_entry_detail(journal_entry: JournalEntry) -> str:
     """Shows the journal entry detail.
 
     :param journal_entry: The journal entry.
     :return: The detail.
     """
     journal_entry_op: JournalEntryOperator \
         = get_journal_entry_op(journal_entry)
     return journal_entry_op.render_detail_template(journal_entry)
 
 
-@bp.get("/<journalEntry:journal_entry>/edit", endpoint="edit")
+@bp.get("<journalEntry:journal_entry>/edit", endpoint="edit")
 @has_permission(can_edit)
 def show_journal_entry_edit_form(journal_entry: JournalEntry) -> str:
     """Shows the form to edit a journal entry.
 
     :param journal_entry: The journal entry.
     :return: The form to edit the journal entry.
     """
@@ -129,15 +129,15 @@
         form.obj = journal_entry
         form.validate()
     else:
         form = journal_entry_op.form(obj=journal_entry)
     return journal_entry_op.render_edit_template(journal_entry, form)
 
 
-@bp.post("/<journalEntry:journal_entry>/update", endpoint="update")
+@bp.post("<journalEntry:journal_entry>/update", endpoint="update")
 @has_permission(can_edit)
 def update_journal_entry(journal_entry: JournalEntry) -> redirect:
     """Updates a journal entry.
 
     :param journal_entry: The journal entry.
     :return: The redirection to the journal entry detail on success, or the
         journal entry edit form on error.
@@ -162,15 +162,15 @@
     journal_entry.updated_at = sa.func.now()
     db.session.commit()
     flash(s(lazy_gettext("The journal entry is updated successfully.")),
           "success")
     return redirect(inherit_next(__get_detail_uri(journal_entry)))
 
 
-@bp.post("/<journalEntry:journal_entry>/delete", endpoint="delete")
+@bp.post("<journalEntry:journal_entry>/delete", endpoint="delete")
 @has_permission(can_edit)
 def delete_journal_entry(journal_entry: JournalEntry) -> redirect:
     """Deletes a journal entry.
 
     :param journal_entry: The journal entry.
     :return: The redirection to the journal entry list on success, or the
         journal entry detail on error.
@@ -182,30 +182,30 @@
     sort_journal_entries_in(journal_entry.date, journal_entry.id)
     db.session.commit()
     flash(s(lazy_gettext("The journal entry is deleted successfully.")),
           "success")
     return redirect(or_next(__get_default_page_uri()))
 
 
-@bp.get("/dates/<date:journal_entry_date>", endpoint="order")
+@bp.get("dates/<date:journal_entry_date>", endpoint="order")
 @has_permission(can_view)
 def show_journal_entry_order(journal_entry_date: date) -> str:
     """Shows the order of the journal entries in a same date.
 
     :param journal_entry_date: The date.
     :return: The order of the journal entries in the date.
     """
     journal_entries: list[JournalEntry] = JournalEntry.query \
         .filter(JournalEntry.date == journal_entry_date) \
         .order_by(JournalEntry.no).all()
     return render_template("accounting/journal-entry/order.html",
                            date=journal_entry_date, list=journal_entries)
 
 
-@bp.post("/dates/<date:journal_entry_date>", endpoint="sort")
+@bp.post("dates/<date:journal_entry_date>", endpoint="sort")
 @has_permission(can_edit)
 def sort_journal_entries(journal_entry_date: date) -> redirect:
     """Reorders the journal entries in a date.
 
     :param journal_entry_date: The date.
     :return: The redirection to the incoming account or the account list.  The
         reordering operation does not fail.
```

### Comparing `mia-accounting-1.1.0/src/accounting/locale.py` & `mia-accounting-1.2.0/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/models.py` & `mia-accounting-1.2.0/src/accounting/models.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/option/__init__.py` & `mia-accounting-1.2.0/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/option/forms.py` & `mia-accounting-1.2.0/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/option/views.py` & `mia-accounting-1.2.0/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/__init__.py` & `mia-accounting-1.2.0/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/converters.py` & `mia-accounting-1.2.0/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/period/__init__.py` & `mia-accounting-1.2.0/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/period/chooser.py` & `mia-accounting-1.2.0/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/period/description.py` & `mia-accounting-1.2.0/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/period/month_end.py` & `mia-accounting-1.2.0/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/period/parser.py` & `mia-accounting-1.2.0/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/period/period.py` & `mia-accounting-1.2.0/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.2.0/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/period/specification.py` & `mia-accounting-1.2.0/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/reports/__init__.py` & `mia-accounting-1.2.0/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.2.0/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.2.0/src/accounting/report/reports/income_expenses.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.2.0/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/reports/journal.py` & `mia-accounting-1.2.0/src/accounting/report/reports/journal.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/reports/ledger.py` & `mia-accounting-1.2.0/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/reports/search.py` & `mia-accounting-1.2.0/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.2.0/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.2.0/src/accounting/report/reports/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.2.0/src/accounting/report/reports/unapplied_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/template_filters.py` & `mia-accounting-1.2.0/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/utils/__init__.py` & `mia-accounting-1.2.0/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.2.0/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/utils/base_report.py` & `mia-accounting-1.2.0/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.2.0/src/accounting/report/utils/csv_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 """
 import csv
 from abc import ABC, abstractmethod
 from datetime import timedelta, date
 from decimal import Decimal
 from io import StringIO
+from urllib.parse import quote
 
 from flask import Response
 
 from accounting.report.period import Period
 
 
 class BaseCSVRow(ABC):
@@ -49,15 +50,15 @@
     """
     with StringIO() as fp:
         writer = csv.writer(fp)
         writer.writerows([x.values for x in rows])
         fp.seek(0)
         response: Response = Response(fp.read(), mimetype="text/csv")
         response.headers["Content-Disposition"] \
-            = f"attachment; filename={filename}"
+            = f"attachment; filename={quote(filename)}"
         return response
 
 
 def period_spec(period: Period) -> str:
     """Constructs the period specification to be used in the filename.
 
     :param period: The period.
```

### Comparing `mia-accounting-1.1.0/src/accounting/report/utils/option_link.py` & `mia-accounting-1.2.0/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.2.0/src/accounting/report/utils/report_chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/utils/report_type.py` & `mia-accounting-1.2.0/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.2.0/src/accounting/report/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/report/utils/urls.py` & `mia-accounting-1.2.0/src/accounting/report/utils/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,17 +43,18 @@
     """Returns the URL of a ledger.
 
     :param currency: The currency.
     :param account: The account.
     :param period: The period.
     :return: The URL of the ledger.
     """
-    if period.is_default:
-        return url_for("accounting-report.ledger-default",
-                       currency=currency, account=account)
+    if currency.code == default_currency_code() \
+            and account.code == Account.CASH_CODE \
+            and period.is_default:
+        return url_for("accounting-report.ledger-default")
     return url_for("accounting-report.ledger",
                    currency=currency, account=account,
                    period=period)
 
 
 def income_expenses_url(currency: Currency, account: CurrentAccount,
                         period: Period) -> str:
@@ -64,60 +65,54 @@
     :param period: The period.
     :return: The URL of the income and expenses log.
     """
     if currency.code == default_currency_code() \
             and account.code == options.default_ie_account_code \
             and period.is_default:
         return url_for("accounting-report.default")
-    if period.is_default:
-        return url_for("accounting-report.income-expenses-default",
-                       currency=currency, account=account)
     return url_for("accounting-report.income-expenses",
                    currency=currency, account=account,
                    period=period)
 
 
 def trial_balance_url(currency: Currency, period: Period) -> str:
     """Returns the URL of a trial balance.
 
     :param currency: The currency.
     :param period: The period.
     :return: The URL of the trial balance.
     """
-    if period.is_default:
-        return url_for("accounting-report.trial-balance-default",
-                       currency=currency)
+    if currency.code == default_currency_code() and period.is_default:
+        return url_for("accounting-report.trial-balance-default")
     return url_for("accounting-report.trial-balance",
                    currency=currency, period=period)
 
 
 def income_statement_url(currency: Currency, period: Period) -> str:
     """Returns the URL of an income statement.
 
     :param currency: The currency.
     :param period: The period.
     :return: The URL of the income statement.
     """
-    if period.is_default:
-        return url_for("accounting-report.income-statement-default",
-                       currency=currency)
+    if currency.code == default_currency_code() and period.is_default:
+        return url_for("accounting-report.income-statement-default")
     return url_for("accounting-report.income-statement",
                    currency=currency, period=period)
 
 
 def balance_sheet_url(currency: Currency, period: Period) -> str:
     """Returns the URL of a balance sheet.
 
     :param currency: The currency.
     :param period: The period.
     :return: The URL of the balance sheet.
     """
-    if period.is_default:
-        return url_for("accounting-report.balance-sheet-default",
-                       currency=currency)
+    if currency.code == default_currency_code() and period.is_default:
+        return url_for("accounting-report.balance-sheet-default")
     return url_for("accounting-report.balance-sheet",
                    currency=currency, period=period)
 
 
 def unapplied_url(account: Account | None) -> str:
     """Returns the URL of the unapplied original line items.
```

### Comparing `mia-accounting-1.1.0/src/accounting/report/views.py` & `mia-accounting-1.2.0/src/accounting/report/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,18 +40,15 @@
 @bp.get("", endpoint="default")
 @has_permission(can_view)
 def get_default_report() -> str | Response:
     """Returns the income and expenses log in the default period.
 
     :return: The income and expenses log in the default period.
     """
-    return __get_income_expenses(
-        db.session.get(Currency, default_currency_code()),
-        options.default_ie_account,
-        get_period())
+    return get_default_income_expenses()
 
 
 @bp.get("journal", endpoint="journal-default")
 @has_permission(can_view)
 def get_default_journal() -> str | Response:
     """Returns the journal in the default period.
 
@@ -79,25 +76,23 @@
     """
     report: Journal = Journal(period)
     if "as" in request.args and request.args["as"] == "csv":
         return report.csv()
     return report.html()
 
 
-@bp.get("ledger/<currency:currency>/<account:account>",
-        endpoint="ledger-default")
+@bp.get("ledger", endpoint="ledger-default")
 @has_permission(can_view)
-def get_default_ledger(currency: Currency, account: Account) -> str | Response:
-    """Returns the ledger in the default period.
+def get_default_ledger() -> str | Response:
+    """Returns the ledger in the default currency, cash, and default period.
 
-    :param currency: The currency.
-    :param account: The account.
-    :return: The ledger in the default period.
+    :return: The ledger in the default currency, cash, and default period.
     """
-    return __get_ledger(currency, account, get_period())
+    return __get_ledger(db.session.get(Currency, default_currency_code()),
+                        Account.cash(), get_period())
 
 
 @bp.get("ledger/<currency:currency>/<account:account>/<period:period>",
         endpoint="ledger")
 @has_permission(can_view)
 def get_ledger(currency: Currency, account: Account, period: Period) \
         -> str | Response:
@@ -122,26 +117,25 @@
     """
     report: Ledger = Ledger(currency, account, period)
     if "as" in request.args and request.args["as"] == "csv":
         return report.csv()
     return report.html()
 
 
-@bp.get("income-expenses/<currency:currency>/<currentAccount:account>",
-        endpoint="income-expenses-default")
+@bp.get("income-expenses", endpoint="income-expenses-default")
 @has_permission(can_view)
-def get_default_income_expenses(currency: Currency, account: CurrentAccount) \
-        -> str | Response:
+def get_default_income_expenses() -> str | Response:
     """Returns the income and expenses log in the default period.
 
-    :param currency: The currency.
-    :param account: The account.
     :return: The income and expenses log in the default period.
     """
-    return __get_income_expenses(currency, account, get_period())
+    return __get_income_expenses(
+        db.session.get(Currency, default_currency_code()),
+        options.default_ie_account,
+        get_period())
 
 
 @bp.get("income-expenses/<currency:currency>/<currentAccount:account>/"
         "<period:period>", endpoint="income-expenses")
 @has_permission(can_view)
 def get_income_expenses(currency: Currency, account: CurrentAccount,
                         period: Period) -> str | Response:
@@ -166,24 +160,23 @@
     """
     report: IncomeExpenses = IncomeExpenses(currency, account, period)
     if "as" in request.args and request.args["as"] == "csv":
         return report.csv()
     return report.html()
 
 
-@bp.get("trial-balance/<currency:currency>",
-        endpoint="trial-balance-default")
+@bp.get("trial-balance", endpoint="trial-balance-default")
 @has_permission(can_view)
-def get_default_trial_balance(currency: Currency) -> str | Response:
+def get_default_trial_balance() -> str | Response:
     """Returns the trial balance in the default period.
 
-    :param currency: The currency.
     :return: The trial balance in the default period.
     """
-    return __get_trial_balance(currency, get_period())
+    return __get_trial_balance(
+        db.session.get(Currency, default_currency_code()), get_period())
 
 
 @bp.get("trial-balance/<currency:currency>/<period:period>",
         endpoint="trial-balance")
 @has_permission(can_view)
 def get_trial_balance(currency: Currency, period: Period) -> str | Response:
     """Returns the trial balance.
@@ -204,24 +197,23 @@
     """
     report: TrialBalance = TrialBalance(currency, period)
     if "as" in request.args and request.args["as"] == "csv":
         return report.csv()
     return report.html()
 
 
-@bp.get("income-statement/<currency:currency>",
-        endpoint="income-statement-default")
+@bp.get("income-statement", endpoint="income-statement-default")
 @has_permission(can_view)
-def get_default_income_statement(currency: Currency) -> str | Response:
+def get_default_income_statement() -> str | Response:
     """Returns the income statement in the default period.
 
-    :param currency: The currency.
     :return: The income statement in the default period.
     """
-    return __get_income_statement(currency, get_period())
+    return __get_income_statement(
+        db.session.get(Currency, default_currency_code()), get_period())
 
 
 @bp.get("income-statement/<currency:currency>/<period:period>",
         endpoint="income-statement")
 @has_permission(can_view)
 def get_income_statement(currency: Currency, period: Period) -> str | Response:
     """Returns the income statement.
@@ -243,24 +235,23 @@
     """
     report: IncomeStatement = IncomeStatement(currency, period)
     if "as" in request.args and request.args["as"] == "csv":
         return report.csv()
     return report.html()
 
 
-@bp.get("balance-sheet/<currency:currency>",
-        endpoint="balance-sheet-default")
+@bp.get("balance-sheet", endpoint="balance-sheet-default")
 @has_permission(can_view)
-def get_default_balance_sheet(currency: Currency) -> str | Response:
+def get_default_balance_sheet() -> str | Response:
     """Returns the balance sheet in the default period.
 
-    :param currency: The currency.
     :return: The balance sheet in the default period.
     """
-    return __get_balance_sheet(currency, get_period())
+    return __get_balance_sheet(
+        db.session.get(Currency, default_currency_code()), get_period())
 
 
 @bp.get("balance-sheet/<currency:currency>/<period:period>",
         endpoint="balance-sheet")
 @has_permission(can_view)
 def get_balance_sheet(currency: Currency, period: Period) \
         -> str | Response:
```

### Comparing `mia-accounting-1.1.0/src/accounting/static/css/style.css` & `mia-accounting-1.2.0/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/account-form.js` & `mia-accounting-1.2.0/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/account-order.js` & `mia-accounting-1.2.0/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/currency-form.js` & `mia-accounting-1.2.0/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/description-editor.js` & `mia-accounting-1.2.0/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.2.0/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.2.0/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.2.0/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.2.0/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.2.0/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.2.0/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/option-form.js` & `mia-accounting-1.2.0/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.2.0/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.2.0/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/template_filters.py` & `mia-accounting-1.2.0/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/template_globals.py` & `mia-accounting-1.2.0/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/base.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/include/nav.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/report/unapplied.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/unmatched-offset/dashboard.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/unmatched-offset/dashboard.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/templates/accounting/unmatched-offset/list.html` & `mia-accounting-1.2.0/src/accounting/templates/accounting/unmatched-offset/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/translations/accounting.pot` & `mia-accounting-1.2.0/src/accounting/translations/accounting.pot`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-09 00:22+0800\n"
+"POT-Creation-Date: 2023-04-09 01:41+0800\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `mia-accounting-1.1.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.2.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.1.0\n"
+"Project-Id-Version: mia-accounting 1.1.1\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-09 00:22+0800\n"
-"PO-Revision-Date: 2023-04-09 00:37+0800\n"
+"POT-Creation-Date: 2023-04-09 01:41+0800\n"
+"PO-Revision-Date: 2023-04-09 01:41+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -332,15 +332,15 @@
 msgid "March"
 msgstr "三月"
 
 msgid "Match"
 msgstr "抵销"
 
 msgid "Matches %(matches)s from %(total)s unapplied line items."
-msgstr "%(total)s 笔未抵销原始分录中，配对抵销掉 %(matches) 笔。"
+msgstr "%(total)s 笔未抵销原始分录中，配对抵销掉 %(matches)s 笔。"
 
 msgid "May"
 msgstr "五月"
 
 msgid "Month"
 msgstr "月"
```

### Comparing `mia-accounting-1.1.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.2.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # Copyright (C) 2023 imacat
 # This file is distributed under the same license as the Mia! Accounting
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.1.0\n"
+"Project-Id-Version: mia-accounting 1.1.1\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-09 00:22+0800\n"
-"PO-Revision-Date: 2023-04-09 00:37+0800\n"
+"POT-Creation-Date: 2023-04-09 01:41+0800\n"
+"PO-Revision-Date: 2023-04-09 01:41+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -1246,15 +1246,15 @@
 #: src/accounting/templates/accounting/report/trial-balance.html:29
 #: src/accounting/templates/accounting/report/trial-balance.html:49
 #, python-format
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s试算表"
 
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:24
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:41x
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:41
 msgid "Accounts with Unapplied Original Line Items"
 msgstr "有未抵销原始分录的科目"
 
 #: src/accounting/templates/accounting/report/unapplied.html:28
 #, python-format
 msgid "Unapplied Original Line Items of %(account)s"
 msgstr "%(account)s未抵销原始分录"
@@ -1323,16 +1323,15 @@
 msgstr "你确定要抵销下列原始分录与抵销分录吗？结果无法复原。请先备份数据库，并仔细核对抵销分录是否正确。"
 
 #: src/accounting/templates/accounting/unmatched-offset/list.html:81
 #, python-format
 msgid ""
 "%(matches)s unapplied original line items out of %(total)s can match with"
 " their offsets."
-msgstr ""
-"%(total)s 笔未抵销原始分录中，可配对抵销掉 %(matches)s 笔。"
+msgstr "%(total)s 笔未抵销原始分录中，可配对抵销掉 %(matches)s 笔。"
 
 #: src/accounting/templates/accounting/unmatched-offset/list.html:83
 #, python-format
 msgid "%(total)s unapplied original line items without matching offsets."
 msgstr "%(total)s 笔未抵销原始分录，无法自动配对抵销。"
 
 #: src/accounting/templates/accounting/unmatched-offset/list.html:85
@@ -1351,15 +1350,15 @@
 #: src/accounting/unmatched_offset/views.py:71
 msgid "No more offset to match automatically."
 msgstr "无法自动配对抵销。"
 
 #: src/accounting/unmatched_offset/views.py:77
 #, python-format
 msgid "Matches %(matches)s from %(total)s unapplied line items."
-msgstr "%(total)s 笔未抵销原始分录中，配对抵销掉 %(matches) 笔。"
+msgstr "%(total)s 笔未抵销原始分录中，配对抵销掉 %(matches)s 笔。"
 
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr "流动资产与负债"
 
 #: src/accounting/utils/pagination.py:206
 msgctxt "Pagination|"
```

### Comparing `mia-accounting-1.1.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.2.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.1.0\n"
+"Project-Id-Version: mia-accounting 1.1.1\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-09 00:22+0800\n"
-"PO-Revision-Date: 2023-04-09 00:37+0800\n"
+"POT-Creation-Date: 2023-04-09 01:41+0800\n"
+"PO-Revision-Date: 2023-04-09 01:41+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -332,15 +332,15 @@
 msgid "March"
 msgstr "三月"
 
 msgid "Match"
 msgstr "抵銷"
 
 msgid "Matches %(matches)s from %(total)s unapplied line items."
-msgstr "%(total)s 筆未抵銷原始分錄中，配對抵銷掉 %(matches) 筆。"
+msgstr "%(total)s 筆未抵銷原始分錄中，配對抵銷掉 %(matches)s 筆。"
 
 msgid "May"
 msgstr "五月"
 
 msgid "Month"
 msgstr "月"
```

### Comparing `mia-accounting-1.1.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.2.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # Copyright (C) 2023 imacat
 # This file is distributed under the same license as the Mia! Accounting
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.1.0\n"
+"Project-Id-Version: mia-accounting 1.1.1\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-09 00:22+0800\n"
-"PO-Revision-Date: 2023-04-09 00:37+0800\n"
+"POT-Creation-Date: 2023-04-09 01:41+0800\n"
+"PO-Revision-Date: 2023-04-09 01:41+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -1246,15 +1246,15 @@
 #: src/accounting/templates/accounting/report/trial-balance.html:29
 #: src/accounting/templates/accounting/report/trial-balance.html:49
 #, python-format
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s試算表"
 
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:24
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:41x
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:41
 msgid "Accounts with Unapplied Original Line Items"
 msgstr "有未抵銷原始分錄的科目"
 
 #: src/accounting/templates/accounting/report/unapplied.html:28
 #, python-format
 msgid "Unapplied Original Line Items of %(account)s"
 msgstr "%(account)s未抵銷原始分錄"
@@ -1323,16 +1323,15 @@
 msgstr "你確定要抵銷下列原始分錄與抵銷分錄嗎？結果無法復原。請先備份資料庫，並仔細核對抵銷分錄是否正確。"
 
 #: src/accounting/templates/accounting/unmatched-offset/list.html:81
 #, python-format
 msgid ""
 "%(matches)s unapplied original line items out of %(total)s can match with"
 " their offsets."
-msgstr ""
-"%(total)s 筆未抵銷原始分錄中，可配對抵銷掉 %(matches)s 筆。"
+msgstr "%(total)s 筆未抵銷原始分錄中，可配對抵銷掉 %(matches)s 筆。"
 
 #: src/accounting/templates/accounting/unmatched-offset/list.html:83
 #, python-format
 msgid "%(total)s unapplied original line items without matching offsets."
 msgstr "%(total)s 筆未抵銷原始分錄，無法自動配對抵銷。"
 
 #: src/accounting/templates/accounting/unmatched-offset/list.html:85
@@ -1351,15 +1350,15 @@
 #: src/accounting/unmatched_offset/views.py:71
 msgid "No more offset to match automatically."
 msgstr "無法自動配對抵銷。"
 
 #: src/accounting/unmatched_offset/views.py:77
 #, python-format
 msgid "Matches %(matches)s from %(total)s unapplied line items."
-msgstr "%(total)s 筆未抵銷原始分錄中，配對抵銷掉 %(matches) 筆。"
+msgstr "%(total)s 筆未抵銷原始分錄中，配對抵銷掉 %(matches)s 筆。"
 
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr "流動資產與負債"
 
 #: src/accounting/utils/pagination.py:206
 msgctxt "Pagination|"
```

### Comparing `mia-accounting-1.1.0/src/accounting/unmatched_offset/__init__.py` & `mia-accounting-1.2.0/src/accounting/unmatched_offset/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/unmatched_offset/queries.py` & `mia-accounting-1.2.0/src/accounting/unmatched_offset/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/unmatched_offset/views.py` & `mia-accounting-1.2.0/src/accounting/unmatched_offset/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/__init__.py` & `mia-accounting-1.2.0/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/cast.py` & `mia-accounting-1.2.0/src/accounting/utils/cast.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/current_account.py` & `mia-accounting-1.2.0/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/flash_errors.py` & `mia-accounting-1.2.0/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.2.0/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/next_uri.py` & `mia-accounting-1.2.0/src/accounting/utils/next_uri.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/offset_alias.py` & `mia-accounting-1.2.0/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/offset_matcher.py` & `mia-accounting-1.2.0/src/accounting/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/options.py` & `mia-accounting-1.2.0/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/pagination.py` & `mia-accounting-1.2.0/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/permission.py` & `mia-accounting-1.2.0/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/query.py` & `mia-accounting-1.2.0/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/random_id.py` & `mia-accounting-1.2.0/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/strip_text.py` & `mia-accounting-1.2.0/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/unapplied.py` & `mia-accounting-1.2.0/src/accounting/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/accounting/utils/user.py` & `mia-accounting-1.2.0/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.2.0/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
```

### Comparing `mia-accounting-1.1.0/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.2.0/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -216,20 +216,20 @@
 tests/babel-utils.py
 tests/test_account.py
 tests/test_base_account.py
 tests/test_currency.py
 tests/test_description_editor.py
 tests/test_journal_entry.py
 tests/test_offset.py
-tests/test_offset_matcher.py
 tests/test_option.py
+tests/test_report.py
+tests/test_unmatched_offset.py
 tests/test_utils.py
 tests/testlib.py
 tests/testlib_journal_entry.py
-tests/testlib_offset.py
 tests/test_site/__init__.py
 tests/test_site/auth.py
 tests/test_site/locale.py
 tests/test_site/static/favicon.svg
 tests/test_site/templates/base.html
 tests/test_site/templates/home.html
 tests/test_site/templates/login.html
```

### Comparing `mia-accounting-1.1.0/tests/babel-utils-test-site.py` & `mia-accounting-1.2.0/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/babel-utils.py` & `mia-accounting-1.2.0/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_account.py` & `mia-accounting-1.2.0/tests/test_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import httpx
 import sqlalchemy as sa
 from click.testing import Result
 from flask import Flask
 from flask.testing import FlaskCliRunner
 
 from test_site import db
-from testlib import NEXT_URI, create_test_app, get_client, set_locale
-from testlib_journal_entry import add_journal_entry
+from testlib import NEXT_URI, create_test_app, get_client, set_locale, \
+    add_journal_entry
 
 
 class AccountData:
     """The account data."""
 
     def __init__(self, base_code: str, no: int, title: str):
         """Constructs the account data.
```

### Comparing `mia-accounting-1.1.0/tests/test_base_account.py` & `mia-accounting-1.2.0/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_currency.py` & `mia-accounting-1.2.0/tests/test_currency.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 import httpx
 from click.testing import Result
 from flask import Flask
 from flask.testing import FlaskCliRunner
 
 from test_site import db
-from testlib import NEXT_URI, create_test_app, get_client, set_locale
-from testlib_journal_entry import add_journal_entry
+from testlib import NEXT_URI, create_test_app, get_client, set_locale, \
+    add_journal_entry
 
 
 class CurrencyData:
     """The currency data."""
 
     def __init__(self, code: str, name: str):
         """Constructs the currency data.
```

### Comparing `mia-accounting-1.1.0/tests/test_description_editor.py` & `mia-accounting-1.2.0/tests/test_description_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 import unittest
 from datetime import date
 
 from click.testing import Result
 from flask import Flask
 from flask.testing import FlaskCliRunner
 
-from testlib import NEXT_URI, Accounts, create_test_app, get_client
-from testlib_journal_entry import add_journal_entry
+from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
+    add_journal_entry
 
 
 class DescriptionEditorTestCase(unittest.TestCase):
     """The description editor test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
```

### Comparing `mia-accounting-1.1.0/tests/test_journal_entry.py` & `mia-accounting-1.2.0/tests/test_journal_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 
 import httpx
 from click.testing import Result
 from flask import Flask
 from flask.testing import FlaskCliRunner
 
 from test_site import db
-from testlib import NEXT_URI, Accounts, create_test_app, get_client
+from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
+    add_journal_entry, match_journal_entry_detail
 from testlib_journal_entry import NON_EMPTY_NOTE, EMPTY_NOTE, \
     get_add_form, get_unchanged_update_form, get_update_form, \
-    match_journal_entry_detail, set_negative_amount, \
-    remove_debit_in_a_currency, remove_credit_in_a_currency, add_journal_entry
+    set_negative_amount, remove_debit_in_a_currency, \
+    remove_credit_in_a_currency
 
 PREFIX: str = "/accounting/journal-entries"
 """The URL prefix for the journal entry management."""
 RETURN_TO_URI: str = "/accounting"
 """The URL to return to after the operation."""
```

### Comparing `mia-accounting-1.1.0/tests/test_offset.py` & `mia-accounting-1.2.0/tests/test_offset.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,27 +13,28 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The test for the offset.
 
 """
+from __future__ import annotations
+
 import unittest
 from decimal import Decimal
 
 import httpx
 from click.testing import Result
 from flask import Flask
 from flask.testing import FlaskCliRunner
 
 from test_site import db
-from testlib import Accounts, create_test_app, get_client
-from testlib_journal_entry import match_journal_entry_detail
-from testlib_offset import TestData, JournalEntryLineItemData, \
-    JournalEntryData, CurrencyData
+from testlib import Accounts, create_test_app, get_client, \
+    match_journal_entry_detail, JournalEntryLineItemData, \
+    JournalEntryCurrencyData, JournalEntryData, BaseTestData
 
 PREFIX: str = "/accounting/journal-entries"
 """The URL prefix for the journal entry management."""
 
 
 class OffsetTestCase(unittest.TestCase):
     """The offset test case."""
@@ -62,30 +63,31 @@
             result = runner.invoke(args=["accounting-init-accounts",
                                          "-u", "editor"])
             self.assertEqual(result.exit_code, 0)
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
-        self.data: TestData = TestData(self.app, self.client, self.csrf_token)
+        self.data: OffsetTestData = OffsetTestData(
+            self.app, self.client, self.csrf_token)
 
     def test_add_receivable_offset(self) -> None:
         """Tests to add the receivable offset.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntry
         create_uri: str = f"{PREFIX}/create/receipt?next=%2F_next"
         store_uri: str = f"{PREFIX}/store/receipt"
         form: dict[str, str]
         old_amount: Decimal
         response: httpx.Response
 
         journal_entry_data: JournalEntryData = JournalEntryData(
-            self.data.l_r_or3d.journal_entry.days, [CurrencyData(
+            self.data.l_r_or3d.journal_entry.days, [JournalEntryCurrencyData(
                 "USD",
                 [],
                 [JournalEntryLineItemData(
                     Accounts.RECEIVABLE,
                     self.data.l_r_or1d.description, "300",
                     original_line_item=self.data.l_r_or1d),
                  JournalEntryLineItemData(
@@ -103,15 +105,15 @@
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The same debit or credit
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-credit-1-original_line_item_id"] \
-            = self.data.l_p_or1c.id
+            = str(self.data.l_p_or1c.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_or1c.account
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The original line item does not need offset
@@ -127,15 +129,15 @@
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-credit-1-original_line_item_id"] \
-            = self.data.l_p_of1d.id
+            = str(self.data.l_p_of1d.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_of1d.account
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same currency
         form = journal_entry_data.new_form(self.csrf_token)
@@ -213,15 +215,15 @@
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The same debit or credit
         form = journal_entry_data.update_form(self.csrf_token)
         form["currency-1-credit-1-original_line_item_id"] \
-            = self.data.l_p_or1c.id
+            = str(self.data.l_p_or1c.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_or1c.account
         form["currency-1-debit-1-amount"] = "100"
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
@@ -238,15 +240,15 @@
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
         form = journal_entry_data.update_form(self.csrf_token)
         form["currency-1-credit-1-original_line_item_id"] \
-            = self.data.l_p_of1d.id
+            = str(self.data.l_p_of1d.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_of1d.account
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same currency
         form = journal_entry_data.update_form(self.csrf_token)
@@ -401,15 +403,15 @@
         from accounting.models import Account, JournalEntry
         create_uri: str = f"{PREFIX}/create/disbursement?next=%2F_next"
         store_uri: str = f"{PREFIX}/store/disbursement"
         form: dict[str, str]
         response: httpx.Response
 
         journal_entry_data: JournalEntryData = JournalEntryData(
-            self.data.l_p_or3c.journal_entry.days, [CurrencyData(
+            self.data.l_p_or3c.journal_entry.days, [JournalEntryCurrencyData(
                 "USD",
                 [JournalEntryLineItemData(
                     Accounts.PAYABLE,
                     self.data.l_p_or1c.description, "500",
                     original_line_item=self.data.l_p_or1c),
                  JournalEntryLineItemData(
                      Accounts.PAYABLE,
@@ -427,15 +429,15 @@
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The same debit or credit
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-debit-1-original_line_item_id"] \
-            = self.data.l_r_or1d.id
+            = str(self.data.l_r_or1d.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_or1d.account
         form["currency-1-debit-1-amount"] = "100"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The original line item does not need offset
@@ -451,15 +453,15 @@
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-debit-1-original_line_item_id"] \
-            = self.data.l_r_of1c.id
+            = str(self.data.l_r_of1c.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_of1c.account
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same currency
         form = journal_entry_data.new_form(self.csrf_token)
@@ -537,15 +539,15 @@
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The same debit or credit
         form = journal_entry_data.update_form(self.csrf_token)
         form["currency-1-debit-1-original_line_item_id"] \
-            = self.data.l_r_or1d.id
+            = str(self.data.l_r_or1d.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_or1d.account
         form["currency-1-debit-1-amount"] = "100"
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
@@ -562,15 +564,15 @@
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
         form = journal_entry_data.update_form(self.csrf_token)
         form["currency-1-debit-1-original_line_item_id"] \
-            = self.data.l_r_of1c.id
+            = str(self.data.l_r_of1c.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_of1c.account
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same currency
         form = journal_entry_data.update_form(self.csrf_token)
@@ -716,7 +718,118 @@
                 JournalEntry, journal_entry_data.id)
             self.assertIsNotNone(journal_entry_or)
             journal_entry_of: JournalEntry | None = db.session.get(
                 JournalEntry, self.data.j_p_of1.id)
             self.assertIsNotNone(journal_entry_of)
             self.assertEqual(journal_entry_or.date, journal_entry_of.date)
             self.assertLess(journal_entry_or.no, journal_entry_of.no)
+
+
+class OffsetTestData(BaseTestData):
+    """The offset test data."""
+
+    def _init_data(self) -> None:
+        # Receivable original line items
+        self.l_r_or1d, self.l_r_or1c = self._couple(
+            "Accountant", "1200", Accounts.RECEIVABLE, Accounts.SERVICE)
+        self.l_r_or2d, self.l_r_or2c = self._couple(
+            "Toy", "600", Accounts.RECEIVABLE, Accounts.SALES)
+        self.l_r_or3d, self.l_r_or3c = self._couple(
+            "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
+        self.l_r_or4d, self.l_r_or4c = self._couple(
+            "Interest", "3.4", Accounts.RECEIVABLE, Accounts.INTEREST)
+
+        # Payable original line items
+        self.l_p_or1d, self.l_p_or1c = self._couple(
+            "Airplane", "2000", Accounts.TRAVEL, Accounts.PAYABLE)
+        self.l_p_or2d, self.l_p_or2c = self._couple(
+            "Phone", "900", Accounts.OFFICE, Accounts.PAYABLE)
+        self.l_p_or3d, self.l_p_or3c = self._couple(
+            "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
+        self.l_p_or4d, self.l_p_or4c = self._couple(
+            "Envelop", "0.9", Accounts.OFFICE, Accounts.PAYABLE)
+
+        # Original journal entries
+        self.j_r_or1: JournalEntryData = JournalEntryData(
+            50, [JournalEntryCurrencyData(
+                "USD", [self.l_r_or1d, self.l_r_or4d],
+                [self.l_r_or1c, self.l_r_or4c])])
+        self.j_r_or2: JournalEntryData = JournalEntryData(
+            30, [JournalEntryCurrencyData(
+                "USD", [self.l_r_or2d, self.l_r_or3d],
+                [self.l_r_or2c, self.l_r_or3c])])
+        self.j_p_or1: JournalEntryData = JournalEntryData(
+            40, [JournalEntryCurrencyData(
+                "USD", [self.l_p_or1d, self.l_p_or4d],
+                [self.l_p_or1c, self.l_p_or4c])])
+        self.j_p_or2: JournalEntryData = JournalEntryData(
+            20, [JournalEntryCurrencyData(
+                "USD", [self.l_p_or2d, self.l_p_or3d],
+                [self.l_p_or2c, self.l_p_or3c])])
+
+        self._add_journal_entry(self.j_r_or1)
+        self._add_journal_entry(self.j_r_or2)
+        self._add_journal_entry(self.j_p_or1)
+        self._add_journal_entry(self.j_p_or2)
+
+        # Receivable offset items
+        self.l_r_of1d, self.l_r_of1c = self._couple(
+            "Accountant", "500", Accounts.CASH, Accounts.RECEIVABLE)
+        self.l_r_of1c.original_line_item = self.l_r_or1d
+        self.l_r_of2d, self.l_r_of2c = self._couple(
+            "Accountant", "200", Accounts.CASH, Accounts.RECEIVABLE)
+        self.l_r_of2c.original_line_item = self.l_r_or1d
+        self.l_r_of3d, self.l_r_of3c = self._couple(
+            "Accountant", "100", Accounts.CASH, Accounts.RECEIVABLE)
+        self.l_r_of3c.original_line_item = self.l_r_or1d
+        self.l_r_of4d, self.l_r_of4c = self._couple(
+            "Toy", "240", Accounts.CASH, Accounts.RECEIVABLE)
+        self.l_r_of4c.original_line_item = self.l_r_or2d
+        self.l_r_of5d, self.l_r_of5c = self._couple(
+            "Interest", "3.4", Accounts.CASH, Accounts.RECEIVABLE)
+        self.l_r_of5c.original_line_item = self.l_r_or4d
+
+        # Payable offset items
+        self.l_p_of1d, self.l_p_of1c = self._couple(
+            "Airplane", "800", Accounts.PAYABLE, Accounts.CASH)
+        self.l_p_of1d.original_line_item = self.l_p_or1c
+        self.l_p_of2d, self.l_p_of2c = self._couple(
+            "Airplane", "300", Accounts.PAYABLE, Accounts.CASH)
+        self.l_p_of2d.original_line_item = self.l_p_or1c
+        self.l_p_of3d, self.l_p_of3c = self._couple(
+            "Airplane", "100", Accounts.PAYABLE, Accounts.CASH)
+        self.l_p_of3d.original_line_item = self.l_p_or1c
+        self.l_p_of4d, self.l_p_of4c = self._couple(
+            "Phone", "400", Accounts.PAYABLE, Accounts.CASH)
+        self.l_p_of4d.original_line_item = self.l_p_or2c
+        self.l_p_of5d, self.l_p_of5c = self._couple(
+            "Envelop", "0.9", Accounts.PAYABLE, Accounts.CASH)
+        self.l_p_of5d.original_line_item = self.l_p_or4c
+
+        # Offset journal entries
+        self.j_r_of1: JournalEntryData = JournalEntryData(
+            25, [JournalEntryCurrencyData(
+                "USD", [self.l_r_of1d], [self.l_r_of1c])])
+        self.j_r_of2: JournalEntryData = JournalEntryData(
+            20, [JournalEntryCurrencyData(
+                "USD", [self.l_r_of2d, self.l_r_of3d, self.l_r_of4d],
+                [self.l_r_of2c, self.l_r_of3c, self.l_r_of4c])])
+        self.j_r_of3: JournalEntryData = JournalEntryData(
+            15, [JournalEntryCurrencyData(
+                "USD", [self.l_r_of5d], [self.l_r_of5c])])
+        self.j_p_of1: JournalEntryData = JournalEntryData(
+            15, [JournalEntryCurrencyData(
+                "USD", [self.l_p_of1d], [self.l_p_of1c])])
+        self.j_p_of2: JournalEntryData = JournalEntryData(
+            10, [JournalEntryCurrencyData(
+                "USD", [self.l_p_of2d, self.l_p_of3d, self.l_p_of4d],
+                [self.l_p_of2c, self.l_p_of3c, self.l_p_of4c])])
+        self.j_p_of3: JournalEntryData = JournalEntryData(
+            5, [JournalEntryCurrencyData(
+                "USD", [self.l_p_of5d], [self.l_p_of5c])])
+
+        self._add_journal_entry(self.j_r_of1)
+        self._add_journal_entry(self.j_r_of2)
+        self._add_journal_entry(self.j_r_of3)
+        self._add_journal_entry(self.j_p_of1)
+        self._add_journal_entry(self.j_p_of2)
+        self._add_journal_entry(self.j_p_of3)
```

### Comparing `mia-accounting-1.1.0/tests/test_offset_matcher.py` & `mia-accounting-1.2.0/tests/test_unmatched_offset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # The Mia! Accounting Project.
-# Author: imacat@mail.imacat.idv.tw (imacat), 2023/3/11
+# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/8
 
 #  Copyright (c) 2023 imacat.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-"""The test for the offset matcher.
+"""The test for the unmatched offsets.
 
 """
 import unittest
 
 import httpx
 from click.testing import Result
 from flask import Flask
 from flask.testing import FlaskCliRunner
 
 from test_site import db
-from testlib import create_test_app, get_client, Accounts
-from testlib_journal_entry import match_journal_entry_detail
-from testlib_offset import JournalEntryData, CurrencyData, \
-    JournalEntryLineItemData
+from testlib import create_test_app, get_client, Accounts, \
+    JournalEntryCurrencyData, JournalEntryData, BaseTestData
 
+PREFIX: str = "/accounting/unmatched-offsets"
+"""The URL prefix for the unmatched offset management."""
 
-class OffsetMatcherTestCase(unittest.TestCase):
-    """The offset matcher test case."""
+
+class UnmatchedOffsetTestCase(unittest.TestCase):
+    """The unmatched offset test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
@@ -59,27 +60,105 @@
                                          "-u", "editor"])
             self.assertEqual(result.exit_code, 0)
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
+    def test_nobody(self) -> None:
+        """Test the permission as nobody.
+
+        :return: None.
+        """
+        client, csrf_token = get_client(self.app, "nobody")
+        DifferentTestData(self.app, self.client, self.csrf_token)
+        response: httpx.Response
+
+        response = client.get(PREFIX)
+        self.assertEqual(response.status_code, 403)
+
+        response = client.get(f"{PREFIX}/{Accounts.PAYABLE}")
+        self.assertEqual(response.status_code, 403)
+
+        response = client.post(f"{PREFIX}/{Accounts.PAYABLE}",
+                               data={"csrf_token": csrf_token})
+        self.assertEqual(response.status_code, 403)
+
+    def test_viewer(self) -> None:
+        """Test the permission as viewer.
+
+        :return: None.
+        """
+        client, csrf_token = get_client(self.app, "viewer")
+        DifferentTestData(self.app, self.client, self.csrf_token)
+        response: httpx.Response
+
+        response = client.get(PREFIX)
+        self.assertEqual(response.status_code, 403)
+
+        response = client.get(f"{PREFIX}/{Accounts.PAYABLE}")
+        self.assertEqual(response.status_code, 403)
+
+        response = client.post(f"{PREFIX}/{Accounts.PAYABLE}",
+                               data={"csrf_token": csrf_token})
+        self.assertEqual(response.status_code, 403)
+
+    def test_editor(self) -> None:
+        """Test the permission as editor.
+
+        :return: None.
+        """
+        DifferentTestData(self.app, self.client, self.csrf_token)
+        response: httpx.Response
+
+        response = self.client.get(PREFIX)
+        self.assertEqual(response.status_code, 200)
+
+        response = self.client.get(f"{PREFIX}/{Accounts.PAYABLE}")
+        self.assertEqual(response.status_code, 200)
+
+        response = self.client.post(f"{PREFIX}/{Accounts.PAYABLE}",
+                                    data={"csrf_token": self.csrf_token})
+        self.assertEqual(response.status_code, 302)
+        self.assertEqual(response.headers["Location"],
+                         f"{PREFIX}/{Accounts.PAYABLE}")
+
+    def test_empty_db(self) -> None:
+        """Test the empty database.
+
+        :return: None.
+        """
+        response: httpx.Response
+
+        response = self.client.get(PREFIX)
+        self.assertEqual(response.status_code, 200)
+
+        response = self.client.get(f"{PREFIX}/{Accounts.PAYABLE}")
+        self.assertEqual(response.status_code, 200)
+
+        response = self.client.post(f"{PREFIX}/{Accounts.PAYABLE}",
+                                    data={"csrf_token": self.csrf_token})
+        self.assertEqual(response.status_code, 302)
+        self.assertEqual(response.headers["Location"],
+                         f"{PREFIX}/{Accounts.PAYABLE}")
+
     def test_different(self) -> None:
         """Tests to match against different descriptions and amounts.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntryLineItem
         from accounting.utils.offset_matcher import OffsetMatcher
         data: DifferentTestData \
             = DifferentTestData(self.app, self.client, self.csrf_token)
         account: Account | None
         line_item: JournalEntryLineItem | None
         matcher: OffsetMatcher
         list_uri: str
+        match_uri: str
         response: httpx.Response
 
         # The receivables
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
             matcher = OffsetMatcher(account)
@@ -96,16 +175,17 @@
             for line_item_id in {data.l_r_of1c.id, data.l_r_of2c.id,
                                  data.l_r_of3c.id, data.l_r_of4c.id,
                                  data.l_r_of5c.id}:
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
 
-        list_uri = f"/accounting/unmatched-offsets/{Accounts.RECEIVABLE}"
-        response = self.client.post(list_uri,
+        list_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
+        match_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
+        response = self.client.post(match_uri,
                                     data={"csrf_token": self.csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], list_uri)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
@@ -145,16 +225,17 @@
             for line_item_id in {data.l_p_of1d.id, data.l_p_of2d.id,
                                  data.l_p_of3d.id, data.l_p_of4d.id,
                                  data.l_p_of5d.id}:
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
 
-        list_uri = f"/accounting/unmatched-offsets/{Accounts.PAYABLE}"
-        response = self.client.post(list_uri,
+        list_uri = f"{PREFIX}/{Accounts.PAYABLE}"
+        match_uri = f"{PREFIX}/{Accounts.PAYABLE}"
+        response = self.client.post(match_uri,
                                     data={"csrf_token": self.csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], list_uri)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
@@ -185,14 +266,15 @@
         from accounting.utils.offset_matcher import OffsetMatcher
         data: SameTestData \
             = SameTestData(self.app, self.client, self.csrf_token)
         account: Account | None
         line_item: JournalEntryLineItem | None
         matcher: OffsetMatcher
         list_uri: str
+        match_uri: str
         response: httpx.Response
 
         # The receivables
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
             matcher = OffsetMatcher(account)
@@ -216,16 +298,17 @@
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_r_of3c.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_r_or2d.id)
 
-        list_uri = f"/accounting/unmatched-offsets/{Accounts.RECEIVABLE}"
-        response = self.client.post(list_uri,
+        list_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
+        match_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
+        response = self.client.post(match_uri,
                                     data={"csrf_token": self.csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], list_uri)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
@@ -281,16 +364,17 @@
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_p_of3d.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_p_or2c.id)
 
-        list_uri = f"/accounting/unmatched-offsets/{Accounts.PAYABLE}"
-        response = self.client.post(list_uri,
+        list_uri = f"{PREFIX}/{Accounts.PAYABLE}"
+        match_uri = f"{PREFIX}/{Accounts.PAYABLE}"
+        response = self.client.post(match_uri,
                                     data={"csrf_token": self.csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], list_uri)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
@@ -318,375 +402,183 @@
             self.assertEqual(line_item.original_line_item_id, data.l_p_or3c.id)
             line_item = db.session.get(JournalEntryLineItem, data.l_p_of6d.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_p_or4c.id)
 
 
-class DifferentTestData:
+class DifferentTestData(BaseTestData):
     """The test data for different descriptions and amounts."""
 
-    def __init__(self, app: Flask, client: httpx.Client, csrf_token: str):
-        """Constructs the test data.
-
-        :param app: The Flask application.
-        :param client: The client.
-        :param csrf_token: The CSRF token.
-        """
-        self.app: Flask = app
-        self.client: httpx.Client = client
-        self.csrf_token: str = csrf_token
-
-        def couple(description: str, amount: str, debit: str, credit: str) \
-                -> tuple[JournalEntryLineItemData, JournalEntryLineItemData]:
-            """Returns a couple of debit-credit line items.
-
-            :param description: The description.
-            :param amount: The amount.
-            :param debit: The debit account code.
-            :param credit: The credit account code.
-            :return: The debit line item and credit line item.
-            """
-            return JournalEntryLineItemData(debit, description, amount),\
-                JournalEntryLineItemData(credit, description, amount)
-
+    def _init_data(self) -> None:
         # Receivable original line items
-        self.l_r_or1d, self.l_r_or1c = couple(
+        self.l_r_or1d, self.l_r_or1c = self._couple(
             "Accountant", "1200", Accounts.RECEIVABLE, Accounts.SERVICE)
-        self.l_r_or2d, self.l_r_or2c = couple(
+        self.l_r_or2d, self.l_r_or2c = self._couple(
             "Toy", "600", Accounts.RECEIVABLE, Accounts.SALES)
-        self.l_r_or3d, self.l_r_or3c = couple(
+        self.l_r_or3d, self.l_r_or3c = self._couple(
             "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
-        self.l_r_or4d, self.l_r_or4c = couple(
+        self.l_r_or4d, self.l_r_or4c = self._couple(
             "Interest", "3.4", Accounts.RECEIVABLE, Accounts.INTEREST)
 
         # Payable original line items
-        self.l_p_or1d, self.l_p_or1c = couple(
+        self.l_p_or1d, self.l_p_or1c = self._couple(
             "Airplane", "2000", Accounts.TRAVEL, Accounts.PAYABLE)
-        self.l_p_or2d, self.l_p_or2c = couple(
+        self.l_p_or2d, self.l_p_or2c = self._couple(
             "Phone", "900", Accounts.OFFICE, Accounts.PAYABLE)
-        self.l_p_or3d, self.l_p_or3c = couple(
+        self.l_p_or3d, self.l_p_or3c = self._couple(
             "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
-        self.l_p_or4d, self.l_p_or4c = couple(
+        self.l_p_or4d, self.l_p_or4c = self._couple(
             "Envelop", "0.9", Accounts.OFFICE, Accounts.PAYABLE)
 
         # Original journal entries
         self.j_r_or1: JournalEntryData = JournalEntryData(
-            50, [CurrencyData("USD", [self.l_r_or1d, self.l_r_or4d],
-                              [self.l_r_or1c, self.l_r_or4c])])
+            50, [JournalEntryCurrencyData(
+                "USD", [self.l_r_or1d, self.l_r_or4d],
+                [self.l_r_or1c, self.l_r_or4c])])
         self.j_r_or2: JournalEntryData = JournalEntryData(
-            30, [CurrencyData("USD", [self.l_r_or2d, self.l_r_or3d],
-                              [self.l_r_or2c, self.l_r_or3c])])
+            30, [JournalEntryCurrencyData(
+                "USD", [self.l_r_or2d, self.l_r_or3d],
+                [self.l_r_or2c, self.l_r_or3c])])
         self.j_p_or1: JournalEntryData = JournalEntryData(
-            40, [CurrencyData("USD", [self.l_p_or1d, self.l_p_or4d],
-                              [self.l_p_or1c, self.l_p_or4c])])
+            40, [JournalEntryCurrencyData(
+                "USD", [self.l_p_or1d, self.l_p_or4d],
+                [self.l_p_or1c, self.l_p_or4c])])
         self.j_p_or2: JournalEntryData = JournalEntryData(
-            20, [CurrencyData("USD", [self.l_p_or2d, self.l_p_or3d],
-                              [self.l_p_or2c, self.l_p_or3c])])
-
-        self.__add_journal_entry(self.j_r_or1)
-        self.__add_journal_entry(self.j_r_or2)
-        self.__add_journal_entry(self.j_p_or1)
-        self.__add_journal_entry(self.j_p_or2)
+            20, [JournalEntryCurrencyData(
+                "USD", [self.l_p_or2d, self.l_p_or3d],
+                [self.l_p_or2c, self.l_p_or3c])])
+
+        self._add_journal_entry(self.j_r_or1)
+        self._add_journal_entry(self.j_r_or2)
+        self._add_journal_entry(self.j_p_or1)
+        self._add_journal_entry(self.j_p_or2)
 
         # Receivable offset items
-        self.l_r_of1d, self.l_r_of1c = couple(
+        self.l_r_of1d, self.l_r_of1c = self._couple(
             "Accountant", "500", Accounts.CASH, Accounts.RECEIVABLE)
-        self.l_r_of2d, self.l_r_of2c = couple(
+        self.l_r_of2d, self.l_r_of2c = self._couple(
             "Accountant", "200", Accounts.CASH, Accounts.RECEIVABLE)
-        self.l_r_of3d, self.l_r_of3c = couple(
+        self.l_r_of3d, self.l_r_of3c = self._couple(
             "Accountant", "100", Accounts.CASH, Accounts.RECEIVABLE)
-        self.l_r_of4d, self.l_r_of4c = couple(
+        self.l_r_of4d, self.l_r_of4c = self._couple(
             "Toy", "240", Accounts.CASH, Accounts.RECEIVABLE)
-        self.l_r_of5d, self.l_r_of5c = couple(
+        self.l_r_of5d, self.l_r_of5c = self._couple(
             "Interest", "3.4", Accounts.CASH, Accounts.RECEIVABLE)
 
         # Payable offset items
-        self.l_p_of1d, self.l_p_of1c = couple(
+        self.l_p_of1d, self.l_p_of1c = self._couple(
             "Airplane", "800", Accounts.PAYABLE, Accounts.CASH)
-        self.l_p_of2d, self.l_p_of2c = couple(
+        self.l_p_of2d, self.l_p_of2c = self._couple(
             "Airplane", "300", Accounts.PAYABLE, Accounts.CASH)
-        self.l_p_of3d, self.l_p_of3c = couple(
+        self.l_p_of3d, self.l_p_of3c = self._couple(
             "Airplane", "100", Accounts.PAYABLE, Accounts.CASH)
-        self.l_p_of4d, self.l_p_of4c = couple(
+        self.l_p_of4d, self.l_p_of4c = self._couple(
             "Phone", "400", Accounts.PAYABLE, Accounts.CASH)
-        self.l_p_of5d, self.l_p_of5c = couple(
+        self.l_p_of5d, self.l_p_of5c = self._couple(
             "Envelop", "0.9", Accounts.PAYABLE, Accounts.CASH)
 
         # Offset journal entries
         self.j_r_of1: JournalEntryData = JournalEntryData(
-            25, [CurrencyData("USD", [self.l_r_of1d], [self.l_r_of1c])])
+            25, [JournalEntryCurrencyData(
+                "USD", [self.l_r_of1d], [self.l_r_of1c])])
         self.j_r_of2: JournalEntryData = JournalEntryData(
-            20, [CurrencyData("USD",
-                              [self.l_r_of2d, self.l_r_of3d, self.l_r_of4d],
-                              [self.l_r_of2c, self.l_r_of3c, self.l_r_of4c])])
+            20, [JournalEntryCurrencyData(
+                "USD", [self.l_r_of2d, self.l_r_of3d, self.l_r_of4d],
+                [self.l_r_of2c, self.l_r_of3c, self.l_r_of4c])])
         self.j_r_of3: JournalEntryData = JournalEntryData(
-            15, [CurrencyData("USD", [self.l_r_of5d], [self.l_r_of5c])])
+            15, [JournalEntryCurrencyData(
+                "USD", [self.l_r_of5d], [self.l_r_of5c])])
         self.j_p_of1: JournalEntryData = JournalEntryData(
-            15, [CurrencyData("USD", [self.l_p_of1d], [self.l_p_of1c])])
+            15, [JournalEntryCurrencyData(
+                "USD", [self.l_p_of1d], [self.l_p_of1c])])
         self.j_p_of2: JournalEntryData = JournalEntryData(
-            10, [CurrencyData("USD",
-                              [self.l_p_of2d, self.l_p_of3d, self.l_p_of4d],
-                              [self.l_p_of2c, self.l_p_of3c, self.l_p_of4c])])
+            10, [JournalEntryCurrencyData(
+                "USD", [self.l_p_of2d, self.l_p_of3d, self.l_p_of4d],
+                [self.l_p_of2c, self.l_p_of3c, self.l_p_of4c])])
         self.j_p_of3: JournalEntryData = JournalEntryData(
-            5, [CurrencyData("USD", [self.l_p_of5d], [self.l_p_of5c])])
+            5, [JournalEntryCurrencyData(
+                "USD", [self.l_p_of5d], [self.l_p_of5c])])
 
-        self.__set_is_need_offset(False)
-        self.__add_journal_entry(self.j_r_of1)
-        self.__add_journal_entry(self.j_r_of2)
-        self.__add_journal_entry(self.j_r_of3)
-        self.__add_journal_entry(self.j_p_of1)
-        self.__add_journal_entry(self.j_p_of2)
-        self.__add_journal_entry(self.j_p_of3)
-        self.__set_is_need_offset(True)
-
-    def __set_is_need_offset(self, is_need_offset: bool) -> None:
-        """Sets whether the payables and receivables need offset.
-
-        :param is_need_offset: True if payables and receivables need offset, or
-            False otherwise.
-        :return:
-        """
-        from accounting.models import Account
-        with self.app.app_context():
-            for code in {Accounts.RECEIVABLE, Accounts.PAYABLE}:
-                account: Account | None = Account.find_by_code(code)
-                assert account is not None
-                account.is_need_offset = is_need_offset
-            db.session.commit()
-
-    def __add_journal_entry(self, journal_entry_data: JournalEntryData) \
-            -> None:
-        """Adds a journal entry.
+        self._set_need_offset({Accounts.RECEIVABLE, Accounts.PAYABLE}, False)
+        self._add_journal_entry(self.j_r_of1)
+        self._add_journal_entry(self.j_r_of2)
+        self._add_journal_entry(self.j_r_of3)
+        self._add_journal_entry(self.j_p_of1)
+        self._add_journal_entry(self.j_p_of2)
+        self._add_journal_entry(self.j_p_of3)
+        self._set_need_offset({Accounts.RECEIVABLE, Accounts.PAYABLE}, True)
 
-        :param journal_entry_data: The journal entry data.
-        :return: None.
-        """
-        from accounting.models import JournalEntry
-        store_uri: str = "/accounting/journal-entries/store/transfer"
-
-        response: httpx.Response = self.client.post(
-            store_uri, data=journal_entry_data.new_form(self.csrf_token))
-        assert response.status_code == 302
-        journal_entry_id: int \
-            = match_journal_entry_detail(response.headers["Location"])
-        journal_entry_data.id = journal_entry_id
-        with self.app.app_context():
-            journal_entry: JournalEntry | None \
-                = db.session.get(JournalEntry, journal_entry_id)
-            assert journal_entry is not None
-            for i in range(len(journal_entry.currencies)):
-                for j in range(len(journal_entry.currencies[i].debit)):
-                    journal_entry_data.currencies[i].debit[j].id \
-                        = journal_entry.currencies[i].debit[j].id
-                for j in range(len(journal_entry.currencies[i].credit)):
-                    journal_entry_data.currencies[i].credit[j].id \
-                        = journal_entry.currencies[i].credit[j].id
 
-
-class SameTestData:
+class SameTestData(BaseTestData):
     """The test data with same descriptions and amounts."""
 
-    def __init__(self, app: Flask, client: httpx.Client, csrf_token: str):
-        """Constructs the test data.
-
-        :param app: The Flask application.
-        :param client: The client.
-        :param csrf_token: The CSRF token.
-        """
-        self.app: Flask = app
-        self.client: httpx.Client = client
-        self.csrf_token: str = csrf_token
-
-        def couple(description: str, amount: str, debit: str, credit: str) \
-                -> tuple[JournalEntryLineItemData, JournalEntryLineItemData]:
-            """Returns a couple of debit-credit line items.
-
-            :param description: The description.
-            :param amount: The amount.
-            :param debit: The debit account code.
-            :param credit: The credit account code.
-            :return: The debit line item and credit line item.
-            """
-            return JournalEntryLineItemData(debit, description, amount),\
-                JournalEntryLineItemData(credit, description, amount)
-
+    def _init_data(self) -> None:
         # Receivable original line items
-        self.l_r_or1d, self.l_r_or1c = couple(
-            "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
-        self.l_r_or2d, self.l_r_or2c = couple(
-            "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
-        self.l_r_or3d, self.l_r_or3c = couple(
-            "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
-        self.l_r_or4d, self.l_r_or4c = couple(
-            "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
-        self.l_r_or5d, self.l_r_or5c = couple(
-            "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
-        self.l_r_or6d, self.l_r_or6c = couple(
-            "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
+        self.l_r_or1d, self.l_r_or1c = self._add_simple_journal_entry(
+            60, "USD", "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
+        self.l_r_or2d, self.l_r_or2c = self._add_simple_journal_entry(
+            50, "USD", "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
+        self.l_r_or3d, self.l_r_or3c = self._add_simple_journal_entry(
+            40, "USD", "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
+        self.l_r_or4d, self.l_r_or4c = self._add_simple_journal_entry(
+            30, "USD", "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
+        self.l_r_or5d, self.l_r_or5c = self._add_simple_journal_entry(
+            20, "USD", "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
+        self.l_r_or6d, self.l_r_or6c = self._add_simple_journal_entry(
+            10, "USD", "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
 
         # Payable original line items
-        self.l_p_or1d, self.l_p_or1c = couple(
-            "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
-        self.l_p_or2d, self.l_p_or2c = couple(
-            "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
-        self.l_p_or3d, self.l_p_or3c = couple(
-            "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
-        self.l_p_or4d, self.l_p_or4c = couple(
-            "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
-        self.l_p_or5d, self.l_p_or5c = couple(
-            "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
-        self.l_p_or6d, self.l_p_or6c = couple(
-            "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
+        self.l_p_or1d, self.l_p_or1c = self._add_simple_journal_entry(
+            60, "USD", "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
+        self.l_p_or2d, self.l_p_or2c = self._add_simple_journal_entry(
+            50, "USD", "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
+        self.l_p_or3d, self.l_p_or3c = self._add_simple_journal_entry(
+            40, "USD", "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
+        self.l_p_or4d, self.l_p_or4c = self._add_simple_journal_entry(
+            30, "USD", "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
+        self.l_p_or5d, self.l_p_or5c = self._add_simple_journal_entry(
+            20, "USD", "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
+        self.l_p_or6d, self.l_p_or6c = self._add_simple_journal_entry(
+            10, "USD", "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
 
-        # Original journal entries
-        self.j_r_or1: JournalEntryData = JournalEntryData(
-            60, [CurrencyData("USD", [self.l_r_or1d], [self.l_r_or1c])])
-        self.j_r_or2: JournalEntryData = JournalEntryData(
-            50, [CurrencyData("USD", [self.l_r_or2d], [self.l_r_or2c])])
-        self.j_r_or3: JournalEntryData = JournalEntryData(
-            40, [CurrencyData("USD", [self.l_r_or3d], [self.l_r_or3c])])
-        self.j_r_or4: JournalEntryData = JournalEntryData(
-            30, [CurrencyData("USD", [self.l_r_or4d], [self.l_r_or4c])])
-        self.j_r_or5: JournalEntryData = JournalEntryData(
-            20, [CurrencyData("USD", [self.l_r_or5d], [self.l_r_or5c])])
-        self.j_r_or6: JournalEntryData = JournalEntryData(
-            10, [CurrencyData("USD", [self.l_r_or6d], [self.l_r_or6c])])
-        self.j_p_or1: JournalEntryData = JournalEntryData(
-            60, [CurrencyData("USD", [self.l_p_or1d], [self.l_p_or1c])])
-        self.j_p_or2: JournalEntryData = JournalEntryData(
-            50, [CurrencyData("USD", [self.l_p_or2d], [self.l_p_or2c])])
-        self.j_p_or3: JournalEntryData = JournalEntryData(
-            40, [CurrencyData("USD", [self.l_p_or3d], [self.l_p_or3c])])
-        self.j_p_or4: JournalEntryData = JournalEntryData(
-            30, [CurrencyData("USD", [self.l_p_or4d], [self.l_p_or4c])])
-        self.j_p_or5: JournalEntryData = JournalEntryData(
-            20, [CurrencyData("USD", [self.l_p_or5d], [self.l_p_or5c])])
-        self.j_p_or6: JournalEntryData = JournalEntryData(
-            10, [CurrencyData("USD", [self.l_p_or6d], [self.l_p_or6c])])
-
-        self.__add_journal_entry(self.j_r_or1)
-        self.__add_journal_entry(self.j_r_or2)
-        self.__add_journal_entry(self.j_r_or3)
-        self.__add_journal_entry(self.j_r_or4)
-        self.__add_journal_entry(self.j_r_or5)
-        self.__add_journal_entry(self.j_r_or6)
-        self.__add_journal_entry(self.j_p_or1)
-        self.__add_journal_entry(self.j_p_or2)
-        self.__add_journal_entry(self.j_p_or3)
-        self.__add_journal_entry(self.j_p_or4)
-        self.__add_journal_entry(self.j_p_or5)
-        self.__add_journal_entry(self.j_p_or6)
+        self._set_need_offset({Accounts.RECEIVABLE, Accounts.PAYABLE}, False)
 
         # Receivable offset items
-        self.l_r_of1d, self.l_r_of1c = couple(
-            "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
-        self.l_r_of2d, self.l_r_of2c = couple(
-            "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
-        self.l_r_of3d, self.l_r_of3c = couple(
+        self.l_r_of1d, self.l_r_of1c = self._add_simple_journal_entry(
+            65, "USD", "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
+        self.l_r_of2d, self.l_r_of2c = self._add_simple_journal_entry(
+            35, "USD", "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
+        self.l_r_of3d, self.l_r_of3c = self._couple(
             "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
         self.l_r_of3c.original_line_item = self.l_r_or2d
-        self.l_r_of4d, self.l_r_of4c = couple(
-            "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
-        self.l_r_of5d, self.l_r_of5c = couple(
-            "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
-        self.l_r_of6d, self.l_r_of6c = couple(
-            "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
+        j_r_of3: JournalEntryData = JournalEntryData(
+            35, [JournalEntryCurrencyData(
+                "USD", [self.l_r_of3d], [self.l_r_of3c])])
+        self.l_r_of4d, self.l_r_of4c = self._add_simple_journal_entry(
+            35, "USD", "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
+        self.l_r_of5d, self.l_r_of5c = self._add_simple_journal_entry(
+            35, "USD", "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
+        self.l_r_of6d, self.l_r_of6c = self._add_simple_journal_entry(
+            15, "USD", "Noodles", "100", Accounts.CASH, Accounts.RECEIVABLE)
 
         # Payable offset items
-        self.l_p_of1d, self.l_p_of1c = couple(
-            "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
-        self.l_p_of2d, self.l_p_of2c = couple(
-            "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
-        self.l_p_of3d, self.l_p_of3c = couple(
+        self.l_p_of1d, self.l_p_of1c = self._add_simple_journal_entry(
+            65, "USD", "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
+        self.l_p_of2d, self.l_p_of2c = self._add_simple_journal_entry(
+            35, "USD", "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
+        self.l_p_of3d, self.l_p_of3c = self._couple(
             "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
         self.l_p_of3d.original_line_item = self.l_p_or2c
-        self.l_p_of4d, self.l_p_of4c = couple(
-            "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
-        self.l_p_of5d, self.l_p_of5c = couple(
-            "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
-        self.l_p_of6d, self.l_p_of6c = couple(
-            "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
-
-        # Offset journal entries
-        self.j_r_of1: JournalEntryData = JournalEntryData(
-            65, [CurrencyData("USD", [self.l_r_of1d], [self.l_r_of1c])])
-        self.j_r_of2: JournalEntryData = JournalEntryData(
-            35, [CurrencyData("USD", [self.l_r_of2d], [self.l_r_of2c])])
-        self.j_r_of3: JournalEntryData = JournalEntryData(
-            35, [CurrencyData("USD", [self.l_r_of3d], [self.l_r_of3c])])
-        self.j_r_of4: JournalEntryData = JournalEntryData(
-            35, [CurrencyData("USD", [self.l_r_of4d], [self.l_r_of4c])])
-        self.j_r_of5: JournalEntryData = JournalEntryData(
-            35, [CurrencyData("USD", [self.l_r_of5d], [self.l_r_of5c])])
-        self.j_r_of6: JournalEntryData = JournalEntryData(
-            15, [CurrencyData("USD", [self.l_r_of6d], [self.l_r_of6c])])
-        self.j_p_of1: JournalEntryData = JournalEntryData(
-            65, [CurrencyData("USD", [self.l_p_of1d], [self.l_p_of1c])])
-        self.j_p_of2: JournalEntryData = JournalEntryData(
-            35, [CurrencyData("USD", [self.l_p_of2d], [self.l_p_of2c])])
-        self.j_p_of3: JournalEntryData = JournalEntryData(
-            35, [CurrencyData("USD", [self.l_p_of3d], [self.l_p_of3c])])
-        self.j_p_of4: JournalEntryData = JournalEntryData(
-            35, [CurrencyData("USD", [self.l_p_of4d], [self.l_p_of4c])])
-        self.j_p_of5: JournalEntryData = JournalEntryData(
-            35, [CurrencyData("USD", [self.l_p_of5d], [self.l_p_of5c])])
-        self.j_p_of6: JournalEntryData = JournalEntryData(
-            15, [CurrencyData("USD", [self.l_p_of6d], [self.l_p_of6c])])
-
-        self.__set_is_need_offset(False)
-        self.__add_journal_entry(self.j_r_of1)
-        self.__add_journal_entry(self.j_r_of2)
-        self.__add_journal_entry(self.j_r_of4)
-        self.__add_journal_entry(self.j_r_of5)
-        self.__add_journal_entry(self.j_r_of6)
-        self.__add_journal_entry(self.j_p_of1)
-        self.__add_journal_entry(self.j_p_of2)
-        self.__add_journal_entry(self.j_p_of4)
-        self.__add_journal_entry(self.j_p_of5)
-        self.__add_journal_entry(self.j_p_of6)
-        self.__set_is_need_offset(True)
-        self.__add_journal_entry(self.j_r_of3)
-        self.__add_journal_entry(self.j_p_of3)
-
-    def __set_is_need_offset(self, is_need_offset: bool) -> None:
-        """Sets whether the payables and receivables need offset.
-
-        :param is_need_offset: True if payables and receivables need offset, or
-            False otherwise.
-        :return:
-        """
-        from accounting.models import Account
-        with self.app.app_context():
-            for code in {Accounts.RECEIVABLE, Accounts.PAYABLE}:
-                account: Account | None = Account.find_by_code(code)
-                assert account is not None
-                account.is_need_offset = is_need_offset
-            db.session.commit()
-
-    def __add_journal_entry(self, journal_entry_data: JournalEntryData) \
-            -> None:
-        """Adds a journal entry.
-
-        :param journal_entry_data: The journal entry data.
-        :return: None.
-        """
-        from accounting.models import JournalEntry
-        store_uri: str = "/accounting/journal-entries/store/transfer"
-
-        response: httpx.Response = self.client.post(
-            store_uri, data=journal_entry_data.new_form(self.csrf_token))
-        assert response.status_code == 302
-        journal_entry_id: int \
-            = match_journal_entry_detail(response.headers["Location"])
-        journal_entry_data.id = journal_entry_id
-        with self.app.app_context():
-            journal_entry: JournalEntry | None \
-                = db.session.get(JournalEntry, journal_entry_id)
-            assert journal_entry is not None
-            for i in range(len(journal_entry.currencies)):
-                for j in range(len(journal_entry.currencies[i].debit)):
-                    journal_entry_data.currencies[i].debit[j].id \
-                        = journal_entry.currencies[i].debit[j].id
-                for j in range(len(journal_entry.currencies[i].credit)):
-                    journal_entry_data.currencies[i].credit[j].id \
-                        = journal_entry.currencies[i].credit[j].id
+        j_p_of3: JournalEntryData = JournalEntryData(
+            35, [JournalEntryCurrencyData(
+                "USD", [self.l_p_of3d], [self.l_p_of3c])])
+        self.l_p_of4d, self.l_p_of4c = self._add_simple_journal_entry(
+            35, "USD", "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
+        self.l_p_of5d, self.l_p_of5c = self._add_simple_journal_entry(
+            35, "USD", "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
+        self.l_p_of6d, self.l_p_of6c = self._add_simple_journal_entry(
+            15, "USD", "Steak", "120", Accounts.PAYABLE, Accounts.CASH)
+
+        self._set_need_offset({Accounts.RECEIVABLE, Accounts.PAYABLE}, True)
+        self._add_journal_entry(j_r_of3)
+        self._add_journal_entry(j_p_of3)
```

### Comparing `mia-accounting-1.1.0/tests/test_option.py` & `mia-accounting-1.2.0/tests/test_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import httpx
 from click.testing import Result
 from flask import Flask
 from flask.testing import FlaskCliRunner
 
 from test_site import db
 from testlib import NEXT_URI, Accounts, create_test_app, get_client
-from testlib_offset import TestData
 
 PREFIX: str = "/accounting/options"
 """The URL prefix for the option management."""
 DETAIL_URI: str = f"{PREFIX}?next=%2F_next"
 """THE URI for the option detail."""
 EDIT_URI: str = f"{PREFIX}/edit?next=%2F_next"
 """THE URI for the form to edit the options."""
@@ -64,15 +63,14 @@
             self.assertEqual(result.exit_code, 0)
             result = runner.invoke(args=["accounting-init-accounts",
                                          "-u", "editor"])
             self.assertEqual(result.exit_code, 0)
             Option.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "admin")
-        self.data: TestData = TestData(self.app, self.client, self.csrf_token)
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "nobody")
```

### Comparing `mia-accounting-1.1.0/tests/test_site/__init__.py` & `mia-accounting-1.2.0/tests/test_site/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/auth.py` & `mia-accounting-1.2.0/tests/test_site/auth.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/locale.py` & `mia-accounting-1.2.0/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/static/favicon.svg` & `mia-accounting-1.2.0/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/templates/base.html` & `mia-accounting-1.2.0/tests/test_site/templates/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/templates/home.html` & `mia-accounting-1.2.0/tests/test_site/templates/home.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/templates/login.html` & `mia-accounting-1.2.0/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/translations/messages.pot` & `mia-accounting-1.2.0/tests/test_site/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.2.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.2.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.2.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.2.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/test_utils.py` & `mia-accounting-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.1.0/tests/testlib_journal_entry.py` & `mia-accounting-1.2.0/tests/testlib_journal_entry.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The common test libraries for the journal entry test cases.
 
 """
 import re
-from decimal import Decimal
 from datetime import date
+from decimal import Decimal
 from secrets import randbelow
 
-import httpx
 from flask import Flask
 
 from test_site import db
 from testlib import NEXT_URI, Accounts
 
 NON_EMPTY_NOTE: str = "  This is \n\na test."
 """The stripped content of an non-empty note."""
@@ -371,47 +370,14 @@
     :return: The prefix of the currency.
     """
     key: str = [x for x in form if form[x] == code][0]
     m: re.Match = re.match(r"^(.+-)code$", key)
     return m.group(1)
 
 
-def add_journal_entry(client: httpx.Client, form: dict[str, str]) -> int:
-    """Adds a transfer journal entry.
-
-    :param client: The client.
-    :param form: The form data.
-    :return: The newly-added journal entry ID.
-    """
-    prefix: str = "/accounting/journal-entries"
-    journal_entry_type: str = "transfer"
-    if len({x for x in form if "-debit-" in x}) == 0:
-        journal_entry_type = "receipt"
-    elif len({x for x in form if "-credit-" in x}) == 0:
-        journal_entry_type = "disbursement"
-    store_uri = f"{prefix}/store/{journal_entry_type}"
-    response: httpx.Response = client.post(store_uri, data=form)
-    assert response.status_code == 302
-    return match_journal_entry_detail(response.headers["Location"])
-
-
-def match_journal_entry_detail(location: str) -> int:
-    """Validates if the redirect location is the journal entry detail, and
-    returns the journal entry ID on success.
-
-    :param location: The redirect location.
-    :return: The journal entry ID.
-    :raise AssertionError: When the location is not the journal entry detail.
-    """
-    m: re.Match = re.match(
-        r"^/accounting/journal-entries/(\d+)\?next=%2F_next", location)
-    assert m is not None
-    return int(m.group(1))
-
-
 def set_negative_amount(form: dict[str, str]) -> None:
     """Sets a negative amount in the form data, keeping the balance.
 
     :param form: The form data.
     :return: None.
     """
     amount_keys: list[str] = []
```

