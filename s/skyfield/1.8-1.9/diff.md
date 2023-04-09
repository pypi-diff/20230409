# Comparing `tmp/skyfield-1.8.tar.gz` & `tmp/skyfield-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skyfield-1.8.tar", last modified: Wed Sep 12 23:27:20 2018, max compression
+gzip compressed data, was "dist/skyfield-1.9.tar", last modified: Sun Sep 23 21:08:16 2018, max compression
```

## Comparing `skyfield-1.8.tar` & `skyfield-1.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-12 23:27:20.000000 skyfield-1.8/
--rw-r-----   0 brandon   (1000) brandon   (1000)     2589 2018-09-12 23:27:20.000000 skyfield-1.8/PKG-INFO
--rw-r-----   0 brandon   (1000) brandon   (1000)     1101 2018-07-27 03:57:12.000000 skyfield-1.8/LICENSE
--rw-r-----   0 brandon   (1000) brandon   (1000)     1286 2018-01-19 12:43:35.000000 skyfield-1.8/README.rst
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-12 23:27:20.000000 skyfield-1.8/skyfield/
--rw-r-----   0 brandon   (1000) brandon   (1000)    31350 2018-09-11 10:06:27.000000 skyfield-1.8/skyfield/timelib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    20928 2018-09-10 01:25:57.000000 skyfield-1.8/skyfield/positionlib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     8891 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/vectorlib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     2145 2017-01-14 17:47:33.000000 skyfield-1.8/skyfield/precessionlib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      793 2017-01-14 17:47:33.000000 skyfield-1.8/skyfield/framelib.py
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-12 23:27:20.000000 skyfield-1.8/skyfield/tests/
--rw-r-----   0 brandon   (1000) brandon   (1000)     2394 2018-03-03 12:52:10.000000 skyfield-1.8/skyfield/tests/test_strs_and_reprs.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     4928 2018-07-27 03:38:46.000000 skyfield-1.8/skyfield/tests/test_against_horizons.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     1854 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/tests/test_units.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      423 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/tests/fixes.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     1588 2018-09-12 10:28:43.000000 skyfield-1.8/skyfield/tests/test_almanac.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    11745 2018-09-09 16:30:51.000000 skyfield-1.8/skyfield/tests/test_timelib.py
--rw-r--r--   0 brandon   (1000) brandon   (1000)    25603 2018-07-27 02:54:52.000000 skyfield-1.8/skyfield/tests/test_elementslib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     4673 2018-07-27 02:18:42.000000 skyfield-1.8/skyfield/tests/test_earth_satellites.py
--rw-r-----   0 brandon   (1000) brandon   (1000)   140843 2018-09-09 21:04:49.000000 skyfield-1.8/skyfield/tests/test_against_novas.py
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-12 23:27:20.000000 skyfield-1.8/skyfield/tests/data/
--rw-r-----   0 brandon   (1000) brandon   (1000)     9376 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/tests/data/de430-2015-03-02.bsp
--rw-r-----   0 brandon   (1000) brandon   (1000)    27840 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/tests/data/jup310-2053-10-08.bsp
--rw-r-----   0 brandon   (1000) brandon   (1000)    27024 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/tests/data/jup310-2015-03-02.bsp
--rw-r-----   0 brandon   (1000) brandon   (1000)     1520 2018-02-11 22:13:41.000000 skyfield-1.8/skyfield/tests/test_earth_deflection.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      793 2017-01-14 17:47:33.000000 skyfield-1.8/skyfield/tests/test_functions.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     3657 2018-09-05 21:26:57.000000 skyfield-1.8/skyfield/tests/test_positions.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      714 2018-09-03 14:12:25.000000 skyfield-1.8/skyfield/tests/test_topos.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     3611 2018-07-27 02:18:42.000000 skyfield-1.8/skyfield/tests/test_api.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     2004 2018-05-28 20:48:59.000000 skyfield-1.8/skyfield/tests/test_vectors.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     1309 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/tests/deprecations.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     2724 2018-08-05 21:16:05.000000 skyfield-1.8/skyfield/tests/test_io.py
--rw-r-----   0 brandon   (1000) brandon   (1000)        0 2017-01-14 17:47:33.000000 skyfield-1.8/skyfield/tests/__init__.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     3454 2018-09-04 10:17:26.000000 skyfield-1.8/skyfield/tests/test_io_parsing.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     2157 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/tests/test_angles.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      680 2018-09-03 20:56:52.000000 skyfield-1.8/skyfield/constants.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     1476 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/errors.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     7542 2018-07-28 19:08:55.000000 skyfield-1.8/skyfield/charting.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     7547 2018-07-27 02:18:42.000000 skyfield-1.8/skyfield/sgp4lib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      430 2018-05-14 23:52:00.000000 skyfield-1.8/skyfield/descriptorlib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     2230 2018-07-27 02:18:42.000000 skyfield-1.8/skyfield/projections.py
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-12 23:27:20.000000 skyfield-1.8/skyfield/data/
--rw-r-----   0 brandon   (1000) brandon   (1000)    10576 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/data/historic_deltat.npy
--rw-r-----   0 brandon   (1000) brandon   (1000)    15728 2018-09-09 19:32:18.000000 skyfield-1.8/skyfield/data/nutation.npz
--rw-r-----   0 brandon   (1000) brandon   (1000)     1342 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/data/earth_orientation.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      528 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/data/morrison_stephenson_deltat.npy
--rw-r-----   0 brandon   (1000) brandon   (1000)     4682 2017-01-14 17:47:33.000000 skyfield-1.8/skyfield/data/spice.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     2793 2018-09-04 00:17:03.000000 skyfield-1.8/skyfield/data/hipparcos.py
--rw-r--r--   0 brandon   (1000) brandon   (1000)     2453 2018-07-27 02:54:52.000000 skyfield-1.8/skyfield/data/gravitational_parameters.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      706 2017-01-14 17:47:33.000000 skyfield-1.8/skyfield/data/horizons.py
--rw-r-----   0 brandon   (1000) brandon   (1000)       72 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/data/__init__.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     3515 2018-09-09 19:32:18.000000 skyfield-1.8/skyfield/functions.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     6566 2018-09-04 01:00:47.000000 skyfield-1.8/skyfield/starlib.py
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-12 23:27:20.000000 skyfield-1.8/skyfield/documentation/
--rw-r-----   0 brandon   (1000) brandon   (1000)      884 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/documentation/api-units.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)      529 2018-02-03 16:25:00.000000 skyfield-1.8/skyfield/documentation/api-ephemeris.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)      309 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/documentation/api-stars.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     2375 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/documentation/installation.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)      553 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/documentation/api-iokit.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     7682 2018-09-12 10:34:32.000000 skyfield-1.8/skyfield/documentation/api.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     6965 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/documentation/planets.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)      319 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/documentation/api-satellites.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     4739 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/documentation/bibliography.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     2604 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/documentation/astropy.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)      539 2018-09-12 10:42:33.000000 skyfield-1.8/skyfield/documentation/toc.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     2858 2018-07-27 02:54:52.000000 skyfield-1.8/skyfield/documentation/index.rst
--rw-r--r--   0 brandon   (1000) brandon   (1000)     3495 2018-07-27 02:54:52.000000 skyfield-1.8/skyfield/documentation/elements.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     3639 2018-09-12 10:31:42.000000 skyfield-1.8/skyfield/documentation/almanac.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)      238 2018-09-04 10:13:06.000000 skyfield-1.8/skyfield/documentation/api-elements.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)    25465 2018-09-05 21:26:57.000000 skyfield-1.8/skyfield/documentation/time.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     1987 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/documentation/api-vectors.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)    13625 2018-07-27 02:18:42.000000 skyfield-1.8/skyfield/documentation/earth-satellites.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)    10074 2018-09-05 21:44:23.000000 skyfield-1.8/skyfield/documentation/stars.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     1727 2018-07-27 02:18:42.000000 skyfield-1.8/skyfield/documentation/api-position.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     8041 2018-09-03 18:43:15.000000 skyfield-1.8/skyfield/documentation/design.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)      414 2018-09-12 10:42:06.000000 skyfield-1.8/skyfield/documentation/api-almanac.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     5379 2018-07-27 03:12:25.000000 skyfield-1.8/skyfield/documentation/files.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)    19643 2018-07-27 02:54:52.000000 skyfield-1.8/skyfield/documentation/positions.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)      195 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/documentation/api-topos.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     1537 2018-07-09 03:09:24.000000 skyfield-1.8/skyfield/documentation/api-time.rst
--rw-r-----   0 brandon   (1000) brandon   (1000)     4233 2018-07-09 03:09:24.000000 skyfield-1.8/skyfield/api.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    11360 2018-09-09 22:09:51.000000 skyfield-1.8/skyfield/nutationlib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     6320 2018-01-19 12:43:35.000000 skyfield-1.8/skyfield/relativity.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     8982 2018-05-14 23:41:29.000000 skyfield-1.8/skyfield/jpllib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     3598 2018-04-15 22:11:09.000000 skyfield-1.8/skyfield/toposlib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     6543 2018-09-12 10:57:03.000000 skyfield-1.8/skyfield/almanac.py
--rw-r--r--   0 brandon   (1000) brandon   (1000)    13427 2018-09-04 10:14:06.000000 skyfield-1.8/skyfield/elementslib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     2756 2018-09-04 02:08:43.000000 skyfield-1.8/skyfield/named_stars.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     6104 2018-09-03 14:14:15.000000 skyfield-1.8/skyfield/earthlib.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      314 2018-09-12 11:06:08.000000 skyfield-1.8/skyfield/__init__.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    19262 2018-08-05 21:11:48.000000 skyfield-1.8/skyfield/iokit.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    15815 2018-09-10 01:39:19.000000 skyfield-1.8/skyfield/units.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     1573 2018-09-09 21:25:29.000000 skyfield-1.8/setup.py
+drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-23 21:08:16.000000 skyfield-1.9/
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2589 2018-09-23 21:08:16.000000 skyfield-1.9/PKG-INFO
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1101 2018-07-27 03:57:12.000000 skyfield-1.9/LICENSE
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1286 2018-01-19 12:43:35.000000 skyfield-1.9/README.rst
+drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-23 21:08:16.000000 skyfield-1.9/skyfield/
+-rw-r-----   0 brandon   (1000) brandon   (1000)    31688 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/timelib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    20497 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/positionlib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     8891 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/vectorlib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2145 2017-01-14 17:47:33.000000 skyfield-1.9/skyfield/precessionlib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      793 2017-01-14 17:47:33.000000 skyfield-1.9/skyfield/framelib.py
+drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-23 21:08:16.000000 skyfield-1.9/skyfield/tests/
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2394 2018-03-03 12:52:10.000000 skyfield-1.9/skyfield/tests/test_strs_and_reprs.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     4928 2018-07-27 03:38:46.000000 skyfield-1.9/skyfield/tests/test_against_horizons.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1854 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/tests/test_units.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      423 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/tests/fixes.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2045 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/tests/test_almanac.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    11745 2018-09-09 16:30:51.000000 skyfield-1.9/skyfield/tests/test_timelib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    25731 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/tests/test_elementslib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     4673 2018-07-27 02:18:42.000000 skyfield-1.9/skyfield/tests/test_earth_satellites.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)   140843 2018-09-09 21:04:49.000000 skyfield-1.9/skyfield/tests/test_against_novas.py
+drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-23 21:08:16.000000 skyfield-1.9/skyfield/tests/data/
+-rw-r-----   0 brandon   (1000) brandon   (1000)     9376 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/tests/data/de430-2015-03-02.bsp
+-rw-r-----   0 brandon   (1000) brandon   (1000)    27840 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/tests/data/jup310-2053-10-08.bsp
+-rw-r-----   0 brandon   (1000) brandon   (1000)    27024 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/tests/data/jup310-2015-03-02.bsp
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1520 2018-02-11 22:13:41.000000 skyfield-1.9/skyfield/tests/test_earth_deflection.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      793 2017-01-14 17:47:33.000000 skyfield-1.9/skyfield/tests/test_functions.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     4990 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/tests/test_positions.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      714 2018-09-03 14:12:25.000000 skyfield-1.9/skyfield/tests/test_topos.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     3611 2018-07-27 02:18:42.000000 skyfield-1.9/skyfield/tests/test_api.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2004 2018-05-28 20:48:59.000000 skyfield-1.9/skyfield/tests/test_vectors.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1309 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/tests/deprecations.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2724 2018-08-05 21:16:05.000000 skyfield-1.9/skyfield/tests/test_io.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)        0 2017-01-14 17:47:33.000000 skyfield-1.9/skyfield/tests/__init__.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     3454 2018-09-04 10:17:26.000000 skyfield-1.9/skyfield/tests/test_io_parsing.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2157 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/tests/test_angles.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      680 2018-09-03 20:56:52.000000 skyfield-1.9/skyfield/constants.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1476 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/errors.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     7542 2018-07-28 19:08:55.000000 skyfield-1.9/skyfield/charting.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     7547 2018-07-27 02:18:42.000000 skyfield-1.9/skyfield/sgp4lib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      430 2018-05-14 23:52:00.000000 skyfield-1.9/skyfield/descriptorlib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2230 2018-07-27 02:18:42.000000 skyfield-1.9/skyfield/projections.py
+drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-23 21:08:16.000000 skyfield-1.9/skyfield/data/
+-rw-r-----   0 brandon   (1000) brandon   (1000)    10576 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/data/historic_deltat.npy
+-rw-r-----   0 brandon   (1000) brandon   (1000)    15728 2018-09-09 19:32:18.000000 skyfield-1.9/skyfield/data/nutation.npz
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1342 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/data/earth_orientation.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      528 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/data/morrison_stephenson_deltat.npy
+-rw-r-----   0 brandon   (1000) brandon   (1000)     4682 2017-01-14 17:47:33.000000 skyfield-1.9/skyfield/data/spice.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2793 2018-09-04 00:17:03.000000 skyfield-1.9/skyfield/data/hipparcos.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2453 2018-07-27 02:54:52.000000 skyfield-1.9/skyfield/data/gravitational_parameters.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      706 2017-01-14 17:47:33.000000 skyfield-1.9/skyfield/data/horizons.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)       72 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/data/__init__.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     3515 2018-09-09 19:32:18.000000 skyfield-1.9/skyfield/functions.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     6566 2018-09-04 01:00:47.000000 skyfield-1.9/skyfield/starlib.py
+drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-09-23 21:08:16.000000 skyfield-1.9/skyfield/documentation/
+-rw-r-----   0 brandon   (1000) brandon   (1000)      884 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/documentation/api-units.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)      529 2018-02-03 16:25:00.000000 skyfield-1.9/skyfield/documentation/api-ephemeris.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)      309 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/documentation/api-stars.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2375 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/documentation/installation.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)      553 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/documentation/api-iokit.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     7693 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/documentation/api.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     6965 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/documentation/planets.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)      319 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/documentation/api-satellites.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     4739 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/documentation/bibliography.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2604 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/documentation/astropy.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)      539 2018-09-12 10:42:33.000000 skyfield-1.9/skyfield/documentation/toc.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2858 2018-07-27 02:54:52.000000 skyfield-1.9/skyfield/documentation/index.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     4454 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/documentation/elements.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     4322 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/documentation/almanac.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)      238 2018-09-04 10:13:06.000000 skyfield-1.9/skyfield/documentation/api-elements.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)    25465 2018-09-05 21:26:57.000000 skyfield-1.9/skyfield/documentation/time.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1987 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/documentation/api-vectors.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)    13625 2018-07-27 02:18:42.000000 skyfield-1.9/skyfield/documentation/earth-satellites.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)    10074 2018-09-05 21:44:23.000000 skyfield-1.9/skyfield/documentation/stars.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1727 2018-07-27 02:18:42.000000 skyfield-1.9/skyfield/documentation/api-position.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     8041 2018-09-03 18:43:15.000000 skyfield-1.9/skyfield/documentation/design.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)      441 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/documentation/api-almanac.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     5379 2018-07-27 03:12:25.000000 skyfield-1.9/skyfield/documentation/files.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)    19643 2018-07-27 02:54:52.000000 skyfield-1.9/skyfield/documentation/positions.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)      195 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/documentation/api-topos.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1537 2018-07-09 03:09:24.000000 skyfield-1.9/skyfield/documentation/api-time.rst
+-rw-r-----   0 brandon   (1000) brandon   (1000)     4233 2018-07-09 03:09:24.000000 skyfield-1.9/skyfield/api.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    11360 2018-09-09 22:09:51.000000 skyfield-1.9/skyfield/nutationlib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     6320 2018-01-19 12:43:35.000000 skyfield-1.9/skyfield/relativity.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     8982 2018-05-14 23:41:29.000000 skyfield-1.9/skyfield/jpllib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     3598 2018-04-15 22:11:09.000000 skyfield-1.9/skyfield/toposlib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     7434 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/almanac.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    13530 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/elementslib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2756 2018-09-04 02:08:43.000000 skyfield-1.9/skyfield/named_stars.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     6104 2018-09-03 14:14:15.000000 skyfield-1.9/skyfield/earthlib.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      314 2018-09-23 21:07:24.000000 skyfield-1.9/skyfield/__init__.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    19262 2018-08-05 21:11:48.000000 skyfield-1.9/skyfield/iokit.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    15815 2018-09-10 01:39:19.000000 skyfield-1.9/skyfield/units.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1573 2018-09-09 21:25:29.000000 skyfield-1.9/setup.py
```

### Comparing `skyfield-1.8/PKG-INFO` & `skyfield-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: skyfield
-Version: 1.8
+Version: 1.9
 Summary: Elegant astronomy for Python
 Home-page: http://github.com/brandon-rhodes/python-skyfield/
 Author: Brandon Rhodes
 Author-email: brandon@rhodesmill.org
 License: MIT
 Description: 
         ====================================
```

### Comparing `skyfield-1.8/LICENSE` & `skyfield-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/README.rst` & `skyfield-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/timelib.py` & `skyfield-1.9/skyfield/timelib.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,31 +457,39 @@
             utcs = [utc] * self.shape[0]
             argsets = zip(year, month, day, hour, minute, second, milli, utcs)
             dt = array([datetime(*args) for args in argsets])
         else:
             dt = datetime(year, month, day, hour, minute, second, milli, utc)
         return dt, leap_second
 
-    def utc_iso(self, places=0):
+    def utc_iso(self, delimiter='T', places=0):
         """Convert to an ISO 8601 string like ``2014-01-18T01:35:38Z`` in UTC.
 
         If this time is an array of dates, then a sequence of strings is
         returned instead of a single string.
 
         """
+        # "places" used to be the 1st argument, so continue to allow an
+        # integer in that spot.  TODO: deprecate this in Skyfield 2.0
+        # and remove it in 3.0.
+        if isinstance(delimiter, int):
+            places = delimiter
+            delimiter = 'T'
+
         if places:
             power_of_ten = 10 ** places
             offset = _half_second / power_of_ten
             year, month, day, hour, minute, second = self._utc_tuple(offset)
             second, fraction = divmod(second, 1.0)
             fraction *= power_of_ten
-            format = '%%04d-%%02d-%%02dT%%02d:%%02d:%%02d.%%0%ddZ' % places
+            format = '%04d-%02d-%02d{0}%02d:%02d:%02d.%0{1}dZ'.format(
+                delimiter, places)
             args = (year, month, day, hour, minute, second, fraction)
         else:
-            format = '%04d-%02d-%02dT%02d:%02d:%02dZ'
+            format = '%04d-%02d-%02d{0}%02d:%02d:%02dZ'.format(delimiter)
             args = self._utc_tuple(_half_second)
 
         if self.shape:
             return [format % tup for tup in zip(*args)]
         else:
             return format % args
```

### Comparing `skyfield-1.8/skyfield/positionlib.py` & `skyfield-1.9/skyfield/positionlib.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,44 +196,36 @@
         """Compute J2000 ecliptic position vector (x, y, z).
 
         If you instead want the coordinates referenced to the dynamical
         system defined by the Earth's true equator and equinox, provide
         an epoch time.
 
         """
-        position_au = self.position.au
-        if epoch is not None:
-            if isinstance(epoch, Time):
-                pass
-            elif isinstance(epoch, float):
-                epoch = Time(None, tt=epoch)
-            elif epoch == 'date':
-                epoch = self.t
-            else:
-                raise ValueError('the epoch= must be a Time object,'
-                                 ' a floating point Terrestrial Time (TT),'
-                                 ' or the string "date" for epoch-of-date')
-            position_au = einsum('ij...,j...->i...', epoch.M, position_au)
-            oblm, oblt, eqeq, psi, eps = epoch._earth_tilt
-            e = oblt*DEG2RAD
-            E = rot_x(e)
-            if not epoch.shape:
-                vector = E.T.dot(position_au)
-            else:
-                result_array = empty((E.T.shape[0], E.T.shape[1]))
-                for a in range(0, E.T.shape[0]):
-                    vector = E.T[a, 0:].dot(position_au.T[a, 0:])
-                    result_array[a, 0:] = vector
-                vector = result_array
-        else:
-            vector = _ECLIPJ2000.dot(position_au)
-        if len(vector.shape) is 1:
+        if epoch is None:
+            vector = _ECLIPJ2000.dot(self.position.au)
             return Distance(vector)
+
+        position_au = self.position.au
+
+        if isinstance(epoch, Time):
+            pass
+        elif isinstance(epoch, float):
+            epoch = Time(None, tt=epoch)
+        elif epoch == 'date':
+            epoch = self.t
         else:
-            return Distance(vector.T)
+            raise ValueError('the epoch= must be a Time object,'
+                             ' a floating point Terrestrial Time (TT),'
+                             ' or the string "date" for epoch-of-date')
+
+        oblm, oblt, eqeq, psi, eps = epoch._earth_tilt
+        e = oblt * DEG2RAD
+        rotation = einsum('ij...,jk...->ik...', rot_x(-e), epoch.M)
+        position_au = einsum('ij...,j...->i...', rotation, position_au)
+        return Distance(position_au)
 
     def ecliptic_velocity(self):
         """Compute J2000 ecliptic velocity vector (x_dot, y_dot, z_dot)"""
         vector = _ECLIPJ2000.dot(self.velocity.au_per_d)
         return Velocity(vector)
 
     def ecliptic_latlon(self, epoch=None):
```

### Comparing `skyfield-1.8/skyfield/vectorlib.py` & `skyfield-1.9/skyfield/vectorlib.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/precessionlib.py` & `skyfield-1.9/skyfield/precessionlib.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/framelib.py` & `skyfield-1.9/skyfield/framelib.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_strs_and_reprs.py` & `skyfield-1.9/skyfield/tests/test_strs_and_reprs.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_against_horizons.py` & `skyfield-1.9/skyfield/tests/test_against_horizons.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_units.py` & `skyfield-1.9/skyfield/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_almanac.py` & `skyfield-1.9/skyfield/tests/test_almanac.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,29 @@
     e = api.load('de421.bsp')
     i = almanac.fraction_illuminated(e, 'moon', t0[-1]).round(2)
     assert i == 0.62
     i = almanac.fraction_illuminated(e, 'moon', t0).round(2)
     assert (i == (0, 0, 0.03, 0.08, 0.15, 0.24, 0.33, 0.43, 0.52, 0.62)).all()
 
 # Compare with USNO:
+# http://aa.usno.navy.mil/seasons?year=2018&tz=+0
+
+def test_seasons():
+    ts = api.load.timescale()
+    t0 = ts.utc(2018, 9, 20)
+    t1 = ts.utc(2018, 12, 31)
+    e = api.load('de421.bsp')
+    t, y = almanac.find_discrete(t0, t1, almanac.seasons(e))
+    t.tt += half_minute
+    strings = t.utc_strftime('%Y-%m-%d %H:%M')
+    print(strings)
+    assert strings == ['2018-09-23 01:54', '2018-12-21 22:23']
+    assert (y == (2, 3)).all()
+
+# Compare with USNO:
 # http://aa.usno.navy.mil/rstt/onedaytable?ID=AA&year=2018&month=9&day=12&state=OH&place=Bluffton
 
 def test_sunrise_sunset():
     ts = api.load.timescale()
     t0 = ts.utc(2018, 9, 12, 4)
     t1 = ts.utc(2018, 9, 13, 4)
     e = api.load('de421.bsp')
```

### Comparing `skyfield-1.8/skyfield/tests/test_timelib.py` & `skyfield-1.9/skyfield/tests/test_timelib.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_elementslib.py` & `skyfield-1.9/skyfield/tests/test_elementslib.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,19 @@
                  dict_['TA'],
                  dict_['A'],
                  dict_['AD'],
                  dict_['PR']])
     return array_
 
 
+def test_repr(ts):
+    elements = osculating_elements_of((moon-earth).at(ts.utc(2015, 3, 2, 12)))
+    assert repr(elements) == '<Elements 1 sets>'
+
+
 def test_single_time(ts):
     """Tests creation of an OsculatingElements object with a single set of elements
     """
     elements = osculating_elements_of((moon-earth).at(ts.utc(2015, 3, 2, 12)))
     check_types(elements, 1)
 
 
@@ -254,15 +259,15 @@
                            2.568213873445825E-03,
                            2.711246366755283E-03,
                            2.726324301628867E+01])
     epsilon = array([1e-10, 1e-12, 1e-7, 1e-6, 1e-6, 1e-8, 1e-9, 1e-6, 1e-7, 1e-13, 1e-12, 1e-8])
     compare(calc_data, horizons_data, epsilon)
 
 
-def BROKEN_test_ecliptic_km_d(ts):
+def test_ecliptic_km_d(ts):
     """Tests against data from Horizons in km and days, with ecliptic reference plane
     """
     geocentric_pos = (moon - earth).at(ts.tdb(2015, 3, 2, 2))
     calc_data = horizons_array(osculating_elements_of(geocentric_pos, ECLIPTIC), units='km_d')
     horizons_data = array([5.569337304355707E-02,
                           3.628019705296879E+05,
                           5.216521657765558E+00,
@@ -275,15 +280,15 @@
                           3.841993269696947E+05,
                           4.055966834097015E+05,
                           2.726324301628867E+01])
     epsilon = array([1e-10, 1e-4, 1e-8, 1e-6, 1e-6, 1e-8, 1e-9, 1e-6, 1e-7, 1e-4, 1e-4, 1e-8])
     compare(calc_data, horizons_data, epsilon)
 
 
-def BROKEN_test_ecliptic_km_s(ts):
+def test_ecliptic_km_s(ts):
     """Tests against data from Horizons in km and seconds, with ecliptic reference plane
     """
     geocentric_pos = (moon - earth).at(ts.tdb(2015, 3, 2, 2))
     calc_data = horizons_array(osculating_elements_of(geocentric_pos, ECLIPTIC), units='km_s')
     horizons_data = array([5.569337304355707E-02,
                            3.628019705296879E+05,
                            5.216521657765558E+00,
@@ -296,15 +301,15 @@
                            3.841993269696947E+05,
                            4.055966834097015E+05,
                            2.355544196607342E+06])
     epsilon = array([1e-10, 1e-4, 1e-8, 1e-6, 1e-6, 1e-8, 1e-14, 1e-6, 1e-7, 1e-4, 1e-4, 1e-3])
     compare(calc_data, horizons_data, epsilon)
 
 
-def BROKEN_test_ecliptic_au_d(ts):
+def test_ecliptic_au_d(ts):
     """Tests against data from Horizons in au and days, with ecliptic reference plane
     """
     geocentric_pos = (moon - earth).at(ts.tdb(2015, 3, 2, 2))
     elem = osculating_elements_of(geocentric_pos, ECLIPTIC)
     calc_data = horizons_array(elem, units='au_d')
     horizons_data = array([5.569337304355707E-02,
                            2.425181380136368E-03,
```

### Comparing `skyfield-1.8/skyfield/tests/test_earth_satellites.py` & `skyfield-1.9/skyfield/tests/test_earth_satellites.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_against_novas.py` & `skyfield-1.9/skyfield/tests/test_against_novas.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/data/de430-2015-03-02.bsp` & `skyfield-1.9/skyfield/tests/data/de430-2015-03-02.bsp`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/data/jup310-2053-10-08.bsp` & `skyfield-1.9/skyfield/tests/data/jup310-2053-10-08.bsp`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/data/jup310-2015-03-02.bsp` & `skyfield-1.9/skyfield/tests/data/jup310-2015-03-02.bsp`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_earth_deflection.py` & `skyfield-1.9/skyfield/tests/test_earth_deflection.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_functions.py` & `skyfield-1.9/skyfield/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_topos.py` & `skyfield-1.9/skyfield/tests/test_topos.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_api.py` & `skyfield-1.9/skyfield/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_vectors.py` & `skyfield-1.9/skyfield/tests/test_vectors.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/deprecations.py` & `skyfield-1.9/skyfield/tests/deprecations.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_io.py` & `skyfield-1.9/skyfield/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_io_parsing.py` & `skyfield-1.9/skyfield/tests/test_io_parsing.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/tests/test_angles.py` & `skyfield-1.9/skyfield/tests/test_angles.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/constants.py` & `skyfield-1.9/skyfield/constants.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/errors.py` & `skyfield-1.9/skyfield/errors.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/charting.py` & `skyfield-1.9/skyfield/charting.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/sgp4lib.py` & `skyfield-1.9/skyfield/sgp4lib.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/projections.py` & `skyfield-1.9/skyfield/projections.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/data/historic_deltat.npy` & `skyfield-1.9/skyfield/data/historic_deltat.npy`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/data/nutation.npz` & `skyfield-1.9/skyfield/data/nutation.npz`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/data/earth_orientation.py` & `skyfield-1.9/skyfield/data/earth_orientation.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/data/morrison_stephenson_deltat.npy` & `skyfield-1.9/skyfield/data/morrison_stephenson_deltat.npy`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/data/spice.py` & `skyfield-1.9/skyfield/data/spice.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/data/hipparcos.py` & `skyfield-1.9/skyfield/data/hipparcos.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/data/gravitational_parameters.py` & `skyfield-1.9/skyfield/data/gravitational_parameters.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/data/horizons.py` & `skyfield-1.9/skyfield/data/horizons.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/functions.py` & `skyfield-1.9/skyfield/functions.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/starlib.py` & `skyfield-1.9/skyfield/starlib.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/api-units.rst` & `skyfield-1.9/skyfield/documentation/api-units.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/api-ephemeris.rst` & `skyfield-1.9/skyfield/documentation/api-ephemeris.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/installation.rst` & `skyfield-1.9/skyfield/documentation/installation.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/api-iokit.rst` & `skyfield-1.9/skyfield/documentation/api-iokit.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/api.rst` & `skyfield-1.9/skyfield/documentation/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 Routines to search for events like sunrise, sunset, and Moon phase.
 
 .. autosummary::
 
    phase_angle
    fraction_illuminated
    find_discrete
+   seasons
    sunrise_sunset
    moon_phases
 
 Topocentric Locations
 =====================
 
 .. currentmodule:: skyfield.toposlib
```

### Comparing `skyfield-1.8/skyfield/documentation/planets.rst` & `skyfield-1.9/skyfield/documentation/planets.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/bibliography.rst` & `skyfield-1.9/skyfield/documentation/bibliography.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/astropy.rst` & `skyfield-1.9/skyfield/documentation/astropy.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/toc.rst` & `skyfield-1.9/skyfield/documentation/toc.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/index.rst` & `skyfield-1.9/skyfield/documentation/index.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/almanac.rst` & `skyfield-1.9/skyfield/documentation/almanac.rst`

 * *Files 11% similar despite different names*

```diff
@@ -67,14 +67,40 @@
 
 .. testoutput::
 
     2018-09-10 05:15
 
 The results should then agree with the tables produced by the USNO.
 
+The Seasons
+===========
+
+Create a start time and an end time to ask for all of the equinoxes and
+solstices that fall in between.
+
+.. testcode::
+
+    t0 = ts.utc(2018, 1, 1)
+    t1 = ts.utc(2018, 12, 31)
+    t, y = almanac.find_discrete(t0, t1, almanac.seasons(e))
+
+    for yi, ti in zip(y, t):
+        print(yi, almanac.SEASON_EVENTS[yi], ti.utc_iso(' '))
+
+.. testoutput::
+
+    0 Vernal Equinox 2018-03-20 16:15:27Z
+    1 Summer Solstice 2018-06-21 10:07:18Z
+    2 Autumnal Equinox 2018-09-23 01:54:06Z
+    3 Winter Solstice 2018-12-21 22:22:44Z
+
+The result ``t`` will be an array of times, and ``y`` will be ``0``
+through ``3`` for the Vernal Equinox through the Winter Solstice.
+
+
 Sunrise and Sunset
 ==================
 
 Because sunrise and sunset differ depending on your location on the
 Earth’s surface, you first need to create a Topos object describing your
 geographic location.
```

### Comparing `skyfield-1.8/skyfield/documentation/time.rst` & `skyfield-1.9/skyfield/documentation/time.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/api-vectors.rst` & `skyfield-1.9/skyfield/documentation/api-vectors.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/earth-satellites.rst` & `skyfield-1.9/skyfield/documentation/earth-satellites.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/stars.rst` & `skyfield-1.9/skyfield/documentation/stars.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/api-position.rst` & `skyfield-1.9/skyfield/documentation/api-position.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/design.rst` & `skyfield-1.9/skyfield/documentation/design.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/files.rst` & `skyfield-1.9/skyfield/documentation/files.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/positions.rst` & `skyfield-1.9/skyfield/documentation/positions.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/documentation/api-time.rst` & `skyfield-1.9/skyfield/documentation/api-time.rst`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/api.py` & `skyfield-1.9/skyfield/api.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/nutationlib.py` & `skyfield-1.9/skyfield/nutationlib.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/relativity.py` & `skyfield-1.9/skyfield/relativity.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/jpllib.py` & `skyfield-1.9/skyfield/jpllib.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/toposlib.py` & `skyfield-1.9/skyfield/toposlib.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/almanac.py` & `skyfield-1.9/skyfield/almanac.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,15 +129,51 @@
 
         jd = o(starts, start_mask).flatten() + o(ends, end_mask).flatten()
 
     return ts.tt_jd(ends), y.take(indices)
 
 # Discrete circumstances to search.
 
+SEASONS = [
+    'Spring',
+    'Summer',
+    'Autumn',
+    'Winter',
+]
+
+SEASON_EVENTS = [
+    'Vernal Equinox',
+    'Summer Solstice',
+    'Autumnal Equinox',
+    'Winter Solstice',
+]
+
+def seasons(ephemeris):
+    """Build a function of time that returns the quarter of the year.
+
+    The function that this returns will expect a single argument that is
+    a :class:`~skyfield.timelib.Time` and will return 0 through 3 for
+    the seasons Spring, Summer, Autumn, and Winter.
+
+    """
+    earth = ephemeris['earth']
+    sun = ephemeris['sun']
+
+    def season_at(t):
+        """Return season 0 (Spring) through 3 (Winter) at time `t`."""
+        t._nutation_angles = iau2000b(t.tt)
+        e = earth.at(t)
+        _, slon, _ = e.observe(sun).apparent().ecliptic_latlon('date')
+        return (slon.radians // (tau / 4) % 4).astype(int)
+
+    season_at.rough_period = 90.0
+    return season_at
+
 def sunrise_sunset(ephemeris, topos):
+
     """Build a function of time that returns whether the sun is up.
 
     The function that this returns will expect a single argument that is
     a :class:`~skyfield.timelib.Time` and will return ``True`` if the
     sun is up, else ``False``.
 
     """
```

### Comparing `skyfield-1.8/skyfield/elementslib.py` & `skyfield-1.9/skyfield/elementslib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Computation of osculating elements that matches NASA HORIZONS."""
 
 from .functions import dots, length_of, angle_between
 from .constants import DAY_S, tau
 from .data.gravitational_parameters import GM_dict
-from .units import Distance, Angle
+from .units import Distance, Angle, Velocity
 from .descriptorlib import reify
 from numpy import (array, arctan2, sin, arctan, tan, inf, repeat, float64,
                    sinh, sqrt, arccos, arctanh, zeros_like, ones_like, divide,
                    where, pi, cross)
 
 def osculating_elements_of(position, reference_frame=None):
     """Produce the osculating orbital elements for a position.
@@ -16,21 +16,27 @@
     instance like that returned by the ``at()`` method of any Solar
     System body, specifying a position, a velocity, and a time.  An
     instance of :class:`~skyfield.elementslib.OsculatingElements` is
     returned.
 
     """
     mu = GM_dict.get(position.center, 0) + GM_dict.get(position.target, 0)
-    return OsculatingElements(
-        position.position,
-        position.velocity,
-        position.t,
-        mu,
-        reference_frame,
-    )
+    
+    if reference_frame is not None:
+        position_vec = Distance(reference_frame.dot(position.position.au))
+        velocity_vec = Velocity(reference_frame.dot(position.velocity.au_per_d))
+    else:
+        position_vec = position.position
+        velocity_vec = position.velocity
+        
+    return OsculatingElements(position_vec,
+                              velocity_vec,
+                              position.t,
+                              mu)
+
 
 class OsculatingElements(object):
     """
     Contains one or more sets of osculating orbital elements. Different
     elements are accessed as attributes of the ``OsculatingElements`` object.
 
     An ``OsculatingElements`` object can be initialized with the following
@@ -40,33 +46,26 @@
         Position vector with shape (3,) or (3, n)
     velocity : Velocity object
         Velocity vector with shape (3,) or (3, n)
     time: Time object
         The times of the position and velocity vectors
     mu_km_s: float
         Gravitational parameter (G*M) in units of km^3/s^2
-    ref_frame : 3x3 array
-        Rotation matrix from ICRF to reference frame of the elements
 
     """
-    def __init__(self, position, velocity, time, mu_km_s, ref_frame=None):
+    def __init__(self, position, velocity, time, mu_km_s):
         self._pos_vec = position.km
         self._vel_vec = velocity.km_per_s
         self.time = time
         self._mu = mu_km_s
 
         self._h_vec = cross(self._pos_vec, self._vel_vec, 0, 0).T
         self._e_vec = eccentricity_vector(self._pos_vec, self._vel_vec, self._mu)
         self._n_vec = node_vector(self._h_vec)
 
-        self.size = position.km[0].size
-        self.shape = position.km[0].shape
-
-        self._ref_frame = ref_frame
-
     @reify
     def apoapsis_distance(self):
         Q = apoapsis_distance(self.semi_latus_rectum.km, self.eccentricity)
         return Distance(km=Q)
 
     @reify
     def argument_of_latitude(self):
@@ -173,15 +172,15 @@
         Om = self.longitude_of_ascending_node.radians
         w = self.argument_of_periapsis.radians
         v = self.true_anomaly.radians
         l = (Om + w + v)%tau
         return Angle(radians=l)
 
     def __repr__(self):
-        return '<Elements {} sets>'.format(self.size)
+        return '<Elements {0} sets>'.format(self.time.tt.size)
 
 # a = semi-major axis
 # b = semi-minor axis
 # e = eccentricity
 # E = eccentric anomaly
 # h = specific angular momentum
 # i = inclination
```

### Comparing `skyfield-1.8/skyfield/named_stars.py` & `skyfield-1.9/skyfield/named_stars.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/earthlib.py` & `skyfield-1.9/skyfield/earthlib.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/iokit.py` & `skyfield-1.9/skyfield/iokit.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/skyfield/units.py` & `skyfield-1.9/skyfield/units.py`

 * *Files identical despite different names*

### Comparing `skyfield-1.8/setup.py` & `skyfield-1.9/setup.py`

 * *Files identical despite different names*

