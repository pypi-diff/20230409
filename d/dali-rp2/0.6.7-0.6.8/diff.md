# Comparing `tmp/dali-rp2-0.6.7.tar.gz` & `tmp/dali-rp2-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dali-rp2-0.6.7.tar", last modified: Sat Apr  1 23:15:03 2023, max compression
+gzip compressed data, was "dali-rp2-0.6.8.tar", last modified: Sun Apr  9 03:08:33 2023, max compression
```

## Comparing `dali-rp2-0.6.7.tar` & `dali-rp2-0.6.8.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.581433 dali-rp2-0.6.7/
--rw-r--r--   0 marcoz     (501) staff       (20)    10322 2023-04-01 22:55:20.000000 dali-rp2-0.6.7/CHANGELOG.md
--rw-r--r--   0 marcoz     (501) staff       (20)     3098 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/CONTRIBUTING.md
--rw-r--r--   0 marcoz     (501) staff       (20)    11357 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/LICENSE
--rw-r--r--   0 marcoz     (501) staff       (20)      214 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/MANIFEST.in
--rw-r--r--   0 marcoz     (501) staff       (20)    22271 2023-04-01 23:15:03.581510 dali-rp2-0.6.7/PKG-INFO
--rw-r--r--   0 marcoz     (501) staff       (20)    25117 2023-04-01 22:57:50.000000 dali-rp2-0.6.7/README.dev.md
--rw-r--r--   0 marcoz     (501) staff       (20)    10386 2023-04-01 22:57:50.000000 dali-rp2-0.6.7/README.md
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.556604 dali-rp2-0.6.7/docs/
--rw-r--r--   0 marcoz     (501) staff       (20)    42979 2023-03-27 04:35:29.000000 dali-rp2-0.6.7/docs/configuration_file.md
--rw-r--r--   0 marcoz     (501) staff       (20)     7936 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/docs/developer_faq.md
--rw-r--r--   0 marcoz     (501) staff       (20)     9765 2023-03-15 01:40:20.000000 dali-rp2-0.6.7/docs/user_faq.md
--rw-r--r--   0 marcoz     (501) staff       (20)      276 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/pyproject.toml
--rw-r--r--   0 marcoz     (501) staff       (20)     2227 2023-04-01 23:15:03.583013 dali-rp2-0.6.7/setup.cfg
--rw-r--r--   0 marcoz     (501) staff       (20)       92 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/setup.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.552777 dali-rp2-0.6.7/src/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.562495 dali-rp2-0.6.7/src/dali/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/__init__.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)    32069 2023-03-15 01:25:07.000000 dali-rp2-0.6.7/src/dali/abstract_ccxt_input_plugin.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2682 2023-03-15 01:25:21.000000 dali-rp2-0.6.7/src/dali/abstract_input_plugin.py
--rw-r--r--   0 marcoz     (501) staff       (20)    11488 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/abstract_pair_converter_plugin.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9563 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/abstract_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1393 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/cache.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     8487 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/ccxt_pagination.py
--rw-r--r--   0 marcoz     (501) staff       (20)     7309 2023-03-15 01:08:00.000000 dali-rp2-0.6.7/src/dali/configuration.py
--rw-r--r--   0 marcoz     (501) staff       (20)     3793 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/configuration_generator.py
--rw-r--r--   0 marcoz     (501) staff       (20)    18170 2023-04-01 22:57:50.000000 dali-rp2-0.6.7/src/dali/dali_main.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.563105 dali-rp2-0.6.7/src/dali/data/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/data/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)    18654 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/data/template.ods
--rw-r--r--   0 marcoz     (501) staff       (20)     2221 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/historical_bar.py
--rw-r--r--   0 marcoz     (501) staff       (20)     6571 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/in_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5429 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/intra_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)      674 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/logger.py
--rw-r--r--   0 marcoz     (501) staff       (20)    10625 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/ods_generator.py
--rw-r--r--   0 marcoz     (501) staff       (20)     6323 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/out_transaction.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.563565 dali-rp2-0.6.7/src/dali/plugin/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/__init__.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.564207 dali-rp2-0.6.7/src/dali/plugin/country/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/country/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)      728 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/country/jp.py
--rw-r--r--   0 marcoz     (501) staff       (20)      722 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/country/us.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.564392 dali-rp2-0.6.7/src/dali/plugin/input/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/input/__init__.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.567175 dali-rp2-0.6.7/src/dali/plugin/input/csv/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/__init__.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     7470 2023-03-15 01:28:27.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/binance_com_supplemental.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     6753 2023-03-15 01:28:27.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/bitbank_supplemental.py
--rw-r--r--   0 marcoz     (501) staff       (20)    13273 2023-03-15 01:28:27.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/blockfi.py
--rw-r--r--   0 marcoz     (501) staff       (20)     3662 2023-03-15 01:28:27.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/coincheck_supplemental.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5982 2023-03-15 01:28:27.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/ledger.py
--rw-r--r--   0 marcoz     (501) staff       (20)    10890 2023-03-15 01:28:27.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/manual.py
--rw-r--r--   0 marcoz     (501) staff       (20)     7545 2023-03-15 01:28:27.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/nexo.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     8413 2023-03-15 01:28:27.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/pionex.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4991 2023-03-27 04:39:21.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/trezor.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4639 2023-03-27 04:40:05.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/trezor_old.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5018 2023-03-27 04:41:07.000000 dali-rp2-0.6.7/src/dali/plugin/input/csv/trezor_v2.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.567846 dali-rp2-0.6.7/src/dali/plugin/input/ods/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-15 01:07:08.000000 dali-rp2-0.6.7/src/dali/plugin/input/ods/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)     6768 2023-03-15 01:28:27.000000 dali-rp2-0.6.7/src/dali/plugin/input/ods/rp2_input.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.569404 dali-rp2-0.6.7/src/dali/plugin/input/rest/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/input/rest/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)    50079 2023-03-15 01:36:01.000000 dali-rp2-0.6.7/src/dali/plugin/input/rest/binance_com.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5045 2023-03-15 01:36:15.000000 dali-rp2-0.6.7/src/dali/plugin/input/rest/bitbank.py
--rw-r--r--   0 marcoz     (501) staff       (20)    47555 2023-04-01 22:53:55.000000 dali-rp2-0.6.7/src/dali/plugin/input/rest/coinbase.py
--rw-r--r--   0 marcoz     (501) staff       (20)    24540 2023-03-15 01:28:27.000000 dali-rp2-0.6.7/src/dali/plugin/input/rest/coinbase_pro.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.571087 dali-rp2-0.6.7/src/dali/plugin/pair_converter/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/pair_converter/__init__.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)    21078 2023-03-18 05:56:18.000000 dali-rp2-0.6.7/src/dali/plugin/pair_converter/ccxt.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     1102 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/pair_converter/ccxt_binance.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     1186 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/pair_converter/ccxt_kraken.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.571437 dali-rp2-0.6.7/src/dali/plugin/pair_converter/csv/
--rwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/pair_converter/csv/__init__.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)    15593 2023-03-18 05:56:18.000000 dali-rp2-0.6.7/src/dali/plugin/pair_converter/csv/kraken.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2880 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/plugin/pair_converter/historic_crypto.py
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/py.typed
--rw-r--r--   0 marcoz     (501) staff       (20)    30850 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/src/dali/transaction_resolver.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.577923 dali-rp2-0.6.7/src/dali_rp2.egg-info/
--rw-r--r--   0 marcoz     (501) staff       (20)    22271 2023-04-01 23:15:03.000000 dali-rp2-0.6.7/src/dali_rp2.egg-info/PKG-INFO
--rw-r--r--   0 marcoz     (501) staff       (20)     2728 2023-04-01 23:15:03.000000 dali-rp2-0.6.7/src/dali_rp2.egg-info/SOURCES.txt
--rw-r--r--   0 marcoz     (501) staff       (20)        1 2023-04-01 23:15:03.000000 dali-rp2-0.6.7/src/dali_rp2.egg-info/dependency_links.txt
--rw-r--r--   0 marcoz     (501) staff       (20)      106 2023-04-01 23:15:03.000000 dali-rp2-0.6.7/src/dali_rp2.egg-info/entry_points.txt
--rw-r--r--   0 marcoz     (501) staff       (20)      323 2023-04-01 23:15:03.000000 dali-rp2-0.6.7/src/dali_rp2.egg-info/requires.txt
--rw-r--r--   0 marcoz     (501) staff       (20)        5 2023-04-01 23:15:03.000000 dali-rp2-0.6.7/src/dali_rp2.egg-info/top_level.txt
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 23:15:03.581313 dali-rp2-0.6.7/tests/
--rw-r--r--   0 marcoz     (501) staff       (20)     4774 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/tests/ods_diff.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4479 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/tests/test_cache.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4868 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/tests/test_historical_bar.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4543 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/tests/test_ods_output_diff.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)    47913 2023-03-15 01:34:26.000000 dali-rp2-0.6.7/tests/test_plugin_binance_com.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     6070 2023-03-15 01:34:26.000000 dali-rp2-0.6.7/tests/test_plugin_binance_com_supplemental_csv.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     2696 2023-03-15 01:34:26.000000 dali-rp2-0.6.7/tests/test_plugin_bitbank_supplemental_csv.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)    22733 2023-03-18 05:56:18.000000 dali-rp2-0.6.7/tests/test_plugin_ccxt.py
--rw-r--r--   0 marcoz     (501) staff       (20)     8194 2023-03-15 01:35:08.000000 dali-rp2-0.6.7/tests/test_plugin_coinbase.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5550 2023-03-15 01:34:26.000000 dali-rp2-0.6.7/tests/test_plugin_coinbase_pro.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1782 2023-03-15 01:34:26.000000 dali-rp2-0.6.7/tests/test_plugin_coincheck_supplemental.py
--rw-r--r--   0 marcoz     (501) staff       (20)     3805 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/tests/test_plugin_historic_crypto.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2646 2023-03-18 05:56:18.000000 dali-rp2-0.6.7/tests/test_plugin_kraken_csv_download.py
--rw-r--r--   0 marcoz     (501) staff       (20)     7483 2023-03-15 01:56:17.000000 dali-rp2-0.6.7/tests/test_plugin_ods_rp2_input.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     6300 2023-03-15 01:34:26.000000 dali-rp2-0.6.7/tests/test_plugin_pionex.py
--rw-r--r--   0 marcoz     (501) staff       (20)     3463 2023-03-12 00:51:26.000000 dali-rp2-0.6.7/tests/test_transaction_resolver.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.038009 dali-rp2-0.6.8/
+-rw-r--r--   0 marcoz     (501) staff       (20)    10454 2023-04-09 02:57:20.000000 dali-rp2-0.6.8/CHANGELOG.md
+-rw-r--r--   0 marcoz     (501) staff       (20)     3098 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/CONTRIBUTING.md
+-rw-r--r--   0 marcoz     (501) staff       (20)    11357 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/LICENSE
+-rw-r--r--   0 marcoz     (501) staff       (20)      214 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/MANIFEST.in
+-rw-r--r--   0 marcoz     (501) staff       (20)    22439 2023-04-09 03:08:33.038101 dali-rp2-0.6.8/PKG-INFO
+-rw-r--r--   0 marcoz     (501) staff       (20)    25113 2023-04-09 02:57:52.000000 dali-rp2-0.6.8/README.dev.md
+-rw-r--r--   0 marcoz     (501) staff       (20)    10422 2023-04-09 02:57:52.000000 dali-rp2-0.6.8/README.md
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.015135 dali-rp2-0.6.8/docs/
+-rw-r--r--   0 marcoz     (501) staff       (20)    43363 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/docs/configuration_file.md
+-rw-r--r--   0 marcoz     (501) staff       (20)     7936 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/docs/developer_faq.md
+-rw-r--r--   0 marcoz     (501) staff       (20)     9765 2023-03-15 01:40:20.000000 dali-rp2-0.6.8/docs/user_faq.md
+-rw-r--r--   0 marcoz     (501) staff       (20)      276 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/pyproject.toml
+-rw-r--r--   0 marcoz     (501) staff       (20)     2227 2023-04-09 03:08:33.039127 dali-rp2-0.6.8/setup.cfg
+-rw-r--r--   0 marcoz     (501) staff       (20)       92 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/setup.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.009644 dali-rp2-0.6.8/src/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.020733 dali-rp2-0.6.8/src/dali/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/__init__.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    32063 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/abstract_ccxt_input_plugin.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     2682 2023-03-15 01:25:21.000000 dali-rp2-0.6.8/src/dali/abstract_input_plugin.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    11488 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/abstract_pair_converter_plugin.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     9563 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/abstract_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1393 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/cache.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     8482 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/ccxt_pagination.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     7310 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/configuration.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3792 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/configuration_generator.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    18169 2023-04-09 02:57:52.000000 dali-rp2-0.6.8/src/dali/dali_main.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.021144 dali-rp2-0.6.8/src/dali/data/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/data/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    18654 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/data/template.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)     2221 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/historical_bar.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     6570 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/in_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5428 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/intra_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)      674 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/logger.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    10623 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/ods_generator.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     6323 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/out_transaction.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.021414 dali-rp2-0.6.8/src/dali/plugin/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/plugin/__init__.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.021884 dali-rp2-0.6.8/src/dali/plugin/country/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/plugin/country/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)      728 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/plugin/country/jp.py
+-rw-r--r--   0 marcoz     (501) staff       (20)      722 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/plugin/country/us.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.022048 dali-rp2-0.6.8/src/dali/plugin/input/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/plugin/input/__init__.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.024173 dali-rp2-0.6.8/src/dali/plugin/input/csv/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/__init__.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     7468 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/binance_com_supplemental.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     6750 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/bitbank_supplemental.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    13269 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/blockfi.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3660 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/coincheck_supplemental.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5980 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/ledger.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    10885 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/manual.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     7544 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/nexo.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     8410 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/pionex.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4988 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/trezor.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4636 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/trezor_old.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5016 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/plugin/input/csv/trezor_v2.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.024514 dali-rp2-0.6.8/src/dali/plugin/input/ods/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-15 01:07:08.000000 dali-rp2-0.6.8/src/dali/plugin/input/ods/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     6845 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/plugin/input/ods/rp2_input.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.025478 dali-rp2-0.6.8/src/dali/plugin/input/rest/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/plugin/input/rest/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    50065 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/plugin/input/rest/binance_com.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5042 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/plugin/input/rest/bitbank.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    47529 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/plugin/input/rest/coinbase.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    24564 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/src/dali/plugin/input/rest/coinbase_pro.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.026261 dali-rp2-0.6.8/src/dali/plugin/pair_converter/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/plugin/pair_converter/__init__.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    21072 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/plugin/pair_converter/ccxt.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     1101 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/plugin/pair_converter/ccxt_binance.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     1185 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/plugin/pair_converter/ccxt_kraken.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.026531 dali-rp2-0.6.8/src/dali/plugin/pair_converter/csv/
+-rwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/plugin/pair_converter/csv/__init__.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    15590 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/plugin/pair_converter/csv/kraken.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     2880 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/plugin/pair_converter/historic_crypto.py
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/src/dali/py.typed
+-rw-r--r--   0 marcoz     (501) staff       (20)    30848 2023-04-05 05:17:09.000000 dali-rp2-0.6.8/src/dali/transaction_resolver.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.034496 dali-rp2-0.6.8/src/dali_rp2.egg-info/
+-rw-r--r--   0 marcoz     (501) staff       (20)    22439 2023-04-09 03:08:32.000000 dali-rp2-0.6.8/src/dali_rp2.egg-info/PKG-INFO
+-rw-r--r--   0 marcoz     (501) staff       (20)     2728 2023-04-09 03:08:32.000000 dali-rp2-0.6.8/src/dali_rp2.egg-info/SOURCES.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)        1 2023-04-09 03:08:32.000000 dali-rp2-0.6.8/src/dali_rp2.egg-info/dependency_links.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)      106 2023-04-09 03:08:32.000000 dali-rp2-0.6.8/src/dali_rp2.egg-info/entry_points.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)      323 2023-04-09 03:08:32.000000 dali-rp2-0.6.8/src/dali_rp2.egg-info/requires.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)        5 2023-04-09 03:08:32.000000 dali-rp2-0.6.8/src/dali_rp2.egg-info/top_level.txt
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-09 03:08:33.037889 dali-rp2-0.6.8/tests/
+-rw-r--r--   0 marcoz     (501) staff       (20)     4772 2023-04-09 03:00:13.000000 dali-rp2-0.6.8/tests/ods_diff.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4479 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/tests/test_cache.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4868 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/tests/test_historical_bar.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4541 2023-04-09 03:00:13.000000 dali-rp2-0.6.8/tests/test_ods_output_diff.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    47912 2023-04-09 02:54:12.000000 dali-rp2-0.6.8/tests/test_plugin_binance_com.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     6070 2023-03-15 01:34:26.000000 dali-rp2-0.6.8/tests/test_plugin_binance_com_supplemental_csv.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     2696 2023-03-15 01:34:26.000000 dali-rp2-0.6.8/tests/test_plugin_bitbank_supplemental_csv.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    22733 2023-03-18 05:56:18.000000 dali-rp2-0.6.8/tests/test_plugin_ccxt.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     8194 2023-03-15 01:35:08.000000 dali-rp2-0.6.8/tests/test_plugin_coinbase.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5550 2023-03-15 01:34:26.000000 dali-rp2-0.6.8/tests/test_plugin_coinbase_pro.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1782 2023-03-15 01:34:26.000000 dali-rp2-0.6.8/tests/test_plugin_coincheck_supplemental.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3805 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/tests/test_plugin_historic_crypto.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     2646 2023-03-18 05:56:18.000000 dali-rp2-0.6.8/tests/test_plugin_kraken_csv_download.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     7436 2023-04-09 03:00:13.000000 dali-rp2-0.6.8/tests/test_plugin_ods_rp2_input.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     6300 2023-03-15 01:34:26.000000 dali-rp2-0.6.8/tests/test_plugin_pionex.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3463 2023-03-12 00:51:26.000000 dali-rp2-0.6.8/tests/test_transaction_resolver.py
```

### Comparing `dali-rp2-0.6.7/CHANGELOG.md` & `dali-rp2-0.6.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 # RP2 Change Log
 
+## 0.6.8
+* Coinbase data loader: added a new flavor of transfer transaction that was slightly different from the other ones (#137)
+
 ## 0.6.7
 * Coinbase data loader: fixed bug in advanced trade buy logic was not accounting for fee correctly
 * Coinbase data loader: added support for moving coins into staking pool (#132)
 
 ## 0.6.5
 * new Trezor CSV plugin supporting the latest format from Trezor Suite
```

### Comparing `dali-rp2-0.6.7/CONTRIBUTING.md` & `dali-rp2-0.6.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/LICENSE` & `dali-rp2-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/PKG-INFO` & `dali-rp2-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dali-rp2
-Version: 0.6.7
+Version: 0.6.8
 Summary: Data loader and input generator for RP2 (https://pypi.org/project/rp2/), the privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: DaLI removes the need to manually prepare RP2 input files. Just like RP2, DaLI is also free, open-source and it prioritizes user privacy.
 Home-page: https://github.com/eprbell/dali-rp2
 Author: eprbell
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eprbell/dali-rp2
 Project-URL: Developer Documentation, https://github.com/eprbell/dali-rp2/blob/main/README.dev.md
 Project-URL: User Documentation, https://github.com/eprbell/dali-rp2/blob/main/README.md
@@ -35,15 +35,15 @@
 
 <!--- Unless required by applicable law or agreed to in writing, software --->
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
-# DaLI for RP2 v0.6.7
+# DaLI for RP2 v0.6.8
 
 Privacy-focused, free, extensible data loader for RP2 (the crypto tax calculator)
 
 [![Static Analysis / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/windows_unit_tests.yml)
@@ -67,30 +67,30 @@
 * **[Reporting Bugs](#reporting-bugs)**
 * **[Contributing](#contributing)**
 * **[Developer Documentation](#developer-documentation)**
 * **[Frequently Asked Questions](#frequently-asked-questions)**
 * **[Change Log](#change-log)**
 
 ## Introduction
-[DaLI](https://github.com/eprbell/dali-rp2) (Data Loader Interface) is a data loader and input generator for [RP2](https://github.com/eprbell/rp2), the privacy-focused, free, non-commercial, open-source cryptocurrency tax calculator: DaLI removes the need to manually prepare RP2 input files. Just like RP2, DaLI is also free, non-commercial, open-source and it prioritizes user privacy by storing crypto transaction data on the user's computer and never sending it anywhere else.
+[DaLI](https://github.com/eprbell/dali-rp2) (Data Loader Interface) is a data loader and input generator for [RP2](https://github.com/eprbell/rp2), the privacy-focused, free, non-commercial, open-source, community-driven multi-country cryptocurrency tax calculator: DaLI removes the need to manually prepare RP2 input files. Just like RP2, DaLI is also free, non-commercial, open-source and it prioritizes user privacy by storing crypto transaction data on the user's computer and never sending it anywhere else.
 
 It performs the following operations:
 * it reads in crypto transaction information from multiples native sources: CSV files and/or REST-based services;
 * it analyzes, processes and merges this data;
-* it uses the processed data to generate an ODS input file for RP2 and its respective JSON configuration file.
+* it uses the processed data to generate an ODS input file for RP2 and its respective configuration file.
 
 DaLI has a programmable plugin architecture for [data loaders](https://github.com/eprbell/dali-rp2/blob/main/README.dev.md#data-loader-plugin-development) (both CSV and REST-based), [pair converters](https://github.com/eprbell/dali-rp2/blob/main/README.dev.md#pair-converter-plugin-development) and [countries](https://github.com/eprbell/dali-rp2/blob/main/README.dev.md#country-plugin-development). While some exchanges and wallets are already supported out-of-the-box, more are needed: help us make DaLI a robust open-source, community-driven crypto data loader by [contributing](https://github.com/eprbell/dali-rp2/tree/main/CONTRIBUTING.md#contributing-to-the-repository) plugins for exchanges and wallets! Check [open issues](https://github.com/eprbell/dali-rp2/issues) or open a new one.
 
 DaLI has [unit test](https://github.com/eprbell/dali-rp2/tree/main/tests/) coverage to reduce the risk of regression.
 
 Note that DaLI has RP2 as a dependency, so installing DaLI causes RP2 to be installed as well.
 
 **IMPORTANT DISCLAIMER**:
 * DaLI offers no guarantee of correctness (read the [license](https://github.com/eprbell/dali-rp2/tree/main/LICENSE)): always verify results with the help of a tax professional.
-* The author of DaLI and RP2 is not a tax professional, but has used RP2 personally for a few years.
+* The author of DaLI and RP2 is not a tax professional, but has used RP2 and DaLI personally for a few years.
 
 ## License
 DaLI is released under the terms of Apache License Version 2.0. For more information see [LICENSE](https://github.com/eprbell/dali-rp2/tree/main/LICENSE) or <http://www.apache.org/licenses/LICENSE-2.0>.
 
 ## Download
 The latest version of DaLI can be downloaded at: <https://pypi.org/project/dali-rp2/>
 
@@ -229,14 +229,17 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 # RP2 Change Log
 
+## 0.6.8
+* Coinbase data loader: added a new flavor of transfer transaction that was slightly different from the other ones (#137)
+
 ## 0.6.7
 * Coinbase data loader: fixed bug in advanced trade buy logic was not accounting for fee correctly
 * Coinbase data loader: added support for moving coins into staking pool (#132)
 
 ## 0.6.5
 * new Trezor CSV plugin supporting the latest format from Trezor Suite
```

### Comparing `dali-rp2-0.6.7/README.dev.md` & `dali-rp2-0.6.8/README.dev.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 <!--- Unless required by applicable law or agreed to in writing, software --->
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
-# DaLI for RP2 v0.6.7 Developer Guide
+# DaLI for RP2 v0.6.8 Developer Guide
 [![Static Analysis / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/windows_unit_tests.yml)
 [![CodeQL/Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/codeql-analysis.yml)
 
 ## Table of Contents
@@ -177,15 +177,15 @@
 * security check: `bandit -r src`
 * reformat code: `black src tests`
 * sort imports: `isort .`
 * run pre-commit tests without committing: `pre-commit run --all-files`
 
 Logs are stored in the `log` directory. To generate debug logs, prepend the command line with `LOG_LEVEL=DEBUG`, e.g.:
 ```
-LOG_LEVEL=DEBUG bin/dali_us -s -o output/ config/test_config.ini
+LOG_LEVEL=DEBUG dali_us -s -o output/ config/test_config.ini
 ```
 
 ### Unit Tests
 Unit tests are in the [tests](tests) directory. Please add unit tests for any new code.
 
 ## Creating a Release
 This section is for project maintainers.
```

### Comparing `dali-rp2-0.6.7/README.md` & `dali-rp2-0.6.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 <!--- Unless required by applicable law or agreed to in writing, software --->
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
-# DaLI for RP2 v0.6.7
+# DaLI for RP2 v0.6.8
 
 Privacy-focused, free, extensible data loader for RP2 (the crypto tax calculator)
 
 [![Static Analysis / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/windows_unit_tests.yml)
@@ -40,30 +40,30 @@
 * **[Reporting Bugs](#reporting-bugs)**
 * **[Contributing](#contributing)**
 * **[Developer Documentation](#developer-documentation)**
 * **[Frequently Asked Questions](#frequently-asked-questions)**
 * **[Change Log](#change-log)**
 
 ## Introduction
-[DaLI](https://github.com/eprbell/dali-rp2) (Data Loader Interface) is a data loader and input generator for [RP2](https://github.com/eprbell/rp2), the privacy-focused, free, non-commercial, open-source cryptocurrency tax calculator: DaLI removes the need to manually prepare RP2 input files. Just like RP2, DaLI is also free, non-commercial, open-source and it prioritizes user privacy by storing crypto transaction data on the user's computer and never sending it anywhere else.
+[DaLI](https://github.com/eprbell/dali-rp2) (Data Loader Interface) is a data loader and input generator for [RP2](https://github.com/eprbell/rp2), the privacy-focused, free, non-commercial, open-source, community-driven multi-country cryptocurrency tax calculator: DaLI removes the need to manually prepare RP2 input files. Just like RP2, DaLI is also free, non-commercial, open-source and it prioritizes user privacy by storing crypto transaction data on the user's computer and never sending it anywhere else.
 
 It performs the following operations:
 * it reads in crypto transaction information from multiples native sources: CSV files and/or REST-based services;
 * it analyzes, processes and merges this data;
-* it uses the processed data to generate an ODS input file for RP2 and its respective JSON configuration file.
+* it uses the processed data to generate an ODS input file for RP2 and its respective configuration file.
 
 DaLI has a programmable plugin architecture for [data loaders](https://github.com/eprbell/dali-rp2/blob/main/README.dev.md#data-loader-plugin-development) (both CSV and REST-based), [pair converters](https://github.com/eprbell/dali-rp2/blob/main/README.dev.md#pair-converter-plugin-development) and [countries](https://github.com/eprbell/dali-rp2/blob/main/README.dev.md#country-plugin-development). While some exchanges and wallets are already supported out-of-the-box, more are needed: help us make DaLI a robust open-source, community-driven crypto data loader by [contributing](https://github.com/eprbell/dali-rp2/tree/main/CONTRIBUTING.md#contributing-to-the-repository) plugins for exchanges and wallets! Check [open issues](https://github.com/eprbell/dali-rp2/issues) or open a new one.
 
 DaLI has [unit test](https://github.com/eprbell/dali-rp2/tree/main/tests/) coverage to reduce the risk of regression.
 
 Note that DaLI has RP2 as a dependency, so installing DaLI causes RP2 to be installed as well.
 
 **IMPORTANT DISCLAIMER**:
 * DaLI offers no guarantee of correctness (read the [license](https://github.com/eprbell/dali-rp2/tree/main/LICENSE)): always verify results with the help of a tax professional.
-* The author of DaLI and RP2 is not a tax professional, but has used RP2 personally for a few years.
+* The author of DaLI and RP2 is not a tax professional, but has used RP2 and DaLI personally for a few years.
 
 ## License
 DaLI is released under the terms of Apache License Version 2.0. For more information see [LICENSE](https://github.com/eprbell/dali-rp2/tree/main/LICENSE) or <http://www.apache.org/licenses/LICENSE-2.0>.
 
 ## Download
 The latest version of DaLI can be downloaded at: <https://pypi.org/project/dali-rp2/>
```

### Comparing `dali-rp2-0.6.7/docs/configuration_file.md` & `dali-rp2-0.6.8/docs/configuration_file.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
 **IMPORTANT NOTE**:
 * When setting up API key/secret, only use 参照 (reference) 権限 (authority) (DaLI does NOT need 取引 (transaction) or 出勤 (withdrawal) authority).
 * store your API key and secret safely and NEVER share it with anyone!
 
 Initialize this plugin section as follows:
 <pre>
-[dali.plugin.input.rest.binance_com <em>&lt;qualifiers&gt;</em>]
+[dali.plugin.input.rest.bitbank <em>&lt;qualifiers&gt;</em>]
 account_holder = <em>&lt;account_holder&gt;</em>
 api_key = <em>&lt;api_key&gt;</em>
 api_secret = <em>&lt;api_secret&gt;</em>
 username = <em>&lt;username&gt;</em>
 native_fiat = <em>&lt;native_fiat&gt;</em>
 thread_count = <em>&lt;thread_count&gt;</em>
 </pre>
@@ -174,15 +174,15 @@
 * `autoinvest_csv_file` can be retrieved by clicking [Wallet] -> [Earn] -> [History] -> [auto-invest] -> [export]
 * `betheth_csv_file` can be retrieved by clicking [Wallet] -> [Earn] -> [History] -> [ETH 2.0 Staking] -> [export]
 * You can currently only retrieve 6 months of data at one time, 5 times a month.
 
 ### Bitbank Supplemental Section (CSV)
 This plugin is CSV-based and parses CSV files generated by Bitbank. It only supports withdrawals, which are not covered by the REST API. Initialize it as follows:
 <pre>
-[dali.plugin.input.csv.binance_com <em>&lt;qualifiers&gt;</em>]
+[dali.plugin.input.csv.bitbank_supplemental <em>&lt;qualifiers&gt;</em>]
 account_holder = <em>&lt;account_holder&gt;</em>
 withdrawals_csv_file = <em>&lt;withdrawals_csv_file&gt;</em>
 withdrawal_code = <em>&lt;withdrawal_code&gt;</em>
 deposits_csv_file = <em>&lt;deposits_csv_file&gt;</em>
 deposits_code = <em>&lt;deposits_code&gt;</em>
 native_fiat = <em>&lt;native_fiat&gt;</em>
 </pre>
@@ -234,25 +234,25 @@
 Notes:
 
 * Locking or unlocking transactions are skipped. They are internal to Nexo.
 
 ### Pionex Section (CSV)
 This plugin is CSV-based and parses CSV files generated by Pionex. It currently supports trades, deposits and withdrawals. Initialize it as follows:
 <pre>
-[dali.plugin.input.csv.binance_com <em>&lt;qualifiers&gt;</em>]
+[dali.plugin.input.csv.pionex <em>&lt;qualifiers&gt;</em>]
 account_holder = <em>&lt;account_holder&gt;</em>
 trades_csv_file = <em>&lt;trades_csv_file&gt;</em>
 transfers_csv_file = <em>&lt;transfers_csv_file&gt;</em>
 native_fiat = <em>&lt;native_fiat&gt;</em>
 </pre>
 
 Notes:
-* The `trades_csv_file` and `transfers_csv_file` must be extracted from the .xlsx that is downloadable from the app. How to export transaction history is detailed [here](https://www.pionex.com/blog/how-to-export-pionex-transaction-history-statement%E3%80%90app-version%E3%80%91/).
-* The sheet from the exported .xlsx labeled "for-cointracker" needs to be saved seperately as a CSV. This is used as the `trades_csv_file`.
-* The sheet from the exported .xlsx labeled "depositwithdraw" needs to be saved seperately as a CSV. This is used as the `transfers_csv_file`.
+* The `trades_csv_file` and `transfers_csv_file` must be extracted from the .zip that is downloadable from the app. How to export transaction history is detailed [here](https://www.pionex.com/blog/how-to-export-pionex-transaction-history-statement%E3%80%90app-version%E3%80%91/).
+* The `for-cointracker.csv` file is used as input to the `trades_csv_file` parameter.
+* The `deposit-withdraw.csv` file is used as the input to the`transfers_csv_file` parameter.
 
 ### Trezor Section (CSV)
 This plugin is CSV-based and parses the original format of CSV files generated by Trezor Suite (try also the [Trezor V2 plugin](#trezor-v2-section-csv), if this doesn't work). Initialize it as follows:
 <pre>
 [dali.plugin.input.csv.trezor <em>&lt;qualifiers&gt;</em>]
 account_holder = <em>&lt;account_holder&gt;</em>
 account_nickname = <em>&lt;account_nickname&gt;</em>
@@ -317,14 +317,15 @@
 * `transaction_type`: AIRDROP, BUY, DONATE, GIFT, HARDFORK, INCOME, INTEREST, MINING, STAKING or WAGES;
 * `spot_price`: value of 1 unit of the given cryptocurrency at the time the transaction occurred; If the value is unavailable, to direct DaLI to read it from Internet historical data, write in `__unknown` and use the `-s` command line switch;
 * `crypto_in`: how much of the given cryptocurrency was acquired with the transaction (without fee);
 * `crypto_fee` (optional): transaction fee (if it was paid in crypto). This is mutually exclusive with `fiat_fee`;
 * `fiat_in_no_fee` (optional): fiat value of the transaction without fee;
 * `fiat_in_with_fee` (optional): fiat value of the transaction with fee;
 * `fiat_fee` (optional): transaction fee (if it was paid in fiat). This is mutually exclusive with `crypto_fee`;
+* `fiat_ticker` (optional): the 3 letter [ISO 4217 code](https://en.wikipedia.org/wiki/ISO_4217#List_of_ISO_4217_currency_codes) of the fiat currency being used;
 * `notes` (optional): user-provided description of the transaction.
 
 The `out_csv_file` contains transactions describing crypto being disposed of. Line 1 is considered a header line and it's ignored. Subsequent lines have the following format:
 * `unique_id` (optional): unique identifier for the transaction. It's useful to match partial intra transactions (see below) and it can be omitted in other cases;
 * `timestamp`: [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) format time at which the transaction occurred. Timestamps must always include: year, month, day, hour, minute, second and timezone (milliseconds are optional). E.g.: "2020-01-21 11:15:00+00:00";
 * `asset`: which cryptocurrency was transacted (e.g. BTC, ETH, etc.);
 * `exchange`: exchange or wallet on which the transaction occurred;
@@ -332,27 +333,29 @@
 * `transaction_type`: DONATE, GIFT or SELL;
 * `spot_price`: value of 1 unit of the given cryptocurrency at the time the transaction occurred; If the value is unavailable, to direct DaLI to read it from Internet historical data, write in `__unknown` and use the `-s` command line switch;
 * `crypto_out_no_fee`: how much of the given cryptocurrency was sold or sent with the transaction (excluding fee);
 * `crypto_fee`: crypto value of the transaction fee;
 * `crypto_out_with_fee` (optional): how much of the given cryptocurrency was sold or sent with the transaction (including fee);
 * `fiat_out_no_fee` (optional): fiat value of the transaction without fee;
 * `fiat_fee` (optional): fiat value of the transaction fee;
+* `fiat_ticker` (optional): the 3 letter [ISO 4217 code](https://en.wikipedia.org/wiki/ISO_4217#List_of_ISO_4217_currency_codes) of the fiat currency being used;
 * `notes` (optional): user-provided description of the transaction.
 
 The `intra_csv_file` contains transactions describing crypto being moved across accounts controlled by the same user (or people filing together). Line 1 is considered a header line and it's ignored. Subsequent lines have the following format:
 * `unique_id`: unique identifier for the transaction. It's useful to match partial intra transactions (see below) and it can be omitted in other cases;
 * `timestamp`: [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) format time at which the transaction occurred. Timestamps must always include: year, month, day, hour, minute, second and timezone (milliseconds are optional). E.g.: "2020-01-21 11:15:00+00:00";
 * `asset`: which cryptocurrency was transacted (e.g. BTC, ETH, etc.);
 * `from_exchange` (optional): exchange or wallet from which the transfer of cryptocurrency occurred;
 * `from_holder` (optional): owner of the exchange account or wallet from which the transfer of cryptocurrency occurred;
 * `to_exchange` (optional): exchange or wallet to which the transfer of cryptocurrency occurred;
 * `to_holder` (optional): owner of the exchange account or wallet to which the transfer of cryptocurrency occurred;
 * `spot_price` (optional): value of 1 unit of the given cryptocurrency at the time the transaction occurred; If the value is unavailable, to direct DaLI to read it from Internet historical data, write in `__unknown` and use the `-s` command line switch;
 * `crypto_sent` (optional): how much of the given cryptocurrency was sent with the transaction;
 * `crypto_received` (optional): how much of the given cryptocurrency was received with the transaction;
+* `fiat_ticker` (optional): the 3 letter [ISO 4217 code](https://en.wikipedia.org/wiki/ISO_4217#List_of_ISO_4217_currency_codes) of the fiat currency being used;
 * `notes` (optional): user-provided description of the transaction.
 
 Note that empty (separator) lines are allowed in all three CSV files to increase readability.
 
 #### Partial Transactions and Transaction Resolution
 The manual CSV plugin is typically used for two purposes:
 * add complete in/out/intra transactions for exchanges or wallets that are not yet supported by DaLI;
@@ -590,15 +593,15 @@
 crypto_fee = 8
 crypto_out_with_fee = 9
 fiat_out_no_fee = 10
 fiat_fee = 11
 unique_id = 12
 notes = 13
 
-[in_header]
+[intra_header]
 timestamp = 0
 asset = 1
 from_exchange = 2
 from_holder = 3
 to_exchange = 4
 to_holder = 5
 spot_price = 6
```

### Comparing `dali-rp2-0.6.7/docs/developer_faq.md` & `dali-rp2-0.6.8/docs/developer_faq.md`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/docs/user_faq.md` & `dali-rp2-0.6.8/docs/user_faq.md`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/setup.cfg` & `dali-rp2-0.6.8/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dali-rp2
-version = 0.6.7
+version = 0.6.8
 description = Data loader and input generator for RP2 (https://pypi.org/project/rp2/), the privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: DaLI removes the need to manually prepare RP2 input files. Just like RP2, DaLI is also free, open-source and it prioritizes user privacy.
 long_description_content_type = text/markdown
 long_description = file: README.md, CHANGELOG.md
 keywords = accounting, altcoin, bitcoin, BTC, capital gains, cost basis, crypto, cryptocurrency, data loader, DeFi, ETH, ethereum, exchange, finance, form 8949, NFT, privacy, wallet, tax
 license = Apache License 2.0
 author = eprbell
 url = https://github.com/eprbell/dali-rp2
```

### Comparing `dali-rp2-0.6.7/src/dali/abstract_ccxt_input_plugin.py` & `dali-rp2-0.6.8/src/dali/abstract_ccxt_input_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,25 +84,23 @@
 class ProcessOperationResult(NamedTuple):
     in_transactions: List[InTransaction]
     out_transactions: List[OutTransaction]
     intra_transactions: List[IntraTransaction]
 
 
 class AbstractCcxtInputPlugin(AbstractInputPlugin):
-
     __DEFAULT_THREAD_COUNT: int = 1
 
     def __init__(
         self,
         account_holder: str,
         exchange_start_time: datetime,
         native_fiat: Optional[str],
         thread_count: Optional[int],
     ) -> None:
-
         super().__init__(account_holder, native_fiat)
         self.__logger: logging.Logger = create_logger(f"{self.exchange_name()}/{self.account_holder}")
         self.__cache_key: str = f"{str(self.exchange_name()).lower()}-{account_holder}"
         self.__client: Exchange = self._initialize_client()
         self.__thread_count = thread_count if thread_count else self.__DEFAULT_THREAD_COUNT
         self.__markets: List[str] = []
         self.__start_time: datetime = exchange_start_time
@@ -127,15 +125,14 @@
         raise NotImplementedError("Abstract method")
 
     # Some exchanges require you to loop through all markets for trades
     def _get_process_trades_pagination_detail_set(self) -> Optional[AbstractPaginationDetailSet]:
         raise NotImplementedError("Abstract method")
 
     def _get_markets(self) -> List[str]:
-
         if self.__markets:
             return self.__markets
 
         ccxt_markets: Any = self._client.fetch_markets()
         market_list: List[str] = []
         for market in ccxt_markets:
             self.__logger.debug("Market: %s", json.dumps(market))
@@ -297,15 +294,14 @@
         raise NotImplementedError("Abstract method")
 
     def _process_trades(
         self,
         in_transactions: List[InTransaction],
         out_transactions: List[OutTransaction],
     ) -> None:
-
         processing_result_list: List[Optional[ProcessOperationResult]] = []
         pagination_detail_set: Optional[AbstractPaginationDetailSet] = self._get_process_trades_pagination_detail_set()
         # Strip optionality
         if not pagination_detail_set:
             raise RP2RuntimeError("No pagination details for trades.")
 
         has_pagination_detail_set: AbstractPaginationDetailSet = pagination_detail_set
@@ -366,15 +362,14 @@
             # End of pagination details
             pass
 
     def _process_withdrawals(
         self,
         intra_transactions: List[IntraTransaction],
     ) -> None:
-
         processing_result_list: List[Optional[ProcessOperationResult]] = []
         pagination_detail_set: Optional[AbstractPaginationDetailSet] = self._get_process_withdrawals_pagination_detail_set()
         # Strip optionality
         if not pagination_detail_set:
             raise RP2RuntimeError("No pagination details for withdrawals.")
 
         has_pagination_detail_set: AbstractPaginationDetailSet = pagination_detail_set
@@ -443,15 +438,14 @@
             pass
 
     def __safe_api_call(
         self,
         function: Callable[..., Iterable[Dict[str, Union[str, float]]]],
         params: Dict[str, Any],
     ) -> Iterable[Dict[str, Union[str, float]]]:
-
         results: Iterable[Dict[str, Union[str, float]]] = {}
         request_count: int = 0
 
         # Most exceptions are caused by request limits of the underlying APIs
         while request_count < 9:
             try:
                 if "code" in params:
```

### Comparing `dali-rp2-0.6.7/src/dali/abstract_input_plugin.py` & `dali-rp2-0.6.8/src/dali/abstract_input_plugin.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/abstract_pair_converter_plugin.py` & `dali-rp2-0.6.8/src/dali/abstract_pair_converter_plugin.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/abstract_transaction.py` & `dali-rp2-0.6.8/src/dali/abstract_transaction.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/cache.py` & `dali-rp2-0.6.8/src/dali/cache.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/ccxt_pagination.py` & `dali-rp2-0.6.8/src/dali/ccxt_pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         start_time_key: str,
         end_time_key: str,
         window: int,
         limit: Optional[int] = None,
         markets: Optional[List[str]] = None,
         params: Optional[Dict[str, Union[int, str, None]]] = None,
     ) -> None:
-
         super().__init__(exchange_start_time, limit, markets, params, window)
         self.__start_time_key: str = start_time_key
         self.__end_time_key: str = end_time_key
 
     def _get_window(self) -> int:
         if self.__window:
             return self.__window
@@ -158,24 +157,22 @@
         self,
         exchange_start_time: int,
         limit: Optional[int] = None,
         markets: Optional[List[str]] = None,
         params: Optional[Dict[str, Union[int, str, None]]] = None,
         window: Optional[int] = None,
     ) -> None:
-
         super().__init__(limit, markets, params)
         self.__end_of_data = False
         self.__since: int = exchange_start_time
         self.__exchange_start_time: int = exchange_start_time
         self.__now: int = int(datetime.now().timestamp()) * _MS_IN_SECOND
         self.__window: Optional[int] = window
 
     def update_fetched_elements(self, current_results: Any) -> None:
-
         end_of_market: bool = False
 
         # Update Since if needed otherwise end_of_market
         if len(current_results) == self._get_limit():
             # All times are inclusive
             self.__since = current_results[len(current_results) - 1][_TIMESTAMP] + 1
         elif self.__window:
@@ -222,21 +219,19 @@
         start_time_key: str,
         end_time_key: str,
         window: int,
         limit: Optional[int] = None,
         markets: Optional[List[str]] = None,
         params: Optional[Dict[str, Union[int, str, None]]] = None,
     ) -> None:
-
         super().__init__(exchange_start_time, limit, markets, params, window)
         self.__start_time_key: str = start_time_key
         self.__end_time_key: str = end_time_key
 
     def __next__(self) -> PaginationDetails:
-
         while not self._is_end_of_data():
             base_details: PaginationDetails = super().__next__()
             if base_details.params:
                 base_details.params[self.__start_time_key] = base_details.since
                 base_details.params[self.__end_time_key] = self._get_end_of_window()
             else:
                 base_details._replace(params={self.__start_time_key: base_details.since, self.__end_time_key: self._get_end_of_window()})
```

### Comparing `dali-rp2-0.6.7/src/dali/configuration.py` & `dali-rp2-0.6.8/src/dali/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from enum import Enum
 from typing import Dict, Optional, Set, Union
+
 from rp2.rp2_error import RP2ValueError
 
 
 # Configuration file keywords
 class Keyword(Enum):
     AIRDROP: str = "airdrop"
     ASSET: str = "asset"
```

### Comparing `dali-rp2-0.6.7/src/dali/configuration_generator.py` & `dali-rp2-0.6.8/src/dali/configuration_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 def generate_configuration_file(
     output_dir_path: str,
     output_file_prefix: str,
     output_file_name: str,
     transactions: List[AbstractTransaction],
     global_configuration: Dict[str, Any],
 ) -> Any:
-
     if not isinstance(output_dir_path, str):
         raise RP2RuntimeError(f"Internal error: parameter output_dir_path is not of type string: {repr(output_dir_path)}")
     if not isinstance(output_file_prefix, str):
         raise RP2RuntimeError(f"Internal error: parameter output_file_prefix is not of type string: {repr(output_file_prefix)}")
     if not isinstance(output_file_name, str):
         raise RP2RuntimeError(f"Internal error: parameter output_file_name is not of type string: {repr(output_file_name)}")
     if not isinstance(transactions, List):
```

### Comparing `dali-rp2-0.6.7/src/dali/dali_main.py` & `dali-rp2-0.6.8/src/dali/dali_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     PairConverterPlugin as CcxtPairConverterPlugin,
 )
 from dali.plugin.pair_converter.historic_crypto import (
     PairConverterPlugin as HistoricCryptoPairConverterPlugin,
 )
 from dali.transaction_resolver import resolve_transactions
 
-_VERSION: str = "0.6.7"
+_VERSION: str = "0.6.8"
 
 
 class _InputPluginHelperArgs(NamedTuple):
     input_plugin: AbstractInputPlugin
     package_name: str
     country: AbstractCountry
     use_cache: bool
@@ -67,15 +67,14 @@
     if "RP2_ENABLE_PROFILER" in os.environ:
         cProfile.runctx("_dali_main_internal(country)", globals(), locals())
     else:
         _dali_main_internal(country)
 
 
 def _dali_main_internal(country: AbstractCountry) -> None:
-
     args: Namespace
     parser: ArgumentParser
 
     dali_configuration: Dict[str, Any] = DEFAULT_CONFIGURATION
 
     parser = _setup_argument_parser()
     args = parser.parse_args()
```

### Comparing `dali-rp2-0.6.7/src/dali/data/template.ods` & `dali-rp2-0.6.8/src/dali/data/template.ods`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/historical_bar.py` & `dali-rp2-0.6.8/src/dali/historical_bar.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/in_transaction.py` & `dali-rp2-0.6.8/src/dali/in_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
                 f"Internal error: both 'crypto_fee' and 'fiat_fee' are defined, instead of only one: their values are {crypto_fee} and {fiat_fee} respectively"
             )
 
         self.__constructor_parameter_dictionary: Dict[str, Union[str, bool, Optional[str], Optional[bool]]] = {}
         self.__is_unresolved: bool = self._setup_constructor_parameter_dictionary(self.__constructor_parameter_dictionary)
 
     def to_string(self, indent: int = 0, repr_format: bool = True, extra_data: Optional[List[str]] = None) -> str:
-
         class_specific_data: List[str] = []
         stringify: Callable[[object], str] = repr
         if not repr_format:
             stringify = str
         class_specific_data = [
             f"{Keyword.EXCHANGE.value}={stringify(self.exchange)}",
             f"{Keyword.HOLDER.value}={stringify(self.holder)}",
```

### Comparing `dali-rp2-0.6.7/src/dali/intra_transaction.py` & `dali-rp2-0.6.8/src/dali/intra_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
         self.__crypto_received: str = self._validate_numeric_field(
             Keyword.CRYPTO_RECEIVED.value, crypto_received, raw_data, disallow_empty=True, disallow_unknown=False
         )
         self.__constructor_parameter_dictionary: Dict[str, Union[str, bool, Optional[str], Optional[bool]]] = {}
         self.__is_unresolved: bool = self._setup_constructor_parameter_dictionary(self.__constructor_parameter_dictionary)
 
     def to_string(self, indent: int = 0, repr_format: bool = True, extra_data: Optional[List[str]] = None) -> str:
-
         class_specific_data: List[str] = []
         stringify: Callable[[object], str] = repr
         if not repr_format:
             stringify = str
         class_specific_data = [
             f"{Keyword.FROM_EXCHANGE.value}={stringify(self.from_exchange)}",
             f"{Keyword.FROM_HOLDER.value}={stringify(self.from_holder)}",
```

### Comparing `dali-rp2-0.6.7/src/dali/logger.py` & `dali-rp2-0.6.8/src/dali/logger.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/ods_generator.py` & `dali-rp2-0.6.8/src/dali/ods_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 def generate_input_file(
     output_dir_path: str,
     output_file_prefix: str,
     output_file_name: str,
     transactions: List[AbstractTransaction],
     global_configuration: Dict[str, Any],
 ) -> Any:
-
     native_fiat: str = global_configuration[Keyword.NATIVE_FIAT.value]
 
     _table_to_header: Dict[str, Dict[str, str]] = {
         _IN: {
             Keyword.UNIQUE_ID.value: "Unique ID",
             Keyword.TIMESTAMP.value: "Timestamp",
             Keyword.ASSET.value: "Asset",
@@ -250,15 +249,14 @@
     sheet: Any,
     row_index: int,
     column_index: int,
     value: Any,
     visual_style: str = "transparent",
     data_style: str = "default",
 ) -> None:
-
     if value is None:
         return
 
     is_formula: bool = False
     if isinstance(value, str) and value and value[0] == "=":
         # If the value starts with '=' it is assumed to be a formula
         is_formula = True
```

### Comparing `dali-rp2-0.6.7/src/dali/out_transaction.py` & `dali-rp2-0.6.8/src/dali/out_transaction.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/plugin/country/jp.py` & `dali-rp2-0.6.8/src/dali/plugin/country/jp.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/plugin/country/us.py` & `dali-rp2-0.6.8/src/dali/plugin/country/us.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/binance_com_supplemental.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/binance_com_supplemental.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from dali.abstract_transaction import AbstractTransaction
 from dali.configuration import Keyword
 from dali.in_transaction import InTransaction
 from dali.out_transaction import OutTransaction
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __BINANCE_COM: str = "Binance.com"
     __BINANCE_COM_SUPPLEMENTAL_CSV: str = "Binance.com_Supplemental_CSV"
 
     __TIMESTAMP_INDEX: int = 0
     __AUTO_BASE_SYMBOL: int = 1
     __AUTO_QUOTE_AMOUNT_SYMBOL: int = 2
     __AUTO_TRADING_FEE_SYMBOL: int = 3
@@ -51,15 +50,14 @@
     def __init__(
         self,
         account_holder: str,
         autoinvest_csv_file: Optional[str] = None,
         betheth_csv_file: Optional[str] = None,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__autoinvest_csv_file: Optional[str] = autoinvest_csv_file
         self.__betheth_csv_file: Optional[str] = betheth_csv_file
         self.__logger: logging.Logger = create_logger(f"{self.__BINANCE_COM_SUPPLEMENTAL_CSV}/{self.account_holder}")
 
     def load(self, country: AbstractCountry) -> List[AbstractTransaction]:
         result: List[AbstractTransaction] = []
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/bitbank_supplemental.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/bitbank_supplemental.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,26 @@
 import logging
 from csv import reader
 from datetime import datetime
 from datetime import timezone as DatetimeTimezone
 from typing import List, Optional
 
 from pytz import timezone as PytzTimezone
-
 from rp2.abstract_country import AbstractCountry
 from rp2.logger import create_logger
 from rp2.rp2_error import RP2ValueError
 
 from dali.abstract_input_plugin import AbstractInputPlugin
 from dali.abstract_transaction import AbstractTransaction
 from dali.configuration import Keyword
 from dali.in_transaction import InTransaction
 from dali.intra_transaction import IntraTransaction
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __BITBANK: str = "Bitbank.cc"
     __BITBANK_PLUGIN: str = "Bitbank_Supplemental_CSV"
 
     __TIMESTAMP_INDEX: int = 0
     __SENT_AMOUNT: int = 1
     __DEPOSIT_TOTAL: int = 1
     __TRANSACTION_FEE: int = 2
@@ -56,15 +54,14 @@
         account_holder: str,
         deposits_csv_file: Optional[str] = None,
         deposits_code: Optional[str] = None,
         withdrawals_csv_file: Optional[str] = None,
         withdrawals_code: Optional[str] = None,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__deposits_csv_file: Optional[str] = deposits_csv_file
         self.__deposits_code: Optional[str] = deposits_code
         self.__withdrawals_csv_file: Optional[str] = withdrawals_csv_file
         # Code of the asset being withdrawn since it is NOT included in the CSV file.
         self.__withdrawals_code: Optional[str] = withdrawals_code
         self.__logger: logging.Logger = create_logger(f"{self.__BITBANK_PLUGIN}/{self.account_holder}")
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/blockfi.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/blockfi.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 _TYPE: str = "Type"
 _WITHDRAWAL: str = "Withdrawal"
 _BIA_WITHDRAWAL: str = "BIA Withdraw"
 _WITHDRAWAL_FEE: str = "Withdrawal Fee"
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __BLOCKFI: str = "BlockFi"
 
     __CURRENCY_INDEX: int = 0
     __AMOUNT_INDEX: int = 1
     __TYPE_INDEX: int = 2
     __TIMESTAMP_INDEX: int = 3
     #    __SPOT_PRICE_INDEX: int = 4 # It used to be present in the CSV, but sometime in 2021 BlockFi removed this field.
@@ -65,15 +64,14 @@
     def __init__(
         self,
         account_holder: str,
         transaction_csv_file: str,
         trade_csv_file: Optional[str] = None,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__transaction_csv_file: str = transaction_csv_file
         self.__trade_csv_file: Optional[str] = trade_csv_file
         self.__logger: logging.Logger = create_logger(f"{self.__BLOCKFI}/{self.account_holder}")
 
     def load(self, country: AbstractCountry) -> List[AbstractTransaction]:
         result: List[AbstractTransaction] = []
@@ -228,15 +226,15 @@
         with open(file_path, encoding="utf-8") as csv_file:
             lines = reader(csv_file)
             # skip csv header
             header = next(lines)
             self.__logger.debug("Header: %s", header)
 
             column_index: Dict[str, int] = {}
-            for (index, name) in enumerate(header):
+            for index, name in enumerate(header):
                 column_index[name] = index
 
             for line in lines:
                 raw_data: str = self.__DELIMITER.join(line)
                 self.__logger.debug("Transaction: %s", raw_data)
 
                 transaction_type: str = line[column_index[_TYPE]]
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/coincheck_supplemental.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/coincheck_supplemental.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from dali.abstract_input_plugin import AbstractInputPlugin
 from dali.abstract_transaction import AbstractTransaction
 from dali.configuration import Keyword
 from dali.in_transaction import InTransaction
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __COINCHECK: str = "Coincheck"
     __COINCHECK_SUPPLEMENTAL_PLUGIN: str = "Coincheck_Supplemental_CSV"
 
     __ID: int = 0
     __AMOUNT_PURCHASED: int = 1
     __TOTAL_PRICE: int = 2
     __CRYPTO_ASSET: int = 3
@@ -46,15 +45,14 @@
 
     def __init__(
         self,
         account_holder: str,
         buys_csv_file: str,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__buys_csv_file: str = buys_csv_file
         self.__logger: logging.Logger = create_logger(f"{self.__COINCHECK_SUPPLEMENTAL_PLUGIN}/{self.account_holder}")
 
     def load(self, country: AbstractCountry) -> List[AbstractTransaction]:
         return self.parse_buys_file(self.__buys_csv_file)
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/ledger.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/ledger.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,31 +34,30 @@
 #       service provider, Kaiko
 
 
 import logging
 from csv import reader
 from datetime import datetime
 from typing import List, Optional
-import dateutil
 
+import dateutil
 from rp2.abstract_country import AbstractCountry
 from rp2.logger import create_logger
 from rp2.rp2_decimal import ZERO, RP2Decimal
 
 from dali.abstract_input_plugin import AbstractInputPlugin
 from dali.abstract_transaction import AbstractTransaction
 from dali.configuration import Keyword
 from dali.intra_transaction import IntraTransaction
 
 _SENT: str = "OUT"
 _RECV: str = "IN"
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __LEDGER: str = "Ledger"
 
     __TIMESTAMP_INDEX: int = 0
     __CURRENCY_INDEX: int = 1
     __OPERATION_TYPE_INDEX: int = 2
     __QUANTITY_INDEX: int = 3
     __FEE_INDEX: int = 4
@@ -73,15 +72,14 @@
     def __init__(
         self,
         account_holder: str,
         account_nickname: str,
         csv_file: str,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__account_nickname: str = account_nickname
         self.__csv_file: str = csv_file
         self.__logger: logging.Logger = create_logger(f"{self.__LEDGER}/{self.__account_nickname}/{self.account_holder}")
 
     def load(self, country: AbstractCountry) -> List[AbstractTransaction]:
         result: List[AbstractTransaction] = []
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/manual.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/manual.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from dali.configuration import Keyword
 from dali.in_transaction import InTransaction
 from dali.intra_transaction import IntraTransaction
 from dali.out_transaction import OutTransaction
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __MANUAL: str = "Manual"
 
     __IN_UNIQUE_ID_INDEX: int = 0
     __IN_TIMESTAMP_INDEX: int = 1
     __IN_ASSET_INDEX: int = 2
     __IN_EXCHANGE_INDEX: int = 3
     __IN_HOLDER_INDEX: int = 4
@@ -82,15 +81,14 @@
     def __init__(
         self,
         in_csv_file: str,
         out_csv_file: str,
         intra_csv_file: str,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder="", native_fiat=native_fiat)
 
         self.__in_csv_file: str = in_csv_file
         self.__out_csv_file: str = out_csv_file
         self.__intra_csv_file: str = intra_csv_file
 
         self.__logger: logging.Logger = create_logger(self.__MANUAL)
@@ -101,15 +99,14 @@
         self._load_in_file(result)
         self._load_out_file(result)
         self._load_intra_file(result)
 
         return result
 
     def _load_in_file(self, transactions: List[AbstractTransaction]) -> None:
-
         if not self.__in_csv_file:
             return
 
         with open(self.__in_csv_file, encoding="utf-8") as csv_file:
             lines = reader(csv_file)
             header_found: bool = False
             for line in lines:
@@ -149,15 +146,14 @@
                         fiat_in_with_fee=line[self.__IN_FIAT_IN_WITH_FEE_INDEX],
                         fiat_fee=line[self.__IN_FIAT_FEE_INDEX],
                         notes=line[self.__IN_NOTES_INDEX],
                     )
                 )
 
     def _load_out_file(self, transactions: List[AbstractTransaction]) -> None:
-
         if not self.__out_csv_file:
             return
 
         with open(self.__out_csv_file, encoding="utf-8") as csv_file:
             lines = reader(csv_file)
             header_found: bool = False
             for line in lines:
@@ -198,15 +194,14 @@
                         fiat_out_no_fee=line[self.__OUT_FIAT_OUT_NO_FEE_INDEX],
                         fiat_fee=line[self.__OUT_FIAT_FEE_INDEX],
                         notes=line[self.__OUT_NOTES_INDEX],
                     )
                 )
 
     def _load_intra_file(self, transactions: List[AbstractTransaction]) -> None:
-
         if not self.__intra_csv_file:
             return
 
         with open(self.__intra_csv_file, encoding="utf-8") as csv_file:
             lines = reader(csv_file)
             header_found: bool = False
             for line in lines:
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/nexo.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/nexo.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
     def __init__(
         self,
         account_holder: str,
         transaction_csv_file: str,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__transaction_csv_file: str = transaction_csv_file
         self.__logger: logging.Logger = create_logger(f"{self.__NEXO}/{self.account_holder}")
 
     def load(self, country: AbstractCountry) -> List[AbstractTransaction]:
         result: List[AbstractTransaction] = []
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/pionex.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/pionex.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 from dali.configuration import Keyword
 from dali.in_transaction import InTransaction
 from dali.intra_transaction import IntraTransaction
 from dali.out_transaction import OutTransaction
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __PIONEX: str = "Pionex"
     __PIONEX_PLUGIN: str = "Pionex_CSV"
 
     __TIMESTAMP_INDEX: int = 0
     __RECEIVED_AMOUNT: int = 1
     __TRANSACTION_TYPE: int = 1
     __ASSET_RECEIVED: int = 2
@@ -61,15 +60,14 @@
     def __init__(
         self,
         account_holder: str,
         trades_csv_file: Optional[str] = None,
         transfers_csv_file: Optional[str] = None,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__trades_csv_file: Optional[str] = trades_csv_file
         self.__transfers_csv_file: Optional[str] = transfers_csv_file
         self.__logger: logging.Logger = create_logger(f"{self.__PIONEX_PLUGIN}/{self.account_holder}")
 
     def load(self, country: AbstractCountry) -> List[AbstractTransaction]:
         result: List[AbstractTransaction] = []
@@ -149,15 +147,14 @@
 
         with open(file_path, encoding="utf-8") as csv_file:
             lines = reader(csv_file)
 
             header = next(lines)
             self.__logger.debug("Header: %s", header)
             for line in lines:
-
                 raw_data: str = self.__DELIMITER.join(line)
                 self.__logger.debug("Transaction: %s", raw_data)
 
                 asset: str = (
                     line[self.__ASSET_TRANSFERED][: -len(line[self.__CHAIN_USED])]
                     if (line[self.__ASSET_TRANSFERED].endswith(line[self.__CHAIN_USED]))
                     else (line[self.__ASSET_TRANSFERED])
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/trezor.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/trezor.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,28 @@
 
 import logging
 from csv import reader
 from datetime import datetime
 from typing import List, Optional
 
 import pytz
-
 from rp2.abstract_country import AbstractCountry
 from rp2.logger import create_logger
 from rp2.rp2_decimal import ZERO, RP2Decimal
 
 from dali.abstract_input_plugin import AbstractInputPlugin
 from dali.abstract_transaction import AbstractTransaction
 from dali.configuration import Keyword
 from dali.intra_transaction import IntraTransaction
 
 _SENT: str = "SENT"
 _RECV: str = "RECV"
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __TREZOR: str = "Trezor"
 
     __TIMESTAMP_INDEX: int = 0
     __TYPE_INDEX: int = 1
     __TRANSACTION_ID_INDEX: int = 2
     __FEE_INDEX: int = 4
     __TOTAL_INDEX: int = 5
@@ -52,15 +50,14 @@
         account_holder: str,
         account_nickname: str,
         currency: str,
         timezone: str,
         csv_file: str,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__account_nickname: str = account_nickname
         self.__currency: str = currency
         self.__timezone = pytz.timezone(timezone)
         self.__csv_file: str = csv_file
 
         self.__logger: logging.Logger = create_logger(f"{self.__TREZOR}/{currency}/{self.__account_nickname}/{self.account_holder}")
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/trezor_old.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/trezor_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,28 @@
 
 import logging
 from csv import reader
 from datetime import datetime
 from typing import List, Optional
 
 import pytz
-
 from rp2.abstract_country import AbstractCountry
 from rp2.logger import create_logger
 from rp2.rp2_decimal import RP2Decimal
 
 from dali.abstract_input_plugin import AbstractInputPlugin
 from dali.abstract_transaction import AbstractTransaction
 from dali.configuration import Keyword
 from dali.intra_transaction import IntraTransaction
 
 _OUT: str = "OUT"
 _IN: str = "IN"
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __TREZOR_OLD: str = "Trezor Old"
 
     __DATE_INDEX: int = 0
     __TIME_INDEX: int = 1
     __TRANSACTION_ID_INDEX: int = 2
     __TYPE_INDEX: int = 4
     __TOTAL_INDEX: int = 6
@@ -52,15 +50,14 @@
         account_holder: str,
         account_nickname: str,
         currency: str,
         timezone: str,
         csv_file: str,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__account_nickname: str = account_nickname
         self.__currency: str = currency
         self.__timezone = pytz.timezone(timezone)
         self.__csv_file: str = csv_file
 
         self.__logger: logging.Logger = create_logger(f"{self.__TREZOR_OLD}/{currency}/{self.__account_nickname}/{self.account_holder}")
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/csv/trezor_v2.py` & `dali-rp2-0.6.8/src/dali/plugin/input/csv/trezor_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,35 +12,34 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # This plugin parses a newer (circa 2023) version of the CSV format generated by Trezor Suite.
 # CSV Format: timestamp, date, time, type, transaction_id, fee, fee unit, address, label, amount, amount unit, fiat, other
 
 import logging
+import re
 from csv import reader
 from datetime import datetime
-import re
-from dateutil.parser import parse
 from typing import List, Optional
 
+from dateutil.parser import parse
 from rp2.abstract_country import AbstractCountry
 from rp2.logger import create_logger
 from rp2.rp2_decimal import ZERO, RP2Decimal
 
 from dali.abstract_input_plugin import AbstractInputPlugin
 from dali.abstract_transaction import AbstractTransaction
 from dali.configuration import Keyword
 from dali.intra_transaction import IntraTransaction
 
 _SENT: str = "SENT"
 _RECV: str = "RECV"
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __TREZOR_V2: str = "Trezor V2"
 
     __DATE_INDEX: int = 1
     __TIME_INDEX: int = 2
     __TYPE_INDEX: int = 3
     __TRANSACTION_ID_INDEX: int = 4
     __FEE_INDEX: int = 5
@@ -52,15 +51,14 @@
         self,
         account_holder: str,
         account_nickname: str,
         currency: str,
         csv_file: str,
         native_fiat: Optional[str] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__account_nickname: str = account_nickname
         self.__currency: str = currency
         self.__csv_file: str = csv_file
 
         self.__logger: logging.Logger = create_logger(f"{self.__TREZOR_V2}/{currency}/{self.__account_nickname}/{self.account_holder}")
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/ods/rp2_input.py` & `dali-rp2-0.6.8/src/dali/plugin/input/ods/rp2_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from typing import List, Optional, cast
 
 from rp2.abstract_country import AbstractCountry
-from rp2.configuration import Configuration, MAX_DATE, MIN_DATE
+from rp2.configuration import MAX_DATE, MIN_DATE, Configuration
 from rp2.in_transaction import InTransaction as RP2InTransaction
 from rp2.input_data import InputData
 from rp2.intra_transaction import IntraTransaction as RP2IntraTransaction
 from rp2.logger import create_logger
-from rp2.ods_parser import parse_ods, open_ods
+from rp2.ods_parser import open_ods, parse_ods
 from rp2.out_transaction import OutTransaction as RP2OutTransaction
 
 from dali.abstract_input_plugin import AbstractInputPlugin
 from dali.abstract_transaction import AbstractTransaction
 from dali.in_transaction import InTransaction
 from dali.intra_transaction import IntraTransaction
 from dali.out_transaction import OutTransaction
@@ -57,40 +57,38 @@
 
         input_file_handle: object = open_ods(configuration=rp2_configuration, input_file_path=self.__input_file)
         assets = sorted(list(rp2_configuration.assets))
 
         for asset in assets:
             self.__logger.info("Processing %s", asset)
 
-            input_data: InputData = parse_ods(
-                configuration=rp2_configuration,
-                asset=asset,
-                input_file_handle=input_file_handle
-            )
+            input_data: InputData = parse_ods(configuration=rp2_configuration, asset=asset, input_file_handle=input_file_handle)
             self.__logger.debug("InputData object: %s", input_data)
             for asset_entry in input_data.unfiltered_in_transaction_set:
                 in_transaction: RP2InTransaction = cast(RP2InTransaction, asset_entry)
                 self.__logger.debug("Transaction: %s", str(in_transaction))
-                result.append(InTransaction(
-                    plugin=self.__RP2_INPUT,
-                    unique_id=in_transaction.unique_id,
-                    raw_data=str(in_transaction),
-                    timestamp=str(in_transaction.timestamp),
-                    asset=in_transaction.asset,
-                    exchange=in_transaction.exchange,
-                    holder=in_transaction.holder,
-                    transaction_type=in_transaction.transaction_type.value,
-                    spot_price=str(in_transaction.spot_price),
-                    crypto_in=str(in_transaction.crypto_in),
-                    crypto_fee=str(in_transaction.crypto_fee) if in_transaction.crypto_fee else None,
-                    fiat_in_no_fee=str(in_transaction.fiat_in_no_fee) if in_transaction.fiat_in_no_fee else None,
-                    fiat_in_with_fee=str(in_transaction.fiat_in_with_fee) if in_transaction.fiat_in_with_fee else None,
-                    fiat_fee=str(in_transaction.fiat_fee) if in_transaction.fiat_fee else None,
-                    notes=str(in_transaction.notes) if in_transaction.notes else None
-                ))
+                result.append(
+                    InTransaction(
+                        plugin=self.__RP2_INPUT,
+                        unique_id=in_transaction.unique_id,
+                        raw_data=str(in_transaction),
+                        timestamp=str(in_transaction.timestamp),
+                        asset=in_transaction.asset,
+                        exchange=in_transaction.exchange,
+                        holder=in_transaction.holder,
+                        transaction_type=in_transaction.transaction_type.value,
+                        spot_price=str(in_transaction.spot_price),
+                        crypto_in=str(in_transaction.crypto_in),
+                        crypto_fee=str(in_transaction.crypto_fee) if in_transaction.crypto_fee else None,
+                        fiat_in_no_fee=str(in_transaction.fiat_in_no_fee) if in_transaction.fiat_in_no_fee else None,
+                        fiat_in_with_fee=str(in_transaction.fiat_in_with_fee) if in_transaction.fiat_in_with_fee else None,
+                        fiat_fee=str(in_transaction.fiat_fee) if in_transaction.fiat_fee else None,
+                        notes=str(in_transaction.notes) if in_transaction.notes else None,
+                    )
+                )
 
             for asset_transfer in input_data.unfiltered_intra_transaction_set:
                 intra_transaction: RP2IntraTransaction = cast(RP2IntraTransaction, asset_transfer)
                 self.__logger.debug("Transaction: %s", str(intra_transaction))
                 result.append(
                     IntraTransaction(
                         plugin=self.__RP2_INPUT,
@@ -101,16 +99,17 @@
                         from_exchange=intra_transaction.from_exchange,
                         from_holder=intra_transaction.from_holder,
                         to_exchange=intra_transaction.to_exchange,
                         to_holder=intra_transaction.to_holder,
                         spot_price=str(intra_transaction.spot_price) if intra_transaction.spot_price else None,
                         crypto_sent=str(intra_transaction.crypto_sent),
                         crypto_received=str(intra_transaction.crypto_received),
-                        notes=str(intra_transaction.notes) if intra_transaction.notes else None
-                    ))
+                        notes=str(intra_transaction.notes) if intra_transaction.notes else None,
+                    )
+                )
 
             for asset_exit in input_data.unfiltered_out_transaction_set:
                 out_transaction: RP2OutTransaction = cast(RP2OutTransaction, asset_exit)
                 self.__logger.debug("Transaction: %s", str(out_transaction))
                 result.append(
                     OutTransaction(
                         plugin=self.__RP2_INPUT,
@@ -123,10 +122,11 @@
                         transaction_type=out_transaction.transaction_type.value,
                         spot_price=str(out_transaction.spot_price),
                         crypto_out_no_fee=str(out_transaction.crypto_out_no_fee),
                         crypto_fee=str(out_transaction.crypto_fee),
                         crypto_out_with_fee=str(out_transaction.crypto_out_with_fee),
                         fiat_out_no_fee=str(out_transaction.fiat_out_no_fee) if out_transaction.fiat_out_no_fee else None,
                         fiat_fee=str(out_transaction.fiat_fee) if out_transaction.fiat_fee else None,
-                        notes=str(out_transaction.notes) if out_transaction.notes else None
-                    ))
+                        notes=str(out_transaction.notes) if out_transaction.notes else None,
+                    )
+                )
         return result
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/rest/binance_com.py` & `dali-rp2-0.6.8/src/dali/plugin/input/rest/binance_com.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import json
 import re
 from datetime import datetime
 from multiprocessing.pool import ThreadPool
 from typing import Any, Dict, List, Optional, Union
 
 from ccxt import Exchange, binance
-
 from rp2.rp2_decimal import ZERO, RP2Decimal
 from rp2.rp2_error import RP2RuntimeError
 
 from dali.abstract_ccxt_input_plugin import (
     AbstractCcxtInputPlugin,
     ProcessOperationResult,
     Trade,
@@ -146,29 +145,27 @@
 
 _AIRDROP_LIST = [_SOLO_AIRDROP]
 _INTEREST_LIST = [_FLEXIBLE, _FLEXIBLE_SAVINGS, _LOCKED, _LOCKED_SAVINGS]
 _STAKING_LIST = [_ETH_STAKING, _LOCKED_STAKING, _BNB_VAULT, _LAUNCH_POOL, _GENERAL_STAKING]
 
 
 class InputPlugin(AbstractCcxtInputPlugin):
-
     __EXCHANGE_NAME: str = "Binance.com"
     __PLUGIN_NAME: str = "Binance.com_REST"
     __DEFAULT_THREAD_COUNT: int = 1
 
     def __init__(
         self,
         account_holder: str,
         api_key: str,
         api_secret: str,
         native_fiat: str,
         username: Optional[str] = None,
         thread_count: Optional[int] = __DEFAULT_THREAD_COUNT,
     ) -> None:
-
         self.__api_key = api_key
         self.__api_secret = api_secret
         # We will have a default start time of July 13th, 2017 since Binance Exchange officially launched on July 14th Beijing Time.
         super().__init__(account_holder, datetime(2017, 7, 13, 0, 0, 0, 0), native_fiat, thread_count)
         self.__username = username
 
         # We have to know what markets and algos are on Binance so that we can pull orders using the market
@@ -231,15 +228,14 @@
     ### Multiple transaction processing
 
     def _process_gains(
         self,
         in_transactions: List[InTransaction],
         out_transactions: List[OutTransaction],
     ) -> None:
-
         ### Regular Dividends from Staking (including Eth staking) and Savings (Lending) after around May 8th, 2021 01:00 UTC.
 
         # We need milliseconds for Binance
         current_start = self._start_time_ms
         now_time = int(datetime.now().timestamp()) * _MS_IN_SECOND
         processing_result_list: List[Optional[ProcessOperationResult]] = []
 
@@ -320,15 +316,14 @@
         total_current_payments: Dict[int, int] = {}
 
         # Subscriptions organized [asset][amount] = timestamp in milliseconds
         current_subscriptions: Dict[str, Dict[str, Dict[str, str]]] = {}
 
         # We will step backward in time from the switch over
         while current_start < now_time:
-
             self._logger.debug("Pulling locked staking from older api system from %s to %s", current_start, current_end)
 
             locked_staking = self._client.sapi_get_staking_stakingrecord(
                 params=({_START_TIME: current_start, _END_TIME: current_end, _PRODUCT: _STAKING, _TXN_TYPE: _INTEREST_PARAMETER, _SIZE: _INTEREST_SIZE_LIMIT})
             )
             # [
             #   {
@@ -388,15 +383,14 @@
             #         "type": "NORMAL",
             #         "status": "SUCCESS",
             #     }
             # ]
             # NOTE: all values are str
 
             for subscription in locked_subscriptions:
-
                 # If the dict already exists add another key, if not add new dict
                 if current_subscriptions.get(subscription[_ASSET]):
                     current_subscriptions[subscription[_ASSET]][f"{RP2Decimal(subscription[_AMOUNT]):.13f}"] = subscription
                 else:
                     current_subscriptions[subscription[_ASSET]] = {f"{RP2Decimal(subscription[_AMOUNT]):.13f}": subscription}
 
             locked_redemptions = self._client.sapi_get_staking_stakingrecord(
@@ -419,27 +413,24 @@
             #             "deliverDate": "1624148093000"
             #             "status": "PAID",
             #         }
             # ]
             # NOTE: all values are str
 
             for redemption in locked_redemptions:
-
                 redemption_amount: str = f"{RP2Decimal(redemption[_AMOUNT]):.13f}"
 
                 # Check if there is a subscription with this asset and if the redemption amount is equal to the subscription amount
                 if redemption[_ASSET] in current_subscriptions and redemption_amount not in current_subscriptions[redemption[_ASSET]]:
-
                     # If they do not equal we need to calculate what the amended principal should be based on total interest paid to that productId
                     total_interest_earned: RP2Decimal = total_current_interest[redemption[_POSITION_ID]]
                     original_principal: str = f"{(RP2Decimal(redemption[_AMOUNT]) + RP2Decimal(str(total_interest_earned))):.13f}"
                     earliest_redemption_timestamp: int = 0
 
                     if str(original_principal) in current_subscriptions[redemption[_ASSET]]:
-
                         subscription_time: int = int(current_subscriptions[redemption[_ASSET]][str(original_principal)][_TIME])
                         lockperiod_in_ms: int = int(current_subscriptions[redemption[_ASSET]][str(original_principal)][_LOCK_PERIOD]) * _ONE_DAY_IN_MS
                         earliest_redemption_timestamp = subscription_time + lockperiod_in_ms
 
                     else:
                         raise RP2RuntimeError(
                             f"Internal Error: Principal ({original_principal}) minus paid interest ({RP2Decimal(str(total_interest_earned))}) does not equal"
@@ -471,15 +462,14 @@
                     else:
                         raise RP2RuntimeError(
                             f"Internal Error: The redemption time ({self._rp2_timestamp_from_ms_epoch(redemption[_TIME])}) is not in the redemption window "
                             f"({self._rp2_timestamp_from_ms_epoch(str(earliest_redemption_timestamp))} + 2 days)."
                         )
 
                 elif redemption[_ASSET] in current_subscriptions and redemption_amount in current_subscriptions[redemption[_ASSET]]:
-
                     self._logger.debug("Locked Savings positionId %s redeemed successfully.", redemption[_POSITION_ID])
 
                 else:
                     raise RP2RuntimeError(f"Internal Error: Orphaned Redemption. Please open an issue at {self.ISSUES_URL}.")
 
             # if we returned the limit, we need to roll the window forward to the last time
             if len(locked_redemptions) < _INTEREST_SIZE_LIMIT:
@@ -493,15 +483,14 @@
 
         # Reset window
         current_start = self._start_time_ms
         current_end = current_start + _THIRTY_DAYS_IN_MS
 
         # We will step backward in time from the switch over
         while current_start < earliest_record_epoch:
-
             self._logger.debug("Pulling flexible saving from older api system from %s to %s", current_start, current_end)
 
             flexible_saving = self._client.sapi_get_lending_union_interesthistory(
                 params=({_START_TIME: current_start, _END_TIME: current_end, _LENDING_TYPE: _DAILY, _SIZE: _INTEREST_SIZE_LIMIT})
             )
             # [
             #     {
@@ -636,15 +625,14 @@
 
     def _process_implicit_api(  # pylint: disable=unused-argument
         self,
         in_transactions: List[InTransaction],
         out_transactions: List[OutTransaction],
         intra_transactions: List[IntraTransaction],
     ) -> None:
-
         # We need milliseconds for Binance
         now_time = int(datetime.now().timestamp()) * _MS_IN_SECOND
 
         processing_result_list: List[Optional[ProcessOperationResult]] = []
 
         # Crypto Bought with fiat. Technically this is a deposit of fiat that is used for a market order that fills immediately.
         # No limit on the date range
@@ -763,15 +751,14 @@
             dust_trades = self._client.fetch_my_dust_trades(params=({_START_TIME: current_start, _END_TIME: current_end}))
             # CCXT returns the same json as .fetch_trades()
 
             # Binance only returns 100 dust trades per call. If we hit the limit we will have to crawl
             # over each 'dribblet'. Each dribblet can have multiple assets converted into BNB at the same time.
             # If the user converts more than 100 assets at one time, we can not retrieve accurate records.
             if len(dust_trades) == _DUST_TRADE_RECORD_LIMIT:
-
                 first_dribblet = [x for x in dust_trades if x[_DIV_TIME] == dust_trades[0][_DIV_TIME]]
                 if len(first_dribblet) == _DUST_TRADE_RECORD_LIMIT:
                     raise RP2RuntimeError(
                         f"Internal error: too many assets dusted at the same time: " f"{self._rp2_timestamp_from_ms_epoch(str(dust_trades[0][_DIV_TIME]))}"
                     )
 
                 with ThreadPool(self._thread_count) as pool:
@@ -934,15 +921,14 @@
     def _process_fiat_payment(self, transaction: Any, notes: Optional[str] = None) -> ProcessOperationResult:
         self._logger.debug("Fiat Payment: %s", json.dumps(transaction))
         in_transaction_list: List[InTransaction] = []
         out_transaction_list: List[OutTransaction] = []
 
         if transaction[_STATUS] == "Completed":
             if self.is_native_fiat(transaction[_FIAT_CURRENCY]):
-
                 # For double entry accounting purposes we must create a fiat InTransaction
                 in_transaction_list.append(
                     InTransaction(
                         plugin=self.__PLUGIN_NAME,
                         unique_id=transaction[_ORDER_NO],
                         raw_data=json.dumps(transaction),
                         timestamp=self._rp2_timestamp_from_ms_epoch(transaction[_CREATE_TIME]),
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/rest/bitbank.py` & `dali-rp2-0.6.8/src/dali/plugin/input/rest/bitbank.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 # https://docs.ccxt.com/en/latest/index.html
 
 import json
 from datetime import datetime
 from typing import Any, List, Optional
 
 from ccxt import bitbank
-
 from rp2.rp2_decimal import ZERO, RP2Decimal
 
 from dali.abstract_ccxt_input_plugin import (
     AbstractCcxtInputPlugin,
     ProcessOperationResult,
 )
 from dali.ccxt_pagination import (
@@ -52,28 +51,26 @@
 _CURRENCY: str = "currency"
 _FEE: str = "fee"
 _ID: str = "id"
 _TIMESTAMP: str = "timestamp"
 
 
 class InputPlugin(AbstractCcxtInputPlugin):
-
     __EXCHANGE_NAME: str = "Bitbank.cc"
     __PLUGIN_NAME: str = "Bitbank.cc_REST"
     __DEFAULT_THREAD_COUNT: int = 1
 
     def __init__(
         self,
         account_holder: str,
         api_key: str,
         api_secret: str,
         native_fiat: str,
         thread_count: Optional[int] = __DEFAULT_THREAD_COUNT,
     ) -> None:
-
         self.__api_key = api_key
         self.__api_secret = api_secret
         # We will have a default start time of March 1st, 2017 since Bitbank Exchange officially launched on March 1st Japan Time.
         super().__init__(account_holder, datetime(2017, 3, 1, 0, 0, 0, 0), native_fiat, thread_count)
 
     def exchange_name(self) -> str:
         return self.__EXCHANGE_NAME
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/rest/coinbase.py` & `dali-rp2-0.6.8/src/dali/plugin/input/rest/coinbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from typing import Any, Dict, List, NamedTuple, Optional, cast
 
 import requests
 from requests import PreparedRequest
 from requests.auth import AuthBase
 from requests.models import Response
 from requests.sessions import Session
-
 from rp2.abstract_country import AbstractCountry
 from rp2.logger import create_logger
 from rp2.rp2_decimal import ZERO, RP2Decimal
 from rp2.rp2_error import RP2RuntimeError
 
 from dali.abstract_input_plugin import AbstractInputPlugin
 from dali.abstract_transaction import AbstractTransaction
@@ -110,15 +109,14 @@
 
 class _SwapPair(NamedTuple):
     in_transaction: Optional[_InTransactionAndIndex]
     out_transaction: Optional[_OutTransactionAndIndex]
 
 
 class _CoinbaseAuth(AuthBase):
-
     __API_VERSION: str = "2017-11-27"
 
     def __init__(self, api_key: str, api_secret: str) -> None:
         self.__api_key: str = api_key
         self.__api_secret: str = api_secret
 
     def __call__(self, request: PreparedRequest) -> PreparedRequest:
@@ -134,15 +132,14 @@
                 "CB-ACCESS-TIMESTAMP": timestamp,
             }
         )
         return request
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __API_URL: str = "https://api.coinbase.com"
     __DEFAULT_THREAD_COUNT: int = 3
     __MAX_THREAD_COUNT: int = 4
     # Coinbase returns very low precision fiat data (only 2 decimal digits): if the value is less than 1c Coinbase
     # rounds it to zero, which causes various computation problems (spot_price, etc.). As a workaround, when this
     # condition is detected the plugin sets affected fields to UNKNOWN or None (depending on their nature), so that
     # they can be filled later by the transaction resolver and RP2.
@@ -156,15 +153,14 @@
         self,
         account_holder: str,
         api_key: str,
         api_secret: str,
         native_fiat: Optional[str] = None,
         thread_count: Optional[int] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__api_url: str = InputPlugin.__API_URL
         self.__auth: _CoinbaseAuth = _CoinbaseAuth(api_key, api_secret)
         self.__session: Session = requests.Session()
         self.__logger: logging.Logger = create_logger(f"{self.__COINBASE}/{self.account_holder}")
         self.__cache_key: str = f"{self.__COINBASE.lower()}-{account_holder}"
         self.__thread_count = thread_count if thread_count else self.__DEFAULT_THREAD_COUNT
@@ -418,23 +414,20 @@
                         f"{out_transaction.crypto_out_with_fee} {out_transaction.asset} -> "
                         f"{in_transaction.crypto_in} {in_transaction.asset} "
                         f"({in_transaction.asset} in-transaction unique id: {in_transaction.unique_id})"
                     ),
                 )
 
     def _is_credit_card_spend(self, transaction: Any) -> bool:
-
         return (  # type: ignore
             transaction[_TYPE] is None
             and _TO in transaction
             and _EMAIL in transaction[_TO]
             and transaction[_TO][_EMAIL] == "treasury+coinbase-card@coinbase.com"
-        ) or (
-            transaction[_TYPE] == _CARDSPEND
-        )
+        ) or (transaction[_TYPE] == _CARDSPEND)
 
     def _process_account(self, account: Dict[str, Any]) -> Optional[_ProcessAccountResult]:
         currency: str = account[_CURRENCY][_CODE]
         account_id: str = account[_ID]
         in_transaction_list: List[InTransaction] = []
         out_transaction_list: List[OutTransaction] = []
         intra_transaction_list: List[IntraTransaction] = []
@@ -557,15 +550,15 @@
                     crypto_received=str(-amount),
                 )
             )
         elif transaction_type == _SEND:
             transaction_network = transaction[_NETWORK]
             crypto_hash: str = transaction_network[_HASH] if _HASH in transaction_network else Keyword.UNKNOWN.value
             if amount < ZERO:
-                if ( # pylint: disable=too-many-boolean-expressions
+                if (  # pylint: disable=too-many-boolean-expressions
                     _TO in transaction
                     and transaction[_TO] is not None
                     and _RESOURCE in transaction[_TO]
                     and transaction[_TO][_RESOURCE] == _USER
                     and transaction_network[_STATUS] == _OFF_BLOCKCHAIN
                     and _SUBTITLE in transaction[_DETAILS]
                     and _EMAIL in transaction[_TO]
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/input/rest/coinbase_pro.py` & `dali-rp2-0.6.8/src/dali/plugin/input/rest/coinbase_pro.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from typing import Any, Dict, List, NamedTuple, Optional, cast
 
 import requests
 from requests import PreparedRequest
 from requests.auth import AuthBase
 from requests.models import Response
 from requests.sessions import Session
-
 from rp2.abstract_country import AbstractCountry
 from rp2.logger import create_logger
 from rp2.rp2_decimal import ZERO, RP2Decimal
 from rp2.rp2_error import RP2RuntimeError
 
 from dali.abstract_input_plugin import AbstractInputPlugin
 from dali.abstract_transaction import AbstractTransaction, AssetAndUniqueId
@@ -66,14 +65,15 @@
 _SIDE: str = "side"
 _SIZE: str = "size"
 _TO_ACCOUNT_ID: str = "to_account_id"
 _TRADE_ID: str = "trade_id"
 _TRANSFER: str = "transfer"
 _TRANSFER_ID: str = "transfer_id"
 _TRANSFER_TYPE: str = "transfer_type"
+_TX_SERVICE_TRANSACTION_ID: str = "tx_service_transaction_id"
 _TYPE: str = "type"
 _USD_VOLUME: str = "usd_volume"
 _WITHDRAW: str = "withdraw"
 
 
 class _ProcessAccountResult(NamedTuple):
     in_transactions: List[InTransaction]
@@ -108,15 +108,14 @@
                 "CB-ACCESS-PASSPHRASE": self.__api_passphrase,
             }
         )
         return request
 
 
 class InputPlugin(AbstractInputPlugin):
-
     __API_URL: str = "https://api.pro.coinbase.com/"
     __DEFAULT_THREAD_COUNT: int = 2
     __MAX_THREAD_COUNT: int = 4
     __TIMEOUT: int = 30
 
     __COINBASE_PRO: str = "Coinbase Pro"
 
@@ -129,15 +128,14 @@
         account_holder: str,
         api_key: str,
         api_secret: str,
         api_passphrase: str,
         native_fiat: Optional[str] = None,
         thread_count: Optional[int] = None,
     ) -> None:
-
         super().__init__(account_holder=account_holder, native_fiat=native_fiat)
         self.__api_url: str = InputPlugin.__API_URL
         self.__auth = _CoinbaseProAuth(api_key, api_secret, api_passphrase)
         self.__session: Session = requests.Session()
         self.__logger: logging.Logger = create_logger(f"{self.__COINBASE_PRO}/{self.account_holder}")
         self.__cache_key: str = f"coinbase_pro-{account_holder}"
         self.__thread_count = thread_count if thread_count else self.__DEFAULT_THREAD_COUNT
@@ -227,19 +225,19 @@
         transfer_id: str = transaction_details[_TRANSFER_ID]
         transfer: Any = self.__get_transfer(transfer_id)
         transfer_details: Any = transfer[_DETAILS]
         crypto_hash: str = Keyword.UNKNOWN.value
         raw_data: str = f"{json.dumps(transaction)}//{json.dumps(transfer)}"
 
         self.__logger.debug("Transfer: %s", json.dumps(transfer))
-        if _CRYPTO_TRANSACTION_HASH not in transfer_details:
-            self.__logger.debug("Transfer to/from Coinbase already captured by Coinbase plugin: ignoring.")
-            return
-
-        if _COINBASE_TRANSACTION_ID in transfer_details:
+        if (
+            _CRYPTO_TRANSACTION_HASH not in transfer_details
+            or _TX_SERVICE_TRANSACTION_ID not in transfer_details
+            or _COINBASE_TRANSACTION_ID in transfer_details
+        ):
             self.__logger.debug("Transfer is a Coinbase transaction already captured by Coinbase plugin: ignoring.")
             return
 
         crypto_hash = transfer_details[_CRYPTO_TRANSACTION_HASH]
 
         if transaction_details[_TRANSFER_TYPE] == _DEPOSIT:
             intra_transaction_list.append(
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/pair_converter/ccxt.py` & `dali-rp2-0.6.8/src/dali/plugin/pair_converter/ccxt.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,14 @@
         self,
         historical_price_type: str,
         default_exchange: Optional[str] = None,
         fiat_priority: Optional[str] = None,
         google_api_key: Optional[str] = None,
         exchange_locked: Optional[bool] = None,
     ) -> None:
-
         super().__init__(historical_price_type=historical_price_type, fiat_priority=fiat_priority)
         self.__logger: logging.Logger = create_logger(f"{self.name()}/{historical_price_type}")
 
         self.__exchanges: Dict[str, Exchange] = {}
         self.__exchange_markets: Dict[str, Dict[str, List[str]]] = {}
         self.__google_api_key: Optional[str] = google_api_key
         self.__exchange_locked: bool = exchange_locked if exchange_locked is not None else False
@@ -186,15 +185,14 @@
         return self.__exchange_markets
 
     @property
     def exchange_graphs(self) -> Dict[str, Dict[str, Dict[str, None]]]:
         return self.__exchange_graphs
 
     def _bfs_cyclic(self, graph: Dict[str, Dict[str, None]], start: str, end: str) -> Optional[List[str]]:
-
         # maintain a queue of paths
         # TO BE IMPLEMENTED - using on vertex queue and one dict?
         # https://github.com/eprbell/dali-rp2/pull/53#discussion_r924058754
         queue: List[List[str]] = []
         visited: Dict[str, None] = {}
 
         # push the first path into the queue
@@ -209,15 +207,14 @@
 
             # path found
             if node == end:
                 return path
 
             # enumerate all adjacent nodes, construct a new path and push it into the queue
             for adjacent in graph.get(node, {}):
-
                 # prevents an infinite loop.
                 if adjacent not in visited:
                     new_path: List[str] = list(path)
                     new_path.append(adjacent)
                     queue.append(new_path)
                     visited[adjacent] = None
 
@@ -281,15 +278,14 @@
         conversion_route: List[AssetPairAndHistoricalPrice] = []
         last_node: Optional[str] = None
         hop_bar: Optional[HistoricalBar] = None
 
         # Build conversion stack, we will iterate over this to find the price for each conversion
         # Then multiply them together to get our final price.
         for node in pricing_path:
-
             if last_node:
                 conversion_route.append(
                     AssetPairAndHistoricalPrice(
                         from_asset=last_node,
                         to_asset=node,
                         exchange=current_markets[(last_node + node)][0],
                         historical_data=None,
@@ -372,15 +368,14 @@
             historical_bar = self._get_bar_from_cache(key)
             self.__exchange_csv_reader[exchange] = csv_reader
             if historical_bar is not None:
                 self.__logger.debug("Retrieved bar cache - %s for %s/%s->%s for %s", historical_bar, key.timestamp, key.from_asset, key.to_asset, key.exchange)
                 return historical_bar
 
         while retry_count < len(_TIME_GRANULARITY):
-
             timeframe: str = _TIME_GRANULARITY[retry_count]
             request_count: int = 0
             historical_data: List[List[Union[int, float]]] = []
 
             # Most exceptions are caused by request limits of the underlying APIs
             while request_count < 9:
                 try:
@@ -457,15 +452,14 @@
 
             if current_graph.get(base_asset) and (quote_asset not in current_graph[base_asset]):
                 current_graph[base_asset][quote_asset] = None
             else:
                 current_graph[base_asset] = {quote_asset: None}
 
     def _add_exchange_to_memcache(self, exchange: str) -> None:
-
         if exchange not in self.__exchanges:
             # initializes the cctx exchange instance which is used to get the historical data
             # https://docs.ccxt.com/en/latest/manual.html#notes-on-rate-limiter
             current_exchange: Exchange = _EXCHANGE_DICT[exchange]({"enableRateLimit": True})
         else:
             current_exchange = self.__exchanges[exchange]
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/pair_converter/ccxt_binance.py` & `dali-rp2-0.6.8/src/dali/plugin/pair_converter/ccxt_binance.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,13 @@
 
 class PairConverterPlugin(CcxtPairConverterPlugin):
     def __init__(
         self,
         historical_price_type: str,
         fiat_priority: Optional[str] = None,
     ) -> None:
-
         super().__init__(
             historical_price_type=historical_price_type,
             default_exchange="Binance.com",
             fiat_priority=fiat_priority,
             exchange_locked=True,
         )
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/pair_converter/ccxt_kraken.py` & `dali-rp2-0.6.8/src/dali/plugin/pair_converter/ccxt_kraken.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 class PairConverterPlugin(CcxtPairConverterPlugin):
     def __init__(
         self,
         historical_price_type: str,
         fiat_priority: Optional[str] = None,
         google_api_key: Optional[str] = None,
     ) -> None:
-
         super().__init__(
             historical_price_type=historical_price_type,
             default_exchange="Kraken",
             fiat_priority=fiat_priority,
             google_api_key=google_api_key,
             exchange_locked=True,
         )
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/pair_converter/csv/kraken.py` & `dali-rp2-0.6.8/src/dali/plugin/pair_converter/csv/kraken.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 
 class _PairStartEnd(NamedTuple):
     end: int
     start: int
 
 
 class Kraken:
-
     __KRAKEN_OHLCVT: str = "Kraken.com_CSVOHLCVT"
 
     __CACHE_DIRECTORY: str = ".dali_cache/kraken/"
     __CACHE_KEY: str = "Kraken-csv-download"
 
     __TIMEOUT: int = 30
     __THREAD_COUNT: int = 3
@@ -109,15 +108,14 @@
 
     __DELIMITER: str = ","
 
     def __init__(
         self,
         google_api_key: str,
     ) -> None:
-
         self.__google_api_key: str = google_api_key
         self.__logger: logging.Logger = create_logger(self.__KRAKEN_OHLCVT)
         self.__session: Session = requests.Session()
         self.__cached_pairs: Dict[str, _PairStartEnd] = {}
         self.__cache_loaded: bool = False
 
         if not path.exists(self.__CACHE_DIRECTORY):
@@ -149,15 +147,14 @@
                 next_timestamp += chunk_size
             chunk.append(line)
         if chunk:
             position = _PAIR_END
             yield position, chunk
 
     def _split_chunks_size_n(self, file_name: str, csv_file: str, chunk_size: int = _CHUNK_SIZE) -> None:
-
         pair, duration_in_minutes = file_name.strip(".csv").split("_", 1)
         chunk_size *= min(int(duration_in_minutes), _MAX_MULTIPLIER)
         file_timestamp: str
         pair_start: Optional[int] = None
         pair_end: int
         pair_duration: str = pair + duration_in_minutes
```

### Comparing `dali-rp2-0.6.7/src/dali/plugin/pair_converter/historic_crypto.py` & `dali-rp2-0.6.8/src/dali/plugin/pair_converter/historic_crypto.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/src/dali/transaction_resolver.py` & `dali-rp2-0.6.8/src/dali/transaction_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,15 +474,14 @@
 
 
 def _resolve_intra_intra_transaction(
     transaction1: IntraTransaction,
     transaction2: IntraTransaction,
     notes: Optional[str],
 ) -> IntraTransaction:
-
     # Pick the max of the two timestamps as the timestamp of the new resolved transaction
     timestamp: datetime = max(transaction1.timestamp_value, transaction2.timestamp_value)
     from_exchange: str = _resolve_fields(
         f"transaction1.{Keyword.FROM_EXCHANGE.value}",
         f"transaction2.{Keyword.FROM_EXCHANGE.value}",
         transaction1.from_exchange,
         transaction2.from_exchange,
@@ -596,15 +595,14 @@
 
 
 def _resolve_in_out_transaction(
     in_transaction: InTransaction,
     out_transaction: OutTransaction,
     notes: Optional[str],
 ) -> IntraTransaction:
-
     timestamp: datetime = in_transaction.timestamp_value
     from_exchange: str = out_transaction.exchange
     from_holder: str = out_transaction.holder
     to_exchange: str = in_transaction.exchange
     to_holder: str = in_transaction.holder
     spot_price: str = _resolve_fields(
         f"out_transaction.{Keyword.SPOT_PRICE.value}",
```

### Comparing `dali-rp2-0.6.7/src/dali_rp2.egg-info/PKG-INFO` & `dali-rp2-0.6.8/src/dali_rp2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dali-rp2
-Version: 0.6.7
+Version: 0.6.8
 Summary: Data loader and input generator for RP2 (https://pypi.org/project/rp2/), the privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: DaLI removes the need to manually prepare RP2 input files. Just like RP2, DaLI is also free, open-source and it prioritizes user privacy.
 Home-page: https://github.com/eprbell/dali-rp2
 Author: eprbell
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eprbell/dali-rp2
 Project-URL: Developer Documentation, https://github.com/eprbell/dali-rp2/blob/main/README.dev.md
 Project-URL: User Documentation, https://github.com/eprbell/dali-rp2/blob/main/README.md
@@ -35,15 +35,15 @@
 
 <!--- Unless required by applicable law or agreed to in writing, software --->
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
-# DaLI for RP2 v0.6.7
+# DaLI for RP2 v0.6.8
 
 Privacy-focused, free, extensible data loader for RP2 (the crypto tax calculator)
 
 [![Static Analysis / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/dali-rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/dali-rp2/actions/workflows/windows_unit_tests.yml)
@@ -67,30 +67,30 @@
 * **[Reporting Bugs](#reporting-bugs)**
 * **[Contributing](#contributing)**
 * **[Developer Documentation](#developer-documentation)**
 * **[Frequently Asked Questions](#frequently-asked-questions)**
 * **[Change Log](#change-log)**
 
 ## Introduction
-[DaLI](https://github.com/eprbell/dali-rp2) (Data Loader Interface) is a data loader and input generator for [RP2](https://github.com/eprbell/rp2), the privacy-focused, free, non-commercial, open-source cryptocurrency tax calculator: DaLI removes the need to manually prepare RP2 input files. Just like RP2, DaLI is also free, non-commercial, open-source and it prioritizes user privacy by storing crypto transaction data on the user's computer and never sending it anywhere else.
+[DaLI](https://github.com/eprbell/dali-rp2) (Data Loader Interface) is a data loader and input generator for [RP2](https://github.com/eprbell/rp2), the privacy-focused, free, non-commercial, open-source, community-driven multi-country cryptocurrency tax calculator: DaLI removes the need to manually prepare RP2 input files. Just like RP2, DaLI is also free, non-commercial, open-source and it prioritizes user privacy by storing crypto transaction data on the user's computer and never sending it anywhere else.
 
 It performs the following operations:
 * it reads in crypto transaction information from multiples native sources: CSV files and/or REST-based services;
 * it analyzes, processes and merges this data;
-* it uses the processed data to generate an ODS input file for RP2 and its respective JSON configuration file.
+* it uses the processed data to generate an ODS input file for RP2 and its respective configuration file.
 
 DaLI has a programmable plugin architecture for [data loaders](https://github.com/eprbell/dali-rp2/blob/main/README.dev.md#data-loader-plugin-development) (both CSV and REST-based), [pair converters](https://github.com/eprbell/dali-rp2/blob/main/README.dev.md#pair-converter-plugin-development) and [countries](https://github.com/eprbell/dali-rp2/blob/main/README.dev.md#country-plugin-development). While some exchanges and wallets are already supported out-of-the-box, more are needed: help us make DaLI a robust open-source, community-driven crypto data loader by [contributing](https://github.com/eprbell/dali-rp2/tree/main/CONTRIBUTING.md#contributing-to-the-repository) plugins for exchanges and wallets! Check [open issues](https://github.com/eprbell/dali-rp2/issues) or open a new one.
 
 DaLI has [unit test](https://github.com/eprbell/dali-rp2/tree/main/tests/) coverage to reduce the risk of regression.
 
 Note that DaLI has RP2 as a dependency, so installing DaLI causes RP2 to be installed as well.
 
 **IMPORTANT DISCLAIMER**:
 * DaLI offers no guarantee of correctness (read the [license](https://github.com/eprbell/dali-rp2/tree/main/LICENSE)): always verify results with the help of a tax professional.
-* The author of DaLI and RP2 is not a tax professional, but has used RP2 personally for a few years.
+* The author of DaLI and RP2 is not a tax professional, but has used RP2 and DaLI personally for a few years.
 
 ## License
 DaLI is released under the terms of Apache License Version 2.0. For more information see [LICENSE](https://github.com/eprbell/dali-rp2/tree/main/LICENSE) or <http://www.apache.org/licenses/LICENSE-2.0>.
 
 ## Download
 The latest version of DaLI can be downloaded at: <https://pypi.org/project/dali-rp2/>
 
@@ -229,14 +229,17 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 # RP2 Change Log
 
+## 0.6.8
+* Coinbase data loader: added a new flavor of transfer transaction that was slightly different from the other ones (#137)
+
 ## 0.6.7
 * Coinbase data loader: fixed bug in advanced trade buy logic was not accounting for fee correctly
 * Coinbase data loader: added support for moving coins into staking pool (#132)
 
 ## 0.6.5
 * new Trezor CSV plugin supporting the latest format from Trezor Suite
```

### Comparing `dali-rp2-0.6.7/src/dali_rp2.egg-info/SOURCES.txt` & `dali-rp2-0.6.8/src/dali_rp2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/ods_diff.py` & `dali-rp2-0.6.8/tests/ods_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     if value is None:
         value = ""
 
     return value
 
 
 def ods_diff(file1_path: Path, file2_path: Path, generate_ascii_representation: bool) -> str:  # pylint: disable=too-many-branches
-
     if not file1_path.exists():
         return f"Error: {file1_path} does not exist"
     if not file2_path.exists():
         return f"Error: {file2_path} does not exist"
 
     file1: Any = ezodf.opendoc(str(file1_path))
     file2: Any = ezodf.opendoc(str(file2_path))
@@ -118,15 +117,14 @@
                 temp_file.flush()
                 print(f"ASCII representation of {file_path}: {temp_file.name}")
 
     return "\n".join(unified_diff(contents1, contents2, lineterm=""))
 
 
 def main() -> None:
-
     parser: ArgumentParser = ArgumentParser(description="Generate yearly capital gain/loss report and account balances for crypto holdings.")
     parser.add_argument(
         "-a",
         "--ascii-representation",
         action="store_true",
         help="Save ASCII representation of ODS files in temporary directory",
     )
```

### Comparing `dali-rp2-0.6.7/tests/test_cache.py` & `dali-rp2-0.6.8/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_historical_bar.py` & `dali-rp2-0.6.8/tests/test_historical_bar.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_ods_output_diff.py` & `dali-rp2-0.6.8/tests/test_ods_output_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 CONFIG_PATH: Path = ROOT_PATH / Path("config")
 INPUT_PATH: Path = ROOT_PATH / Path("input")
 GOLDEN_PATH: Path = INPUT_PATH / Path("golden")
 OUTPUT_PATH: Path = ROOT_PATH / Path("output")
 
 
 class TestODSOutputDiff(unittest.TestCase):
-
     output_dir: Path
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.output_dir = OUTPUT_PATH / Path(__file__[:-3]).name
         shutil.rmtree(cls.output_dir, ignore_errors=True)
         shutil.rmtree(CACHE_PATH, ignore_errors=True)
@@ -50,15 +49,14 @@
     @classmethod
     def _generate(
         cls,
         output_dir: Path,
         test_name: str,
         config: str,
     ) -> None:
-
         arguments: List[str] = [
             "dali_us",
             "-s",
             "-o",
             str(output_dir),
             "-p",
             f"{test_name}_",
```

### Comparing `dali-rp2-0.6.7/tests/test_plugin_binance_com.py` & `dali-rp2-0.6.8/tests/test_plugin_binance_com.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 import datetime
 from itertools import chain, repeat
 from typing import Any, Dict, List, Union
 
 from ccxt import Exchange
 from dateutil import parser
-
 from rp2.plugin.country.us import US
 from rp2.rp2_decimal import RP2Decimal
 
 from dali.configuration import Keyword
 from dali.in_transaction import InTransaction
 from dali.intra_transaction import IntraTransaction
 from dali.out_transaction import OutTransaction
```

### Comparing `dali-rp2-0.6.7/tests/test_plugin_binance_com_supplemental_csv.py` & `dali-rp2-0.6.8/tests/test_plugin_binance_com_supplemental_csv.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_plugin_bitbank_supplemental_csv.py` & `dali-rp2-0.6.8/tests/test_plugin_bitbank_supplemental_csv.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_plugin_ccxt.py` & `dali-rp2-0.6.8/tests/test_plugin_ccxt.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_plugin_coinbase.py` & `dali-rp2-0.6.8/tests/test_plugin_coinbase.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_plugin_coinbase_pro.py` & `dali-rp2-0.6.8/tests/test_plugin_coinbase_pro.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_plugin_coincheck_supplemental.py` & `dali-rp2-0.6.8/tests/test_plugin_coincheck_supplemental.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_plugin_historic_crypto.py` & `dali-rp2-0.6.8/tests/test_plugin_historic_crypto.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_plugin_kraken_csv_download.py` & `dali-rp2-0.6.8/tests/test_plugin_kraken_csv_download.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_plugin_ods_rp2_input.py` & `dali-rp2-0.6.8/tests/test_plugin_ods_rp2_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,34 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List
 import unittest
+from typing import List
 
-from rp2.rp2_decimal import ZERO, RP2Decimal
 from rp2.plugin.country.us import US
+from rp2.rp2_decimal import ZERO, RP2Decimal
 
-from dali.configuration import Keyword
 from dali.abstract_transaction import AbstractTransaction
+from dali.configuration import Keyword
 from dali.in_transaction import InTransaction
-from dali.out_transaction import OutTransaction
 from dali.intra_transaction import IntraTransaction
+from dali.out_transaction import OutTransaction
 from dali.plugin.input.ods.rp2_input import InputPlugin
 
 
 class TestRP2InputOds(unittest.TestCase):
-
     transactions: List[AbstractTransaction]
 
     @classmethod
     def setUpClass(cls) -> None:
-        plugin = InputPlugin(
-            configuration_path='input/test_ods_rp2_input.ini',
-            input_file='input/test_ods_rp2_input.ods',
-            native_fiat="USD"
-        )
+        plugin = InputPlugin(configuration_path="input/test_ods_rp2_input.ini", input_file="input/test_ods_rp2_input.ods", native_fiat="USD")
         cls.transactions = plugin.load(US())
 
     def test_all_transactions_found(self) -> None:
         assert len(self.transactions) == 9
 
     def test_in_transactions(self) -> None:
         # Buy BTC transaction 1
```

### Comparing `dali-rp2-0.6.7/tests/test_plugin_pionex.py` & `dali-rp2-0.6.8/tests/test_plugin_pionex.py`

 * *Files identical despite different names*

### Comparing `dali-rp2-0.6.7/tests/test_transaction_resolver.py` & `dali-rp2-0.6.8/tests/test_transaction_resolver.py`

 * *Files identical despite different names*

