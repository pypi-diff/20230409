# Comparing `tmp/exchange_calendars-4.2.5.tar.gz` & `tmp/exchange_calendars-4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars-4.2.5.tar", last modified: Fri Jan 27 15:30:35 2023, max compression
+gzip compressed data, was "exchange_calendars-4.2.6.tar", last modified: Sun Apr  9 08:25:16 2023, max compression
```

## Comparing `exchange_calendars-4.2.5.tar` & `exchange_calendars-4.2.6.tar`

### file list

```diff
@@ -1,236 +1,236 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:35.910506 exchange_calendars-4.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    38414 2023-01-27 15:30:35.910506 exchange_calendars-4.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:35.830505 exchange_calendars-4.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/docs/changes_archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:35.830505 exchange_calendars-4.2.5/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    91635 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/docs/tutorials/calendar_methods.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37097 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/docs/tutorials/calendar_properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/docs/tutorials/minutes.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/docs/tutorials/sessions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   149635 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/docs/tutorials/trading_index.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:35.834505 exchange_calendars-4.2.5/etc/
--rw-r--r--   0 runner    (1001) docker     (123)   141885 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/NYSE-Historical-Closings.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/check_holidays.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3854 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/ecal
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/factory_bounds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50169 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/lunisolar
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/make_exchange_calendar_test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/requirements_lunisolar.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/requirements_minpandas.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/requirements_update_xkrx_holidays.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/etc/update_xkrx_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:35.850505 exchange_calendars-4.2.5/exchange_calendars/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-27 15:30:35.000000 exchange_calendars-4.2.5/exchange_calendars/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/always_open.py
--rw-r--r--   0 runner    (1001) docker     (123)    24828 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/calendar_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/calendar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/common_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/ecal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   108025 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_aixk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_asex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_bvmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_cmes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_iepa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xasx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbkk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xcbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xcse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xdub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xfra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xhel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xhkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xjse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xkar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xkls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xkrx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xlim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xlis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xlon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xmad.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xmex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xmil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xnys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xnze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xosl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xpra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xsgo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xshg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xsto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xswx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xtae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xtai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xtks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xtse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xwar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xwbo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/lunisolar_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:35.854505 exchange_calendars-4.2.5/exchange_calendars/pandas_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/pandas_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/pandas_extensions/holiday.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/pandas_extensions/korean_holiday.py
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/pandas_extensions/offsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/precomputed_exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/tase_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/us_futures_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/us_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:35.854505 exchange_calendars-4.2.5/exchange_calendars/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/weekday_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/xbkk_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/xkls_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)    34830 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/xkrx_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/exchange_calendars/xtks_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:35.854505 exchange_calendars-4.2.5/exchange_calendars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38414 2023-01-27 15:30:35.000000 exchange_calendars-4.2.5/exchange_calendars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-01-27 15:30:35.000000 exchange_calendars-4.2.5/exchange_calendars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 15:30:35.000000 exchange_calendars-4.2.5/exchange_calendars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-27 15:30:35.000000 exchange_calendars-4.2.5/exchange_calendars.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-27 15:30:35.000000 exchange_calendars-4.2.5/exchange_calendars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-27 15:30:35.000000 exchange_calendars-4.2.5/exchange_calendars.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-27 15:30:35.910506 exchange_calendars-4.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:35.870506 exchange_calendars-4.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:30:35.910506 exchange_calendars-4.2.5/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/24-5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/24-7.csv
--rw-r--r--   0 runner    (1001) docker     (123)   110144 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/aixk.csv
--rw-r--r--   0 runner    (1001) docker     (123)   496439 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/asex.csv
--rw-r--r--   0 runner    (1001) docker     (123)   537779 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/bvmf.csv
--rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/cmes.csv
--rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/iepa.csv
--rw-r--r--   0 runner    (1001) docker     (123)   114134 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)   492279 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xams.csv
--rw-r--r--   0 runner    (1001) docker     (123)   560074 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xasx.csv
--rw-r--r--   0 runner    (1001) docker     (123)   494164 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xbkk.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486819 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xbog.csv
--rw-r--r--   0 runner    (1001) docker     (123)   418309 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xbom.csv
--rw-r--r--   0 runner    (1001) docker     (123)   492344 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xbru.csv
--rw-r--r--   0 runner    (1001) docker     (123)   530954 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xbse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   499559 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xbud.csv
--rw-r--r--   0 runner    (1001) docker     (123)   498389 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xbue.csv
--rw-r--r--   0 runner    (1001) docker     (123)   547139 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xcbf.csv
--rw-r--r--   0 runner    (1001) docker     (123)   484804 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xcse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   507099 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xdub.csv
--rw-r--r--   0 runner    (1001) docker     (123)   552404 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xetr.csv
--rw-r--r--   0 runner    (1001) docker     (123)   551104 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xfra.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486559 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xhel.csv
--rw-r--r--   0 runner    (1001) docker     (123)   868914 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xhkg.csv
--rw-r--r--   0 runner    (1001) docker     (123)   145764 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xice.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500014 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xidx.csv
--rw-r--r--   0 runner    (1001) docker     (123)   502614 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xist.csv
--rw-r--r--   0 runner    (1001) docker     (123)   499819 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xjse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   504889 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xkar.csv
--rw-r--r--   0 runner    (1001) docker     (123)   499299 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xkls.csv
--rw-r--r--   0 runner    (1001) docker     (123)   793869 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xkrx.csv
--rw-r--r--   0 runner    (1001) docker     (123)   501444 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xlim.csv
--rw-r--r--   0 runner    (1001) docker     (123)   488119 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xlis.csv
--rw-r--r--   0 runner    (1001) docker     (123)   553574 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xlon.csv
--rw-r--r--   0 runner    (1001) docker     (123)   541224 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xmad.csv
--rw-r--r--   0 runner    (1001) docker     (123)   503979 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xmex.csv
--rw-r--r--   0 runner    (1001) docker     (123)   490784 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xmil.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500079 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xmos.csv
--rw-r--r--   0 runner    (1001) docker     (123)   541094 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xnys.csv
--rw-r--r--   0 runner    (1001) docker     (123)   550909 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xnze.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486299 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xosl.csv
--rw-r--r--   0 runner    (1001) docker     (123)   493059 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xpar.csv
--rw-r--r--   0 runner    (1001) docker     (123)   504694 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xphs.csv
--rw-r--r--   0 runner    (1001) docker     (123)   501184 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xpra.csv
--rw-r--r--   0 runner    (1001) docker     (123)   618964 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xses.csv
--rw-r--r--   0 runner    (1001) docker     (123)   498714 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xsgo.csv
--rw-r--r--   0 runner    (1001) docker     (123)   840979 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xshg.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xsto.csv
--rw-r--r--   0 runner    (1001) docker     (123)   485129 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xswx.csv
--rw-r--r--   0 runner    (1001) docker     (123)    79204 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xtae.csv
--rw-r--r--   0 runner    (1001) docker     (123)   548374 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xtai.csv
--rw-r--r--   0 runner    (1001) docker     (123)   617749 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xtks.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xtse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500989 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xwar.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500079 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/resources/xwbo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_aixk_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_always_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_asex_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_bvmf_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_calendar_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    69067 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_calendar_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_cmes_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)   162037 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_iepa_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_weekday_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xams_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xasx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xbkk_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xbog_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xbom_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xbru_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xbse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xbud_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xbue_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xcbf_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xcse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xdub_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xetr_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xfra_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xhel_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xhkg_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xice_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xidx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xist_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xjse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xkar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xkls_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xkrx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xlim_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xlis_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xlon_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xmad_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xmex_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xmil_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xmos_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xnys_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xnze_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xosl_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xpar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xphs_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xpra_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xses_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xsgo_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xshg_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xsto_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xswx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xtae_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xtai_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xtks_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xtse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xwar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-01-27 15:30:24.000000 exchange_calendars-4.2.5/tests/test_xwbo_calendar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.742903 exchange_calendars-4.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    38414 2023-04-09 08:25:16.742903 exchange_calendars-4.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.678897 exchange_calendars-4.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/changes_archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.678897 exchange_calendars-4.2.6/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    91635 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/tutorials/calendar_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37097 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/tutorials/calendar_properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/tutorials/minutes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/tutorials/sessions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   149635 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/tutorials/trading_index.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.678897 exchange_calendars-4.2.6/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)   141885 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/NYSE-Historical-Closings.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/check_holidays.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3854 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/ecal
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/factory_bounds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50169 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/lunisolar
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/make_exchange_calendar_test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/requirements_lunisolar.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/requirements_minpandas.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/requirements_update_xkrx_holidays.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/update_xkrx_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.690898 exchange_calendars-4.2.6/exchange_calendars/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/always_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24837 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/calendar_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/calendar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/common_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/ecal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108025 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_aixk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_asex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_bvmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_cmes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_iepa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xasx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbkk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xcbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xcse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xdub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xfra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xhel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xhkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xjse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkrx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xnys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xnze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xosl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xpra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xsgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xshg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xsto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xswx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xwar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xwbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/lunisolar_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.690898 exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/korean_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/offsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/precomputed_exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/tase_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/us_futures_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/us_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.690898 exchange_calendars-4.2.6/exchange_calendars/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/weekday_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/xbkk_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/xkls_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34830 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/xkrx_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/xtks_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.690898 exchange_calendars-4.2.6/exchange_calendars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38414 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-09 08:25:16.742903 exchange_calendars-4.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.702899 exchange_calendars-4.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.742903 exchange_calendars-4.2.6/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/24-5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/24-7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   110144 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/aixk.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   496439 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/asex.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   537779 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/bvmf.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/cmes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/iepa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   114134 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   492279 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xams.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   560074 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xasx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   494164 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbkk.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486819 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbog.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   418309 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbom.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   492344 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbru.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   530954 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   499559 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbud.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   498389 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbue.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   547139 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xcbf.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   484804 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xcse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   507099 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xdub.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   552404 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xetr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   551104 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xfra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486559 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xhel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   868914 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xhkg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   145764 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xice.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   500014 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xidx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   502614 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   499819 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xjse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   504889 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xkar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   499299 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xkls.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   793869 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xkrx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   501444 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xlim.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   488119 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xlis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   553509 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xlon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   541224 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xmad.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   503979 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xmex.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   490784 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xmil.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   500079 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xmos.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   541094 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xnys.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   550909 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xnze.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486299 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xosl.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   493059 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xpar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   504694 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xphs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   501184 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xpra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   618964 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xses.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   498714 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xsgo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   855469 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xshg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xsto.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   485129 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xswx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    79204 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xtae.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   548374 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xtai.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   617749 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xtks.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xtse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   500989 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xwar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   500079 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xwbo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_aixk_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_always_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_asex_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_bvmf_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_calendar_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69070 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_calendar_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_cmes_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162253 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_iepa_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_weekday_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xams_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xasx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbkk_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbog_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbom_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbru_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbud_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbue_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xcbf_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xcse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xdub_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xetr_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xfra_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xhel_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xhkg_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xice_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xidx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xist_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xjse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xkar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xkls_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xkrx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xlim_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xlis_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xlon_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xmad_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xmex_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xmil_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xmos_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xnys_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xnze_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xosl_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xpar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xphs_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xpra_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xses_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xsgo_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xshg_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xsto_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xswx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xtae_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xtai_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xtks_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xtse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xwar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xwbo_calendar.py
```

### Comparing `exchange_calendars-4.2.5/.gitignore` & `exchange_calendars-4.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/LICENSE` & `exchange_calendars-4.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/PKG-INFO` & `exchange_calendars-4.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange_calendars
-Version: 4.2.5
+Version: 4.2.6
 Summary: Calendars for securities exchanges
 Author: Gerry Manoim
 Author-email: gerrymanoim@gmail.com
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `exchange_calendars-4.2.5/README.md` & `exchange_calendars-4.2.6/README.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/docs/changes_archive.md` & `exchange_calendars-4.2.6/docs/changes_archive.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/docs/tutorials/calendar_methods.ipynb` & `exchange_calendars-4.2.6/docs/tutorials/calendar_methods.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/docs/tutorials/calendar_properties.ipynb` & `exchange_calendars-4.2.6/docs/tutorials/calendar_properties.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/docs/tutorials/minutes.ipynb` & `exchange_calendars-4.2.6/docs/tutorials/minutes.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/docs/tutorials/sessions.ipynb` & `exchange_calendars-4.2.6/docs/tutorials/sessions.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/docs/tutorials/trading_index.ipynb` & `exchange_calendars-4.2.6/docs/tutorials/trading_index.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/etc/NYSE-Historical-Closings.pdf` & `exchange_calendars-4.2.6/etc/NYSE-Historical-Closings.pdf`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/etc/bench.py` & `exchange_calendars-4.2.6/etc/bench.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/etc/check_holidays.py` & `exchange_calendars-4.2.6/etc/check_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/etc/ecal` & `exchange_calendars-4.2.6/etc/ecal`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/etc/factory_bounds.py` & `exchange_calendars-4.2.6/etc/factory_bounds.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/etc/lunisolar` & `exchange_calendars-4.2.6/etc/lunisolar`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/etc/make_exchange_calendar_test_csv.py` & `exchange_calendars-4.2.6/etc/make_exchange_calendar_test_csv.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/etc/requirements.txt` & `exchange_calendars-4.2.6/etc/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    pip-compile --output-file=etc/requirements.txt pyproject.toml
 #
 korean-lunar-calendar==0.3.1
     # via exchange-calendars (pyproject.toml)
-numpy==1.24.1
+numpy==1.24.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
-pandas==1.5.2
+pandas==2.0.0
     # via exchange-calendars (pyproject.toml)
-pyluach==2.0.2
+pyluach==2.2.0
     # via exchange-calendars (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
-pytz==2022.7
+pytz==2023.3
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
 six==1.16.0
     # via python-dateutil
 toolz==0.12.0
     # via exchange-calendars (pyproject.toml)
+tzdata==2023.3
+    # via pandas
```

### Comparing `exchange_calendars-4.2.5/etc/requirements_dev.txt` & `exchange_calendars-4.2.6/etc/requirements_minpandas.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,93 +1,96 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
-#    pip-compile --extra=dev --output-file=etc/requirements_dev.txt pyproject.toml
+#    pip-compile --extra=dev --output-file=etc/requirements_minpandas.txt pyproject.toml
+#
+# To upgrade with pandas==1.1.0 fixed run:
+#
+#    pip-compile --upgrade --upgrade-package pandas==1.1 --extra=dev --output-file=etc/requirements_minpandas.txt pyproject.toml
 #
 attrs==22.2.0
     # via
     #   hypothesis
     #   pytest
-build==0.9.0
+build==0.10.0
     # via pip-tools
 click==8.1.3
     # via pip-tools
 colorama==0.4.6
     # via
     #   build
     #   click
     #   pytest
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via
     #   hypothesis
     #   pytest
 execnet==1.9.0
     # via pytest-xdist
 flake8==6.0.0
     # via exchange-calendars (pyproject.toml)
-hypothesis==6.61.0
+hypothesis==6.71.0
     # via exchange-calendars (pyproject.toml)
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
 korean-lunar-calendar==0.3.1
     # via exchange-calendars (pyproject.toml)
 mccabe==0.7.0
     # via flake8
-numpy==1.24.1
+numpy==1.24.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
-packaging==22.0
+packaging==23.0
     # via
     #   build
     #   pytest
-pandas==1.5.2
+pandas==1.1.0
     # via exchange-calendars (pyproject.toml)
-pep517==0.13.0
-    # via build
-pip-tools==6.12.1
+pip-tools==6.13.0
     # via exchange-calendars (pyproject.toml)
 pluggy==1.0.0
     # via pytest
 py-cpuinfo==9.0.0
     # via pytest-benchmark
 pycodestyle==2.10.0
     # via flake8
 pyflakes==3.0.1
     # via flake8
-pyluach==2.0.2
+pyluach==2.2.0
     # via exchange-calendars (pyproject.toml)
-pytest==7.2.0
+pyproject-hooks==1.0.0
+    # via build
+pytest==7.2.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pytest-benchmark
     #   pytest-xdist
 pytest-benchmark==4.0.0
     # via exchange-calendars (pyproject.toml)
-pytest-xdist==3.1.0
+pytest-xdist==3.2.1
     # via exchange-calendars (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
-pytz==2022.7
+pytz==2023.3
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
 six==1.16.0
     # via python-dateutil
 sortedcontainers==2.4.0
     # via hypothesis
 tomli==2.0.1
     # via
     #   build
-    #   pep517
     #   pytest
 toolz==0.12.0
     # via exchange-calendars (pyproject.toml)
-wheel==0.38.4
+wheel==0.40.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `exchange_calendars-4.2.5/etc/requirements_minpandas.txt` & `exchange_calendars-4.2.6/etc/requirements_dev.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,94 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
-#    pip-compile --extra=dev --output-file=etc/requirements_minpandas.txt pyproject.toml
-#
-# To upgrade with pandas==1.1.0 fixed run:
-#
-#    pip-compile --upgrade --upgrade-package pandas==1.1 --extra=dev --output-file=etc/requirements_minpandas.txt pyproject.toml
+#    pip-compile --extra=dev --output-file=etc/requirements_dev.txt pyproject.toml
 #
 attrs==22.2.0
     # via
     #   hypothesis
     #   pytest
-build==0.9.0
+build==0.10.0
     # via pip-tools
 click==8.1.3
     # via pip-tools
 colorama==0.4.6
     # via
     #   build
     #   click
     #   pytest
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via
     #   hypothesis
     #   pytest
 execnet==1.9.0
     # via pytest-xdist
 flake8==6.0.0
     # via exchange-calendars (pyproject.toml)
-hypothesis==6.61.0
+hypothesis==6.71.0
     # via exchange-calendars (pyproject.toml)
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
 korean-lunar-calendar==0.3.1
     # via exchange-calendars (pyproject.toml)
 mccabe==0.7.0
     # via flake8
-numpy==1.24.1
+numpy==1.24.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
-packaging==22.0
+packaging==23.0
     # via
     #   build
     #   pytest
-pandas==1.1.0
+pandas==2.0.0
     # via exchange-calendars (pyproject.toml)
-pep517==0.13.0
-    # via build
-pip-tools==6.12.1
+pip-tools==6.13.0
     # via exchange-calendars (pyproject.toml)
 pluggy==1.0.0
     # via pytest
 py-cpuinfo==9.0.0
     # via pytest-benchmark
 pycodestyle==2.10.0
     # via flake8
 pyflakes==3.0.1
     # via flake8
-pyluach==2.0.2
+pyluach==2.2.0
     # via exchange-calendars (pyproject.toml)
-pytest==7.2.0
+pyproject-hooks==1.0.0
+    # via build
+pytest==7.2.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pytest-benchmark
     #   pytest-xdist
 pytest-benchmark==4.0.0
     # via exchange-calendars (pyproject.toml)
-pytest-xdist==3.1.0
+pytest-xdist==3.2.1
     # via exchange-calendars (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
-pytz==2022.7
+pytz==2023.3
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
 six==1.16.0
     # via python-dateutil
 sortedcontainers==2.4.0
     # via hypothesis
 tomli==2.0.1
     # via
     #   build
-    #   pep517
     #   pytest
 toolz==0.12.0
     # via exchange-calendars (pyproject.toml)
-wheel==0.38.4
+tzdata==2023.3
+    # via pandas
+wheel==0.40.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `exchange_calendars-4.2.5/etc/update_xkrx_holidays.py` & `exchange_calendars-4.2.6/etc/update_xkrx_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/__init__.py` & `exchange_calendars-4.2.6/exchange_calendars/__init__.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/calendar_helpers.py` & `exchange_calendars-4.2.6/exchange_calendars/calendar_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,15 +676,15 @@
 
     def trading_index(self) -> pd.DatetimeIndex:
         """Create trading index as a DatetimeIndex."""
         self.verify_non_overlapping()
         index = self._trading_index()
         if self.has_break:
             index.sort()
-        index = pd.DatetimeIndex(index, tz="UTC")
+        index = pd.DatetimeIndex(index, tz=pytz.UTC)
         return self.curtail_for_times(index)
 
     @contextlib.contextmanager
     def _override_defaults(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
         yield
@@ -714,11 +714,11 @@
         overlaps_next = right[:-1] > left[1:]
         if overlaps_next.any():
             if self.curtail_overlaps:
                 right[:-1][overlaps_next] = left[1:][overlaps_next]
             else:
                 raise errors.IntervalsOverlapError()
 
-        left = pd.DatetimeIndex(left, tz="UTC")
-        right = pd.DatetimeIndex(right, tz="UTC")
+        left = pd.DatetimeIndex(left, tz=pytz.UTC)
+        right = pd.DatetimeIndex(right, tz=pytz.UTC)
         index = pd.IntervalIndex.from_arrays(left, right, self.closed)
         return self.curtail_for_times(index)
```

### Comparing `exchange_calendars-4.2.5/exchange_calendars/calendar_utils.py` & `exchange_calendars-4.2.6/exchange_calendars/calendar_utils.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/common_holidays.py` & `exchange_calendars-4.2.6/exchange_calendars/common_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/ecal.py` & `exchange_calendars-4.2.6/exchange_calendars/ecal.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/errors.py` & `exchange_calendars-4.2.6/exchange_calendars/errors.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_aixk.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_aixk.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_asex.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_asex.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_bvmf.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_bvmf.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_cmes.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_cmes.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_iepa.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_iepa.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xams.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xams.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xasx.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xasx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbkk.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbkk.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbog.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbog.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbom.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbom.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbru.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbru.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbse.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbud.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbud.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xbue.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbue.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xcbf.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xcbf.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xcse.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xcse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xdub.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xdub.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xetr.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xetr.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xfra.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xfra.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xhel.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xhel.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xhkg.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xhkg.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xice.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xice.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xidx.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xidx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xist.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xist.py`

 * *Files 8% similar despite different names*

```diff
@@ -147,14 +147,19 @@
             pd.Timestamp("2003-11-21"),  # Terror attacks
             pd.Timestamp("2003-11-24"),  # Eid al Fitr extra holiday
             pd.Timestamp("2003-11-28"),  # Eid al Fitr extra holiday
             pd.Timestamp("2004-01-23"),  # Bad weather
             pd.Timestamp("2004-12-30"),  # Closure for redenomination
             pd.Timestamp("2004-12-31"),  # Closure for redenomination
             pd.Timestamp("2006-01-13"),  # Eid al Adha extra holiday
+            pd.Timestamp("2023-02-08"),  # Trade suspension after earthquake
+            pd.Timestamp("2023-02-09"),  # Trade suspension after earthquake
+            pd.Timestamp("2023-02-10"),  # Trade suspension after earthquake
+            pd.Timestamp("2023-02-13"),  # Trade suspension after earthquake
+            pd.Timestamp("2023-02-14"),  # Trade suspension after earthquake
         ]
 
         return list(
             chain(
                 misc_adhoc,
                 EidAlFitr1,
                 EidAlFitr2,
```

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xjse.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xjse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xkar.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xkls.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkls.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xkrx.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkrx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xlim.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlim.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xlis.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlis.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xlon.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlon.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,16 @@
             pd.Timestamp("2012-06-04"),
             pd.Timestamp("2012-06-05"),
             # Platinum Jubilee (moved Spring bank holiday followed by Jubilee day)
             pd.Timestamp("2022-06-02"),
             pd.Timestamp("2022-06-03"),
             # Queen Elizabeth II Funeral
             pd.Timestamp("2022-09-19"),
+            # Coronation of King Charles III
+            pd.Timestamp("2023-05-08"),
             # Royal Weddings
             # Wedding Day of Princess Anne and Mark Phillips
             pd.Timestamp("1973-11-14"),
             # Wedding Day of Prince Charles and Diana Spencer
             pd.Timestamp("1981-07-29"),
             # Wedding Day of Prince William and Catherine Middleton
             pd.Timestamp("2011-04-29"),
```

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xmad.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmad.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xmex.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmex.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xmil.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmil.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xmos.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmos.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xnys.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xnys.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xnze.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xnze.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xosl.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xosl.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xpar.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xpar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xphs.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xphs.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xpra.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xpra.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xses.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xses.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xsgo.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xsgo.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xshg.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xshg.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,14 +541,16 @@
         "2023-01-23",
         "2023-01-24",
         "2023-01-25",
         "2023-01-26",
         "2023-01-27",
         "2023-04-05",
         "2023-05-01",
+        "2023-05-02",
+        "2023-05-03",
         "2023-06-22",
         "2023-09-29",
         "2023-10-02",
         "2023-10-03",
         "2023-10-04",
         "2023-10-05",
         "2024-01-01",
```

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xsto.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xsto.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xswx.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xswx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xtae.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtae.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     PassoverInterimDay1,
     PassoverInterimDay2,
     PassoverInterimDay3,
     PassoverInterimDay4,
     SukkothInterimDay1,
     SukkothInterimDay2,
     SukkothInterimDay3,
+    SukkothInterimDay4,
+    SukkothInterimDay5,
     Passover2Eve,
     PassoverEve,
     Pentecost,
     PentecostEve,
     Purim,
     SimchatTorah,
     SimchatTorahEve,
@@ -156,14 +158,16 @@
                         PassoverInterimDay1,
                         PassoverInterimDay2,
                         PassoverInterimDay3,
                         PassoverInterimDay4,
                         SukkothInterimDay1,
                         SukkothInterimDay2,
                         SukkothInterimDay3,
+                        SukkothInterimDay4,
+                        SukkothInterimDay5,
                     ]
                 ),
             ),
             (SUNDAY_CLOSE, SUNDAY),
         ]
 
     @property
```

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xtai.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtai.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xtks.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtks.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xtse.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xwar.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xwar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/exchange_calendar_xwbo.py` & `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xwbo.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/lunisolar_holidays.py` & `exchange_calendars-4.2.6/exchange_calendars/lunisolar_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/pandas_extensions/holiday.py` & `exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/pandas_extensions/korean_holiday.py` & `exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/korean_holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/pandas_extensions/offsets.py` & `exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/offsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     def _apply(self, other):
         if isinstance(other, datetime):
             moved = 0
             remaining = self.n - moved
             bday, interval = self._custom_business_day_for(
                 other, remaining, with_interval=True
             )
-            result = bday.apply(other)
+            result = bday + other
             while not interval.left <= result <= interval.right:
                 previous_other = other
                 if result < interval.left:
                     other = interval.left
                 elif result > interval.right:
                     other = interval.right
                 else:
```

### Comparing `exchange_calendars-4.2.5/exchange_calendars/precomputed_exchange_calendar.py` & `exchange_calendars-4.2.6/exchange_calendars/precomputed_exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/tase_holidays.py` & `exchange_calendars-4.2.6/exchange_calendars/tase_holidays.py`

 * *Files 8% similar despite different names*

```diff
@@ -372,14 +372,28 @@
 SukkothInterimDay3 = Holiday(
     "Sukkoth Interim Day",
     month=1,
     day=1,
     offset=[_Sukkoth(), Day(3)],
     days_of_week=(0, 1, 2, 3, 6)
 )
+SukkothInterimDay4 = Holiday(
+    "Sukkoth Interim Day",
+    month=1,
+    day=1,
+    offset=[_Sukkoth(), Day(4)],
+    days_of_week=(0, 1, 2, 3, 6)
+)
+SukkothInterimDay5 = Holiday(
+    "Sukkoth Interim Day",
+    month=1,
+    day=1,
+    offset=[_Sukkoth(), Day(5)],
+    days_of_week=(0, 1, 2, 3, 6)
+)
 
 # Passover interim days are the days between beginning and end of passover. Any otherwise regular business day in that
 # period becomes an early close day.
 PassoverInterimDay1 = Holiday(
     "Passover Interim Day",
     month=1,
     day=1,
```

### Comparing `exchange_calendars-4.2.5/exchange_calendars/us_futures_calendar.py` & `exchange_calendars-4.2.6/exchange_calendars/us_futures_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/us_holidays.py` & `exchange_calendars-4.2.6/exchange_calendars/us_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/utils/pandas_utils.py` & `exchange_calendars-4.2.6/exchange_calendars/utils/pandas_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     >>> ser = pd.Series(arr, index=arr)
     >>> bv = (
     ...     ((ser >= 10) & (ser < 16))
     ...     | ((ser >= 30) & (ser <= 40))
     ...     | ((ser >= 55) & (ser < 61))
     ... )
     >>> longest_run(bv)
-    Int64Index([30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40], dtype='int64')
+    Index([30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40], dtype='int32')
     >>> pd.testing.assert_index_equal(longest_run(bv), ser.index[30:41])
     """
     # group Trues by only adding to sum when value False.
     trues_grouped = (~ser).cumsum()[ser]  # and only take True Values
     group_sizes = trues_grouped.value_counts()  # count each run
     max_run_size = group_sizes.max()
     max_run_group_id = group_sizes[group_sizes == max_run_size].index[0]
```

### Comparing `exchange_calendars-4.2.5/exchange_calendars/xbkk_holidays.py` & `exchange_calendars-4.2.6/exchange_calendars/xbkk_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/xkls_holidays.py` & `exchange_calendars-4.2.6/exchange_calendars/xkls_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/xkrx_holidays.py` & `exchange_calendars-4.2.6/exchange_calendars/xkrx_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars/xtks_holidays.py` & `exchange_calendars-4.2.6/exchange_calendars/xtks_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/exchange_calendars.egg-info/PKG-INFO` & `exchange_calendars-4.2.6/exchange_calendars.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange-calendars
-Version: 4.2.5
+Version: 4.2.6
 Summary: Calendars for securities exchanges
 Author: Gerry Manoim
 Author-email: gerrymanoim@gmail.com
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `exchange_calendars-4.2.5/exchange_calendars.egg-info/SOURCES.txt` & `exchange_calendars-4.2.6/exchange_calendars.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/pyproject.toml` & `exchange_calendars-4.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/setup.cfg` & `exchange_calendars-4.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/24-5.csv` & `exchange_calendars-4.2.6/tests/resources/24-5.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/24-7.csv` & `exchange_calendars-4.2.6/tests/resources/24-7.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/aixk.csv` & `exchange_calendars-4.2.6/tests/resources/aixk.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/asex.csv` & `exchange_calendars-4.2.6/tests/resources/asex.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/bvmf.csv` & `exchange_calendars-4.2.6/tests/resources/bvmf.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/cmes.csv` & `exchange_calendars-4.2.6/tests/resources/cmes.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/iepa.csv` & `exchange_calendars-4.2.6/tests/resources/iepa.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/test.csv` & `exchange_calendars-4.2.6/tests/resources/test.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xams.csv` & `exchange_calendars-4.2.6/tests/resources/xams.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xasx.csv` & `exchange_calendars-4.2.6/tests/resources/xasx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xbkk.csv` & `exchange_calendars-4.2.6/tests/resources/xbkk.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xbog.csv` & `exchange_calendars-4.2.6/tests/resources/xbog.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xbom.csv` & `exchange_calendars-4.2.6/tests/resources/xbom.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xbru.csv` & `exchange_calendars-4.2.6/tests/resources/xbru.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xbse.csv` & `exchange_calendars-4.2.6/tests/resources/xbse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xbud.csv` & `exchange_calendars-4.2.6/tests/resources/xbud.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xbue.csv` & `exchange_calendars-4.2.6/tests/resources/xbue.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xcbf.csv` & `exchange_calendars-4.2.6/tests/resources/xcbf.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xcse.csv` & `exchange_calendars-4.2.6/tests/resources/xcse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xdub.csv` & `exchange_calendars-4.2.6/tests/resources/xdub.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xetr.csv` & `exchange_calendars-4.2.6/tests/resources/xetr.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xfra.csv` & `exchange_calendars-4.2.6/tests/resources/xfra.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xhel.csv` & `exchange_calendars-4.2.6/tests/resources/xhel.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xhkg.csv` & `exchange_calendars-4.2.6/tests/resources/xhkg.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xice.csv` & `exchange_calendars-4.2.6/tests/resources/xice.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xidx.csv` & `exchange_calendars-4.2.6/tests/resources/xidx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xist.csv` & `exchange_calendars-4.2.6/tests/resources/xist.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xjse.csv` & `exchange_calendars-4.2.6/tests/resources/xjse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xkar.csv` & `exchange_calendars-4.2.6/tests/resources/xkar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xkls.csv` & `exchange_calendars-4.2.6/tests/resources/xkls.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xkrx.csv` & `exchange_calendars-4.2.6/tests/resources/xkrx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xlim.csv` & `exchange_calendars-4.2.6/tests/resources/xlim.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xlis.csv` & `exchange_calendars-4.2.6/tests/resources/xlis.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xlon.csv` & `exchange_calendars-4.2.6/tests/resources/xlon.csv`

 * *Files 0% similar despite different names*

```diff
@@ -8421,15 +8421,14 @@
 2023-04-26T00:00:00Z,2023-04-26T07:00:00Z,2023-04-26T15:30:00Z,,
 2023-04-27T00:00:00Z,2023-04-27T07:00:00Z,2023-04-27T15:30:00Z,,
 2023-04-28T00:00:00Z,2023-04-28T07:00:00Z,2023-04-28T15:30:00Z,,
 2023-05-02T00:00:00Z,2023-05-02T07:00:00Z,2023-05-02T15:30:00Z,,
 2023-05-03T00:00:00Z,2023-05-03T07:00:00Z,2023-05-03T15:30:00Z,,
 2023-05-04T00:00:00Z,2023-05-04T07:00:00Z,2023-05-04T15:30:00Z,,
 2023-05-05T00:00:00Z,2023-05-05T07:00:00Z,2023-05-05T15:30:00Z,,
-2023-05-08T00:00:00Z,2023-05-08T07:00:00Z,2023-05-08T15:30:00Z,,
 2023-05-09T00:00:00Z,2023-05-09T07:00:00Z,2023-05-09T15:30:00Z,,
 2023-05-10T00:00:00Z,2023-05-10T07:00:00Z,2023-05-10T15:30:00Z,,
 2023-05-11T00:00:00Z,2023-05-11T07:00:00Z,2023-05-11T15:30:00Z,,
 2023-05-12T00:00:00Z,2023-05-12T07:00:00Z,2023-05-12T15:30:00Z,,
 2023-05-15T00:00:00Z,2023-05-15T07:00:00Z,2023-05-15T15:30:00Z,,
 2023-05-16T00:00:00Z,2023-05-16T07:00:00Z,2023-05-16T15:30:00Z,,
 2023-05-17T00:00:00Z,2023-05-17T07:00:00Z,2023-05-17T15:30:00Z,,
```

### Comparing `exchange_calendars-4.2.5/tests/resources/xmad.csv` & `exchange_calendars-4.2.6/tests/resources/xmad.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xmex.csv` & `exchange_calendars-4.2.6/tests/resources/xmex.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xmil.csv` & `exchange_calendars-4.2.6/tests/resources/xmil.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xmos.csv` & `exchange_calendars-4.2.6/tests/resources/xmos.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xnys.csv` & `exchange_calendars-4.2.6/tests/resources/xnys.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xnze.csv` & `exchange_calendars-4.2.6/tests/resources/xnze.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xosl.csv` & `exchange_calendars-4.2.6/tests/resources/xosl.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xpar.csv` & `exchange_calendars-4.2.6/tests/resources/xpar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xphs.csv` & `exchange_calendars-4.2.6/tests/resources/xphs.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xpra.csv` & `exchange_calendars-4.2.6/tests/resources/xpra.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xses.csv` & `exchange_calendars-4.2.6/tests/resources/xses.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xsgo.csv` & `exchange_calendars-4.2.6/tests/resources/xsgo.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xshg.csv` & `exchange_calendars-4.2.6/tests/resources/xshg.csv`

 * *Files 0% similar despite different names*

```diff
@@ -7913,16 +7913,14 @@
 2023-04-20T00:00:00Z,2023-04-20T01:30:00Z,2023-04-20T07:00:00Z,2023-04-20T03:30:00Z,2023-04-20T05:00:00Z
 2023-04-21T00:00:00Z,2023-04-21T01:30:00Z,2023-04-21T07:00:00Z,2023-04-21T03:30:00Z,2023-04-21T05:00:00Z
 2023-04-24T00:00:00Z,2023-04-24T01:30:00Z,2023-04-24T07:00:00Z,2023-04-24T03:30:00Z,2023-04-24T05:00:00Z
 2023-04-25T00:00:00Z,2023-04-25T01:30:00Z,2023-04-25T07:00:00Z,2023-04-25T03:30:00Z,2023-04-25T05:00:00Z
 2023-04-26T00:00:00Z,2023-04-26T01:30:00Z,2023-04-26T07:00:00Z,2023-04-26T03:30:00Z,2023-04-26T05:00:00Z
 2023-04-27T00:00:00Z,2023-04-27T01:30:00Z,2023-04-27T07:00:00Z,2023-04-27T03:30:00Z,2023-04-27T05:00:00Z
 2023-04-28T00:00:00Z,2023-04-28T01:30:00Z,2023-04-28T07:00:00Z,2023-04-28T03:30:00Z,2023-04-28T05:00:00Z
-2023-05-02T00:00:00Z,2023-05-02T01:30:00Z,2023-05-02T07:00:00Z,2023-05-02T03:30:00Z,2023-05-02T05:00:00Z
-2023-05-03T00:00:00Z,2023-05-03T01:30:00Z,2023-05-03T07:00:00Z,2023-05-03T03:30:00Z,2023-05-03T05:00:00Z
 2023-05-04T00:00:00Z,2023-05-04T01:30:00Z,2023-05-04T07:00:00Z,2023-05-04T03:30:00Z,2023-05-04T05:00:00Z
 2023-05-05T00:00:00Z,2023-05-05T01:30:00Z,2023-05-05T07:00:00Z,2023-05-05T03:30:00Z,2023-05-05T05:00:00Z
 2023-05-08T00:00:00Z,2023-05-08T01:30:00Z,2023-05-08T07:00:00Z,2023-05-08T03:30:00Z,2023-05-08T05:00:00Z
 2023-05-09T00:00:00Z,2023-05-09T01:30:00Z,2023-05-09T07:00:00Z,2023-05-09T03:30:00Z,2023-05-09T05:00:00Z
 2023-05-10T00:00:00Z,2023-05-10T01:30:00Z,2023-05-10T07:00:00Z,2023-05-10T03:30:00Z,2023-05-10T05:00:00Z
 2023-05-11T00:00:00Z,2023-05-11T01:30:00Z,2023-05-11T07:00:00Z,2023-05-11T03:30:00Z,2023-05-11T05:00:00Z
 2023-05-12T00:00:00Z,2023-05-12T01:30:00Z,2023-05-12T07:00:00Z,2023-05-12T03:30:00Z,2023-05-12T05:00:00Z
@@ -8004,7 +8002,147 @@
 2023-08-29T00:00:00Z,2023-08-29T01:30:00Z,2023-08-29T07:00:00Z,2023-08-29T03:30:00Z,2023-08-29T05:00:00Z
 2023-08-30T00:00:00Z,2023-08-30T01:30:00Z,2023-08-30T07:00:00Z,2023-08-30T03:30:00Z,2023-08-30T05:00:00Z
 2023-08-31T00:00:00Z,2023-08-31T01:30:00Z,2023-08-31T07:00:00Z,2023-08-31T03:30:00Z,2023-08-31T05:00:00Z
 2023-09-01T00:00:00Z,2023-09-01T01:30:00Z,2023-09-01T07:00:00Z,2023-09-01T03:30:00Z,2023-09-01T05:00:00Z
 2023-09-04T00:00:00Z,2023-09-04T01:30:00Z,2023-09-04T07:00:00Z,2023-09-04T03:30:00Z,2023-09-04T05:00:00Z
 2023-09-05T00:00:00Z,2023-09-05T01:30:00Z,2023-09-05T07:00:00Z,2023-09-05T03:30:00Z,2023-09-05T05:00:00Z
 2023-09-06T00:00:00Z,2023-09-06T01:30:00Z,2023-09-06T07:00:00Z,2023-09-06T03:30:00Z,2023-09-06T05:00:00Z
+2023-09-07T00:00:00Z,2023-09-07T01:30:00Z,2023-09-07T07:00:00Z,2023-09-07T03:30:00Z,2023-09-07T05:00:00Z
+2023-09-08T00:00:00Z,2023-09-08T01:30:00Z,2023-09-08T07:00:00Z,2023-09-08T03:30:00Z,2023-09-08T05:00:00Z
+2023-09-11T00:00:00Z,2023-09-11T01:30:00Z,2023-09-11T07:00:00Z,2023-09-11T03:30:00Z,2023-09-11T05:00:00Z
+2023-09-12T00:00:00Z,2023-09-12T01:30:00Z,2023-09-12T07:00:00Z,2023-09-12T03:30:00Z,2023-09-12T05:00:00Z
+2023-09-13T00:00:00Z,2023-09-13T01:30:00Z,2023-09-13T07:00:00Z,2023-09-13T03:30:00Z,2023-09-13T05:00:00Z
+2023-09-14T00:00:00Z,2023-09-14T01:30:00Z,2023-09-14T07:00:00Z,2023-09-14T03:30:00Z,2023-09-14T05:00:00Z
+2023-09-15T00:00:00Z,2023-09-15T01:30:00Z,2023-09-15T07:00:00Z,2023-09-15T03:30:00Z,2023-09-15T05:00:00Z
+2023-09-18T00:00:00Z,2023-09-18T01:30:00Z,2023-09-18T07:00:00Z,2023-09-18T03:30:00Z,2023-09-18T05:00:00Z
+2023-09-19T00:00:00Z,2023-09-19T01:30:00Z,2023-09-19T07:00:00Z,2023-09-19T03:30:00Z,2023-09-19T05:00:00Z
+2023-09-20T00:00:00Z,2023-09-20T01:30:00Z,2023-09-20T07:00:00Z,2023-09-20T03:30:00Z,2023-09-20T05:00:00Z
+2023-09-21T00:00:00Z,2023-09-21T01:30:00Z,2023-09-21T07:00:00Z,2023-09-21T03:30:00Z,2023-09-21T05:00:00Z
+2023-09-22T00:00:00Z,2023-09-22T01:30:00Z,2023-09-22T07:00:00Z,2023-09-22T03:30:00Z,2023-09-22T05:00:00Z
+2023-09-25T00:00:00Z,2023-09-25T01:30:00Z,2023-09-25T07:00:00Z,2023-09-25T03:30:00Z,2023-09-25T05:00:00Z
+2023-09-26T00:00:00Z,2023-09-26T01:30:00Z,2023-09-26T07:00:00Z,2023-09-26T03:30:00Z,2023-09-26T05:00:00Z
+2023-09-27T00:00:00Z,2023-09-27T01:30:00Z,2023-09-27T07:00:00Z,2023-09-27T03:30:00Z,2023-09-27T05:00:00Z
+2023-09-28T00:00:00Z,2023-09-28T01:30:00Z,2023-09-28T07:00:00Z,2023-09-28T03:30:00Z,2023-09-28T05:00:00Z
+2023-10-06T00:00:00Z,2023-10-06T01:30:00Z,2023-10-06T07:00:00Z,2023-10-06T03:30:00Z,2023-10-06T05:00:00Z
+2023-10-09T00:00:00Z,2023-10-09T01:30:00Z,2023-10-09T07:00:00Z,2023-10-09T03:30:00Z,2023-10-09T05:00:00Z
+2023-10-10T00:00:00Z,2023-10-10T01:30:00Z,2023-10-10T07:00:00Z,2023-10-10T03:30:00Z,2023-10-10T05:00:00Z
+2023-10-11T00:00:00Z,2023-10-11T01:30:00Z,2023-10-11T07:00:00Z,2023-10-11T03:30:00Z,2023-10-11T05:00:00Z
+2023-10-12T00:00:00Z,2023-10-12T01:30:00Z,2023-10-12T07:00:00Z,2023-10-12T03:30:00Z,2023-10-12T05:00:00Z
+2023-10-13T00:00:00Z,2023-10-13T01:30:00Z,2023-10-13T07:00:00Z,2023-10-13T03:30:00Z,2023-10-13T05:00:00Z
+2023-10-16T00:00:00Z,2023-10-16T01:30:00Z,2023-10-16T07:00:00Z,2023-10-16T03:30:00Z,2023-10-16T05:00:00Z
+2023-10-17T00:00:00Z,2023-10-17T01:30:00Z,2023-10-17T07:00:00Z,2023-10-17T03:30:00Z,2023-10-17T05:00:00Z
+2023-10-18T00:00:00Z,2023-10-18T01:30:00Z,2023-10-18T07:00:00Z,2023-10-18T03:30:00Z,2023-10-18T05:00:00Z
+2023-10-19T00:00:00Z,2023-10-19T01:30:00Z,2023-10-19T07:00:00Z,2023-10-19T03:30:00Z,2023-10-19T05:00:00Z
+2023-10-20T00:00:00Z,2023-10-20T01:30:00Z,2023-10-20T07:00:00Z,2023-10-20T03:30:00Z,2023-10-20T05:00:00Z
+2023-10-23T00:00:00Z,2023-10-23T01:30:00Z,2023-10-23T07:00:00Z,2023-10-23T03:30:00Z,2023-10-23T05:00:00Z
+2023-10-24T00:00:00Z,2023-10-24T01:30:00Z,2023-10-24T07:00:00Z,2023-10-24T03:30:00Z,2023-10-24T05:00:00Z
+2023-10-25T00:00:00Z,2023-10-25T01:30:00Z,2023-10-25T07:00:00Z,2023-10-25T03:30:00Z,2023-10-25T05:00:00Z
+2023-10-26T00:00:00Z,2023-10-26T01:30:00Z,2023-10-26T07:00:00Z,2023-10-26T03:30:00Z,2023-10-26T05:00:00Z
+2023-10-27T00:00:00Z,2023-10-27T01:30:00Z,2023-10-27T07:00:00Z,2023-10-27T03:30:00Z,2023-10-27T05:00:00Z
+2023-10-30T00:00:00Z,2023-10-30T01:30:00Z,2023-10-30T07:00:00Z,2023-10-30T03:30:00Z,2023-10-30T05:00:00Z
+2023-10-31T00:00:00Z,2023-10-31T01:30:00Z,2023-10-31T07:00:00Z,2023-10-31T03:30:00Z,2023-10-31T05:00:00Z
+2023-11-01T00:00:00Z,2023-11-01T01:30:00Z,2023-11-01T07:00:00Z,2023-11-01T03:30:00Z,2023-11-01T05:00:00Z
+2023-11-02T00:00:00Z,2023-11-02T01:30:00Z,2023-11-02T07:00:00Z,2023-11-02T03:30:00Z,2023-11-02T05:00:00Z
+2023-11-03T00:00:00Z,2023-11-03T01:30:00Z,2023-11-03T07:00:00Z,2023-11-03T03:30:00Z,2023-11-03T05:00:00Z
+2023-11-06T00:00:00Z,2023-11-06T01:30:00Z,2023-11-06T07:00:00Z,2023-11-06T03:30:00Z,2023-11-06T05:00:00Z
+2023-11-07T00:00:00Z,2023-11-07T01:30:00Z,2023-11-07T07:00:00Z,2023-11-07T03:30:00Z,2023-11-07T05:00:00Z
+2023-11-08T00:00:00Z,2023-11-08T01:30:00Z,2023-11-08T07:00:00Z,2023-11-08T03:30:00Z,2023-11-08T05:00:00Z
+2023-11-09T00:00:00Z,2023-11-09T01:30:00Z,2023-11-09T07:00:00Z,2023-11-09T03:30:00Z,2023-11-09T05:00:00Z
+2023-11-10T00:00:00Z,2023-11-10T01:30:00Z,2023-11-10T07:00:00Z,2023-11-10T03:30:00Z,2023-11-10T05:00:00Z
+2023-11-13T00:00:00Z,2023-11-13T01:30:00Z,2023-11-13T07:00:00Z,2023-11-13T03:30:00Z,2023-11-13T05:00:00Z
+2023-11-14T00:00:00Z,2023-11-14T01:30:00Z,2023-11-14T07:00:00Z,2023-11-14T03:30:00Z,2023-11-14T05:00:00Z
+2023-11-15T00:00:00Z,2023-11-15T01:30:00Z,2023-11-15T07:00:00Z,2023-11-15T03:30:00Z,2023-11-15T05:00:00Z
+2023-11-16T00:00:00Z,2023-11-16T01:30:00Z,2023-11-16T07:00:00Z,2023-11-16T03:30:00Z,2023-11-16T05:00:00Z
+2023-11-17T00:00:00Z,2023-11-17T01:30:00Z,2023-11-17T07:00:00Z,2023-11-17T03:30:00Z,2023-11-17T05:00:00Z
+2023-11-20T00:00:00Z,2023-11-20T01:30:00Z,2023-11-20T07:00:00Z,2023-11-20T03:30:00Z,2023-11-20T05:00:00Z
+2023-11-21T00:00:00Z,2023-11-21T01:30:00Z,2023-11-21T07:00:00Z,2023-11-21T03:30:00Z,2023-11-21T05:00:00Z
+2023-11-22T00:00:00Z,2023-11-22T01:30:00Z,2023-11-22T07:00:00Z,2023-11-22T03:30:00Z,2023-11-22T05:00:00Z
+2023-11-23T00:00:00Z,2023-11-23T01:30:00Z,2023-11-23T07:00:00Z,2023-11-23T03:30:00Z,2023-11-23T05:00:00Z
+2023-11-24T00:00:00Z,2023-11-24T01:30:00Z,2023-11-24T07:00:00Z,2023-11-24T03:30:00Z,2023-11-24T05:00:00Z
+2023-11-27T00:00:00Z,2023-11-27T01:30:00Z,2023-11-27T07:00:00Z,2023-11-27T03:30:00Z,2023-11-27T05:00:00Z
+2023-11-28T00:00:00Z,2023-11-28T01:30:00Z,2023-11-28T07:00:00Z,2023-11-28T03:30:00Z,2023-11-28T05:00:00Z
+2023-11-29T00:00:00Z,2023-11-29T01:30:00Z,2023-11-29T07:00:00Z,2023-11-29T03:30:00Z,2023-11-29T05:00:00Z
+2023-11-30T00:00:00Z,2023-11-30T01:30:00Z,2023-11-30T07:00:00Z,2023-11-30T03:30:00Z,2023-11-30T05:00:00Z
+2023-12-01T00:00:00Z,2023-12-01T01:30:00Z,2023-12-01T07:00:00Z,2023-12-01T03:30:00Z,2023-12-01T05:00:00Z
+2023-12-04T00:00:00Z,2023-12-04T01:30:00Z,2023-12-04T07:00:00Z,2023-12-04T03:30:00Z,2023-12-04T05:00:00Z
+2023-12-05T00:00:00Z,2023-12-05T01:30:00Z,2023-12-05T07:00:00Z,2023-12-05T03:30:00Z,2023-12-05T05:00:00Z
+2023-12-06T00:00:00Z,2023-12-06T01:30:00Z,2023-12-06T07:00:00Z,2023-12-06T03:30:00Z,2023-12-06T05:00:00Z
+2023-12-07T00:00:00Z,2023-12-07T01:30:00Z,2023-12-07T07:00:00Z,2023-12-07T03:30:00Z,2023-12-07T05:00:00Z
+2023-12-08T00:00:00Z,2023-12-08T01:30:00Z,2023-12-08T07:00:00Z,2023-12-08T03:30:00Z,2023-12-08T05:00:00Z
+2023-12-11T00:00:00Z,2023-12-11T01:30:00Z,2023-12-11T07:00:00Z,2023-12-11T03:30:00Z,2023-12-11T05:00:00Z
+2023-12-12T00:00:00Z,2023-12-12T01:30:00Z,2023-12-12T07:00:00Z,2023-12-12T03:30:00Z,2023-12-12T05:00:00Z
+2023-12-13T00:00:00Z,2023-12-13T01:30:00Z,2023-12-13T07:00:00Z,2023-12-13T03:30:00Z,2023-12-13T05:00:00Z
+2023-12-14T00:00:00Z,2023-12-14T01:30:00Z,2023-12-14T07:00:00Z,2023-12-14T03:30:00Z,2023-12-14T05:00:00Z
+2023-12-15T00:00:00Z,2023-12-15T01:30:00Z,2023-12-15T07:00:00Z,2023-12-15T03:30:00Z,2023-12-15T05:00:00Z
+2023-12-18T00:00:00Z,2023-12-18T01:30:00Z,2023-12-18T07:00:00Z,2023-12-18T03:30:00Z,2023-12-18T05:00:00Z
+2023-12-19T00:00:00Z,2023-12-19T01:30:00Z,2023-12-19T07:00:00Z,2023-12-19T03:30:00Z,2023-12-19T05:00:00Z
+2023-12-20T00:00:00Z,2023-12-20T01:30:00Z,2023-12-20T07:00:00Z,2023-12-20T03:30:00Z,2023-12-20T05:00:00Z
+2023-12-21T00:00:00Z,2023-12-21T01:30:00Z,2023-12-21T07:00:00Z,2023-12-21T03:30:00Z,2023-12-21T05:00:00Z
+2023-12-22T00:00:00Z,2023-12-22T01:30:00Z,2023-12-22T07:00:00Z,2023-12-22T03:30:00Z,2023-12-22T05:00:00Z
+2023-12-25T00:00:00Z,2023-12-25T01:30:00Z,2023-12-25T07:00:00Z,2023-12-25T03:30:00Z,2023-12-25T05:00:00Z
+2023-12-26T00:00:00Z,2023-12-26T01:30:00Z,2023-12-26T07:00:00Z,2023-12-26T03:30:00Z,2023-12-26T05:00:00Z
+2023-12-27T00:00:00Z,2023-12-27T01:30:00Z,2023-12-27T07:00:00Z,2023-12-27T03:30:00Z,2023-12-27T05:00:00Z
+2023-12-28T00:00:00Z,2023-12-28T01:30:00Z,2023-12-28T07:00:00Z,2023-12-28T03:30:00Z,2023-12-28T05:00:00Z
+2023-12-29T00:00:00Z,2023-12-29T01:30:00Z,2023-12-29T07:00:00Z,2023-12-29T03:30:00Z,2023-12-29T05:00:00Z
+2024-01-02T00:00:00Z,2024-01-02T01:30:00Z,2024-01-02T07:00:00Z,2024-01-02T03:30:00Z,2024-01-02T05:00:00Z
+2024-01-03T00:00:00Z,2024-01-03T01:30:00Z,2024-01-03T07:00:00Z,2024-01-03T03:30:00Z,2024-01-03T05:00:00Z
+2024-01-04T00:00:00Z,2024-01-04T01:30:00Z,2024-01-04T07:00:00Z,2024-01-04T03:30:00Z,2024-01-04T05:00:00Z
+2024-01-05T00:00:00Z,2024-01-05T01:30:00Z,2024-01-05T07:00:00Z,2024-01-05T03:30:00Z,2024-01-05T05:00:00Z
+2024-01-08T00:00:00Z,2024-01-08T01:30:00Z,2024-01-08T07:00:00Z,2024-01-08T03:30:00Z,2024-01-08T05:00:00Z
+2024-01-09T00:00:00Z,2024-01-09T01:30:00Z,2024-01-09T07:00:00Z,2024-01-09T03:30:00Z,2024-01-09T05:00:00Z
+2024-01-10T00:00:00Z,2024-01-10T01:30:00Z,2024-01-10T07:00:00Z,2024-01-10T03:30:00Z,2024-01-10T05:00:00Z
+2024-01-11T00:00:00Z,2024-01-11T01:30:00Z,2024-01-11T07:00:00Z,2024-01-11T03:30:00Z,2024-01-11T05:00:00Z
+2024-01-12T00:00:00Z,2024-01-12T01:30:00Z,2024-01-12T07:00:00Z,2024-01-12T03:30:00Z,2024-01-12T05:00:00Z
+2024-01-15T00:00:00Z,2024-01-15T01:30:00Z,2024-01-15T07:00:00Z,2024-01-15T03:30:00Z,2024-01-15T05:00:00Z
+2024-01-16T00:00:00Z,2024-01-16T01:30:00Z,2024-01-16T07:00:00Z,2024-01-16T03:30:00Z,2024-01-16T05:00:00Z
+2024-01-17T00:00:00Z,2024-01-17T01:30:00Z,2024-01-17T07:00:00Z,2024-01-17T03:30:00Z,2024-01-17T05:00:00Z
+2024-01-18T00:00:00Z,2024-01-18T01:30:00Z,2024-01-18T07:00:00Z,2024-01-18T03:30:00Z,2024-01-18T05:00:00Z
+2024-01-19T00:00:00Z,2024-01-19T01:30:00Z,2024-01-19T07:00:00Z,2024-01-19T03:30:00Z,2024-01-19T05:00:00Z
+2024-01-22T00:00:00Z,2024-01-22T01:30:00Z,2024-01-22T07:00:00Z,2024-01-22T03:30:00Z,2024-01-22T05:00:00Z
+2024-01-23T00:00:00Z,2024-01-23T01:30:00Z,2024-01-23T07:00:00Z,2024-01-23T03:30:00Z,2024-01-23T05:00:00Z
+2024-01-24T00:00:00Z,2024-01-24T01:30:00Z,2024-01-24T07:00:00Z,2024-01-24T03:30:00Z,2024-01-24T05:00:00Z
+2024-01-25T00:00:00Z,2024-01-25T01:30:00Z,2024-01-25T07:00:00Z,2024-01-25T03:30:00Z,2024-01-25T05:00:00Z
+2024-01-26T00:00:00Z,2024-01-26T01:30:00Z,2024-01-26T07:00:00Z,2024-01-26T03:30:00Z,2024-01-26T05:00:00Z
+2024-01-29T00:00:00Z,2024-01-29T01:30:00Z,2024-01-29T07:00:00Z,2024-01-29T03:30:00Z,2024-01-29T05:00:00Z
+2024-01-30T00:00:00Z,2024-01-30T01:30:00Z,2024-01-30T07:00:00Z,2024-01-30T03:30:00Z,2024-01-30T05:00:00Z
+2024-01-31T00:00:00Z,2024-01-31T01:30:00Z,2024-01-31T07:00:00Z,2024-01-31T03:30:00Z,2024-01-31T05:00:00Z
+2024-02-01T00:00:00Z,2024-02-01T01:30:00Z,2024-02-01T07:00:00Z,2024-02-01T03:30:00Z,2024-02-01T05:00:00Z
+2024-02-02T00:00:00Z,2024-02-02T01:30:00Z,2024-02-02T07:00:00Z,2024-02-02T03:30:00Z,2024-02-02T05:00:00Z
+2024-02-05T00:00:00Z,2024-02-05T01:30:00Z,2024-02-05T07:00:00Z,2024-02-05T03:30:00Z,2024-02-05T05:00:00Z
+2024-02-06T00:00:00Z,2024-02-06T01:30:00Z,2024-02-06T07:00:00Z,2024-02-06T03:30:00Z,2024-02-06T05:00:00Z
+2024-02-07T00:00:00Z,2024-02-07T01:30:00Z,2024-02-07T07:00:00Z,2024-02-07T03:30:00Z,2024-02-07T05:00:00Z
+2024-02-08T00:00:00Z,2024-02-08T01:30:00Z,2024-02-08T07:00:00Z,2024-02-08T03:30:00Z,2024-02-08T05:00:00Z
+2024-02-09T00:00:00Z,2024-02-09T01:30:00Z,2024-02-09T07:00:00Z,2024-02-09T03:30:00Z,2024-02-09T05:00:00Z
+2024-02-16T00:00:00Z,2024-02-16T01:30:00Z,2024-02-16T07:00:00Z,2024-02-16T03:30:00Z,2024-02-16T05:00:00Z
+2024-02-19T00:00:00Z,2024-02-19T01:30:00Z,2024-02-19T07:00:00Z,2024-02-19T03:30:00Z,2024-02-19T05:00:00Z
+2024-02-20T00:00:00Z,2024-02-20T01:30:00Z,2024-02-20T07:00:00Z,2024-02-20T03:30:00Z,2024-02-20T05:00:00Z
+2024-02-21T00:00:00Z,2024-02-21T01:30:00Z,2024-02-21T07:00:00Z,2024-02-21T03:30:00Z,2024-02-21T05:00:00Z
+2024-02-22T00:00:00Z,2024-02-22T01:30:00Z,2024-02-22T07:00:00Z,2024-02-22T03:30:00Z,2024-02-22T05:00:00Z
+2024-02-23T00:00:00Z,2024-02-23T01:30:00Z,2024-02-23T07:00:00Z,2024-02-23T03:30:00Z,2024-02-23T05:00:00Z
+2024-02-26T00:00:00Z,2024-02-26T01:30:00Z,2024-02-26T07:00:00Z,2024-02-26T03:30:00Z,2024-02-26T05:00:00Z
+2024-02-27T00:00:00Z,2024-02-27T01:30:00Z,2024-02-27T07:00:00Z,2024-02-27T03:30:00Z,2024-02-27T05:00:00Z
+2024-02-28T00:00:00Z,2024-02-28T01:30:00Z,2024-02-28T07:00:00Z,2024-02-28T03:30:00Z,2024-02-28T05:00:00Z
+2024-02-29T00:00:00Z,2024-02-29T01:30:00Z,2024-02-29T07:00:00Z,2024-02-29T03:30:00Z,2024-02-29T05:00:00Z
+2024-03-01T00:00:00Z,2024-03-01T01:30:00Z,2024-03-01T07:00:00Z,2024-03-01T03:30:00Z,2024-03-01T05:00:00Z
+2024-03-04T00:00:00Z,2024-03-04T01:30:00Z,2024-03-04T07:00:00Z,2024-03-04T03:30:00Z,2024-03-04T05:00:00Z
+2024-03-05T00:00:00Z,2024-03-05T01:30:00Z,2024-03-05T07:00:00Z,2024-03-05T03:30:00Z,2024-03-05T05:00:00Z
+2024-03-06T00:00:00Z,2024-03-06T01:30:00Z,2024-03-06T07:00:00Z,2024-03-06T03:30:00Z,2024-03-06T05:00:00Z
+2024-03-07T00:00:00Z,2024-03-07T01:30:00Z,2024-03-07T07:00:00Z,2024-03-07T03:30:00Z,2024-03-07T05:00:00Z
+2024-03-08T00:00:00Z,2024-03-08T01:30:00Z,2024-03-08T07:00:00Z,2024-03-08T03:30:00Z,2024-03-08T05:00:00Z
+2024-03-11T00:00:00Z,2024-03-11T01:30:00Z,2024-03-11T07:00:00Z,2024-03-11T03:30:00Z,2024-03-11T05:00:00Z
+2024-03-12T00:00:00Z,2024-03-12T01:30:00Z,2024-03-12T07:00:00Z,2024-03-12T03:30:00Z,2024-03-12T05:00:00Z
+2024-03-13T00:00:00Z,2024-03-13T01:30:00Z,2024-03-13T07:00:00Z,2024-03-13T03:30:00Z,2024-03-13T05:00:00Z
+2024-03-14T00:00:00Z,2024-03-14T01:30:00Z,2024-03-14T07:00:00Z,2024-03-14T03:30:00Z,2024-03-14T05:00:00Z
+2024-03-15T00:00:00Z,2024-03-15T01:30:00Z,2024-03-15T07:00:00Z,2024-03-15T03:30:00Z,2024-03-15T05:00:00Z
+2024-03-18T00:00:00Z,2024-03-18T01:30:00Z,2024-03-18T07:00:00Z,2024-03-18T03:30:00Z,2024-03-18T05:00:00Z
+2024-03-19T00:00:00Z,2024-03-19T01:30:00Z,2024-03-19T07:00:00Z,2024-03-19T03:30:00Z,2024-03-19T05:00:00Z
+2024-03-20T00:00:00Z,2024-03-20T01:30:00Z,2024-03-20T07:00:00Z,2024-03-20T03:30:00Z,2024-03-20T05:00:00Z
+2024-03-21T00:00:00Z,2024-03-21T01:30:00Z,2024-03-21T07:00:00Z,2024-03-21T03:30:00Z,2024-03-21T05:00:00Z
+2024-03-22T00:00:00Z,2024-03-22T01:30:00Z,2024-03-22T07:00:00Z,2024-03-22T03:30:00Z,2024-03-22T05:00:00Z
+2024-03-25T00:00:00Z,2024-03-25T01:30:00Z,2024-03-25T07:00:00Z,2024-03-25T03:30:00Z,2024-03-25T05:00:00Z
+2024-03-26T00:00:00Z,2024-03-26T01:30:00Z,2024-03-26T07:00:00Z,2024-03-26T03:30:00Z,2024-03-26T05:00:00Z
+2024-03-27T00:00:00Z,2024-03-27T01:30:00Z,2024-03-27T07:00:00Z,2024-03-27T03:30:00Z,2024-03-27T05:00:00Z
+2024-03-28T00:00:00Z,2024-03-28T01:30:00Z,2024-03-28T07:00:00Z,2024-03-28T03:30:00Z,2024-03-28T05:00:00Z
+2024-03-29T00:00:00Z,2024-03-29T01:30:00Z,2024-03-29T07:00:00Z,2024-03-29T03:30:00Z,2024-03-29T05:00:00Z
+2024-04-01T00:00:00Z,2024-04-01T01:30:00Z,2024-04-01T07:00:00Z,2024-04-01T03:30:00Z,2024-04-01T05:00:00Z
+2024-04-02T00:00:00Z,2024-04-02T01:30:00Z,2024-04-02T07:00:00Z,2024-04-02T03:30:00Z,2024-04-02T05:00:00Z
+2024-04-03T00:00:00Z,2024-04-03T01:30:00Z,2024-04-03T07:00:00Z,2024-04-03T03:30:00Z,2024-04-03T05:00:00Z
```

### Comparing `exchange_calendars-4.2.5/tests/resources/xsto.csv` & `exchange_calendars-4.2.6/tests/resources/xsto.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xswx.csv` & `exchange_calendars-4.2.6/tests/resources/xswx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xtae.csv` & `exchange_calendars-4.2.6/tests/resources/xtae.csv`

 * *Files 0% similar despite different names*

```diff
@@ -426,16 +426,16 @@
 2020-09-24T00:00:00Z,2020-09-24T06:59:00Z,2020-09-24T14:15:00Z,,
 2020-09-29T00:00:00Z,2020-09-29T06:59:00Z,2020-09-29T14:15:00Z,,
 2020-09-30T00:00:00Z,2020-09-30T06:59:00Z,2020-09-30T14:15:00Z,,
 2020-10-01T00:00:00Z,2020-10-01T06:59:00Z,2020-10-01T14:15:00Z,,
 2020-10-04T00:00:00Z,2020-10-04T06:59:00Z,2020-10-04T11:15:00Z,,
 2020-10-05T00:00:00Z,2020-10-05T06:59:00Z,2020-10-05T11:15:00Z,,
 2020-10-06T00:00:00Z,2020-10-06T06:59:00Z,2020-10-06T11:15:00Z,,
-2020-10-07T00:00:00Z,2020-10-07T06:59:00Z,2020-10-07T14:15:00Z,,
-2020-10-08T00:00:00Z,2020-10-08T06:59:00Z,2020-10-08T14:15:00Z,,
+2020-10-07T00:00:00Z,2020-10-07T06:59:00Z,2020-10-07T11:15:00Z,,
+2020-10-08T00:00:00Z,2020-10-08T06:59:00Z,2020-10-08T11:15:00Z,,
 2020-10-11T00:00:00Z,2020-10-11T06:59:00Z,2020-10-11T12:40:00Z,,
 2020-10-12T00:00:00Z,2020-10-12T06:59:00Z,2020-10-12T14:15:00Z,,
 2020-10-13T00:00:00Z,2020-10-13T06:59:00Z,2020-10-13T14:15:00Z,,
 2020-10-14T00:00:00Z,2020-10-14T06:59:00Z,2020-10-14T14:15:00Z,,
 2020-10-15T00:00:00Z,2020-10-15T06:59:00Z,2020-10-15T14:15:00Z,,
 2020-10-18T00:00:00Z,2020-10-18T06:59:00Z,2020-10-18T12:40:00Z,,
 2020-10-19T00:00:00Z,2020-10-19T06:59:00Z,2020-10-19T14:15:00Z,,
@@ -664,15 +664,15 @@
 2021-09-09T00:00:00Z,2021-09-09T06:59:00Z,2021-09-09T14:15:00Z,,
 2021-09-12T00:00:00Z,2021-09-12T06:59:00Z,2021-09-12T12:40:00Z,,
 2021-09-13T00:00:00Z,2021-09-13T06:59:00Z,2021-09-13T14:15:00Z,,
 2021-09-14T00:00:00Z,2021-09-14T06:59:00Z,2021-09-14T14:15:00Z,,
 2021-09-19T00:00:00Z,2021-09-19T06:59:00Z,2021-09-19T12:40:00Z,,
 2021-09-22T00:00:00Z,2021-09-22T06:59:00Z,2021-09-22T11:15:00Z,,
 2021-09-23T00:00:00Z,2021-09-23T06:59:00Z,2021-09-23T11:15:00Z,,
-2021-09-26T00:00:00Z,2021-09-26T06:59:00Z,2021-09-26T12:40:00Z,,
+2021-09-26T00:00:00Z,2021-09-26T06:59:00Z,2021-09-26T11:15:00Z,,
 2021-09-29T00:00:00Z,2021-09-29T06:59:00Z,2021-09-29T14:15:00Z,,
 2021-09-30T00:00:00Z,2021-09-30T06:59:00Z,2021-09-30T14:15:00Z,,
 2021-10-03T00:00:00Z,2021-10-03T06:59:00Z,2021-10-03T12:40:00Z,,
 2021-10-04T00:00:00Z,2021-10-04T06:59:00Z,2021-10-04T14:15:00Z,,
 2021-10-05T00:00:00Z,2021-10-05T06:59:00Z,2021-10-05T14:15:00Z,,
 2021-10-06T00:00:00Z,2021-10-06T06:59:00Z,2021-10-06T14:15:00Z,,
 2021-10-07T00:00:00Z,2021-10-07T06:59:00Z,2021-10-07T14:15:00Z,,
@@ -1162,16 +1162,16 @@
 2023-09-21T00:00:00Z,2023-09-21T06:59:00Z,2023-09-21T14:15:00Z,,
 2023-09-26T00:00:00Z,2023-09-26T06:59:00Z,2023-09-26T14:15:00Z,,
 2023-09-27T00:00:00Z,2023-09-27T06:59:00Z,2023-09-27T14:15:00Z,,
 2023-09-28T00:00:00Z,2023-09-28T06:59:00Z,2023-09-28T14:15:00Z,,
 2023-10-01T00:00:00Z,2023-10-01T06:59:00Z,2023-10-01T11:15:00Z,,
 2023-10-02T00:00:00Z,2023-10-02T06:59:00Z,2023-10-02T11:15:00Z,,
 2023-10-03T00:00:00Z,2023-10-03T06:59:00Z,2023-10-03T11:15:00Z,,
-2023-10-04T00:00:00Z,2023-10-04T06:59:00Z,2023-10-04T14:15:00Z,,
-2023-10-05T00:00:00Z,2023-10-05T06:59:00Z,2023-10-05T14:15:00Z,,
+2023-10-04T00:00:00Z,2023-10-04T06:59:00Z,2023-10-04T11:15:00Z,,
+2023-10-05T00:00:00Z,2023-10-05T06:59:00Z,2023-10-05T11:15:00Z,,
 2023-10-08T00:00:00Z,2023-10-08T06:59:00Z,2023-10-08T12:40:00Z,,
 2023-10-09T00:00:00Z,2023-10-09T06:59:00Z,2023-10-09T14:15:00Z,,
 2023-10-10T00:00:00Z,2023-10-10T06:59:00Z,2023-10-10T14:15:00Z,,
 2023-10-11T00:00:00Z,2023-10-11T06:59:00Z,2023-10-11T14:15:00Z,,
 2023-10-12T00:00:00Z,2023-10-12T06:59:00Z,2023-10-12T14:15:00Z,,
 2023-10-15T00:00:00Z,2023-10-15T06:59:00Z,2023-10-15T12:40:00Z,,
 2023-10-16T00:00:00Z,2023-10-16T06:59:00Z,2023-10-16T14:15:00Z,,
```

### Comparing `exchange_calendars-4.2.5/tests/resources/xtai.csv` & `exchange_calendars-4.2.6/tests/resources/xtai.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xtks.csv` & `exchange_calendars-4.2.6/tests/resources/xtks.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xtse.csv` & `exchange_calendars-4.2.6/tests/resources/xtse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xwar.csv` & `exchange_calendars-4.2.6/tests/resources/xwar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/resources/xwbo.csv` & `exchange_calendars-4.2.6/tests/resources/xwbo.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_aixk_calendar.py` & `exchange_calendars-4.2.6/tests/test_aixk_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_always_open.py` & `exchange_calendars-4.2.6/tests/test_always_open.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_asex_calendar.py` & `exchange_calendars-4.2.6/tests/test_asex_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_bvmf_calendar.py` & `exchange_calendars-4.2.6/tests/test_bvmf_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_calendar_dispatcher.py` & `exchange_calendars-4.2.6/tests/test_calendar_dispatcher.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_calendar_helpers.py` & `exchange_calendars-4.2.6/tests/test_calendar_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -635,15 +635,15 @@
             upper_bounds = pd.concat((am_upper, pm_upper, day_upper))
 
         else:
             lower_bounds, upper_bounds = bounds(opens, closes, force_close, align)
 
         if curtail and not (force_close and force_break_close):
             indices = lower_bounds.argsort()
-            lower_bounds.sort_values(inplace=True)
+            lower_bounds = lower_bounds.sort_values()
             upper_bounds = upper_bounds[indices]
             curtail_mask = upper_bounds > lower_bounds.shift(-1)
             if curtail_mask.any():
                 upper_bounds[curtail_mask] = lower_bounds.shift(-1)[curtail_mask]
 
         return lower_bounds, upper_bounds
```

### Comparing `exchange_calendars-4.2.5/tests/test_cmes_calendar.py` & `exchange_calendars-4.2.6/tests/test_cmes_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_exchange_calendar.py` & `exchange_calendars-4.2.6/tests/test_exchange_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
+import datetime
 import functools
 import itertools
 import pathlib
 import re
 import typing
 from typing import Literal
 from collections import abc
@@ -177,23 +178,24 @@
     filename = name.replace("/", "-").lower() + ".csv"
     path = pathlib.Path(__file__).parent.joinpath("resources", filename)
 
     df = pd.read_csv(
         path,
         index_col=0,
         parse_dates=[0, 1, 2, 3, 4],
-        infer_datetime_format=True,
     )
     # Necessary for csv saved prior to v4.0
     if df.index.tz is not None:
         df.index = df.index.tz_convert(None)
     # Necessary for csv saved prior to v4.0
     for col in df:
         if df[col].dt.tz is None:
             df[col] = df[col].dt.tz_localize(UTC)
+        elif df[col].dt.tz is datetime.timezone.utc:
+            df[col] = df[col].dt.tz_convert(UTC)
     return df
 
 
 class Answers:
     """Inputs and expected output for testing a given calendar and side.
 
     Inputs and expected outputs are provided by public instance methods and
@@ -2142,15 +2144,15 @@
         d = dict(cal.open_times)
         d[pd.Timestamp.min] = d.pop(None)
         s = pd.Series(d).sort_index(ascending=False)
 
         date_to = pd.Timestamp.max
         dtis: list[pd.DatetimeIndex] = []
         # For each period over which a distinct open time prevails...
-        for date_from, time_ in s.iteritems():
+        for date_from, time_ in s.items():
             opens = ans.opens[date_from:date_to]
             sessions = opens.index
             td = pd.Timedelta(hours=time_.hour, minutes=time_.minute)
             # Evaluate session opens as if were all normal open time.
             normal_opens = sessions + pd.Timedelta(cal.open_offset, "D") + td
             normal_opens_utc = normal_opens.tz_localize(cal.tz).tz_convert(UTC)
             # Append those sessions with opens (according to answers) later than
@@ -2182,15 +2184,15 @@
 
         d = dict(cal.close_times)
         d[pd.Timestamp.min] = d.pop(None)
         s = pd.Series(d).sort_index(ascending=False)
 
         date_to = pd.Timestamp.max
         dtis: list[pd.DatetimeIndex] = []
-        for date_from, time_ in s.iteritems():
+        for date_from, time_ in s.items():
             closes = ans.closes[date_from:date_to]  # index to tz-naive
             sessions = closes.index
             td = pd.Timedelta(hours=time_.hour, minutes=time_.minute)
             normal_closes = sessions + pd.Timedelta(cal.close_offset, "D") + td
             normal_closes_utc = normal_closes.tz_localize(cal.tz).tz_convert(UTC)
             dtis.append(sessions[closes < normal_closes_utc])
             if date_from != pd.Timestamp.min:
@@ -3833,22 +3835,26 @@
                     for i, index in enumerate(indexes):
                         # Create closed 'both' trading index for each session/subsession
                         if i == 0 and len(indexes) == 2:
                             ends = ans.break_starts
                         else:
                             ends = ans.closes
                         # index for a 'left' calendar, add end so evaluated as if 'both'
-                        index = index.append(pd.DatetimeIndex([ends[session]]))
+                        index = index.append(
+                            pd.DatetimeIndex([ends[session]], tz=pytz.UTC)
+                        )
 
                         index = index[::mins]  # only want every period
                         if not index[-1] == ends[session]:
                             # if period doesn't coincide with end, add right side of
                             # last interval which lies beyond end.
                             last_indice = index[-1] + period
-                            index = index.append(pd.DatetimeIndex([last_indice]))
+                            index = index.append(
+                                pd.DatetimeIndex([last_indice], tz=pytz.UTC)
+                            )
                         dtis.append(index)
 
                 both_index = unite(dtis)
                 left_index = unite([dti[:-1] for dti in dtis])
                 right_index = unite([dti[1:] for dti in dtis])
                 neither_index = unite([dti[1:-1] for dti in dtis])
```

### Comparing `exchange_calendars-4.2.5/tests/test_iepa_calendar.py` & `exchange_calendars-4.2.6/tests/test_iepa_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_weekday_calendar.py` & `exchange_calendars-4.2.6/tests/test_weekday_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xams_calendar.py` & `exchange_calendars-4.2.6/tests/test_xams_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xasx_calendar.py` & `exchange_calendars-4.2.6/tests/test_xasx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xbkk_calendar.py` & `exchange_calendars-4.2.6/tests/test_xbkk_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xbog_calendar.py` & `exchange_calendars-4.2.6/tests/test_xbog_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xbom_calendar.py` & `exchange_calendars-4.2.6/tests/test_xbom_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xbru_calendar.py` & `exchange_calendars-4.2.6/tests/test_xbru_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xbse_calendar.py` & `exchange_calendars-4.2.6/tests/test_xbse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xbud_calendar.py` & `exchange_calendars-4.2.6/tests/test_xbud_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xbue_calendar.py` & `exchange_calendars-4.2.6/tests/test_xbue_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xcbf_calendar.py` & `exchange_calendars-4.2.6/tests/test_xcbf_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xcse_calendar.py` & `exchange_calendars-4.2.6/tests/test_xcse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xdub_calendar.py` & `exchange_calendars-4.2.6/tests/test_xdub_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xetr_calendar.py` & `exchange_calendars-4.2.6/tests/test_xetr_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xfra_calendar.py` & `exchange_calendars-4.2.6/tests/test_xfra_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xhel_calendar.py` & `exchange_calendars-4.2.6/tests/test_xhel_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xhkg_calendar.py` & `exchange_calendars-4.2.6/tests/test_xhkg_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xice_calendar.py` & `exchange_calendars-4.2.6/tests/test_xice_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xidx_calendar.py` & `exchange_calendars-4.2.6/tests/test_xidx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xist_calendar.py` & `exchange_calendars-4.2.6/tests/test_xist_calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,19 @@
             "2004-12-30",  # Closure for redenomination
             "2004-12-31",  # Closure for redenomination
             # Eid al Adha and Eid al Fitr extra closures
             "2003-02-14",  # Eid al Adha extra holiday
             "2003-11-24",  # Eid al Fitr extra holiday
             "2003-11-28",  # Eid al Fitr extra holiday
             "2006-01-13",  # Eid al Adha extra holiday
+            "2023-02-08",  # Trade suspension after earthquake
+            "2023-02-09",  # Trade suspension after earthquake
+            "2023-02-10",  # Trade suspension after earthquake
+            "2023-02-13",  # Trade suspension after earthquake
+            "2023-02-14",  # Trade suspension after earthquake
         ]
 
     @pytest.fixture
     def non_holidays_sample(self):
         yield [
             # Holidays that fall on a weekend are not made up. Ensure surrounding
             # days are not holidays.
```

### Comparing `exchange_calendars-4.2.5/tests/test_xjse_calendar.py` & `exchange_calendars-4.2.6/tests/test_xjse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xkar_calendar.py` & `exchange_calendars-4.2.6/tests/test_xkar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xkls_calendar.py` & `exchange_calendars-4.2.6/tests/test_xkls_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xkrx_calendar.py` & `exchange_calendars-4.2.6/tests/test_xkrx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xlim_calendar.py` & `exchange_calendars-4.2.6/tests/test_xlim_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xlis_calendar.py` & `exchange_calendars-4.2.6/tests/test_xlis_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xlon_calendar.py` & `exchange_calendars-4.2.6/tests/test_xlon_calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             "2002-06-03",  # Spring Bank 2002
             "2002-06-04",  # Golden Jubilee
             "2011-04-29",  # Royal Wedding
             "2012-06-04",  # Spring Bank 2012
             "2012-06-05",  # Diamond Jubilee
             "2020-05-08",  # VE Day
             "2022-09-19",  # Queen Elizabeth Funeral
+            "2023-05-08",  # Coronation of King Charles III
         ]
 
     @pytest.fixture
     def non_holidays_sample(self):
         # May Bank Holiday was instead observed on VE Day in 2020.
         yield ["2020-05-04"]
```

### Comparing `exchange_calendars-4.2.5/tests/test_xmad_calendar.py` & `exchange_calendars-4.2.6/tests/test_xmad_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xmex_calendar.py` & `exchange_calendars-4.2.6/tests/test_xmex_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xmil_calendar.py` & `exchange_calendars-4.2.6/tests/test_xmil_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xmos_calendar.py` & `exchange_calendars-4.2.6/tests/test_xmos_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xnys_calendar.py` & `exchange_calendars-4.2.6/tests/test_xnys_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xnze_calendar.py` & `exchange_calendars-4.2.6/tests/test_xnze_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xosl_calendar.py` & `exchange_calendars-4.2.6/tests/test_xosl_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xpar_calendar.py` & `exchange_calendars-4.2.6/tests/test_xpar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xphs_calendar.py` & `exchange_calendars-4.2.6/tests/test_xphs_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xpra_calendar.py` & `exchange_calendars-4.2.6/tests/test_xpra_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xses_calendar.py` & `exchange_calendars-4.2.6/tests/test_xses_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xsgo_calendar.py` & `exchange_calendars-4.2.6/tests/test_xsgo_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xshg_calendar.py` & `exchange_calendars-4.2.6/tests/test_xshg_calendar.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,8 +48,11 @@
             "2020-01-31",
 
             # 2022
             "2022-01-31",
             "2022-09-12",
             "2022-10-06",
             "2022-10-07",
+
+            # 2023
+            "2023-05-03",  # Part of Chinese Labor Day 2023
         ]
```

### Comparing `exchange_calendars-4.2.5/tests/test_xsto_calendar.py` & `exchange_calendars-4.2.6/tests/test_xsto_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xswx_calendar.py` & `exchange_calendars-4.2.6/tests/test_xswx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xtae_calendar.py` & `exchange_calendars-4.2.6/tests/test_xtae_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xtai_calendar.py` & `exchange_calendars-4.2.6/tests/test_xtai_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xtks_calendar.py` & `exchange_calendars-4.2.6/tests/test_xtks_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xtse_calendar.py` & `exchange_calendars-4.2.6/tests/test_xtse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xwar_calendar.py` & `exchange_calendars-4.2.6/tests/test_xwar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.5/tests/test_xwbo_calendar.py` & `exchange_calendars-4.2.6/tests/test_xwbo_calendar.py`

 * *Files identical despite different names*

