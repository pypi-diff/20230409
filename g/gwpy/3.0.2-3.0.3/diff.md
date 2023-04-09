# Comparing `tmp/gwpy-3.0.2.tar.gz` & `tmp/gwpy-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwpy-3.0.2.tar", last modified: Thu Nov 24 12:11:17 2022, max compression
+gzip compressed data, was "gwpy-3.0.3.tar", last modified: Sun Apr  9 14:51:14 2023, max compression
```

## Comparing `gwpy-3.0.2.tar` & `gwpy-3.0.3.tar`

### file list

```diff
@@ -1,436 +1,441 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.374914 gwpy-3.0.2/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      524 2022-07-19 10:06:33.000000 gwpy-3.0.2/.codeclimate.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      498 2022-11-23 15:25:42.000000 gwpy-3.0.2/.codecov.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      483 2022-08-02 16:08:04.000000 gwpy-3.0.2/.flake8
--rw-r--r--   0 duncan    (1000) duncan    (1000)       30 2021-03-07 21:23:43.000000 gwpy-3.0.2/.gitattributes
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.224914 gwpy-3.0.2/.github/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.244914 gwpy-3.0.2/.github/workflows/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5205 2022-11-24 12:06:48.000000 gwpy-3.0.2/.github/workflows/conda.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2920 2022-11-23 15:25:42.000000 gwpy-3.0.2/.github/workflows/dependencies.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3119 2022-11-24 09:25:46.000000 gwpy-3.0.2/.github/workflows/dist.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1234 2022-08-02 16:08:04.000000 gwpy-3.0.2/.github/workflows/lint.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      726 2022-11-23 15:25:42.000000 gwpy-3.0.2/.gitignore
--rw-r--r--   0 duncan    (1000) duncan    (1000)       44 2022-07-19 10:06:33.000000 gwpy-3.0.2/.pep8speaks.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      133 2021-03-07 21:23:43.000000 gwpy-3.0.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4481 2022-08-02 16:08:04.000000 gwpy-3.0.2/CONTRIBUTING.md
--rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2021-03-07 21:23:43.000000 gwpy-3.0.2/LICENSE
--rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2022-07-19 10:06:33.000000 gwpy-3.0.2/MANIFEST.in
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2022-11-24 12:11:17.374914 gwpy-3.0.2/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1800 2022-08-02 16:08:04.000000 gwpy-3.0.2/README.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.244914 gwpy-3.0.2/docs/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      788 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/Makefile
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.244914 gwpy-3.0.2/docs/_static/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.244914 gwpy-3.0.2/docs/_static/css/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/_static/css/gwpy-sphinx.css
--rw-r--r--   0 duncan    (1000) duncan    (1000)    19634 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/_static/favicon.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)    15166 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/_static/gwpy_white_24.png
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.224914 gwpy-3.0.2/docs/_templates/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.244914 gwpy-3.0.2/docs/_templates/autoclass/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      860 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/_templates/autoclass/class.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.244914 gwpy-3.0.2/docs/_templates/autosummary/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      170 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1145 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      703 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.244914 gwpy-3.0.2/docs/astro/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      735 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/astro/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2653 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/citing.rst.in
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.254914 gwpy-3.0.2/docs/cli/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3090 2022-11-10 14:52:01.000000 gwpy-3.0.2/docs/cli/examples.ini
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2879 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/cli/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13186 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/conf.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.254914 gwpy-3.0.2/docs/detector/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3245 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/detector/channel.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.254914 gwpy-3.0.2/docs/dev/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3787 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/dev/release.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1624 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/env.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.224914 gwpy-3.0.2/docs/examples/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.254914 gwpy-3.0.2/docs/examples/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)    52297 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/gwpy-docs-logo.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2491 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1651 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/install.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2694 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/overview.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.254914 gwpy-3.0.2/docs/plot/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2600 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/plot/colorbars.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2985 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/plot/colors.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      772 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/plot/filter.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2514 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/plot/gps.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3095 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/plot/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1838 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/plot/legend.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1363 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/plot/log.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5046 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/references.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.254914 gwpy-3.0.2/docs/segments/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1513 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/segments/dqsegdb.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6818 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/segments/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6756 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/segments/io.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2124 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/segments/thresholding.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.254914 gwpy-3.0.2/docs/signal/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4369 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/signal/index.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.254914 gwpy-3.0.2/docs/spectrogram/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3771 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/spectrogram/index.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.254914 gwpy-3.0.2/docs/spectrum/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      505 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/spectrum/filtering.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3732 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/spectrum/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4986 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/spectrum/io.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.264914 gwpy-3.0.2/docs/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7364 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/table/filter.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      955 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/table/histogram.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1500 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/table/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    30467 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/table/io.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1756 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/table/plot.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2142 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/table/rate.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.264914 gwpy-3.0.2/docs/time/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1085 2021-03-07 21:23:43.000000 gwpy-3.0.2/docs/time/index.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.264914 gwpy-3.0.2/docs/timeseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11590 2022-11-10 17:06:25.000000 gwpy-3.0.2/docs/timeseries/datafind.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2722 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/timeseries/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10857 2022-11-23 15:25:42.000000 gwpy-3.0.2/docs/timeseries/io.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2744 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/timeseries/opendata.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3032 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/timeseries/plot.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8470 2022-07-19 10:06:33.000000 gwpy-3.0.2/docs/timeseries/statevector.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.264914 gwpy-3.0.2/examples/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.264914 gwpy-3.0.2/examples/frequencyseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2584 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/frequencyseries/coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2065 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/frequencyseries/hoff.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      258 2021-03-07 21:23:43.000000 gwpy-3.0.2/examples/frequencyseries/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2585 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/frequencyseries/inject.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2022-11-07 14:19:34.000000 gwpy-3.0.2/examples/frequencyseries/percentiles.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/frequencyseries/rayleigh.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2203 2022-11-23 15:25:42.000000 gwpy-3.0.2/examples/frequencyseries/transfer_function.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2630 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/frequencyseries/variance.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.264914 gwpy-3.0.2/examples/miscellaneous/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      216 2021-03-07 21:23:43.000000 gwpy-3.0.2/examples/miscellaneous/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3354 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/miscellaneous/open-data-spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2366 2022-07-19 10:06:33.000000 gwpy-3.0.2/examples/miscellaneous/range-spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2490 2022-07-19 10:06:33.000000 gwpy-3.0.2/examples/miscellaneous/range-timeseries.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.264914 gwpy-3.0.2/examples/segments/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      158 2021-03-07 21:23:43.000000 gwpy-3.0.2/examples/segments/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2411 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/segments/open-data.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.264914 gwpy-3.0.2/examples/signal/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5642 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/signal/gw150914.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      179 2021-03-07 21:23:43.000000 gwpy-3.0.2/examples/signal/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3236 2022-07-19 10:06:33.000000 gwpy-3.0.2/examples/signal/qscan.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.274914 gwpy-3.0.2/examples/spectrogram/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2387 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/spectrogram/coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      209 2021-03-07 21:23:43.000000 gwpy-3.0.2/examples/spectrogram/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2627 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/spectrogram/plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2581 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/spectrogram/ratio.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2125 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/spectrogram/rayleigh.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2885 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/spectrogram/spectrogram2.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.274914 gwpy-3.0.2/examples/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2021-03-07 21:23:43.000000 gwpy-3.0.2/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1597 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/table/histogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      198 2021-03-07 21:23:43.000000 gwpy-3.0.2/examples/table/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2317 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/table/rate.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2460 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/table/rate_binned.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2018 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/table/scatter.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2287 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/table/tiles.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3734 2022-07-19 10:06:33.000000 gwpy-3.0.2/examples/test_examples.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.274914 gwpy-3.0.2/examples/timeseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2644 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/timeseries/blrms.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4204 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/timeseries/correlate.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2797 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/timeseries/filter.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      246 2021-03-07 21:23:43.000000 gwpy-3.0.2/examples/timeseries/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2641 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/timeseries/inject.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2466 2022-07-19 10:06:33.000000 gwpy-3.0.2/examples/timeseries/public.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3788 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/timeseries/pycbc-snr.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/timeseries/qscan.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2202 2022-07-19 10:06:33.000000 gwpy-3.0.2/examples/timeseries/statevector.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2476 2022-07-18 20:57:40.000000 gwpy-3.0.2/examples/timeseries/whiten.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.274914 gwpy-3.0.2/gwpy/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1533 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2022-11-24 12:11:17.000000 gwpy-3.0.2/gwpy/_version.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.274914 gwpy-3.0.2/gwpy/astro/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1909 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/astro/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    24880 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/astro/range.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.274914 gwpy-3.0.2/gwpy/astro/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/astro/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6048 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/astro/tests/test_range.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.284914 gwpy-3.0.2/gwpy/cli/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1404 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    34269 2022-11-24 12:06:48.000000 gwpy-3.0.2/gwpy/cli/cliproduct.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4048 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3353 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/coherencegram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5121 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/gwpy_plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9140 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/qtransform.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7131 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4899 2022-11-24 09:22:14.000000 gwpy-3.0.2/gwpy/cli/spectrum.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.284914 gwpy-3.0.2/gwpy/cli/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      744 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/cli/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10831 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/tests/base.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1353 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/tests/test_coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1580 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/tests/test_coherencegram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1718 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/tests/test_gwpy_plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2899 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/tests/test_qtransform.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1509 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/tests/test_spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1416 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/tests/test_spectrum.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1279 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/tests/test_timeseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1999 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/tests/test_transferfunction.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3891 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/timeseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9784 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/cli/transferfunction.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1639 2022-08-23 16:08:03.000000 gwpy-3.0.2/gwpy/conftest.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.284914 gwpy-3.0.2/gwpy/detector/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2252 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/detector/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    26901 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/detector/channel.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.284914 gwpy-3.0.2/gwpy/detector/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1037 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/detector/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3184 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/detector/io/cis.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5689 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/detector/io/clf.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5939 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/detector/io/omega.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.294914 gwpy-3.0.2/gwpy/detector/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/detector/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    18599 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/detector/tests/test_channel.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2548 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/detector/tests/test_units.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7113 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/detector/units.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.294914 gwpy-3.0.2/gwpy/frequencyseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      995 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/frequencyseries/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1943 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/frequencyseries/_fdcommon.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14328 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/frequencyseries/frequencyseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11947 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/frequencyseries/hist.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.294914 gwpy-3.0.2/gwpy/frequencyseries/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      907 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/frequencyseries/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1071 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/frequencyseries/io/ascii.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1036 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/frequencyseries/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1149 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/frequencyseries/io/ligolw.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.294914 gwpy-3.0.2/gwpy/frequencyseries/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      756 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/frequencyseries/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10996 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/frequencyseries/tests/test_frequencyseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4001 2022-11-03 08:28:15.000000 gwpy-3.0.2/gwpy/frequencyseries/tests/test_hist.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.294914 gwpy-3.0.2/gwpy/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      831 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3547 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/io/_framecpp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14662 2022-08-02 13:02:40.000000 gwpy-3.0.2/gwpy/io/cache.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18462 2022-08-02 16:08:04.000000 gwpy-3.0.2/gwpy/io/datafind.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8399 2022-08-02 16:08:04.000000 gwpy-3.0.2/gwpy/io/ffldatafind.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)    19047 2022-10-27 13:33:09.000000 gwpy-3.0.2/gwpy/io/gwf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5257 2022-08-02 13:02:40.000000 gwpy-3.0.2/gwpy/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6928 2022-08-02 13:02:40.000000 gwpy-3.0.2/gwpy/io/kerberos.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    22182 2022-11-24 12:06:48.000000 gwpy-3.0.2/gwpy/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4116 2022-08-02 13:02:40.000000 gwpy-3.0.2/gwpy/io/mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    19331 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/io/nds2.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3518 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/io/registry.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.304914 gwpy-3.0.2/gwpy/io/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      743 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/io/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8287 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/io/tests/test_cache.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10651 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/io/tests/test_datafind.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6277 2022-08-02 16:08:04.000000 gwpy-3.0.2/gwpy/io/tests/test_ffldatafind.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4209 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/io/tests/test_gwf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6476 2022-11-03 08:28:15.000000 gwpy-3.0.2/gwpy/io/tests/test_kerberos.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10717 2022-11-24 12:06:48.000000 gwpy-3.0.2/gwpy/io/tests/test_ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3297 2022-11-03 08:28:15.000000 gwpy-3.0.2/gwpy/io/tests/test_mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12305 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/io/tests/test_nds2.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3984 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/io/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7341 2022-08-02 13:02:40.000000 gwpy-3.0.2/gwpy/io/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.304914 gwpy-3.0.2/gwpy/plot/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1641 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/plot/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    23094 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/axes.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8733 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/plot/bode.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6920 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/colorbar.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3367 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/colors.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    16353 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/gps.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1635 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/legend.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5026 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/log.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    21766 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4816 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/plot/rc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    16943 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/segments.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.314914 gwpy-3.0.2/gwpy/plot/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      740 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/plot/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11527 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/tests/test_axes.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3351 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/plot/tests/test_bode.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1881 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/plot/tests/test_colors.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5456 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/plot/tests/test_gps.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2652 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/plot/tests/test_log.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4398 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/tests/test_plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1252 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/tests/test_rc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5442 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/tests/test_segments.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1953 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/plot/tests/test_tex.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/plot/tests/test_text.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1615 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/plot/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1925 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/plot/tests/utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4244 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/tex.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1989 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/plot/text.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1383 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/plot/units.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1670 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/plot/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.314914 gwpy-3.0.2/gwpy/segments/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1194 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/segments/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    52670 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/segments/flag.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.314914 gwpy-3.0.2/gwpy/segments/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1005 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/segments/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11048 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/segments/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3036 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/segments/io/json.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4907 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/segments/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5007 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/segments/io/segwizard.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9042 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/segments/segments.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.314914 gwpy-3.0.2/gwpy/segments/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/segments/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    29716 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/segments/tests/test_flag.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5360 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/segments/tests/test_segments.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.314914 gwpy-3.0.2/gwpy/signal/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      972 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1189 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/fft.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    20263 2022-11-07 14:19:34.000000 gwpy-3.0.2/gwpy/signal/filter_design.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    24431 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/signal/qtransform.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.324914 gwpy-3.0.2/gwpy/signal/spectral/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1818 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/signal/spectral/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12000 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/spectral/_lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1851 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/spectral/_median_mean.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3577 2022-11-07 14:19:34.000000 gwpy-3.0.2/gwpy/signal/spectral/_pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2346 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/signal/spectral/_registry.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6492 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/signal/spectral/_scipy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14241 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/spectral/_ui.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1669 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/spectral/_utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.324914 gwpy-3.0.2/gwpy/signal/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      747 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4349 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/tests/test_filter_design.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4017 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/tests/test_qtransform.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3543 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/tests/test_spectral_lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2195 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/signal/tests/test_spectral_median_mean.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2249 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/tests/test_spectral_pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1446 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/tests/test_spectral_registry.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1874 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/tests/test_spectral_scipy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3045 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/signal/tests/test_spectral_ui.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1453 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/signal/tests/test_spectral_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1805 2022-11-07 14:19:34.000000 gwpy-3.0.2/gwpy/signal/tests/test_window.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5169 2022-11-07 14:19:34.000000 gwpy-3.0.2/gwpy/signal/window.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.324914 gwpy-3.0.2/gwpy/spectrogram/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      919 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/spectrogram/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5742 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/spectrogram/coherence.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.324914 gwpy-3.0.2/gwpy/spectrogram/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      846 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/spectrogram/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      963 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/spectrogram/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    22206 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/spectrogram/spectrogram.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.324914 gwpy-3.0.2/gwpy/spectrogram/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      752 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/spectrogram/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6538 2022-11-03 08:28:15.000000 gwpy-3.0.2/gwpy/spectrogram/tests/test_spectrogram.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.334914 gwpy-3.0.2/gwpy/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1418 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7918 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/filter.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2645 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/table/filters.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8173 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/gravityspy.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.334914 gwpy-3.0.2/gwpy/table/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1564 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3809 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/table/io/cwb.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/table/io/fetch.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4663 2022-08-02 16:08:04.000000 gwpy-3.0.2/gwpy/table/io/gravityspy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8390 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/io/gstlal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5433 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/table/io/gwf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5205 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/table/io/hacr.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13590 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4434 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/table/io/losc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2604 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/table/io/omega.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1333 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/table/io/omicron.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8894 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/io/pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3318 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/io/root.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3857 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/table/io/snax.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3067 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/table/io/sql.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3183 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/table/io/utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    26330 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/table.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.334914 gwpy-3.0.2/gwpy/table/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/table/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3363 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/tests/test_gravityspy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7979 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/tests/test_io_gstlal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2848 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/tests/test_io_ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8337 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/tests/test_io_pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    30454 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/table/tests/test_table.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.344914 gwpy-3.0.2/gwpy/testing/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/testing/__init__.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.344914 gwpy-3.0.2/gwpy/testing/data/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2021-03-07 21:23:43.000000 gwpy-3.0.2/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)   377295 2021-03-07 21:23:43.000000 gwpy-3.0.2/gwpy/testing/data/HLV-HW100916-968654552-1.gwf
--rw-r--r--   0 duncan    (1000) duncan    (1000)   382679 2021-03-07 21:23:43.000000 gwpy-3.0.2/gwpy/testing/data/HLV-HW100916-968654552-1.hdf
--rw-r--r--   0 duncan    (1000) duncan    (1000)       59 2021-03-07 21:23:43.000000 gwpy-3.0.2/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      564 2022-11-23 15:25:51.000000 gwpy-3.0.2/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2714 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/testing/errors.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3772 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/testing/fixtures.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1480 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/testing/marks.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4131 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/testing/mocks.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11726 2022-11-23 16:09:41.000000 gwpy-3.0.2/gwpy/testing/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.344914 gwpy-3.0.2/gwpy/time/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1812 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/time/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2285 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/time/__main__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8740 2022-11-08 13:29:51.000000 gwpy-3.0.2/gwpy/time/_tconvert.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.344914 gwpy-3.0.2/gwpy/time/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/time/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1362 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/time/tests/test_main.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4499 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/time/tests/test_time.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.354914 gwpy-3.0.2/gwpy/timeseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1134 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/timeseries/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    56972 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/timeseries/core.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.354914 gwpy-3.0.2/gwpy/timeseries/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      938 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/timeseries/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1185 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/timeseries/io/ascii.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/timeseries/io/cache.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/timeseries/io/core.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.354914 gwpy-3.0.2/gwpy/timeseries/io/gwf/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13156 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/timeseries/io/gwf/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    17130 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/timeseries/io/gwf/framecpp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4776 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/timeseries/io/gwf/framel.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6828 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/timeseries/io/gwf/lalframe.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4214 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/timeseries/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9345 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/timeseries/io/losc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7811 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/timeseries/io/nds2.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3595 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/timeseries/io/wav.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    35787 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/timeseries/statevector.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.354914 gwpy-3.0.2/gwpy/timeseries/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      751 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/timeseries/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    17797 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/timeseries/tests/test_core.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2265 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/timeseries/tests/test_io_gwf_framecpp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5001 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/timeseries/tests/test_io_gwf_lalframe.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1833 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/timeseries/tests/test_io_losc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12352 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/timeseries/tests/test_statevector.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    54374 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/timeseries/tests/test_timeseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    87790 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/timeseries/timeseries.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.364914 gwpy-3.0.2/gwpy/types/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1159 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/types/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    15282 2022-08-25 14:19:35.000000 gwpy-3.0.2/gwpy/types/array.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12367 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/types/array2d.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2989 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/types/index.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.364914 gwpy-3.0.2/gwpy/types/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      905 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/types/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2872 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/types/io/ascii.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8002 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/types/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7267 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/types/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    36772 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/types/series.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3567 2022-08-25 14:52:20.000000 gwpy-3.0.2/gwpy/types/sliceutils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.364914 gwpy-3.0.2/gwpy/types/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/types/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8608 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/types/tests/test_array.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9114 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/types/tests/test_array2d.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1762 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/types/tests/test_index.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14861 2022-11-03 08:28:15.000000 gwpy-3.0.2/gwpy/types/tests/test_series.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.364914 gwpy-3.0.2/gwpy/utils/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      933 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/utils/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3723 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/utils/decorators.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1490 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/utils/enum.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1911 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/utils/env.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8507 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/utils/lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3284 2022-11-07 14:19:34.000000 gwpy-3.0.2/gwpy/utils/misc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5057 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/utils/mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1367 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/utils/progress.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3396 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/utils/shell.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.364914 gwpy-3.0.2/gwpy/utils/sphinx/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      770 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/utils/sphinx/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3559 2021-03-07 21:23:43.000000 gwpy-3.0.2/gwpy/utils/sphinx/epydoc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4763 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/utils/sphinx/ex2rst.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3425 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/utils/sphinx/zenodo.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.374914 gwpy-3.0.2/gwpy/utils/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2022-07-18 20:57:40.000000 gwpy-3.0.2/gwpy/utils/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2214 2022-11-03 08:28:15.000000 gwpy-3.0.2/gwpy/utils/tests/test_decorators.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2212 2022-11-03 08:28:15.000000 gwpy-3.0.2/gwpy/utils/tests/test_enum.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2000 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/utils/tests/test_env.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3482 2022-11-23 15:25:42.000000 gwpy-3.0.2/gwpy/utils/tests/test_lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2625 2022-11-07 14:19:34.000000 gwpy-3.0.2/gwpy/utils/tests/test_misc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2089 2022-11-03 08:28:15.000000 gwpy-3.0.2/gwpy/utils/tests/test_mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2367 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/utils/tests/test_shell.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2263 2022-07-19 10:06:33.000000 gwpy-3.0.2/gwpy/utils/tests/test_sphinx_ex2rst.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-24 12:11:17.274914 gwpy-3.0.2/gwpy.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2022-11-24 12:11:17.000000 gwpy-3.0.2/gwpy.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9938 2022-11-24 12:11:17.000000 gwpy-3.0.2/gwpy.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2022-11-24 12:11:17.000000 gwpy-3.0.2/gwpy.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       54 2022-11-24 12:11:17.000000 gwpy-3.0.2/gwpy.egg-info/entry_points.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      776 2022-11-24 12:11:17.000000 gwpy-3.0.2/gwpy.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        5 2022-11-24 12:11:17.000000 gwpy-3.0.2/gwpy.egg-info/top_level.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4627 2022-11-24 12:06:48.000000 gwpy-3.0.2/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)       38 2022-11-24 12:11:17.374914 gwpy-3.0.2/setup.cfg
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)     2989 2022-07-19 10:06:33.000000 gwpy-3.0.2/setup_utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.064681 gwpy-3.0.3/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      524 2023-04-06 10:37:11.000000 gwpy-3.0.3/.codeclimate.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      498 2023-04-06 10:37:11.000000 gwpy-3.0.3/.codecov.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      483 2023-04-06 10:37:11.000000 gwpy-3.0.3/.flake8
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       30 2023-04-06 10:37:11.000000 gwpy-3.0.3/.gitattributes
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.974681 gwpy-3.0.3/.github/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/.github/workflows/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5119 2023-04-09 14:36:48.000000 gwpy-3.0.3/.github/workflows/conda.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2920 2023-04-06 10:37:11.000000 gwpy-3.0.3/.github/workflows/dependencies.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3119 2023-04-06 10:37:11.000000 gwpy-3.0.3/.github/workflows/dist.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1415 2023-04-09 14:36:48.000000 gwpy-3.0.3/.github/workflows/lint.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      726 2023-04-06 10:37:11.000000 gwpy-3.0.3/.gitignore
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       44 2023-04-06 10:37:11.000000 gwpy-3.0.3/.pep8speaks.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      133 2023-04-06 10:37:11.000000 gwpy-3.0.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4481 2023-04-06 10:37:11.000000 gwpy-3.0.3/CONTRIBUTING.md
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2023-04-06 10:37:11.000000 gwpy-3.0.3/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2023-04-06 10:37:11.000000 gwpy-3.0.3/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2023-04-09 14:51:14.064681 gwpy-3.0.3/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1800 2023-04-06 10:37:11.000000 gwpy-3.0.3/README.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      788 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/Makefile
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/_static/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/_static/css/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_static/css/gwpy-sphinx.css
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    19634 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_static/favicon.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    15166 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_static/gwpy_white_24.png
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.974681 gwpy-3.0.3/docs/_templates/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/_templates/autoclass/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      860 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_templates/autoclass/class.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/_templates/autosummary/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      170 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1145 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      703 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/astro/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      735 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/astro/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2653 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/citing.rst.in
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/cli/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5295 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/cli/examples.ini
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2879 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/cli/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13301 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/conf.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/detector/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3245 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/detector/channel.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/dev/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3787 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/dev/release.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1624 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/env.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.974681 gwpy-3.0.3/docs/examples/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/examples/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/external/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1162 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/external/framecpp.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      990 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/external/framel.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3134 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/external/lalsuite.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1025 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/external/nds2.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    52297 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/gwpy-docs-logo.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2491 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1300 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/install.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2694 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/overview.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/plot/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2600 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/colorbars.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2985 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/colors.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      772 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/filter.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2514 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/gps.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3095 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1838 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/legend.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1363 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/log.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5072 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/references.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/segments/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1513 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/segments/dqsegdb.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6818 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/segments/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6756 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/segments/io.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2124 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/segments/thresholding.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/signal/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4369 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/signal/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/spectrogram/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3771 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/spectrogram/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/spectrum/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      505 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/spectrum/filtering.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3732 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/spectrum/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4986 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/spectrum/io.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7364 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/filter.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      955 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/histogram.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1500 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    30445 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/table/io.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1756 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/plot.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2142 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/rate.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/time/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1085 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/time/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/timeseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11634 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/timeseries/datafind.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2722 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/timeseries/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10656 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/timeseries/io.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2744 2023-04-09 14:36:18.000000 gwpy-3.0.3/docs/timeseries/opendata.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3032 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/timeseries/plot.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8470 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/timeseries/statevector.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/examples/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/examples/frequencyseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2584 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2065 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/hoff.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      258 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2585 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/inject.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/percentiles.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/rayleigh.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2203 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/transfer_function.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2630 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/variance.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/examples/miscellaneous/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      216 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/miscellaneous/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3354 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/miscellaneous/open-data-spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2366 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/miscellaneous/range-spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2490 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/miscellaneous/range-timeseries.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/examples/segments/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      158 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/segments/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2411 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/segments/open-data.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/examples/signal/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5642 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/signal/gw150914.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      179 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/signal/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3139 2023-04-09 14:36:48.000000 gwpy-3.0.3/examples/signal/qscan.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/examples/spectrogram/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2387 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      209 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2627 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2581 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/ratio.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2125 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/rayleigh.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2885 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/spectrogram2.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/examples/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1597 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/histogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      198 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2317 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/rate.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2460 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/rate_binned.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2018 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/scatter.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2287 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/tiles.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3734 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/test_examples.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/examples/timeseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2644 2023-04-09 14:36:18.000000 gwpy-3.0.3/examples/timeseries/blrms.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4204 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/correlate.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2797 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/filter.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      246 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2641 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/inject.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2466 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/public.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3788 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/pycbc-snr.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/qscan.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2202 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/statevector.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2476 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/whiten.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1533 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      160 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy/_version.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy/astro/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1909 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/astro/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    24880 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/astro/range.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy/astro/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/astro/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6032 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/astro/tests/test_range.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy/cli/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1404 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    34269 2023-04-09 14:36:18.000000 gwpy-3.0.3/gwpy/cli/cliproduct.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4048 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3353 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/coherencegram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5121 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/gwpy_plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9140 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/qtransform.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7131 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4899 2023-04-09 14:36:18.000000 gwpy-3.0.3/gwpy/cli/spectrum.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy/cli/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      744 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10831 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/base.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1353 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1580 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_coherencegram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1718 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_gwpy_plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2899 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_qtransform.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1509 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1416 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_spectrum.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1279 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_timeseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1999 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_transferfunction.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3891 2023-04-09 14:36:18.000000 gwpy-3.0.3/gwpy/cli/timeseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9784 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/transferfunction.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1639 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/conftest.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/detector/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2252 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    26901 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/channel.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/detector/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1037 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3184 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/io/cis.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5689 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/io/clf.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5939 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/io/omega.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/detector/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    18473 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/detector/tests/test_channel.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2548 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/tests/test_units.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7113 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/units.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/frequencyseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      995 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1943 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/_fdcommon.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14328 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/frequencyseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11947 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/hist.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/frequencyseries/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      907 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1071 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/io/ascii.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1036 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1149 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/io/ligolw.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/frequencyseries/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      756 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11033 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/frequencyseries/tests/test_frequencyseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4005 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/frequencyseries/tests/test_hist.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      831 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4250 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/_framecpp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14662 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/cache.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18462 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/datafind.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8399 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/ffldatafind.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18966 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/gwf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5257 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6928 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/kerberos.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    22182 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4116 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    19331 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/nds2.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3518 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/registry.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/io/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      743 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8567 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_cache.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10606 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_datafind.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6277 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/tests/test_ffldatafind.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4228 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_gwf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6492 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_kerberos.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10701 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3293 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12185 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_nds2.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3971 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7341 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/plot/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1641 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    23094 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/axes.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8733 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/bode.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7041 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/colorbar.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3367 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/colors.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    16720 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/gps.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1635 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/legend.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5030 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/log.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    21766 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4816 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/rc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    16943 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/segments.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/plot/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      740 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11542 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/tests/test_axes.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3351 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_bode.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1881 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_colors.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5456 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_gps.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2652 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_log.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4398 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1252 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_rc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5442 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_segments.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2318 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/tests/test_tex.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_text.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1615 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1925 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4783 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/tex.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1989 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/text.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1383 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/units.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1670 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/segments/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1194 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    52670 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/flag.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/segments/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1005 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11048 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3036 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/io/json.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4907 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5007 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/io/segwizard.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9042 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/segments.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/segments/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    29683 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/segments/tests/test_flag.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5360 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/tests/test_segments.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/signal/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      972 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1189 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/fft.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    20270 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/signal/filter_design.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    24471 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/signal/qtransform.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/signal/spectral/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1818 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12000 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1851 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_median_mean.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3577 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2346 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_registry.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6492 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_scipy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14241 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_ui.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1669 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/signal/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      747 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4349 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_filter_design.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4017 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_qtransform.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3543 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2195 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_median_mean.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2249 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1446 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_registry.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1874 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_scipy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3045 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_ui.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1453 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2726 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/signal/tests/test_window.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5927 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/signal/window.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/spectrogram/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      919 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5742 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/coherence.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/spectrogram/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      846 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      963 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    22206 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/spectrogram.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/spectrogram/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      752 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6590 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/spectrogram/tests/test_spectrogram.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1418 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7918 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/filter.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2645 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/filters.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8173 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/gravityspy.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/table/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1564 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3809 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/cwb.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/fetch.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4663 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/gravityspy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8390 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/gstlal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5433 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/gwf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5205 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/hacr.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13590 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4434 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/losc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2604 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/omega.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1333 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/omicron.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8894 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3318 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/root.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3857 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/snax.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3067 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/sql.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3183 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    26330 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/table.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/table/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3392 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/table/tests/test_gravityspy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7979 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/tests/test_io_gstlal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2848 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/tests/test_io_ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8313 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/table/tests/test_io_pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    30399 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/table/tests/test_table.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/testing/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/__init__.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/testing/data/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)   377295 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/data/HLV-HW100916-968654552-1.gwf
+-rw-r--r--   0 duncan    (1000) duncan    (1000)   382679 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/data/HLV-HW100916-968654552-1.hdf
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       59 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      564 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2783 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/testing/errors.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3772 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/fixtures.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1480 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/marks.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4131 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/mocks.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11726 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/time/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1812 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/time/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2285 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/time/__main__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8975 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/time/_tconvert.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/time/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/time/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1362 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/time/tests/test_main.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5728 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/time/tests/test_time.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/timeseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1134 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    57165 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/core.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/timeseries/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      938 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1185 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/ascii.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/cache.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/core.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/timeseries/io/gwf/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13156 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/gwf/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    17130 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/gwf/framecpp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4776 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/gwf/framel.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6828 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/gwf/lalframe.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4214 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9345 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/losc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7811 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/nds2.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3595 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/wav.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35787 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/statevector.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/timeseries/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      751 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    18215 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_core.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2265 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_io_gwf_framecpp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4969 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_io_gwf_lalframe.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1833 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_io_losc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12356 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_statevector.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    55164 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_timeseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    87612 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/timeseries.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/types/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1159 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    15282 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/array.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12367 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/array2d.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3074 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/types/index.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/types/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      905 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2872 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/io/ascii.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8002 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7267 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    36772 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/series.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3567 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/sliceutils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.064681 gwpy-3.0.3/gwpy/types/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8608 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/tests/test_array.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9081 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/types/tests/test_array2d.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2044 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/types/tests/test_index.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14762 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/types/tests/test_series.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.064681 gwpy-3.0.3/gwpy/utils/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      933 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3723 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/decorators.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1490 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/enum.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1911 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/env.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8507 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3284 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/misc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5057 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1367 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/progress.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3396 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/shell.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.064681 gwpy-3.0.3/gwpy/utils/sphinx/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      770 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/sphinx/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3559 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/sphinx/epydoc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4763 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/sphinx/ex2rst.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3425 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/sphinx/zenodo.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.064681 gwpy-3.0.3/gwpy/utils/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2209 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/utils/tests/test_decorators.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2185 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/utils/tests/test_enum.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2000 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/tests/test_env.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3478 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/utils/tests/test_lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2610 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/utils/tests/test_misc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2062 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/utils/tests/test_mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2367 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/tests/test_shell.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2263 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/tests/test_sphinx_ex2rst.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10040 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       54 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/entry_points.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      793 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        5 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4844 2023-04-09 14:36:48.000000 gwpy-3.0.3/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       38 2023-04-09 14:51:14.064681 gwpy-3.0.3/setup.cfg
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)     2989 2023-04-06 10:37:11.000000 gwpy-3.0.3/setup_utils.py
```

### Comparing `gwpy-3.0.2/.codeclimate.yml` & `gwpy-3.0.3/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/.github/workflows/conda.yml` & `gwpy-3.0.3/.github/workflows/conda.yml`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,14 @@
     - name: Configure conda
       uses: conda-incubator/setup-miniconda@v2
       with:
         activate-environment: test
         miniforge-variant: Mambaforge
         python-version: ${{ matrix.python-version }}
         use-mamba: true
-        # this is needed for caching to work properly:
-        use-only-tar-bz2: true
 
     - name: Conda info
       run: conda info --all
 
     - name: Install dependencies with conda
       run: |
         # parse requirements to install as much as possible with conda
```

### Comparing `gwpy-3.0.2/.github/workflows/dependencies.yml` & `gwpy-3.0.3/.github/workflows/dependencies.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/.github/workflows/dist.yml` & `gwpy-3.0.3/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/.github/workflows/lint.yml` & `gwpy-3.0.3/.github/workflows/lint.yml`

 * *Files 6% similar despite different names*

```diff
@@ -48,11 +48,19 @@
       uses: actions/setup-python@v2
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install \
-            "rstcheck[sphinx,toml]>=6.0.0" \
+            "rstcheck[sphinx]>=6.0.0" \
         ;
+    - name: List packages
+      run: python -m pip list installed
     - name: Lint with rstcheck
-      run: rstcheck . --recursive --report-level error
+      run: |
+        rstcheck . \
+            --config pyproject.toml \
+            --log-level DEBUG \
+            --recursive \
+            --report-level error \
+        ;
```

### Comparing `gwpy-3.0.2/.gitignore` & `gwpy-3.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/CONTRIBUTING.md` & `gwpy-3.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/LICENSE` & `gwpy-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/PKG-INFO` & `gwpy-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpy
-Version: 3.0.2
+Version: 3.0.3
 Summary: A python package for gravitational-wave astrophysics
 Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/gwpy/gwpy/issues
 Project-URL: Discussion Forum, https://gwpy.slack.com
 Project-URL: Documentation, https://gwpy.github.io/docs/
 Project-URL: Source Code, https://github.com/gwpy/gwpy
```

### Comparing `gwpy-3.0.2/README.md` & `gwpy-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/Makefile` & `gwpy-3.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/_static/css/gwpy-sphinx.css` & `gwpy-3.0.3/docs/_static/css/gwpy-sphinx.css`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/_static/favicon.png` & `gwpy-3.0.3/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/_static/gwpy_white_24.png` & `gwpy-3.0.3/docs/_static/gwpy_white_24.png`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/_templates/autoclass/class.rst` & `gwpy-3.0.3/docs/_templates/autoclass/class.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/_templates/autosummary/class.rst` & `gwpy-3.0.3/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/_templates/autosummary/module.rst` & `gwpy-3.0.3/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/astro/index.rst` & `gwpy-3.0.3/docs/astro/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/citing.rst.in` & `gwpy-3.0.3/docs/citing.rst.in`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/cli/index.rst` & `gwpy-3.0.3/docs/cli/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/conf.py` & `gwpy-3.0.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,17 +325,17 @@
 
 ${titleunderline}
 ${title}
 ${titleunderline}
 
 ${description}
 
-.. code:: sh
+.. code-block:: shell
 
-   $$ ${command}
+   ${command}
 
 .. plot::
    :align: center
    :alt: ${title}
    :context: reset
    :format: python
    :include-source: false
@@ -353,15 +353,19 @@
     except FileNotFoundError:
         return True
 
 
 def _render_cli_example(config, section, outdir, logger):
     """Render a :mod:`gwpy.cli` example as RST to be processed by Sphinx.
     """
-    raw = config.get(section, 'command') + " --interactive"
+    # read config values (allow for multi-line definition)
+    raw = config.get(
+        section,
+        'command',
+    ).strip().replace("\n", " ") + " --interactive"
     title = config.get(
         section,
         'title',
         fallback=' '.join(map(str.title, section.split('-'))),
     )
     desc = config.get(section, 'description', fallback='')
```

### Comparing `gwpy-3.0.2/docs/detector/channel.rst` & `gwpy-3.0.3/docs/detector/channel.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/dev/release.rst` & `gwpy-3.0.3/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/env.rst` & `gwpy-3.0.3/docs/env.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.3/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/gwpy-docs-logo.png` & `gwpy-3.0.3/docs/gwpy-docs-logo.png`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/index.rst` & `gwpy-3.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/overview.rst` & `gwpy-3.0.3/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/plot/colorbars.rst` & `gwpy-3.0.3/docs/plot/colorbars.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/plot/colors.rst` & `gwpy-3.0.3/docs/plot/colors.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/plot/filter.rst` & `gwpy-3.0.3/docs/plot/filter.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/plot/gps.rst` & `gwpy-3.0.3/docs/plot/gps.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/plot/index.rst` & `gwpy-3.0.3/docs/plot/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/plot/legend.rst` & `gwpy-3.0.3/docs/plot/legend.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/plot/log.rst` & `gwpy-3.0.3/docs/plot/log.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/references.rst` & `gwpy-3.0.3/docs/references.rst`

 * *Files 3% similar despite different names*

```diff
@@ -50,31 +50,28 @@
 .. |cWBl| replace:: coherent WaveBurst (cWB)
 .. _cWBl: https://gwburst.gitlab.io/documentation/latest/html/
 
 .. |framel| replace:: `framel`
 .. _framel: http://lappweb.in2p3.fr/virgo/FrameL/
 
 .. |LDAStools.frameCPP| replace:: `LDAStools.frameCPP`
-.. _LDAStools.frameCPP: https://ldas-jobs.ligo.caltech.edu/~emaros/share/doc/ldas-tools/framecpp/html/
+.. _LDAStools.frameCPP: https://computing.docs.ligo.org/ldastools/LDAS_Tools/ldas-tools-framecpp/
 
 .. |lal| replace:: `lal`
 .. _lal: http://software.ligo.org/docs/lalsuite/lal/
 
 .. |lal.LIGOTimeGPS| replace:: `lal.LIGOTimeGPS`
 .. _lal.LIGOTimeGPS: http://software.ligo.org/docs/lalsuite/lal/struct_l_i_g_o_time_g_p_s.html
 
 .. |lalframe| replace:: `lalframe`
 .. _lalframe: http://software.ligo.org/docs/lalsuite/lalframe/
 
 .. |MySQLdb| replace:: `MySQLdb`
 .. _MySQLdb: http://mysql-python.sourceforge.net/
 
-.. |nds2| replace:: `nds2`
-.. _nds2: https://www.lsc-group.phys.uwm.edu/daswg/projects/nds-client/doc/manual/
-
 .. |numpydoc| replace:: `numpydoc`
 .. _numpydoc: https://numpydoc.readthedocs.io/
 
 .. |python-ligo-lw| replace:: `python-ligo-lw`
 .. _python-ligo-lw: https://git.ligo.org/kipp.cannon/python-ligo-lw
 
 .. |pycbc| replace:: PyCBC
@@ -91,14 +88,19 @@
 
 .. |sphinx-automodapi| replace:: `sphinx-automodapi`
 .. _sphinx-automodapi: http://sphinx-automodapi.readthedocs.io/
 
 .. |uproot| replace:: `uproot`
 .. _uproot: https://uproot.readthedocs.io/
 
+.. -- Documents ---------------------------------
+
+.. |GWFSpec| replace:: LIGO-T970130
+.. _GWFSpec: https://dcc.ligo.org/LIGO-T970130/public
+
 .. -- Other references --------------------------
 
 .. |GravitySpy| replace:: Gravity Spy
 .. _GravitySpy: https://gravityspy.org
 
 .. |GWOSCl| replace:: The Gravitational-Wave Open Science Centre (GWOSC)
 .. _GWOSCl: https://www.gw-openscience.org/
```

### Comparing `gwpy-3.0.2/docs/segments/dqsegdb.rst` & `gwpy-3.0.3/docs/segments/dqsegdb.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/segments/index.rst` & `gwpy-3.0.3/docs/segments/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/segments/io.rst` & `gwpy-3.0.3/docs/segments/io.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/segments/thresholding.rst` & `gwpy-3.0.3/docs/segments/thresholding.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/signal/index.rst` & `gwpy-3.0.3/docs/signal/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/spectrogram/index.rst` & `gwpy-3.0.3/docs/spectrogram/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/spectrum/index.rst` & `gwpy-3.0.3/docs/spectrum/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/spectrum/io.rst` & `gwpy-3.0.3/docs/spectrum/io.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.3/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/table/filter.rst` & `gwpy-3.0.3/docs/table/filter.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/table/histogram.rst` & `gwpy-3.0.3/docs/table/histogram.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/table/index.rst` & `gwpy-3.0.3/docs/table/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/table/io.rst` & `gwpy-3.0.3/docs/table/io.rst`

 * *Files 1% similar despite different names*

```diff
@@ -618,15 +618,16 @@
 .. _gwpy-table-io-gstlal:
 
 ========================
 GstLAL (``LIGO_LW`` XML)
 ========================
 
 GstLAL is a low-latency search for gravitational waves from compact
-binary coalescences, built using |GStreamer|_ elements and tools from the |LALSuite|_ library.
+binary coalescences, built using |GStreamer|_ elements and tools from the
+:ref:`gwpy-external-lalsuite` library.
 This search writes files on the LIGO Data Grid (LIGO.ORG-authenticated users
 only) in ``LIGO_LW`` XML format, containing tables of events.
 
 Reading
 -------
 
 To read an `EventTable` from a ``gstlal`` format ``LIGO_LW`` XML file, use the
@@ -743,15 +744,15 @@
 
 .. _gwpy-table-io-gwf:
 
 ===
 GWF
 ===
 
-**Additional dependencies:** |LDAStools.frameCPP|_
+**Additional dependencies:** :ref:`gwpy-external-framecpp`
 
 The Gravitational-Wave Frame file format supports tabular data via
 ``FrEvent`` structures, which allow storage of arbitrary event information.
 
 Reading
 -------
 
@@ -772,15 +773,15 @@
 
    >>> t = EventTable.read('events.gwf', 'my-event-name', columns=['time', 'amplitude'])
 
 All ``FrEvent`` structures contain the following columns, any other
 columns are use-specific:
 
 ===============  ====================================================================================
-Column name      Description (from `LIGO-T970130 <https://dcc.ligo.org/LIGO-T970130/public>`_)
+Column name      Description (from |GWFSpec|_)
 ===============  ====================================================================================
 ``time``         Reference time of event, as defined by the search algorithm
 ``amplitude``    Continuous output amplitude returned by event
 ``probability``  Likelihood estimate of event, if available (probability = -1 if cannot be estimated)
 ``timeBefore``   Signal duration before reference time (seconds)
 ``timeAfter``    Signal duration after reference time (seconds)
 ``comment``      Descriptor of event
```

### Comparing `gwpy-3.0.2/docs/table/plot.rst` & `gwpy-3.0.3/docs/table/plot.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/table/rate.rst` & `gwpy-3.0.3/docs/table/rate.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/time/index.rst` & `gwpy-3.0.3/docs/time/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/timeseries/datafind.rst` & `gwpy-3.0.3/docs/timeseries/datafind.rst`

 * *Files 2% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
 The full data set for each detector is archived at the relevant observatory
 and is made freely available to all registered collaboration members.
 A discovery service called |gwdatafind|_ is provided at each location to
 simplify discovering the file(s) that contain the data of interest for any
 research.
 
-These data are also made available remotely using |nds2|_, which enables
-sending data directly over a network to any location.
+These data are also made available remotely using :ref:`gwpy-external-nds2`,
+which enables sending data directly over a network to any location.
 This is used for both the full proprietary data (which requires an
 authorisation credential to access) and also the |GWOSC_AUX_RELEASE|_
 (which is freely available).
 
 .. _gwpy-timeseries-get:
 
 **********************
 :meth:`TimeSeries.get`
 **********************
 
-**Additional dependencies:** |LDAStools.frameCPP|_ or |nds2|_
+**Additional dependencies:** :ref:`gwpy-external-framecpp` or :ref:`gwpy-external-nds2`
 
 GWpy provides the :meth:`TimeSeries.get` method as a one-stop interface
 to all automatically-discoverable data hosted locally at an IGWN
 computing centre, or available remotely.
 
 ============
 How it works
```

### Comparing `gwpy-3.0.2/docs/timeseries/index.rst` & `gwpy-3.0.3/docs/timeseries/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/timeseries/io.rst` & `gwpy-3.0.3/docs/timeseries/io.rst`

 * *Files 6% similar despite different names*

```diff
@@ -41,26 +41,26 @@
 
 Gravitational-wave detector data, including all engineering diagnostic data
 as well as the calibrated 'strain' data that are searched for GW signals,
 are archived in :ref:`GWF <gwpy-timeseries-io-gwf>` files stored at the
 relevant observatory.
 These data are available locally to authenticated users of the associated
 computing centres (typically collaboration members), but are also
-distributed using |CVMFS|_ and are available remotely using |nds2|_.
+distributed using |CVMFS|_ and are available remotely using :ref:`gwpy-external-nds2`.
 Access to these data is restricted to active collaboration members.
 
 Additionally |GWOSCl|_ hosts publicly-accessible 'open' data, with *event*
 datasets made available at the same time as the relevant result publication
 and typically including ~1 hour of data around each published event detection,
 and *bulk* datasets with the entire observing run data available roughly
 18 months after the end of the run.
 
 GWOSC also hosts the |GWOSC_AUX_RELEASE|_, providing public access to
 environmental sensor data around |GW170814|_.
-These data are freely accessible using |nds2|_.
+These data are freely accessible using :ref:`gwpy-external-nds2`.
 
 ======================
 Data discovery methods
 ======================
 
 .. toctree::
 
@@ -105,17 +105,30 @@
 
 .. _gwpy-timeseries-io-gwf:
 
 ===
 GWF
 ===
 
-**Additional dependencies:**  |LDAStools.frameCPP|_ or |framel|_ or |lalframe|_
+**Additional dependencies:**  :ref:`gwpy-external-framecpp` or :ref:`gwpy-external-framel` or :ref:`gwpy-external-lalframe`
 
-The raw observatory data are archived in ``.gwf`` files, a custom binary format that efficiently stores the time streams and all necessary metadata, for more details about this particular data format, take a look at the specification document `LIGO-T970130 <https://dcc.ligo.org/LIGO-T970130/public>`_.
+The raw observatory data are archived in ``.gwf`` files, a custom binary format that efficiently stores the time streams and all necessary metadata, for more details about this particular data format, take a look at the specification document |GWFSpec|_.
+
+GWF library availability
+------------------------
+
+GWpy can use any of the three named GWF input/output libraries, and will try
+to find them in the order they are listed
+(FrameCPP first, then FrameL, then LALFrame).
+If you need to read/write GWF files, any of them will work, but re recommend
+to try and install the libraries in that order; FrameCPP provides a more
+complete Python API than the others.
+
+However, not all libraries may be available on all platforms, the linked pages
+for each library include an up-to-date listing of the supported platforms.
 
 Reading
 -------
 
 To read data from a GWF file, pass the input file path (or paths) and the name of the data channel to read:
 
 .. code-block:: python
@@ -193,32 +206,14 @@
 
 .. code-block:: python
 
    >>> data.write('output.gwf')
 
 **If the output file already exists it will be overwritten.**
 
-GWF library availability
-------------------------
-
-(Last we checked...) The three GWF library interfaces are available on
-the following platforms:
-
-.. table:: GWF library availability by platform
-   :align: left
-   :name: gwf-library-platforms
-
-   =====================  ==============================  =====  =====  =======
-   Library                Conda-forge package name        Linux  macOS  Windows
-   =====================  ==============================  =====  =====  =======
-   |LDASTools.frameCPP|_  ``python-ldas-tools-framecpp``  Yes    Yes    No
-   |framel|_              ``python-framel``               Yes    Yes    Yes
-   |lalframe|_            ``python-lalframe``             Yes    Yes    No
-   =====================  ==============================  =====  =====  =======
-
 .. _gwpy-timeseries-io-hdf5:
 
 ====
 HDF5
 ====
 
 GWpy allows storing data in HDF5 format files, using a custom specification for storage of metadata.
```

### Comparing `gwpy-3.0.2/docs/timeseries/opendata.rst` & `gwpy-3.0.3/docs/timeseries/opendata.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/timeseries/plot.rst` & `gwpy-3.0.3/docs/timeseries/plot.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/docs/timeseries/statevector.rst` & `gwpy-3.0.3/docs/timeseries/statevector.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/frequencyseries/coherence.py` & `gwpy-3.0.3/examples/frequencyseries/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/frequencyseries/hoff.py` & `gwpy-3.0.3/examples/frequencyseries/hoff.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/frequencyseries/inject.py` & `gwpy-3.0.3/examples/frequencyseries/inject.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/frequencyseries/percentiles.py` & `gwpy-3.0.3/examples/frequencyseries/percentiles.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/frequencyseries/rayleigh.py` & `gwpy-3.0.3/examples/frequencyseries/rayleigh.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/frequencyseries/transfer_function.py` & `gwpy-3.0.3/examples/frequencyseries/transfer_function.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/frequencyseries/variance.py` & `gwpy-3.0.3/examples/frequencyseries/variance.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/miscellaneous/open-data-spectrogram.py` & `gwpy-3.0.3/examples/miscellaneous/open-data-spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/miscellaneous/range-spectrogram.py` & `gwpy-3.0.3/examples/miscellaneous/range-spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/miscellaneous/range-timeseries.py` & `gwpy-3.0.3/examples/miscellaneous/range-timeseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/segments/open-data.py` & `gwpy-3.0.3/examples/segments/open-data.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/signal/gw150914.py` & `gwpy-3.0.3/examples/signal/gw150914.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/signal/qscan.py` & `gwpy-3.0.3/examples/signal/qscan.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,41 +43,49 @@
 gps = datasets.event_gps('GW170817')
 data = TimeSeries.fetch_open_data('L1', gps-34, gps+34)
 
 # We can Q-transform these data and scan over time-frequency planes to
 # find the one with the most significant tile near the time of merger:
 
 from gwpy.segments import Segment
-search = Segment(gps-0.25, gps+0.25)
-qgram = data.q_gram(qrange=(4, 150), search=search, mismatch=0.35)
+qgram = data.q_gram(
+    qrange=(4, 150),
+    search=Segment(gps-0.25, gps+0.25),
+    mismatch=0.35,
+)
 
 # .. note::
 #
 #    To recover as much signal as possible, in practice we should suppress
 #    background noise by whitening the data before the Q-transform. This
 #    can be done with :meth:`TimeSeries.whiten`.
 
 # Finally, we can plot the loudest time-frequency plane, focusing on a
 # specific window around the merger time:
 
-from matplotlib.cm import get_cmap
-cmap = get_cmap('viridis')
-plot = qgram.tile('time', 'frequency', 'duration', 'bandwidth',
-                  color='energy', figsize=[8, 4], linewidth=0.1,
-                  edgecolor=cmap(0), antialiased=True)
+plot = qgram.tile(
+    'time',
+    'frequency',
+    'duration',
+    'bandwidth',
+    color='energy',
+)
 ax = plot.gca()
 ax.set_xscale('seconds')
 ax.set_xlim(gps-6, gps+1)
 ax.set_epoch(gps)
 ax.set_yscale('log')
 ax.set_ylim(16, 1024)
 ax.set_ylabel('Frequency [Hz]')
 ax.grid(True, axis='y', which='both')
-ax.colorbar(cmap='viridis', label='Normalized energy', clim=[0, 25])
-cmap = get_cmap('viridis')
-ax.set_facecolor(cmap(0))
+
+from matplotlib import colormaps
+cmap = colormaps['viridis']
+ax.colorbar(cmap=cmap.name, label='Normalized energy', clim=[0, 50])
+ax.set_facecolor(cmap(0))  # colour background to the bottom of the map
+
 plot.show()
 
 # Here we can clearly see the trace of a binary neutron star merger, sweeping
 # up in frequency through a loud saturation glitch in the foreground.
 # For more details on this result, please see
-# https://www.gw-openscience.org/catalog/GWTC-1-confident/single/GW170817/.
+# the 'Science Summary' for |GW170817|_.
```

### Comparing `gwpy-3.0.2/examples/spectrogram/coherence.py` & `gwpy-3.0.3/examples/spectrogram/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/spectrogram/plot.py` & `gwpy-3.0.3/examples/spectrogram/plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/spectrogram/ratio.py` & `gwpy-3.0.3/examples/spectrogram/ratio.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/spectrogram/rayleigh.py` & `gwpy-3.0.3/examples/spectrogram/rayleigh.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/spectrogram/spectrogram2.py` & `gwpy-3.0.3/examples/spectrogram/spectrogram2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.3/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/table/histogram.py` & `gwpy-3.0.3/examples/table/histogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/table/rate.py` & `gwpy-3.0.3/examples/table/rate.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/table/rate_binned.py` & `gwpy-3.0.3/examples/table/rate_binned.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/table/scatter.py` & `gwpy-3.0.3/examples/table/scatter.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/table/tiles.py` & `gwpy-3.0.3/examples/table/tiles.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/test_examples.py` & `gwpy-3.0.3/examples/test_examples.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/timeseries/blrms.py` & `gwpy-3.0.3/examples/timeseries/blrms.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/timeseries/correlate.py` & `gwpy-3.0.3/examples/timeseries/correlate.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/timeseries/filter.py` & `gwpy-3.0.3/examples/timeseries/filter.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/timeseries/inject.py` & `gwpy-3.0.3/examples/timeseries/inject.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/timeseries/public.py` & `gwpy-3.0.3/examples/timeseries/public.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/timeseries/pycbc-snr.py` & `gwpy-3.0.3/examples/timeseries/pycbc-snr.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/timeseries/qscan.py` & `gwpy-3.0.3/examples/timeseries/qscan.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/timeseries/statevector.py` & `gwpy-3.0.3/examples/timeseries/statevector.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/examples/timeseries/whiten.py` & `gwpy-3.0.3/examples/timeseries/whiten.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/__init__.py` & `gwpy-3.0.3/gwpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/astro/__init__.py` & `gwpy-3.0.3/gwpy/astro/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/astro/range.py` & `gwpy-3.0.3/gwpy/astro/range.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/astro/tests/__init__.py` & `gwpy-3.0.3/gwpy/astro/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/astro/tests/test_range.py` & `gwpy-3.0.3/gwpy/astro/tests/test_range.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,17 +85,19 @@
 
 
 # -- inspiral-range -----------------------------
 
 
 @mock.patch.dict("sys.modules", {"inspiral_range": None})
 def test_inspiral_range_missing_dep(psd):
-    with pytest.raises(ModuleNotFoundError) as exc:
+    with pytest.raises(
+        ModuleNotFoundError,
+        match="extra package 'inspiral-range'",
+    ):
         astro.inspiral_range(psd)
-    assert "'inspiral-range'" in str(exc.value)
 
 
 @pytest.mark.requires("inspiral_range")
 def test_inspiral_range_psd(psd):
     """Test for :func:`gwpy.astro.inspiral_range_psd`
     """
     frange = (psd.frequencies.value < 4096)
@@ -203,11 +205,12 @@
 
 
 @pytest.mark.parametrize('range_func', [
     astro.range_timeseries,
     astro.range_spectrogram,
 ])
 def test_range_incompatible_input(range_func):
-    with pytest.raises(TypeError) as exc:
+    with pytest.raises(
+        TypeError,
+        match="Could not produce a spectrogram from the input",
+    ):
         range_func(2, 0.5)
-    assert str(exc.value).startswith(
-        'Could not produce a spectrogram from the input')
```

### Comparing `gwpy-3.0.2/gwpy/cli/__init__.py` & `gwpy-3.0.3/gwpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/cliproduct.py` & `gwpy-3.0.3/gwpy/cli/cliproduct.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/coherence.py` & `gwpy-3.0.3/gwpy/cli/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/coherencegram.py` & `gwpy-3.0.3/gwpy/cli/coherencegram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/gwpy_plot.py` & `gwpy-3.0.3/gwpy/cli/gwpy_plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/qtransform.py` & `gwpy-3.0.3/gwpy/cli/qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/spectrogram.py` & `gwpy-3.0.3/gwpy/cli/spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/spectrum.py` & `gwpy-3.0.3/gwpy/cli/spectrum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/tests/__init__.py` & `gwpy-3.0.3/gwpy/cli/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/tests/base.py` & `gwpy-3.0.3/gwpy/cli/tests/base.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/tests/test_coherence.py` & `gwpy-3.0.3/gwpy/cli/tests/test_coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/tests/test_coherencegram.py` & `gwpy-3.0.3/gwpy/cli/tests/test_coherencegram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/tests/test_gwpy_plot.py` & `gwpy-3.0.3/gwpy/cli/tests/test_gwpy_plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/tests/test_qtransform.py` & `gwpy-3.0.3/gwpy/cli/tests/test_qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/tests/test_spectrogram.py` & `gwpy-3.0.3/gwpy/cli/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/tests/test_spectrum.py` & `gwpy-3.0.3/gwpy/cli/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/tests/test_timeseries.py` & `gwpy-3.0.3/gwpy/cli/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/tests/test_transferfunction.py` & `gwpy-3.0.3/gwpy/cli/tests/test_transferfunction.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/timeseries.py` & `gwpy-3.0.3/gwpy/cli/timeseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/cli/transferfunction.py` & `gwpy-3.0.3/gwpy/cli/transferfunction.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/conftest.py` & `gwpy-3.0.3/gwpy/conftest.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/detector/__init__.py` & `gwpy-3.0.3/gwpy/detector/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/detector/channel.py` & `gwpy-3.0.3/gwpy/detector/channel.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/detector/io/__init__.py` & `gwpy-3.0.3/gwpy/detector/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/detector/io/cis.py` & `gwpy-3.0.3/gwpy/detector/io/cis.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/detector/io/clf.py` & `gwpy-3.0.3/gwpy/detector/io/clf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/detector/io/omega.py` & `gwpy-3.0.3/gwpy/detector/io/omega.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/detector/tests/__init__.py` & `gwpy-3.0.3/gwpy/detector/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/detector/tests/test_channel.py` & `gwpy-3.0.3/gwpy/detector/tests/test_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,25 +167,26 @@
         new = self.TEST_CLASS('test', model=arg)
         assert new.model == model
 
     @pytest.mark.parametrize('arg, type_, ndstype', [
         (None, None, None),
         ('m-trend', 'm-trend', 16),
         (8, 's-trend', 8),
-        ('blah', 'RAISE', '')
     ])
     def test_type_ndstype(self, arg, type_, ndstype):
-        if type_ == 'RAISE':  # check invalid raises correct exception
-            with pytest.raises(ValueError) as exc:
-                c = self.TEST_CLASS('', type=arg)
-            assert str(exc.value) == f'{arg!r} is not a valid Nds2ChannelType'
-        else:
-            c = self.TEST_CLASS('', type=arg)
-            assert getattr(c, 'type') == type_
-            assert getattr(c, 'ndstype') == ndstype
+        c = self.TEST_CLASS('', type=arg)
+        assert getattr(c, 'type') == type_
+        assert getattr(c, 'ndstype') == ndstype
+
+    def test_type_ndstype_error(self):
+        with pytest.raises(
+            ValueError,
+            match="^'blah' is not a valid Nds2ChannelType$",
+        ):
+            self.TEST_CLASS('', type="blah")
 
     @pytest.mark.parametrize('arg, dtype', [
         (None, None),
         (16, numpy.dtype('float64')),
         (float, numpy.dtype('float64')),
         ('float', numpy.dtype('float64')),
         ('float64', numpy.dtype('float64')),
@@ -195,25 +196,26 @@
         new = self.TEST_CLASS('test', dtype=arg)
         assert new.dtype is dtype
 
     @pytest.mark.parametrize('url', [
         None,
         'https://blah',
         'file://local/path',
+    ])
+    def test_url(self, url):
+        new = self.TEST_CLASS('test', url=url)
+        assert new.url == url
+
+    @pytest.mark.parametrize('url', [
         'BAD',
         1,
     ])
-    def test_url(self, url):
-        if url is not None and not str(url).startswith(('http', 'file')):
-            with pytest.raises(ValueError) as exc:
-                new = self.TEST_CLASS('test', url=url)
-            assert str(exc.value) == f"Invalid URL {url!r}"
-        else:
-            new = self.TEST_CLASS('test', url=url)
-            assert new.url == url
+    def test_url_error(self, url):
+        with pytest.raises(ValueError, match=f"^Invalid URL {url!r}$"):
+            self.TEST_CLASS('test', url=url)
 
     def test_frametype(self):
         new = self.TEST_CLASS('test', frametype='BLAH')
         assert new.frametype == 'BLAH'
 
     @pytest.mark.parametrize('name, texname', [
         ('X1:TEST', 'X1:TEST'),
@@ -294,18 +296,22 @@
     def test_parse_channel_name(self, name, pdict):
         # check empty parse via __init__
         c = self.TEST_CLASS('')
         for key in pdict:
             assert getattr(c, key) is None
 
         # check errors
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match=(
+                "^Cannot parse channel name according to "
+                "LIGO channel-naming convention T990033$"
+            ),
+        ):
             self.TEST_CLASS.parse_channel_name('blah')
-        assert str(exc.value) == ('Cannot parse channel name according to '
-                                  'LIGO channel-naming convention T990033')
 
         # check parsing returns expected result
         assert self.TEST_CLASS.parse_channel_name(name) == pdict
 
         # check parsing translates to attributes
         c = self.TEST_CLASS(name)
         for key in pdict:
@@ -345,21 +351,23 @@
                 assert c.name == 'X1:TEST-CHANNEL'
                 assert c.unit == units.m
                 assert c.sample_rate == 16384 * units.Hz
                 assert c.dtype == numpy.dtype('float32')
                 assert c.model == 'x1model'
                 assert c.url == 'https://cis.ligo.org/channel/123456'
             else:
-                with pytest.raises(ValueError) as exc:
+                with pytest.raises(
+                    ValueError,
+                    match=f"^No channels found matching {name!r}$",
+                ):
                     self.TEST_CLASS.query(
                         name,
                         kerberos=False,
                         idp="https://idp.example.com/profile/SAML2/SOAP/ECP",
                     )
-                assert str(exc.value) == f'No channels found matching {name!r}'
 
     @pytest.mark.parametrize('name', ('X1:TEST-CHANNEL', 'Y1:TEST_CHANNEL'))
     @pytest.mark.requires("nds2")
     def test_query_nds2(self, name):
         # mock NDS2 query
         ndsb = mocks.nds2_buffer('X1:TEST-CHANNEL', [], 0, 64, 'm')
         if ndsb.name == name:
```

### Comparing `gwpy-3.0.2/gwpy/detector/tests/test_units.py` & `gwpy-3.0.3/gwpy/detector/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/detector/units.py` & `gwpy-3.0.3/gwpy/detector/units.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/__init__.py` & `gwpy-3.0.3/gwpy/frequencyseries/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/_fdcommon.py` & `gwpy-3.0.3/gwpy/frequencyseries/_fdcommon.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/frequencyseries.py` & `gwpy-3.0.3/gwpy/frequencyseries/frequencyseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/hist.py` & `gwpy-3.0.3/gwpy/frequencyseries/hist.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/io/__init__.py` & `gwpy-3.0.3/gwpy/frequencyseries/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/io/ascii.py` & `gwpy-3.0.3/gwpy/frequencyseries/io/ascii.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/io/hdf5.py` & `gwpy-3.0.3/gwpy/frequencyseries/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/io/ligolw.py` & `gwpy-3.0.3/gwpy/frequencyseries/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/tests/__init__.py` & `gwpy-3.0.3/gwpy/frequencyseries/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/tests/test_frequencyseries.py` & `gwpy-3.0.3/gwpy/frequencyseries/tests/test_frequencyseries.py`

 * *Files 3% similar despite different names*

```diff
@@ -274,29 +274,32 @@
             ligolw,
             channel="X1:TEST-CHANNEL_2",
         )
         assert list(array.value) == [10, 20, 30, 40, 50]
         assert array.epoch is None
 
     @pytest.mark.requires("ligo.lw")
-    def test_read_ligolw_error_multiple_array(self, ligolw):
+    @pytest.mark.parametrize(("args", "match"), [
+        # no name given, 'name' in error message
+        ([], "read: 'channel', 'epoch', 'f0', 'name'$"),
+        # name given, 'name' not in error message
+        (("PSD2",), "read: 'channel', 'epoch', 'f0'$"),
+    ])
+    def test_read_ligolw_error_multiple_array(self, args, match, ligolw):
         # assert errors
-        with pytest.raises(ValueError) as exc:  # multiple <Array> hits
-            FrequencySeries.read(ligolw)
-        assert "'name'" in str(exc.value)
-
-        with pytest.raises(ValueError) as exc:  # multiple <Array> hits
-            FrequencySeries.read(ligolw, "PSD2")
-        assert "'epoch" in str(exc.value) and "'name'" not in str(exc.value)
+        with pytest.raises(
+            ValueError,
+            match=match,
+        ):  # multiple <Array> hits
+            FrequencySeries.read(ligolw, *args)
 
     @pytest.mark.requires("ligo.lw")
     def test_read_ligolw_error_no_array(self, ligolw):
-        with pytest.raises(ValueError) as exc:  # no hits
+        with pytest.raises(ValueError, match="^no <Array> elements found"):
             FrequencySeries.read(ligolw, "blah")
-        assert str(exc.value).startswith("no <Array> elements found")
 
     @pytest.mark.requires("ligo.lw")
     def test_read_ligolw_error_no_match(self, ligolw):
         with pytest.raises(ValueError):  # wrong epoch
             FrequencySeries.read(ligolw, epoch=0)
 
         with pytest.raises(ValueError):  # <Param>s don't match
```

### Comparing `gwpy-3.0.2/gwpy/frequencyseries/tests/test_hist.py` & `gwpy-3.0.3/gwpy/frequencyseries/tests/test_hist.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,19 @@
             array[0::2, 0],
             self.TEST_CLASS._rowclass(
                 array.value[0::2, 0], x0=array.x0, dx=array.dx*2,
                 name=array.name, unit=array.unit, channel=array.channel,
                 epoch=array.epoch,
             ),
         )
-        with pytest.raises(NotImplementedError) as exc:
+        with pytest.raises(
+            NotImplementedError,
+            match="^cannot slice SpectralVariance across bins$",
+        ):
             array[0, ::2]
-        assert str(exc.value) == 'cannot slice SpectralVariance across bins'
 
     # -- test methods ---------------------------
 
     def test_init(self, array):
         utils.assert_array_equal(array.value, self.data)
         utils.assert_array_equal(array.bins.value, self.bins)
         assert array.x0 == 0 * units.Hertz
```

### Comparing `gwpy-3.0.2/gwpy/io/__init__.py` & `gwpy-3.0.3/gwpy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/cache.py` & `gwpy-3.0.3/gwpy/io/cache.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/datafind.py` & `gwpy-3.0.3/gwpy/io/datafind.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/ffldatafind.py` & `gwpy-3.0.3/gwpy/io/ffldatafind.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/gwf.py` & `gwpy-3.0.3/gwpy/io/gwf.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,15 @@
     compression : `int`, `str`, optional
         name of compresion algorithm to use, or its endian-appropriate
         ID, choose from
 
         - ``'RAW'``
         - ``'GZIP'``
         - ``'DIFF_GZIP'``
-        - ``'ZERO_SUPPRESS_WORD_2'``
-        - ``'ZERO_SUPPRESS_WORD_4'``
-        - ``'ZERO_SUPPRESS_WORD_8'``
+        - ``'ZERO_SUPPRESS'``
         - ``'ZERO_SUPPRESS_OTHERWISE_GZIP'``
 
     compression_level : `int`, optional
         compression level for given method, default is ``6`` for GZIP-based
         methods, otherwise ``0``
     """
     from LDAStools import frameCPP
```

### Comparing `gwpy-3.0.2/gwpy/io/hdf5.py` & `gwpy-3.0.3/gwpy/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/kerberos.py` & `gwpy-3.0.3/gwpy/io/kerberos.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/ligolw.py` & `gwpy-3.0.3/gwpy/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/mp.py` & `gwpy-3.0.3/gwpy/io/mp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/nds2.py` & `gwpy-3.0.3/gwpy/io/nds2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/registry.py` & `gwpy-3.0.3/gwpy/io/registry.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/tests/__init__.py` & `gwpy-3.0.3/gwpy/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/tests/test_cache.py` & `gwpy-3.0.3/gwpy/io/tests/test_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,34 +204,44 @@
 
 
 def test_filename_metadata_error():
     with pytest.raises(ValueError):
         io_cache.filename_metadata("A-B-0-4xml.gz")
 
 
-def test_file_segment():
+@pytest.mark.parametrize(("filename", "seg"), [
+    # basic
+    ("A-B-1-2.ext", Segment(1, 3)),
+    # multiple file extensions
+    ("A-B-1-2.ext.gz", Segment(1, 3)),
+    # non-integer
+    ("A-B-1.23-4.ext.gz", Segment(1.23, 5.23)),
+])
+def test_file_segment(filename, seg):
     """Test :func:`gwpy.io.cache.file_segment`
     """
-    # check basic
-    fs = io_cache.file_segment('A-B-1-2.ext')
+    fs = io_cache.file_segment(filename)
     assert isinstance(fs, Segment)
-    assert fs == Segment(1, 3)
+    assert fs == seg
 
     # check mutliple file extensions
     assert io_cache.file_segment('A-B-1-2.ext.gz') == (1, 3)
 
     # check floats (and multiple file extensions)
     assert io_cache.file_segment('A-B-1.23-4.ext.gz') == (1.23, 5.23)
 
-    # test errors
-    with pytest.raises(ValueError) as exc:
+
+def test_file_segment_errors():
+    """Test :func:`gwpy.io.cache.file_segment` error handling.
+    """
+    with pytest.raises(
+        ValueError,
+        match="^Failed to parse 'blah' as a LIGO-T050017-compatible filename$"
+    ):
         io_cache.file_segment('blah')
-    assert str(exc.value) == (
-        "Failed to parse 'blah' as a LIGO-T050017-compatible filename"
-    )
 
 
 def test_flatten(cache):
     """Test :func:`gwpy.io.cache.flatten`
     """
     # check flattened version of single cache is unchanged
     assert io_cache.flatten(cache) == cache
```

### Comparing `gwpy-3.0.2/gwpy/io/tests/test_datafind.py` & `gwpy-3.0.3/gwpy/io/tests/test_datafind.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,17 +103,19 @@
 # -- tests --------------------------------------------------------------------
 
 @mock.patch.dict("os.environ", clear=True)
 def test_gwdatafind_module_error():
     """Test that _gwdatafind_module() will propagate an exception if
     it can't work out how to find data.
     """
-    with pytest.raises(RuntimeError) as exc:
+    with pytest.raises(
+        RuntimeError,
+        match="^unknown datafind configuration",
+    ):
         io_datafind.find_frametype("TEST")
-    assert str(exc.value).startswith("unknown datafind configuration")
 
 
 # -- find_frametype
 
 @_mock_gwdatafind
 def test_find_frametype():
     """Test that `find_frametype` works with basic input.
@@ -148,43 +150,52 @@
 
 
 @_mock_gwdatafind
 def test_find_frametype_error_not_found():
     """Test that `find_frametype` raises the right error for a missing channel.
     """
     # test missing channel raises sensible error
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError,
+        match=(
+            r"^Cannot locate the following channel\(s\) "
+            "in any known frametype:\n    X1:TEST$"
+        )
+    ):
         io_datafind.find_frametype('X1:TEST', allow_tape=True)
-    assert str(exc.value) == (
-        'Cannot locate the following channel(s) '
-        'in any known frametype:\n    X1:TEST')
 
 
 @_mock_gwdatafind
 def test_find_frametype_error_bad_channel():
     """Test that `find_frametype` raises the right error when the channel
     name isn't parsable.
     """
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError,
+        match=(
+            "^Cannot parse interferometer prefix from channel name "
+            r"'bad channel name', cannot proceed with find\(\)$"
+        ),
+    ):
         io_datafind.find_frametype('bad channel name')
-    assert str(exc.value) == ('Cannot parse interferometer prefix '
-                              'from channel name \'bad channel name\','
-                              ' cannot proceed with find()')
 
 
 @_mock_gwdatafind
 def test_find_frametype_error_files_on_tape():
     """Test that `find_frametype` raises the right error when the only
     discovered data are on tape, and we asked for not on tape.
     """
     # check that allow_tape errors get handled properly
-    with mock.patch('gwpy.io.datafind.on_tape', return_value=True):
-        with pytest.raises(ValueError) as exc:
-            io_datafind.find_frametype('X1:TEST', allow_tape=False)
-        assert '[files on tape have not been checked' in str(exc.value)
+    patch = mock.patch('gwpy.io.datafind.on_tape', return_value=True)
+    raises = pytest.raises(
+        ValueError,
+        match=r"\[files on tape have not been checked",
+    )
+    with patch, raises:
+        io_datafind.find_frametype('X1:TEST', allow_tape=False)
 
 
 # -- find_best_frametype
 
 @_mock_gwdatafind
 def test_find_best_frametype():
     """Test that `find_best_frametype` works in general.
@@ -270,17 +281,16 @@
 
 @mock.patch(
     f"{GWDATAFIND_PATH}.find_latest",
     mock.MagicMock(side_effect=IndexError),
 )
 @_mock_gwdatafind
 def test_find_latest_error():
-    with pytest.raises(RuntimeError) as exc:
+    with pytest.raises(RuntimeError, match="^no files found for X-MISSING$"):
         io_datafind.find_latest("X1", "MISSING")
-    assert str(exc.value) == "no files found for X-MISSING"
 
 
 # -- find_types
 
 @mock.patch.dict("os.environ", MOCK_ENV)
 def test_find_types():
     """Check that `find_types` works with default arguments.
```

### Comparing `gwpy-3.0.2/gwpy/io/tests/test_ffldatafind.py` & `gwpy-3.0.3/gwpy/io/tests/test_ffldatafind.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/io/tests/test_gwf.py` & `gwpy-3.0.3/gwpy/io/tests/test_gwf.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,19 +103,22 @@
 def test_num_channels():
     assert io_gwf.num_channels(TEST_GWF_FILE) == 3
 
 
 @pytest.mark.requires("LDAStools.frameCPP")
 def test_get_channel_type():
     assert io_gwf.get_channel_type('L1:LDAS-STRAIN', TEST_GWF_FILE) == 'proc'
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError,
+        match=(
+            "^'X1:NOT-IN_FRAME' not found in table-of-contents "
+            f"for {TEST_GWF_FILE}$"
+        ),
+    ):
         io_gwf.get_channel_type('X1:NOT-IN_FRAME', TEST_GWF_FILE)
-    assert str(exc.value) == (
-        f"'X1:NOT-IN_FRAME' not found in table-of-contents for {TEST_GWF_FILE}"
-    )
 
 
 @pytest.mark.requires("LDAStools.frameCPP")
 def test_channel_in_frame():
     assert io_gwf.channel_in_frame('L1:LDAS-STRAIN', TEST_GWF_FILE) is True
     assert io_gwf.channel_in_frame('X1:NOT-IN_FRAME', TEST_GWF_FILE) is False
```

### Comparing `gwpy-3.0.2/gwpy/io/tests/test_kerberos.py` & `gwpy-3.0.3/gwpy/io/tests/test_kerberos.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,32 +55,36 @@
 def teardown_module():
     if MOCK_ENV is not None:
         MOCK_ENV.stop()
 
 
 @mock.patch('subprocess.check_output', return_value=KLIST)
 def test_parse_keytab(check_output):
-    """Test `gwpy.io.kerberos.parse_keytab
+    """Test `gwpy.io.kerberos.parse_keytab.
     """
     # assert principals get extracted correctly
     principals = io_kerberos.parse_keytab('test.keytab')
     assert principals == [('albert.einstein', 'LIGO.ORG', 1),
                           ('ronald.drever', 'LIGO.ORG', 2)]
 
-    # assert klist fail gets raise appropriately
-    check_output.side_effect = [
-        OSError('something'),
-        subprocess.CalledProcessError(1, 'something else'),
-    ]
-    with pytest.raises(io_kerberos.KerberosError) as exc:
-        io_kerberos.parse_keytab('test.keytab')
-    assert str(exc.value) == "Failed to locate klist, cannot read keytab"
-    with pytest.raises(io_kerberos.KerberosError) as exc:
+
+@mock.patch("subprocess.check_output")
+@pytest.mark.parametrize(("se", "match"), [
+    (OSError, "^Failed to locate klist, cannot read keytab$"),
+    (
+        subprocess.CalledProcessError(1, "error"),
+        "Cannot read keytab 'test.keytab'",
+    ),
+])
+def test_parse_keytab_oserror(mock_check_output, se, match):
+    """Test `gwpy.io.kerberos.parse_keytab` fails appropriately.
+    """
+    mock_check_output.side_effect = se
+    with pytest.raises(io_kerberos.KerberosError, match=match):
         io_kerberos.parse_keytab('test.keytab')
-    assert str(exc.value) == "Cannot read keytab 'test.keytab'"
 
 
 @mock.patch('sys.stdout.isatty', return_value=True)
 @mock.patch('gwpy.io.kerberos.input', return_value='rainer.weiss')
 @mock.patch('getpass.getpass', return_value='test')
 @mock.patch('subprocess.Popen')
 def test_kinit_up(popen, getpass, input_, _, capsys):
```

### Comparing `gwpy-3.0.2/gwpy/io/tests/test_ligolw.py` & `gwpy-3.0.3/gwpy/io/tests/test_ligolw.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,34 +115,38 @@
 
 def test_read_table(llwdoc_with_tables):
     tab = io_ligolw.read_table(llwdoc_with_tables, tablename="process")
     assert tab is llwdoc_with_tables.childNodes[0].childNodes[0]
 
 
 def test_read_table_empty(llwdoc):
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError,
+        match=r"^No tables found in LIGO_LW document\(s\)$",
+    ):
         io_ligolw.read_table(llwdoc)
-    assert str(exc.value) == "No tables found in LIGO_LW document(s)"
 
 
 @pytest.mark.requires("ligo.lw.lsctables")
 def test_read_table_ilwd(tmp_path):
     xmlpath = tmp_path / "test.xml"
     with open(xmlpath, "w") as f:
         f.write(OLD_FORMAT_LIGO_LW_XML)
     tab = io_ligolw.read_table(xmlpath, tablename="sngl_burst")
     assert len(tab) == 3
 
 
 def test_read_table_multiple(llwdoc_with_tables):
-    # check that read_table correctly errors on ambiguity
-    with pytest.raises(ValueError) as exc:
+    """Check that `gwpy.io.ligolw.read_table` correctly errors on ambiguity.
+    """
+    with pytest.raises(
+        ValueError,
+        match="^Multiple tables .* 'process', 'sngl_ringdown'",
+    ):
         io_ligolw.read_table(llwdoc_with_tables)
-    assert str(exc.value).startswith("Multiple tables")
-    assert "'process', 'sngl_ringdown'" in str(exc.value)
 
 
 def test_open_xmldoc(tmp_path, llwdoc_with_tables):
     tmp = tmp_path / "test.xml"
     # write a LIGO_LW file
     with open(tmp, "w") as fobj:
         llwdoc_with_tables.write(fobj)
```

### Comparing `gwpy-3.0.2/gwpy/io/tests/test_mp.py` & `gwpy-3.0.3/gwpy/io/tests/test_mp.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,17 +77,19 @@
     assert tab.colnames == ["a", "b", "c"]
     assert list(tab["a"]) == [7, 10, 1, 4]
 
 
 def test_read_multi_error_empty():
     """Check that an `IndexError` is raised when the input list is empty
     """
-    with pytest.raises(IndexError) as exc:
+    with pytest.raises(
+        IndexError,
+        match="^cannot read int from empty source list$",
+    ):
         io_mp.read_multi(1, int, [])
-    assert str(exc.value) == "cannot read int from empty source list"
 
 
 def test_read_multi_not_a_file():
     """Check that a strange input gets passed along properly
     so that errors can be raise by the reader.
     """
     with pytest.raises(TypeError):
```

### Comparing `gwpy-3.0.2/gwpy/io/tests/test_nds2.py` & `gwpy-3.0.3/gwpy/io/tests/test_nds2.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 
     def test_any(self):
         assert self.TEST_CLASS.any() == 2 * max(self.TEST_CLASS).value - 1
 
     def test_find_errors(self):
         """Test error raising for :meth:`gwpy.io.nds2.Nds2ChannelType.find`
         """
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match=f"'blah' is not a valid {self.TEST_CLASS.__name__}",
+        ):
             self.TEST_CLASS.find('blah')
-        assert str(exc.value) == (
-            f"'blah' is not a valid {self.TEST_CLASS.__name__}"
-        )
 
 
 class TestNds2ChannelType(_TestNds2Enum):
     """Tests of :class:`gwpy.io.nds2.Nds2DataType`
     """
     TEST_CLASS = io_nds2.Nds2ChannelType
 
@@ -219,17 +219,16 @@
 
 
 @pytest.mark.requires("nds2")
 @mock.patch('gwpy.io.nds2.connect', side_effect=RuntimeError('Anything else'))
 def test_auth_connect_error(connect):
     """Test errors from `gwpy.io.nds2.auth_connect`
     """
-    with pytest.raises(RuntimeError) as exc:
+    with pytest.raises(RuntimeError, match="Anything else"):
         io_nds2.auth_connect('host', 'port')
-    assert str(exc.value) == 'Anything else'
     connect.assert_called_once_with("host", "port")
 
 
 @mock.patch('gwpy.io.nds2.auth_connect', return_value=1)
 def test_open_connection(auth_connect):
     """Test the `gwpy.io.nds2.open_connection` decorator
     """
@@ -287,19 +286,19 @@
     onlinechan.channel_type = 1
     conn.find_channels.return_value = [chan, onlinechan]
     assert io_nds2.find_channels(['X1:test'], host='test',
                                  unique=True) == [chan]
 
     # test unique errors (with nds1 protocol)
     conn.find_channels.return_value = [chan, chan]  # any two channels
-    with pytest.raises(ValueError) as exc:
-        assert io_nds2.find_channels(['X1:test'], host='test',
-                                     unique=True) == [chan]
-    assert str(exc.value) == (
-        "unique NDS2 channel match not found for 'X1:test'")
+    with pytest.raises(
+        ValueError,
+        match="^unique NDS2 channel match not found for 'X1:test'$",
+    ):
+        io_nds2.find_channels(['X1:test'], host='test', unique=True)
 
 
 @pytest.mark.requires("nds2")
 @mock.patch('gwpy.io.nds2.find_channels', return_value=['X1:test'])
 @mock.patch('gwpy.io.nds2.auth_connect')
 def test_get_availability(auth_connect, _):
     """Test `gwpy.io.nds2.get_availability`
```

### Comparing `gwpy-3.0.2/gwpy/io/tests/test_utils.py` & `gwpy-3.0.3/gwpy/io/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,19 @@
 @pytest.mark.parametrize("badthing", (
     1,
     ["test.txt"],
 ))
 def test_file_path_errors(badthing):
     """Check that :func:`gwpy.io.utils.file_path` fails when expected
     """
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError,
+        match="^Cannot parse file name for ",
+    ):
         io_utils.file_path(badthing)
-    assert str(exc.value).startswith("Cannot parse file name for")
 
 
 @pytest.mark.requires("lal")
 def test_file_path_cacheentry():
     from lal.utils import CacheEntry
     path = "/path/to/A-B-0-1.txt"
     assert io_utils.file_path(CacheEntry.from_T050017(path)) == path
```

### Comparing `gwpy-3.0.2/gwpy/io/utils.py` & `gwpy-3.0.3/gwpy/io/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/__init__.py` & `gwpy-3.0.3/gwpy/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/axes.py` & `gwpy-3.0.3/gwpy/plot/axes.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/bode.py` & `gwpy-3.0.3/gwpy/plot/bode.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/colorbar.py` & `gwpy-3.0.3/gwpy/plot/colorbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,18 @@
                 continue
     raise ValueError("Cannot determine mappable layer on any axes "
                      "for this colorbar")
 
 
 def _get_axes_class(ax):
     if isinstance(ax, SubplotBase):
-        return ax._axes_class
+        try:  # matplotlib < 3.7.0
+            return ax._axes_class
+        except AttributeError:  # matplotlib >= 3.7.0
+            return type(ax)
     return type(ax)
 
 
 def _scale_width(value, ax):
     fig = ax.figure
     return value / (ax.get_position().width * fig.get_figwidth())
```

### Comparing `gwpy-3.0.2/gwpy/plot/colors.py` & `gwpy-3.0.3/gwpy/plot/colors.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/gps.py` & `gwpy-3.0.3/gwpy/plot/gps.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,29 @@
 """
 
 from decimal import Decimal
 from numbers import Number
 
 import numpy
 
-from matplotlib import (ticker, docstring)
+from matplotlib import ticker
 from matplotlib.scale import (register_scale, LinearScale, get_scale_names)
 from matplotlib.transforms import Transform
 try:
     from matplotlib.scale import _get_scale_docs as get_scale_docs
 except ImportError:  # matplotlib < 3.1
     from matplotlib.scale import get_scale_docs
+try:
+    from matplotlib import _docstring
+except ImportError:  # matplotlib < 3.6
+    try:
+        from matplotlib import docstring as _docstring
+    except ImportError:  # pragma: no cover
+        # maybe matplotlib >= 3.9?
+        _docstring = None
 
 from astropy import units
 
 from ..time import (to_gps, from_gps)
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
@@ -493,11 +501,15 @@
 
 for _unit in TIME_UNITS:
     if _unit is units.kiloyear:  # don't go past 'year' for GPSScale
         break
     register_gps_scale(_gps_scale_factory(_unit))
 
 # update the docstring for matplotlib scale methods
-docstring.interpd.update(
-    scale=' | '.join([repr(x) for x in get_scale_names()]),
-    scale_docs=get_scale_docs().rstrip(),
-)
+try:
+    _docstring.interpd.update(
+        scale=' | '.join([repr(x) for x in get_scale_names()]),
+        scale_docs=get_scale_docs().rstrip(),
+    )
+except AttributeError:  # pragma: no cover
+    # matplotlib._docstring changed/removed/not found
+    pass
```

### Comparing `gwpy-3.0.2/gwpy/plot/legend.py` & `gwpy-3.0.3/gwpy/plot/legend.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/log.py` & `gwpy-3.0.3/gwpy/plot/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # You should have received a copy of the GNU General Public License
 # along with GWpy.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module redefines the matplotlib log scale to give a more
 helpful set of major and minor ticks.
 """
 
-from math import (ceil, floor, log)
+from math import (ceil, floor, isclose, log)
 
 import numpy
 
 from matplotlib import (rcParams, ticker as mticker)
 from matplotlib.scale import (LogScale as _LogScale, register_scale)
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
@@ -104,15 +104,15 @@
 
         # determine whether to label or not
         sign = '-' if x < 0 else ''
         x = abs(x)
         b = self._base
         fx = log(x) / log(b)
 
-        is_x_decade = mticker.is_close_to_int(fx)
+        is_x_decade = isclose(fx, round(fx))
         if self.labelOnlyBase and not is_x_decade:
             return ''
 
         # work out whether to show this label
         # if there are enough major ticks or this formatter doesn't support
         # minor ticks, return a blank string
         exponent = numpy.round(fx) if is_x_decade else numpy.floor(fx)
```

### Comparing `gwpy-3.0.2/gwpy/plot/plot.py` & `gwpy-3.0.3/gwpy/plot/plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/rc.py` & `gwpy-3.0.3/gwpy/plot/rc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/segments.py` & `gwpy-3.0.3/gwpy/plot/segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/__init__.py` & `gwpy-3.0.3/gwpy/plot/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_axes.py` & `gwpy-3.0.3/gwpy/plot/tests/test_axes.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,46 +118,56 @@
 
     @pytest.mark.parametrize('sortbycolor', (False, True))
     def test_scatter_errors(self, ax, sortbycolor):
         # check that errors are handled properly
         x = 1
         y = 'B'
         c = 'something else'
-        with pytest.raises(ValueError) as exc:
-            ax.scatter(x, y, c=c, sortbycolor=sortbycolor)
         if sortbycolor:  # gwpy error
-            msg = "Axes.scatter argument 'sortbycolor'"
+            match = "^Axes.scatter argument 'sortbycolor'"
         else:  # matplotlib error
-            msg = "'c' argument must be a "
-        assert str(exc.value).startswith(msg)
+            match = "^'c' argument must be a "
+        with pytest.raises(ValueError, match=match):
+            ax.scatter(x, y, c=c, sortbycolor=sortbycolor)
 
     def test_imshow(self, ax):
         # standard imshow call
         array = numpy.random.random((10, 10))
         image2 = ax.imshow(array)
         utils.assert_array_equal(image2.get_array(), array)
-        assert image2.get_extent() == (-.5, array.shape[0]-.5,
-                                       array.shape[1]-.5, -.5)
+        assert tuple(image2.get_extent()) == (
+            -.5,
+            array.shape[0]-.5,
+            array.shape[1]-.5,
+            -.5,
+        )
 
     def test_imshow_array2d(self, ax):
         # overloaded imshow call (Array2D)
         array = Array2D(numpy.random.random((10, 10)), dx=.1, dy=.2)
         image = ax.imshow(array)
         utils.assert_array_equal(image.get_array(), array.value.T)
-        assert image.get_extent() == tuple(array.xspan) + tuple(array.yspan)
+        assert tuple(image.get_extent()) == (
+            tuple(array.xspan)
+            + tuple(array.yspan)
+        )
 
         # check log scale uses non-zero boundaries
         ax.clear()
         ax.set_xlim(.1, 1)
         ax.set_ylim(.1, 1)
         ax.set_xscale('log')
         ax.set_yscale('log')
         image = ax.imshow(array)
-        assert image.get_extent() == (1e-300, array.xspan[1],
-                                      1e-300, array.yspan[1])
+        assert tuple(image.get_extent()) == (
+            1e-300,
+            array.xspan[1],
+            1e-300,
+            array.yspan[1],
+        )
 
     def test_pcolormesh(self, ax):
         array = Array2D(numpy.random.random((10, 10)), dx=.1, dy=.2)
         ax.grid(True, which="both", axis="both")
         mesh = ax.pcolormesh(array)
         utils.assert_array_equal(mesh.get_array(), array.T.flatten())
         utils.assert_array_equal(mesh.get_paths()[-1].vertices[2],
@@ -187,18 +197,20 @@
             bins, numpy.logspace(numpy.log10(min_), numpy.log10(max_),
                                  11, endpoint=True),
         )
 
     def test_hist_error(self, ax):
         """Test that `ax.hist` presents the right error message for empty data
         """
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="^cannot generate log-spaced histogram bins",
+        ):
             ax.hist([], logbins=True)
-        assert str(exc.value).startswith('cannot generate log-spaced '
-                                         'histogram bins')
+
         # assert it works if we give the range manually
         ax.hist([], logbins=True, range=(1, 100))
 
     def test_tile(self, ax):
         x = numpy.arange(10)
         y = numpy.arange(x.size)
         w = numpy.ones_like(x) * .8
```

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_bode.py` & `gwpy-3.0.3/gwpy/plot/tests/test_bode.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_colors.py` & `gwpy-3.0.3/gwpy/plot/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_gps.py` & `gwpy-3.0.3/gwpy/plot/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_log.py` & `gwpy-3.0.3/gwpy/plot/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_plot.py` & `gwpy-3.0.3/gwpy/plot/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_rc.py` & `gwpy-3.0.3/gwpy/plot/tests/test_rc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_segments.py` & `gwpy-3.0.3/gwpy/plot/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_tex.py` & `gwpy-3.0.3/gwpy/plot/tests/test_tex.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,30 +30,40 @@
     """Fake which to force pdflatex to being not found
     """
     if arg == "pdflatex":
         return None
     return arg
 
 
-@mock.patch("gwpy.plot.tex.which", return_value="path")
-def test_has_tex_true(_):
-    """Test that `gwpy.plot.tex.has_tex` returns `True` when
-    all of the necessary executables are found
+@mock.patch("gwpy.plot.tex.which", _which)
+def test_has_tex_missing_exe():
+    """Test that `gwpy.plot.tex.has_tex` returns `False` when
+    any one of the necessary executables is missing.
     """
-    assert plot_tex.has_tex()
+    assert not plot_tex.has_tex()
 
 
-@mock.patch("gwpy.plot.tex.which", _which)
-def test_has_tex_false():
+@mock.patch("gwpy.plot.tex._test_usetex", side_effect=RuntimeError)
+def test_has_tex_bad_latex(_):
     """Test that `gwpy.plot.tex.has_tex` returns `False` when
-    any one of the necessary executables is missing.
+    the LaTeX figure fails to render.
     """
     assert not plot_tex.has_tex()
 
 
+@mock.patch("gwpy.plot.tex.which", return_value="path")
+@mock.patch("gwpy.plot.tex._test_usetex")
+def test_has_tex_true(_which_, _test_usetex):
+    """Test that `gwpy.plot.tex.has_tex` returns `True` when
+    all of the necessary executables are found, and the LaTeX figure
+    doesn't raise an exception.
+    """
+    assert plot_tex.has_tex()
+
+
 @pytest.mark.parametrize('in_, out', [
     (1, '1'),
     (100, r'10^{2}'),
     (-500, r'-5\!\!\times\!\!10^{2}'),
     (0.00001, r'10^{-5}'),
 ])
 def test_float_to_latex(in_, out):
```

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_text.py` & `gwpy-3.0.3/gwpy/plot/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/test_utils.py` & `gwpy-3.0.3/gwpy/plot/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tests/utils.py` & `gwpy-3.0.3/gwpy/plot/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/tex.py` & `gwpy-3.0.3/gwpy/plot/tex.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,28 +28,48 @@
 # -- tex configuration --------------------------------------------------------
 
 MACROS = [
     r'\def\rtHz{\ensuremath{\sqrt{\mathrm{Hz}}}}',  # \sqrt{Hz} label
 ]
 
 
+def _test_usetex():
+    """Draw (but don't show) a test image using matplotlib and LaTeX.
+    """
+    from matplotlib import (pyplot, rc_context)
+    with rc_context({"text.usetex": True}):
+        fig = pyplot.figure()
+        ax = fig.gca()
+        ax.set_xlabel(r"\LaTeX")
+        fig.canvas.draw()
+    pyplot.close(fig)
+
+
 def has_tex():
     """Returns whether tex is installed on this system
 
-    Checks for ``latex``, ``pdflatex``, and ``dvipng`` on the path.
+    Checks for ``latex``, ``pdflatex``, and ``dvipng`` on the path, and
+    then attemps to draw an image using LaTeX syntax.
 
     Returns
     -------
     hastex : `bool`
-        `True` if all required executables are found on the path, otherwise
-        `False`
+        `True` if the test image is drawn correctly, otherwise `False`
     """
+    # run basic sanity checks
     for exe in ('latex', 'pdflatex', 'dvipng'):
         if which(exe) is None:
             return False
+
+    # attempt to render an image with latex
+    try:
+        _test_usetex()
+    except Exception:  # failed for any reason
+        return False
+
     return True
 
 
 HAS_TEX = has_tex()
 
 # -- tex formatting -----------------------------------------------------------
```

### Comparing `gwpy-3.0.2/gwpy/plot/text.py` & `gwpy-3.0.3/gwpy/plot/text.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/units.py` & `gwpy-3.0.3/gwpy/plot/units.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/plot/utils.py` & `gwpy-3.0.3/gwpy/plot/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/segments/__init__.py` & `gwpy-3.0.3/gwpy/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/segments/flag.py` & `gwpy-3.0.3/gwpy/segments/flag.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/segments/io/__init__.py` & `gwpy-3.0.3/gwpy/segments/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/segments/io/hdf5.py` & `gwpy-3.0.3/gwpy/segments/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/segments/io/json.py` & `gwpy-3.0.3/gwpy/segments/io/json.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/segments/io/ligolw.py` & `gwpy-3.0.3/gwpy/segments/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/segments/io/segwizard.py` & `gwpy-3.0.3/gwpy/segments/io/segwizard.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/segments/segments.py` & `gwpy-3.0.3/gwpy/segments/segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/segments/tests/__init__.py` & `gwpy-3.0.3/gwpy/segments/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/segments/tests/test_flag.py` & `gwpy-3.0.3/gwpy/segments/tests/test_flag.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,17 +522,19 @@
 
         # flag name malformed
         with pytest.raises(ValueError):
             self.TEST_CLASS.query_dqsegdb('BAD-FLAG_NAME',
                                           SegmentList([(0, 10)]))
 
         # flag not in database
-        with pytest.raises(HTTPError) as exc:
+        with pytest.raises(
+            HTTPError,
+            match=r"^HTTP Error 404: Not found \[X1:GWPY-TEST:0\]$",
+        ):
             self.TEST_CLASS.query_dqsegdb('X1:GWPY-TEST:0', 0, 10)
-        assert str(exc.value) == 'HTTP Error 404: Not found [X1:GWPY-TEST:0]'
 
         # bad syntax
         with pytest.raises(ValueError):
             self.TEST_CLASS.query_dqsegdb(QUERY_FLAGS[0], 1, 2, 3)
         with pytest.raises(ValueError):
             self.TEST_CLASS.query_dqsegdb(QUERY_FLAGS[0], (1, 2, 3))
 
@@ -741,30 +743,31 @@
             names = ['randomname']
 
             def _read(**kwargs):
                 return self.TEST_CLASS.read(h5f, names=names, format='hdf5',
                                             **kwargs)
 
             # check on_missing='error' (default) raises ValueError
-            with pytest.raises(ValueError) as exc:
+            with pytest.raises(
+                ValueError,
+                match="^'randomname' not found in any input file$",
+            ):
                 _read()
-            assert str(exc.value) == ('\'randomname\' not found in any input '
-                                      'file')
 
             # check on_missing='warn' prints warning
             with pytest.warns(UserWarning):
                 _read(on_missing='warn')
 
             # check on_missing='ignore' does nothing
             with warnings.catch_warnings():
                 warnings.simplefilter("error")
                 _read(on_missing='ignore')
 
             # check on_missing=<anything else> raises exception
-            with pytest.raises(ValueError) as exc:
+            with pytest.raises(ValueError):
                 _read(on_missing='blah')
 
     @pytest.mark.requires("ligo.lw.lsctables")
     def test_to_ligolw_tables(self, instance):
         tables = instance.to_ligolw_tables()
         assert len(tables[0]) == len(instance)  # segdef
         assert len(tables[1]) == sum(len(x.known) for x in instance.values())
```

### Comparing `gwpy-3.0.2/gwpy/segments/tests/test_segments.py` & `gwpy-3.0.3/gwpy/segments/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/__init__.py` & `gwpy-3.0.3/gwpy/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/fft.py` & `gwpy-3.0.3/gwpy/signal/fft.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/filter_design.py` & `gwpy-3.0.3/gwpy/signal/filter_design.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import numpy
 from numpy import fft as npfft
 
 from scipy import signal
 
 from astropy.units import (Unit, Quantity)
 
-from .window import planck
+from .window import (get_window, planck)
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 __all__ = ['lowpass', 'highpass', 'bandpass', 'notch', 'concatenate_zpks']
 
 
 def _as_float(x):
     try:
@@ -200,15 +200,15 @@
     -------
     out : `numpy.ndarray`
         the smoothly truncated impulse response
     """
     out = impulse.copy()
     trunc_start = int(ntaps / 2)
     trunc_stop = out.size - trunc_start
-    window = signal.get_window(window, ntaps)
+    window = get_window(window, ntaps)
     out[0:trunc_start] *= window[trunc_start:ntaps]
     out[trunc_stop:out.size] *= window[0:trunc_start]
     out[trunc_start:trunc_stop] = 0
     return out
 
 
 def fir_from_transfer(transfer, ntaps, window='hann', ncorner=None):
```

### Comparing `gwpy-3.0.2/gwpy/signal/qtransform.py` & `gwpy-3.0.3/gwpy/signal/qtransform.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,15 +532,18 @@
         frequency axis by passing `logf=True` at runtime. The `fres` argument
         is then the number of points on the frequency axis. Note, this is
         incompatible with `~matplotlib.axes.Axes.imshow`.
 
         It is also highly recommended to use the `outseg` keyword argument
         when only a small window around a given GPS time is of interest.
         """
-        from scipy.interpolate import (interp2d, InterpolatedUnivariateSpline)
+        from scipy.interpolate import (
+            InterpolatedUnivariateSpline,
+            RectBivariateSpline,
+        )
         from ..spectrogram import Spectrogram
         if outseg is None:
             outseg = self.energies[0].span
         frequencies = self.plane.frequencies
         dtype = self.energies[0].dtype
         # build regular Spectrogram from peak-Q data by interpolating each
         # (Q, frequency) `TimeSeries` to have the same time resolution
@@ -561,15 +564,16 @@
             out[:, i] = interp(xout).astype(dtype, casting="same_kind",
                                             copy=False)
         if fres is None:
             return out
         # interpolate the spectrogram to increase its frequency resolution
         # --- this is done because Duncan doesn't like interpolated images
         #     since they don't support log scaling
-        interp = interp2d(xout, frequencies, out.value.T, kind='cubic')
+        interp = RectBivariateSpline(xout, frequencies, out.value)
+
         if not logf:
             if fres == "<default>":
                 fres = .5
             outfreq = numpy.arange(
                 self.plane.frange[0], self.plane.frange[1], fres,
                 dtype=dtype)
         else:
@@ -577,15 +581,15 @@
                 fres = 500
             outfreq = numpy.geomspace(
                 self.plane.frange[0],
                 self.plane.frange[1],
                 num=int(fres),
             )
         new = type(out)(
-            interp(xout, outfreq).T.astype(
+            interp(xout, outfreq).astype(
                 dtype, casting="same_kind", copy=False),
             t0=outseg[0], dt=tres, frequencies=outfreq,
         )
         new.q = self.plane.q
         return new
 
     def table(self, snrthresh=5.5):
```

### Comparing `gwpy-3.0.2/gwpy/signal/spectral/__init__.py` & `gwpy-3.0.3/gwpy/signal/spectral/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/spectral/_lal.py` & `gwpy-3.0.3/gwpy/signal/spectral/_lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/spectral/_median_mean.py` & `gwpy-3.0.3/gwpy/signal/spectral/_median_mean.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/spectral/_pycbc.py` & `gwpy-3.0.3/gwpy/signal/spectral/_pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/spectral/_registry.py` & `gwpy-3.0.3/gwpy/signal/spectral/_registry.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/spectral/_scipy.py` & `gwpy-3.0.3/gwpy/signal/spectral/_scipy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/spectral/_ui.py` & `gwpy-3.0.3/gwpy/signal/spectral/_ui.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/spectral/_utils.py` & `gwpy-3.0.3/gwpy/signal/spectral/_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/tests/__init__.py` & `gwpy-3.0.3/gwpy/signal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/tests/test_filter_design.py` & `gwpy-3.0.3/gwpy/signal/tests/test_filter_design.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/tests/test_qtransform.py` & `gwpy-3.0.3/gwpy/signal/tests/test_qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/tests/test_spectral_lal.py` & `gwpy-3.0.3/gwpy/signal/tests/test_spectral_lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/tests/test_spectral_median_mean.py` & `gwpy-3.0.3/gwpy/signal/tests/test_spectral_median_mean.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/tests/test_spectral_pycbc.py` & `gwpy-3.0.3/gwpy/signal/tests/test_spectral_pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/tests/test_spectral_registry.py` & `gwpy-3.0.3/gwpy/signal/tests/test_spectral_registry.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/tests/test_spectral_scipy.py` & `gwpy-3.0.3/gwpy/signal/tests/test_spectral_scipy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/tests/test_spectral_ui.py` & `gwpy-3.0.3/gwpy/signal/tests/test_spectral_ui.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/tests/test_spectral_utils.py` & `gwpy-3.0.3/gwpy/signal/tests/test_spectral_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/signal/window.py` & `gwpy-3.0.3/gwpy/signal/window.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,28 +15,49 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GWpy.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilities for signal-processing with windows
 """
 
-import numpy
-
+from functools import wraps
 from math import ceil
 
+import numpy
+
+from scipy.signal import get_window as _get_window
+from scipy.special import expit
 try:
     from scipy.signal.windows._windows import _win_equiv as WINDOWS
 except ImportError:  # scipy < 1.8.0
     from scipy.signal.windows.windows import _win_equiv as WINDOWS
 
-from scipy.special import expit
-
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
+@wraps(_get_window)
+def get_window(window, Nx, *args, **kwargs):
+    """Wrapper around :func:`scipy.signal.get_window` to allow
+    pre-computed window arrays.
+    """
+    # try something floaty
+    try:
+        return _get_window(float(window), Nx, *args, **kwargs)
+    except (TypeError, ValueError):
+        pass
+    # otherwise a name or tuple of params
+    if isinstance(window, (str, tuple)):
+        return _get_window(window, Nx, *args, **kwargs)
+    # otherwise we were given an array
+    window = numpy.asarray(window)
+    assert window.ndim == 1, "multi-dimensional windows are not supported"
+    assert window.size == Nx, "window array wrong size"
+    return window
+
+
 def canonical_name(name):
     """Find the canonical name for the given window in scipy.signal
 
     Parameters
     ----------
     name : `str`
         the name of the window you want
```

### Comparing `gwpy-3.0.2/gwpy/spectrogram/__init__.py` & `gwpy-3.0.3/gwpy/spectrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/spectrogram/coherence.py` & `gwpy-3.0.3/gwpy/spectrogram/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/spectrogram/io/__init__.py` & `gwpy-3.0.3/gwpy/spectrogram/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/spectrogram/io/hdf5.py` & `gwpy-3.0.3/gwpy/spectrogram/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/spectrogram/spectrogram.py` & `gwpy-3.0.3/gwpy/spectrogram/spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/spectrogram/tests/__init__.py` & `gwpy-3.0.3/gwpy/spectrogram/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/spectrogram/tests/test_spectrogram.py` & `gwpy-3.0.3/gwpy/spectrogram/tests/test_spectrogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,23 @@
     def test_new(self):
         super().test_new()
 
         # check handling of epoch vs t0
         a = self.create(epoch=10)
         b = self.create(t0=10)
         utils.assert_quantity_sub_equal(a, b)
-        with pytest.raises(ValueError) as exc:
+
+    def test_new_redundant_args(self):
+        with pytest.raises(
+            ValueError,
+            match="^give only one of epoch or t0$",
+        ):
             self.TEST_CLASS(self.data, epoch=1, t0=1)
-        assert str(exc.value) == 'give only one of epoch or t0'
 
-        # check times
+    def test_new_times(self):
         times = numpy.arange(self.data.shape[0])
         a = self.create(times=times)
         utils.assert_quantity_equal(a.times, times * units.second)
 
     def test_epoch(self, array):
         assert array.epoch.gps == array.x0.value
```

### Comparing `gwpy-3.0.2/gwpy/table/__init__.py` & `gwpy-3.0.3/gwpy/table/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/filter.py` & `gwpy-3.0.3/gwpy/table/filter.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/filters.py` & `gwpy-3.0.3/gwpy/table/filters.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/gravityspy.py` & `gwpy-3.0.3/gwpy/table/gravityspy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/__init__.py` & `gwpy-3.0.3/gwpy/table/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/cwb.py` & `gwpy-3.0.3/gwpy/table/io/cwb.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/fetch.py` & `gwpy-3.0.3/gwpy/table/io/fetch.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/gravityspy.py` & `gwpy-3.0.3/gwpy/table/io/gravityspy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/gstlal.py` & `gwpy-3.0.3/gwpy/table/io/gstlal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/gwf.py` & `gwpy-3.0.3/gwpy/table/io/gwf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/hacr.py` & `gwpy-3.0.3/gwpy/table/io/hacr.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/ligolw.py` & `gwpy-3.0.3/gwpy/table/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/losc.py` & `gwpy-3.0.3/gwpy/table/io/losc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/omega.py` & `gwpy-3.0.3/gwpy/table/io/omega.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/omicron.py` & `gwpy-3.0.3/gwpy/table/io/omicron.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/pycbc.py` & `gwpy-3.0.3/gwpy/table/io/pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/root.py` & `gwpy-3.0.3/gwpy/table/io/root.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/snax.py` & `gwpy-3.0.3/gwpy/table/io/snax.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/sql.py` & `gwpy-3.0.3/gwpy/table/io/sql.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/io/utils.py` & `gwpy-3.0.3/gwpy/table/io/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/table.py` & `gwpy-3.0.3/gwpy/table/table.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/tests/__init__.py` & `gwpy-3.0.3/gwpy/table/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/tests/test_gravityspy.py` & `gwpy-3.0.3/gwpy/table/tests/test_gravityspy.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,16 +66,20 @@
     def test_search_error(self):
         """Test `GravitySpyTable.search` error handling
 
         Mainly to make sure that an HTTP Error is raised instead
         of a JSONDecodeError.
         """
         requests_mock = pytest.importorskip("requests_mock")
-        with requests_mock.Mocker() as rmock, \
-             pytest.raises(requests.HTTPError) as exc:
+        mocker = requests_mock.Mocker()
+        raises = pytest.raises(
+            requests.HTTPError,
+            match="please check the request parameters$",
+        )
+        with mocker as rmock, raises:
             rmock.get(
                 "{}{}{}/?{}".format(
                     table_gravityspy.DEFAULT_HOST,
                     table_gravityspy.SEARCH_PATH,
                     table_gravityspy.SIMILARITY_SEARCH_PATH,
                     "&".join((
                         "howmany=10",
@@ -88,15 +92,14 @@
                 text="<!DOCTYPE html><html></html>",
                 status_code=200,
                 headers={
                     "Content-Type": "text/html; charset=utf-8",
                 },
             )
             self.TABLE.search(gravityspy_id="abcde")
-        assert str(exc.value).endswith("please check the request parameters")
 
     @pytest_skip_network_error
     def test_download(self, tmp_path):
         """Test `GravitySpyTable.download`
         """
         table = self.search()
         table.download(download_path=tmp_path)
```

### Comparing `gwpy-3.0.2/gwpy/table/tests/test_io_gstlal.py` & `gwpy-3.0.3/gwpy/table/tests/test_io_gstlal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/tests/test_io_ligolw.py` & `gwpy-3.0.3/gwpy/table/tests/test_io_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/table/tests/test_io_pycbc.py` & `gwpy-3.0.3/gwpy/table/tests/test_io_pycbc.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,18 +225,19 @@
     pycbclivetable,
     pycbclivefile,
 ):
     """Check that `EventTable` can handle multiple IFOs in a PyCBC-Live file
     """
     with h5py.File(pycbclivefile, "r+") as h5f:
         h5f.create_group('Z1')
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError,
+        match="PyCBC live HDF5 file contains dataset groups",
+    ):
         EventTable.read(pycbclivefile, format="hdf5.pycbc_live")
-    assert str(exc.value).startswith(
-        'PyCBC live HDF5 file contains dataset groups')
 
     # but check that we can still read the original
     table = EventTable.read(
         pycbclivefile,
         format='hdf5.pycbc_live',
         ifo='X1',
     )
```

### Comparing `gwpy-3.0.2/gwpy/table/tests/test_table.py` & `gwpy-3.0.3/gwpy/table/tests/test_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,17 +167,19 @@
 
         # check reading multiple tables works
         t3 = self.TABLE.read([tmp, tmp], format='ligolw',
                              tablename='sngl_burst')
         utils.assert_table_equal(vstack((t2, t2)), t3)
 
         # check writing to existing file raises IOError
-        with pytest.raises(IOError) as exc:
+        with pytest.raises(
+            IOError,
+            match=f"^File exists: {tmp}$",
+        ):
             _write()
-        assert str(exc.value) == 'File exists: %s' % tmp
 
         # check overwrite=True, append=False rewrites table
         _write(overwrite=True)
         t3 = _read()
         utils.assert_table_equal(t2, t3)
 
         # check append=True duplicates table
@@ -197,18 +199,19 @@
         t3 = _read()
         utils.assert_table_equal(t2, t3)
 
         # write another table with append=False and check the first table
         # is gone
         insp.write(tmp, format='ligolw', tablename='sngl_inspiral',
                    append=False, overwrite=True)
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="^document must contain exactly one sngl_burst table$",
+        ):
             _read()
-        assert str(exc.value) == ('document must contain exactly '
-                                  'one sngl_burst table')
 
     @pytest.mark.requires("ligo.lw.lsctables")
     def test_read_write_ligolw_property_columns(self, tmp_path):
         table = self.create(100, ['peak', 'snr', 'central_freq'],
                             ['f8', 'f4', 'f4'])
 
         # write table
@@ -305,17 +308,19 @@
     def test_read_root_multiple_trees(self, tmp_path):
         uproot = pytest.importorskip("uproot")
         tmp = tmp_path / "table.root"
         with uproot.create(tmp) as root:
             a = root.mktree("a", {"branch": "int32"})
             a.extend({"branch": asarray([1, 2, 3, 4, 5])})
             root.mktree("b", {"branch": "int32"})
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="^Multiple trees found",
+        ):
             self.TABLE.read(tmp)
-        assert str(exc.value).startswith('Multiple trees found')
         self.TABLE.read(tmp, treename="a")
 
     @pytest.mark.requires("uproot")
     def test_read_write_root_append(self, table, tmp_path):
         tmp = tmp_path / "table.root"
         # write one tree
         table.write(tmp, treename="a")
@@ -396,28 +401,32 @@
         assert t._get_time_column() == "b"
 
     def test_get_time_column_error_no_match(self, table):
         """Check that `_get_time_column` raises the right exception
         when no matches are found
         """
         t = self.create(1, ("a",))
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match=" no columns named 'time'",
+        ):
             t._get_time_column()
-        assert " no columns named 'time'" in str(exc.value)
 
     def test_get_time_column_error_multiple_match(self):
         # check that two GPS columns causes issues
         t = self.create(
             10,
             ("a", "b", "c"),
             dtypes=(float, LIGOTimeGPS, LIGOTimeGPS),
         )
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match=" multiple columns named 'time'",
+        ):
             t._get_time_column()
-        assert " multiple columns named 'time'" in str(exc.value)
 
     def test_get_time_column_error_empty(self):
         """Check that `_get_time_column` errors properly on an empty table
         """
         t = self.create(0, ("a",))
         with pytest.raises(ValueError):
             t._get_time_column()
@@ -533,17 +542,19 @@
         utils.assert_quantity_sub_equal(rate, rate2)
 
     def test_event_rates_start_end(self):
         """Check that `EventTable.event_rate` can function without explicit
         time column (and no data) if and only if start/end are both given.
         """
         t2 = self.create(10, names=['a', 'b'])
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="please give `timecolumn` keyword",
+        ):
             t2.event_rate(1)
-        assert 'please give `timecolumn` keyword' in str(exc.value)
         with pytest.raises(ValueError):
             t2.event_rate(1, start=0)
         with pytest.raises(ValueError):
             t2.event_rate(1, end=1)
         t2.event_rate(1, start=0, end=10)
 
     def test_binned_event_rates(self, table):
@@ -557,17 +568,19 @@
         assert rates[100].name == 'snr >= 100'
         table.binned_event_rates(100, 'snr', [10, 100], operator='in')
         table.binned_event_rates(100, 'snr', [(0, 10), (10, 100)])
 
         # check that method can function without explicit time column
         # (and no data) if and only if start/end are both given
         t2 = self.create(0, names=['a', 'b'])
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="please give `timecolumn` keyword",
+        ):
             t2.binned_event_rates(1, 'a', (10, 100))
-        assert 'please give `timecolumn` keyword' in str(exc.value)
         with pytest.raises(ValueError):
             t2.binned_event_rates(1, 'a', (10, 100), start=0)
         with pytest.raises(ValueError):
             t2.binned_event_rates(1, 'a', (10, 100), end=1)
         t2.binned_event_rates(1, 'a', (10, 100), start=0, end=10)
 
     def test_plot(self, table):
@@ -604,17 +617,19 @@
         t = clustertable.cluster('time', 'amplitude', 10)
         assert len(t) == 1
         assert all(t['amplitude'] == [11])
         assert all(t['time'] == [0.0])
 
     def test_cluster_window(self, clustertable):
         # check that a non-positive window throws an appropriate ValueError
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="^Window must be a positive value$",
+        ):
             clustertable.cluster('time', 'amplitude', 0)
-        assert str(exc.value) == 'Window must be a positive value'
 
     def test_cluster_multiple(self, clustertable):
         # check that after clustering a table, clustering the table a
         # second time with the same parameters returns the same result
         t_clustered = clustertable.cluster('time', 'amplitude', 0.6)
         utils.assert_table_equal(
             t_clustered,
@@ -674,22 +689,22 @@
     @pytest.mark.parametrize('fmtname', ('Omega', 'cWB'))
     def test_read_write_ascii_error(self, table, tmp_path, fmtname):
         tmp = tmp_path / "table.txt"
         with tmp.open("w"):
             pass  # write empty file
 
         # assert reading blank file doesn't work with column name error
-        with pytest.raises(InconsistentTableError) as exc:
+        with pytest.raises(
+            InconsistentTableError,
+            match=f"^No column names found in {fmtname} header$",
+        ):
             self.TABLE.read(
                 tmp,
                 format="ascii.{}".format(fmtname.lower()),
             )
-        assert str(exc.value) == (
-            'No column names found in {} header'.format(fmtname)
-        )
 
     @pytest.fixture
     def snaxtable(self):
         channel = 'H1:FAKE'
         table = self.create(
             100,
             names=[
```

### Comparing `gwpy-3.0.2/gwpy/testing/__init__.py` & `gwpy-3.0.3/gwpy/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.3/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/testing/data/HLV-HW100916-968654552-1.gwf` & `gwpy-3.0.3/gwpy/testing/data/HLV-HW100916-968654552-1.gwf`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/testing/data/HLV-HW100916-968654552-1.hdf` & `gwpy-3.0.3/gwpy/testing/data/HLV-HW100916-968654552-1.hdf`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz` & `gwpy-3.0.3/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/testing/errors.py` & `gwpy-3.0.3/gwpy/testing/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 import socket
 from functools import wraps
 from ssl import SSLError
 from urllib.error import URLError
 
 import pytest
 
+import requests.exceptions
+
 NETWORK_ERROR = (
     ConnectionError,
+    requests.exceptions.ConnectionError,
     socket.timeout,
     SSLError,
     URLError,
 )
 
 # attempt to also catch errors from pytest_socket,
 # this should enable the test suite to run on machines that
```

### Comparing `gwpy-3.0.2/gwpy/testing/fixtures.py` & `gwpy-3.0.3/gwpy/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/testing/marks.py` & `gwpy-3.0.3/gwpy/testing/marks.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/testing/mocks.py` & `gwpy-3.0.3/gwpy/testing/mocks.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/testing/utils.py` & `gwpy-3.0.3/gwpy/testing/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/time/__init__.py` & `gwpy-3.0.3/gwpy/time/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/time/__main__.py` & `gwpy-3.0.3/gwpy/time/__main__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/time/_tconvert.py` & `gwpy-3.0.3/gwpy/time/_tconvert.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 """
 
 import datetime
 import warnings
 from decimal import Decimal
 from numbers import Number
 
-from dateutil import parser as dateparser
+from dateutil.parser import parse as parse_datestr
 
 from astropy.units import Quantity
 
 from . import (Time, LIGOTimeGPS)
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 __all__ = ['tconvert', 'to_gps', 'from_gps']
@@ -259,27 +259,36 @@
         return DATE_STRINGS[str(datestr).lower()]()
     except KeyError:  # any other string
         pass
 
     # use maya
     try:
         import maya
-        return maya.when(datestr).datetime()
     except ImportError:
-        pass
+        MAYA_ERROR = None
+    else:
+        try:
+            return maya.when(datestr).datetime()
+        except Exception as exc1:
+            MAYA_ERROR = exc1
 
     # use dateutil.parse
     with warnings.catch_warnings():
         # don't allow lazy passing of time-zones
         warnings.simplefilter("error", RuntimeWarning)
         try:
-            return dateparser.parse(datestr)
-        except RuntimeWarning:
-            raise ValueError("Cannot parse date string with timezone "
-                             "without maya, please install maya")
+            return parse_datestr(datestr)
+        except RuntimeWarning as exc:
+            if MAYA_ERROR:
+                raise exc from MAYA_ERROR
+            exc.args = (
+                f"{str(exc).rstrip('.')}. Try installing 'maya' which can "
+                "handle more complex date strings.",
+            )
+            raise
         except (ValueError, TypeError) as exc:  # improve error reporting
             exc.args = ("Cannot parse date string {0!r}: {1}".format(
                 datestr, exc.args[0]),)
             raise
 
 
 def _datetime_to_time(dtm):
```

### Comparing `gwpy-3.0.2/gwpy/time/tests/__init__.py` & `gwpy-3.0.3/gwpy/time/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/time/tests/test_main.py` & `gwpy-3.0.3/gwpy/time/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/time/tests/test_time.py` & `gwpy-3.0.3/gwpy/time/tests/test_time.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GWpy.  If not, see <http://www.gnu.org/licenses/>.
 
 """Tests for :mod:`gwpy.time`
 """
 
+from contextlib import nullcontext
 from datetime import datetime
 from decimal import Decimal
 from operator import attrgetter
+from unittest import mock
 
 import pytest
 
 import numpy
 
-from freezegun import freeze_time
-
 from astropy.time import Time
 from astropy.units import (UnitConversionError, Quantity)
 
 from ... import time
 from .. import LIGOTimeGPS
 
 try:
@@ -50,95 +50,143 @@
 FREEZE = '2015-09-14 09:50:45.391'
 NOW = 1126259462
 TODAY = 1126224017
 TOMORROW = 1126310417
 YESTERDAY = 1126137617
 
 
-def _is_error_type(obj):
-    if isinstance(obj, (list, tuple)):
-        return all(map(_is_error_type, obj))
-    return isinstance(obj, type) and issubclass(obj, Exception)
-
-
-def _test_with_errors(func, in_, out):
-    # assert error
-    if _is_error_type(out):
-        with pytest.raises(out):
-            func(in_)
-    # assert not error
-    else:
-        with freeze_time(FREEZE):
-            assert func(in_) == out
-
-
-# -- test functions -----------------------------------------------------------
-
-@pytest.mark.parametrize('in_, out', [
+@pytest.mark.freeze_time(FREEZE)
+@pytest.mark.parametrize("use_maya", (
+    False,
+    pytest.param(True, marks=pytest.mark.requires("maya")),
+))
+@pytest.mark.parametrize(("in_", "out"), [
     (1126259462, int(GW150914)),
     (1235635623.7500002, LIGOTimeGPS(1235635623, 750000200)),
     (LIGOTimeGPS(1126259462, 391000000), GW150914),
     ('0', 0),
     ('Jan 1 2017', 1167264018),
     ('Sep 14 2015 09:50:45.391', GW150914),
     ((2017, 1, 1), 1167264018),
     (datetime(2017, 1, 1), 1167264018),
     (Time(57754, format='mjd'), 1167264018),
     (Time(57754.0001, format='mjd'), LIGOTimeGPS(1167264026, 640000000)),
     (Quantity(1167264018, 's'), 1167264018),
     (Decimal('1126259462.391000000'), GW150914),
-    pytest.param(GlueGPS(GW150914.gpsSeconds, GW150914.gpsNanoSeconds),
-                 GW150914, marks=pytest.mark.requires("glue")),
+    pytest.param(
+        GlueGPS(GW150914.gpsSeconds, GW150914.gpsNanoSeconds),
+        GW150914,
+        marks=pytest.mark.requires("glue"),
+    ),
     (numpy.int32(NOW), NOW),  # fails with lal-6.18.0
     ('now', NOW),
     ('today', TODAY),
     ('tomorrow', TOMORROW),
     ('yesterday', YESTERDAY),
+])
+def test_to_gps(in_, out, use_maya):
+    """Test that :func:`to_gps` works with and without maya.
+    """
+    if use_maya:  # do nothing
+        ctx = nullcontext()
+    else:  # force 'install maya' to error to use dateutil
+        ctx = mock.patch.dict("sys.modules", {"maya": None})
+    with ctx:
+        assert time.to_gps(in_) == out
+
+
+@pytest.mark.requires("maya")
+@pytest.mark.parametrize(("in_", "out"), [
+    ('Oct 30 2016 12:34 CST', 1161887657),
+])
+def test_to_gps_maya(in_, out):
+    """Test that :func:`gwpy.time.to_gps` works with maya.
+    """
+    assert time.to_gps(in_) == out
+
+
+@pytest.mark.parametrize(("in_", "err"), [
     (Quantity(1, 'm'), UnitConversionError),
     ('random string', (ValueError, TypeError)),
-    pytest.param('Oct 30 2016 12:34 CST', 1161887657,
-                 marks=pytest.mark.requires("maya")),
 ])
-def test_to_gps(in_, out):
-    """Test :func:`gwpy.time.to_gps`
+def test_to_gps_error(in_, err):
+    """Test that :func:`gwpy.time.to_gps` errors when it should.
     """
-    _test_with_errors(time.to_gps, in_, out)
+    with pytest.raises(err):
+        time.to_gps(in_)
+
+
+@mock.patch.dict("sys.modules", {"maya": None})
+def test_to_gps_dateparser_error_propagation_nomaya():
+    with pytest.raises(
+        RuntimeWarning,
+        match=(
+            "tzname CST identified but not understood.(.*) "
+            "Try installing 'maya' (.*)"
+        ),
+    ):
+        time.to_gps("Oct 30 2016 12:34 CST")
+
+
+@pytest.mark.requires("maya")
+@mock.patch("maya.when", side_effect=ValueError("test chain"))
+def test_to_gps_dateparser_error_propagation_maya(_):
+    with pytest.raises(RuntimeWarning) as exc:
+        time.to_gps("Oct 30 2016 12:34 CST")
+    # validate that the maya exception was chained to the dateutil one
+    assert str(exc.value.__cause__) == "test chain"
 
 
 @pytest.mark.parametrize('in_, out', [
     (1167264018, datetime(2017, 1, 1)),
     ('1167264018', datetime(2017, 1, 1)),
     (1126259462.391, datetime(2015, 9, 14, 9, 50, 45, 391000)),
     ('1.13e9', datetime(2015, 10, 27, 16, 53, 3)),
-    pytest.param(GlueGPS(GW150914.gpsSeconds, GW150914.gpsNanoSeconds),
-                 GW150914_DT, marks=pytest.mark.requires("glue")),
+    pytest.param(
+        GlueGPS(GW150914.gpsSeconds, GW150914.gpsNanoSeconds),
+        GW150914_DT,
+        marks=pytest.mark.requires("glue"),
+    ),
+])
+def test_from_gps(in_, out):
+    """Test that :func:`gwpy.time.from_gps` works.
+    """
+    assert time.from_gps(in_) == out
+
+
+@pytest.mark.parametrize(("in_", "err"), [
     ('test', ValueError),
     (1167264017, ValueError),  # gwpy/gwpy#1021
 ])
-def test_from_gps(in_, out):
-    """Test :func:`gwpy.time.from_gps`
+def test_from_gps_error(in_, err):
+    """Test that :func:`gwpy.time.from_gps` errors when it should.
     """
-    _test_with_errors(time.from_gps, in_, out)
+    with pytest.raises(err):
+        time.from_gps(in_)
 
 
+@pytest.mark.freeze_time(FREEZE)
 @pytest.mark.parametrize('in_, out', [
     (float(GW150914), GW150914_DT),
     (GW150914, GW150914_DT),
     (GW150914_DT, GW150914),
-    pytest.param(GlueGPS(float(GW150914)), GW150914_DT,
-                 marks=pytest.mark.requires("glue")),
+    pytest.param(
+        GlueGPS(float(GW150914)),
+        GW150914_DT,
+        marks=pytest.mark.requires("glue"),
+    ),
     ('now', NOW),
     ('today', TODAY),
     ('tomorrow', TOMORROW),
     ('yesterday', YESTERDAY),
 ])
 def test_tconvert(in_, out):
     """Test :func:`gwpy.time.tconvert`
     """
-    _test_with_errors(time.tconvert, in_, out)
+    assert time.tconvert(in_) == out
 
 
 @pytest.mark.parametrize('gpstype', time.gps_types,
                          ids=attrgetter('__module__'))
 def test_gps_types(gpstype):
     assert gpstype.__name__ == 'LIGOTimeGPS'
     gps = gpstype(123, 456000000)
```

### Comparing `gwpy-3.0.2/gwpy/timeseries/__init__.py` & `gwpy-3.0.3/gwpy/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/core.py` & `gwpy-3.0.3/gwpy/timeseries/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1135,16 +1135,20 @@
                     try:
                         return cls.fetch(channels, start, end, host=host_,
                                          port=port_, verbose=verbose,
                                          type=type, dtype=dtype, pad=pad,
                                          scaled=scaled, allow_tape=allow_tape_)
                     except (RuntimeError, ValueError) as exc:
                         error = str(exc)  # need to assign to take out of scope
-                        warnings.warn(error.split('\n', 1)[0],
-                                      io_nds2.NDSWarning)
+                        msg = error.split('\n', 1)[0]
+                        warnings.warn(
+                            f"failed to fetch data for {', '.join(channels)} "
+                            f"in interval [{start}, {end}): {msg}",
+                            io_nds2.NDSWarning,
+                        )
 
                 # if failing occurred because of data on tape, don't try
                 # reading channels individually, the same error will occur
                 if not allow_tape_ and 'Requested data is on tape' in error:
                     continue
 
                 # if we got this far, we can't get all channels in one go
```

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/__init__.py` & `gwpy-3.0.3/gwpy/timeseries/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/ascii.py` & `gwpy-3.0.3/gwpy/timeseries/io/ascii.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/cache.py` & `gwpy-3.0.3/gwpy/timeseries/io/cache.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/core.py` & `gwpy-3.0.3/gwpy/timeseries/io/core.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/gwf/__init__.py` & `gwpy-3.0.3/gwpy/timeseries/io/gwf/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/gwf/framecpp.py` & `gwpy-3.0.3/gwpy/timeseries/io/gwf/framecpp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/gwf/framel.py` & `gwpy-3.0.3/gwpy/timeseries/io/gwf/framel.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/gwf/lalframe.py` & `gwpy-3.0.3/gwpy/timeseries/io/gwf/lalframe.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/hdf5.py` & `gwpy-3.0.3/gwpy/timeseries/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/losc.py` & `gwpy-3.0.3/gwpy/timeseries/io/losc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/nds2.py` & `gwpy-3.0.3/gwpy/timeseries/io/nds2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/io/wav.py` & `gwpy-3.0.3/gwpy/timeseries/io/wav.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/statevector.py` & `gwpy-3.0.3/gwpy/timeseries/statevector.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/tests/__init__.py` & `gwpy-3.0.3/gwpy/timeseries/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/tests/test_core.py` & `gwpy-3.0.3/gwpy/timeseries/tests/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,29 +56,38 @@
         array = super().test_new()
 
         # check time-domain metadata
         assert array.epoch == GPS_EPOCH
         assert array.sample_rate == units.Quantity(1, 'Hertz')
         assert array.dt == units.Quantity(1, 'second')
 
-        # check handling of epoch vs t0
+    def test_new_epoch_t0(self):
+        """Test `gwpy.timeseries.TimeSeriesBase` handling of epoch vs t0.
+        """
         a = self.create(epoch=10)
         b = self.create(t0=10)
         utils.assert_quantity_sub_equal(a, b)
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="^give only one of epoch or t0$",
+        ):
             self.TEST_CLASS(self.data, epoch=1, t0=1)
-        assert str(exc.value) == 'give only one of epoch or t0'
 
+    def test_new_sample_rate_dt(self):
+        """Test `gwpy.timeseries.TimeSeriesBase` handling of sample_rate vs dt.
+        """
         # check handling of sample_rate vs dt
         a = self.create(sample_rate=100)
         b = self.create(dt=0.01)
         utils.assert_quantity_sub_equal(a, b)
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="^give only one of sample_rate or dt$",
+        ):
             self.TEST_CLASS(self.data, sample_rate=1, dt=1)
-        assert str(exc.value) == 'give only one of sample_rate or dt'
 
     def test_epoch(self):
         """Test `gwpy.timeseries.TimeSeriesBase.epoch`
         """
         # check basic conversion from t0 -> epoch
         a = self.create(t0=1126259462)
         assert a.epoch == Time('2015-09-14 09:50:45', format='iso')
@@ -265,17 +274,21 @@
         assert self.TEST_CLASS.EntryClass is self.ENTRY_CLASS
 
     def test_span(self, instance):
         assert isinstance(instance.span, Segment)
         assert instance.span == reduce(
             operator.or_, (ts.span for ts in instance.values()), Segment(0, 0),
         )
-        with pytest.raises(ValueError) as exc:
+
+    def test_span_error_empty(self):
+        with pytest.raises(
+            ValueError,
+            match="cannot calculate span for empty ",
+        ):
             self.TEST_CLASS().span
-        assert 'cannot calculate span for empty ' in str(exc.value)
 
     def test_copy(self, instance):
         copy = instance.copy()
         assert isinstance(copy, self.TEST_CLASS)
         for key in copy:
             assert not shares_memory(copy[key].value, instance[key].value)
             utils.assert_quantity_sub_equal(copy[key], instance[key])
@@ -435,26 +448,30 @@
         """Test :attr:`gwpy.timeseries.TimeSeriesBaseList.segments`
         """
         sl = instance.segments
         assert isinstance(sl, SegmentList)
         assert all(isinstance(s, Segment) for s in sl)
         assert sl == [(0, 100), (101, 1101)]
 
-    def test_append(self):
-        tsl = self.create()
-
-        # test simple append
+    def test_append(self, instance):
+        """Test `TimeSeriesList.append`.
+        """
         new = self.ENTRY_CLASS([1, 2, 3, 4, 5], x0=1102, dx=1)
-        tsl.append(new)
+        instance.append(new)
+        assert len(instance) == 3
+        assert instance[-1] is new
 
-        # test mismatched type raises error
-        with pytest.raises(TypeError) as exc:
-            tsl.append([1, 2, 3, 4, 5])
-        assert str(exc.value) == (
-            "Cannot append type 'list' to %s" % type(tsl).__name__)
+    def test_append_typeerror(self, instance):
+        """Test `TimeSeriesList.append` errors on type differences.
+        """
+        with pytest.raises(
+            TypeError,
+            match=f"^Cannot append type 'list' to {self.TEST_CLASS.__name__}$",
+        ):
+            instance.append([1, 2, 3, 4, 5])
 
     def test_extend(self):
         a = self.create()
         b = a.copy()
         new = self.ENTRY_CLASS([1, 2, 3, 4, 5])
         a.append(new)
         b.extend([new])
```

### Comparing `gwpy-3.0.2/gwpy/timeseries/tests/test_io_gwf_framecpp.py` & `gwpy-3.0.3/gwpy/timeseries/tests/test_io_gwf_framecpp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/tests/test_io_gwf_lalframe.py` & `gwpy-3.0.3/gwpy/timeseries/tests/test_io_gwf_lalframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,19 +86,19 @@
 def test_open_data_source_cache(tmp_path):
     tmp = tmp_path / "test.lcf"
     write_cache([TEST_GWF_FILE], tmp, format="lal")
     return _test_open_data_source(tmp)
 
 
 def test_open_data_source_error():
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError,
+        match=f"^Don't know how to open data source of type {type(None)}$",
+    ):
         gwpy_lalframe.open_data_source(None)
-    assert str(exc.value) == (
-        "Don't know how to open data source of type {}".format(type(None))
-    )
 
 
 def test_get_stream_duration(stream):
     assert gwpy_lalframe.get_stream_duration(stream) == 1.
 
 
 @pytest.mark.parametrize("start, end", [
@@ -127,17 +127,19 @@
         assert ts.name == name
 
         # check data span is what we asked for
         assert numpy.allclose(ts.xspan, (start, end), atol=TEST_GWF_DELTA_T)
 
 
 def test_read_channel_error():
-    with pytest.raises(RuntimeError) as exc:
+    with pytest.raises(
+        RuntimeError,
+        match="^channel 'bad' not found$",
+    ):
         gwpy_lalframe.read(TEST_GWF_FILE, ["bad"])
-    assert str(exc.value) == "channel 'bad' not found"
 
 
 def test_read_deprecated_scaled():
     with pytest.warns(UserWarning):
         gwpy_lalframe.read(
             TEST_GWF_FILE,
             ["L1:LDAS-STRAIN"],
```

### Comparing `gwpy-3.0.2/gwpy/timeseries/tests/test_io_losc.py` & `gwpy-3.0.3/gwpy/timeseries/tests/test_io_losc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/timeseries/tests/test_statevector.py` & `gwpy-3.0.3/gwpy/timeseries/tests/test_statevector.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,17 +280,19 @@
 
         # check that bits in gives bits out
         bs = array.get_bit_series(['Bit 0', 'Bit 3'])
         assert list(bs.keys()) == ['Bit 0', 'Bit 3']
         assert [v.sum() for v in bs.values()] == [50, 41]
 
         # check that invalid bits throws exception
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="^Bit 'blah' not found in StateVector$",
+        ):
             array.get_bit_series(['blah'])
-        assert str(exc.value) == "Bit 'blah' not found in StateVector"
 
     def test_plot(self, array):
         with rc_context(rc={'text.usetex': False}):
             plot = array.plot()
             # make sure there were no lines drawn
             assert len(plot.gca().lines) == 0
             # assert one collection for each of known and active segmentlists
```

### Comparing `gwpy-3.0.2/gwpy/timeseries/tests/test_timeseries.py` & `gwpy-3.0.3/gwpy/timeseries/tests/test_timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from numpy import testing as nptest
 
 from scipy import signal
 
 from astropy import units
 
 from ...frequencyseries import (FrequencySeries, SpectralVariance)
+from ...io.nds2 import NDSWarning
 from ...segments import (Segment, SegmentList, DataQualityFlag)
 from ...signal import filter_design
 from ...signal.window import planck
 from ...spectrogram import Spectrogram
 from ...table import EventTable
 from ...testing import (mocks, utils)
 from ...testing.errors import (
@@ -292,35 +293,44 @@
     @pytest.mark.parametrize('api', [
         pytest.param(
             'framecpp',
             marks=pytest.mark.requires("LDAStools.frameCPP"),
         ),
     ])
     def test_read_write_gwf_error(self, tmp_path, api, gw150914):
+        fmt = f"gwf.{api}"
         tmp = tmp_path / "test.gwf"
-        gw150914.write(tmp, format="gwf.{}".format(api))
-        with pytest.raises(ValueError) as exc:
-            self.TEST_CLASS.read(tmp, "another channel",
-                                 format="gwf.{}".format(api))
-        assert str(exc.value) == (
-            "no Fr{Adc,Proc,Sim}Data structures with the "
-            "name another channel"
-        )
+        gw150914.write(tmp, format=fmt)
+
+        # wrong channel
+        with pytest.raises(
+            ValueError,
+            match=(
+                "^no Fr{Adc,Proc,Sim}Data structures with the "
+                "name another channel$"
+            ),
+        ):
+            self.TEST_CLASS.read(
+                tmp,
+                "another channel",
+                format=fmt,
+            )
 
-        with pytest.raises(ValueError) as exc:
+        # wrong times
+        with pytest.raises(
+            ValueError,
+            match=f"^Failed to read '{gw150914.name}' from '{tmp}'",
+        ):
             self.TEST_CLASS.read(
                 tmp,
                 gw150914.name,
                 start=gw150914.span[0]-1,
                 end=gw150914.span[0],
-                format="gwf.{}".format(api),
+                format=fmt,
             )
-        assert str(exc.value).startswith(
-            "Failed to read {0!r} from {1!r}".format(gw150914.name, str(tmp))
-        )
 
     @pytest.mark.requires("lalframe")
     def test_read_gwf_scaled_lalframe(self):
         with warnings.catch_warnings():
             warnings.simplefilter("error")
             data = self.TEST_CLASS.read(
                 utils.TEST_GWF_FILE,
@@ -408,17 +418,19 @@
     ])
     def test_read_write_hdf5(self, tmp_path, ext, channel):
         array = self.create()
         array.channel = channel
 
         tmp = tmp_path / "test.{}".format(ext)
         # check array with no name fails
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="^Cannot determine HDF5 path",
+        ):
             array.write(tmp, overwrite=True)
-        assert str(exc.value).startswith('Cannot determine HDF5 path')
         array.name = 'TEST'
 
         # write array (with auto-identify)
         array.write(tmp, overwrite=True)
 
         # check reading gives the same data (with/without auto-identify)
         ts = type(array).read(tmp, format='hdf5')
@@ -603,17 +615,35 @@
             return [mocks.nds2_channel(name, 128, '')]
 
         nds_connection.find_channels = find_channels
 
         # run fetch and assert error
         with mock.patch('nds2.connection') as mock_connection:
             mock_connection.return_value = nds_connection
-            with pytest.raises(RuntimeError) as exc:
+            with pytest.raises(RuntimeError, match="no data received"):
                 self.TEST_CLASS.fetch('L1:TEST', 0, 1, host='nds.gwpy')
-            assert 'no data received' in str(exc.value)
+
+    @pytest.mark.requires("nds2")
+    @mock.patch(
+        "gwpy.io.nds2.host_resolution_order",
+        return_value=(["nds.example.com", 31200],),
+    )
+    def test_fetch_warning_message(self, _):
+        """Test that TimeSeries.fetch emits a useful warning on NDS2 issues.
+        """
+        with \
+                pytest.raises(
+                    RuntimeError,
+                    match="Cannot find all relevant data",
+                ), \
+                pytest.warns(
+                    NDSWarning,
+                    match="failed to fetch data for X1:TEST",
+                ):
+            self.TEST_CLASS.fetch("X1:TEST", 0, 1)
 
     @_gwosc_cvmfs
     @mock.patch.dict(
         "os.environ",
         {"GWDATAFIND_SERVER": GWOSC_DATAFIND_SERVER},
     )
     def test_find(self, gw150914_16384):
@@ -1350,14 +1380,19 @@
     def test_q_transform(self, gw150914):
         # test simple q-transform
         qspecgram = gw150914.q_transform(method='scipy-welch', fftlength=2)
         assert isinstance(qspecgram, Spectrogram)
         assert qspecgram.shape == (1000, 2403)
         assert qspecgram.q == 5.65685424949238
         nptest.assert_almost_equal(qspecgram.value.max(), 155.93567, decimal=5)
+        nptest.assert_almost_equal(
+            qspecgram.value.mean(),
+            1.936469,
+            decimal=5,
+        )
 
         # test whitening args
         asd = gw150914.asd(2, 1, method='scipy-welch')
         qsg2 = gw150914.q_transform(method='scipy-welch', whiten=asd)
         utils.assert_quantity_sub_equal(qspecgram, qsg2, almost_equal=True)
 
         asd = gw150914.asd(.5, .25, method='scipy-welch')
@@ -1399,17 +1434,19 @@
         assert isinstance(qspecgram, Spectrogram)
         assert qspecgram.shape == (1000, 500)
         assert qspecgram.q == 5.65685424949238
         nptest.assert_almost_equal(qspecgram.value.max(), 155.93774, decimal=5)
 
     def test_q_transform_nan(self):
         data = TimeSeries(numpy.empty(256*10) * numpy.nan, sample_rate=256)
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match="^Input signal contains non-numerical values$",
+        ):
             data.q_transform(method="median")
-        assert str(exc.value) == 'Input signal contains non-numerical values'
 
     def test_boolean_statetimeseries(self, array):
         comp = array >= 2 * array.unit
         assert isinstance(comp, StateTimeSeries)
         assert comp.unit is units.Unit('')
         assert comp.name == '%s >= 2.0' % (array.name)
         assert (array == array).name == '{0} == {0}'.format(array.name)
```

### Comparing `gwpy-3.0.2/gwpy/timeseries/timeseries.py` & `gwpy-3.0.3/gwpy/timeseries/timeseries.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from numpy import fft as npfft
 from scipy import signal
 
 from astropy import units
 
 from ..segments import (Segment, SegmentList, DataQualityFlag)
 from ..signal import (filter_design, qtransform, spectral)
-from ..signal.window import (recommended_overlap, planck)
+from ..signal.window import (get_window, recommended_overlap, planck)
 from .core import (TimeSeriesBase, TimeSeriesBaseDict, TimeSeriesBaseList,
                    as_series_dict_class)
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 DEFAULT_FFT_METHOD = "median"
 
@@ -212,23 +212,15 @@
         noverlap = int((overlap * self.sample_rate).decompose().value)
 
         navg = divmod(self.size-noverlap, (nfft-noverlap))[0]
 
         # format window
         if window is None:
             window = 'boxcar'
-        if isinstance(window, (str, tuple)):
-            win = signal.get_window(window, nfft)
-        else:
-            win = numpy.asarray(window)
-            if len(win.shape) != 1:
-                raise ValueError('window must be 1-D')
-            elif win.shape[0] != nfft:
-                raise ValueError('Window is the wrong size.')
-        win = win.astype(self.dtype)
+        win = get_window(window, nfft).astype(self.dtype)
         scaling = 1. / numpy.absolute(win).mean()
 
         if nfft % 2:
             nfreqs = (nfft + 1) // 2
         else:
             nfreqs = nfft // 2 + 1
         ffts = Spectrogram(numpy.zeros((navg, nfreqs), dtype=numpy.complex128),
@@ -1152,16 +1144,16 @@
 
         Notes
         -----
         If `self` and `other` have difference
         :attr:`TimeSeries.sample_rate` values, the higher sampled
         `TimeSeries` will be down-sampled to match the lower.
         """
-        csd = other.csd(self, fftlength=fftlength, overlap=overlap,
-                        window=window, **kwargs)
+        csd = self.csd(other, fftlength=fftlength, overlap=overlap,
+                       window=window, **kwargs)
         psd = self.psd(fftlength=fftlength, overlap=overlap, window=window,
                        **kwargs)
 
         # Take the minimum of the frequencyseries csd and psd because the
         # sample rate of different channels might yield different length
         # objects
         size = min(csd.size, psd.size)
@@ -1793,15 +1785,19 @@
         fftlength = fftlength if fftlength else _fft_length_default(self.dt)
         if asd is None:
             asd = self.asd(fftlength, overlap=overlap,
                            method=method, window=window, **kwargs)
         asd = asd.interpolate(1./self.duration.decompose().value)
         # design whitening filter, with highpass if requested
         ncorner = int(highpass / asd.df.decompose().value) if highpass else 0
-        ntaps = int((fduration * self.sample_rate).decompose().value)
+        if isinstance(window, (str, tuple)):
+            ntaps = int((fduration * self.sample_rate).decompose().value)
+        else:
+            window = numpy.asarray(window)
+            ntaps = len(window)
         tdw = filter_design.fir_from_transfer(1/asd.value, ntaps=ntaps,
                                               window=window, ncorner=ncorner)
         # condition the input data and apply the whitening filter
         in_ = self.copy().detrend(detrend)
         out = in_.convolve(tdw, window=window)
         return out * numpy.sqrt(2 * in_.dt.decompose().value)
 
@@ -1969,15 +1965,15 @@
         corrupted at the left and right boundaries. To prevent spectral leakage
         these segments will be windowed before convolving.
         """
         pad = int(numpy.ceil(fir.size/2))
         nfft = min(8*fir.size, self.size)
         # condition the input data
         in_ = self.copy()
-        window = signal.get_window(window, fir.size)
+        window = get_window(window, fir.size)
         in_.value[:pad] *= window[:pad]
         in_.value[-pad:] *= window[-pad:]
         # if FFT length is long enough, perform only one convolution
         if nfft >= self.size/2:
             conv = signal.fftconvolve(in_.value, fir, mode='same')
         # else use the overlap-save algorithm
         else:
```

### Comparing `gwpy-3.0.2/gwpy/types/__init__.py` & `gwpy-3.0.3/gwpy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/array.py` & `gwpy-3.0.3/gwpy/types/array.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/array2d.py` & `gwpy-3.0.3/gwpy/types/array2d.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/index.py` & `gwpy-3.0.3/gwpy/types/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,20 @@
                 numpy.array(start, subok=True, copy=False).dtype,
                 numpy.array(step, subok=True, copy=False).dtype,
             )
         start = Quantity(start, dtype=dtype, copy=False)
         step = Quantity(step, dtype=dtype, copy=False).to(start.unit)
         stop = start + step * num
         return cls(
-            numpy.arange(start.value, stop.value, step.value, dtype=dtype),
+            numpy.arange(
+                start.value,
+                stop.value,
+                step.value,
+                dtype=dtype,
+            )[:num],
             unit=start.unit,
             copy=False,
         )
 
     @property
     def regular(self):
         """`True` if this index is linearly increasing
```

### Comparing `gwpy-3.0.2/gwpy/types/io/__init__.py` & `gwpy-3.0.3/gwpy/types/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/io/ascii.py` & `gwpy-3.0.3/gwpy/types/io/ascii.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/io/hdf5.py` & `gwpy-3.0.3/gwpy/types/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/io/ligolw.py` & `gwpy-3.0.3/gwpy/types/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/series.py` & `gwpy-3.0.3/gwpy/types/series.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/sliceutils.py` & `gwpy-3.0.3/gwpy/types/sliceutils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/tests/__init__.py` & `gwpy-3.0.3/gwpy/types/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/tests/test_array.py` & `gwpy-3.0.3/gwpy/types/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/types/tests/test_array2d.py` & `gwpy-3.0.3/gwpy/types/tests/test_array2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,17 +225,16 @@
         assert a.is_compatible(b)
 
     def test_is_compatible_error_yindex(self, array):
         """Check that `Array2D.is_compatible` errors with mismatching indexes
         """
         y = numpy.logspace(0, 2, num=self.data.shape[1])
         other = self.create(yindex=y)
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(ValueError, match="indexes do not match"):
             array.is_compatible(other)
-        assert "indexes do not match" in str(exc.value)
 
     def test_value_at(self, array):
         assert array.value_at(2, 3) == self.data[2][3] * array.unit
         assert array.value_at(5 * array.xunit, 2 * array.yunit) == (
             self.data[5][2] * array.unit)
         with pytest.raises(IndexError):
             array.value_at(1.6, 4.8)
```

### Comparing `gwpy-3.0.2/gwpy/types/tests/test_index.py` & `gwpy-3.0.3/gwpy/types/tests/test_index.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,25 @@
 from .. import Index
 
 
 class TestIndex(object):
     TEST_CLASS = Index
 
     def test_define_regular(self):
+        """Check for regression against gwpy/gwpy#1596.
+        """
+        ind_len = 1000
+        a = self.TEST_CLASS.define(
+            1262936373.4853957,
+            0.051,
+            ind_len
+        )
+        assert len(a) == ind_len
+
+    def test_define_index_length(self):
         """Check for regression against gwpy/gwpy#1506.
         """
         a = self.TEST_CLASS.define(
             units.Quantity(1000000000),
             units.Quantity(0.01),
             500,
         )
```

### Comparing `gwpy-3.0.2/gwpy/types/tests/test_series.py` & `gwpy-3.0.3/gwpy/types/tests/test_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,42 +218,39 @@
         other = self.create(name='TEST CASE 2')
         assert array.is_compatible(other)
 
     def test_is_compatible_error_dx(self, array):
         """Check that `Series.is_compatible` errors with mismatching ``dx``
         """
         other = self.create(dx=2)
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(ValueError, match="sample sizes do not match"):
             array.is_compatible(other)
-        assert "sample sizes do not match" in str(exc.value)
 
     def test_is_compatible_error_unit(self, array):
         """Check that `Series.is_compatible` errors with mismatching ``unit``
         """
         other = self.create(unit='m')
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(ValueError, match="units do not match"):
             array.is_compatible(other)
-        assert "units do not match" in str(exc.value)
 
     def test_is_compatible_xindex(self):
         """Check that irregular arrays are compatible if their xindexes match
         """
         x = numpy.logspace(0, 2, num=self.data.shape[0])
         a = self.create(xindex=x)
         b = self.create(xindex=x)
         assert a.is_compatible(b)
 
     def test_is_compatible_error_xindex(self, array):
         """Check that `Series.is_compatible` errors with mismatching indexes
         """
         x = numpy.logspace(0, 2, num=self.data.shape[0])
         other = self.create(xindex=x)
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(ValueError, match="indexes do not match"):
             array.is_compatible(other)
-        assert "indexes do not match" in str(exc.value)
 
     def test_is_contiguous(self, array):
         a2 = self.create(x0=array.xspan[1])
         assert array.is_contiguous(a2) == 1
         assert array.is_contiguous(a2.value) == 1
 
         ts3 = self.create(x0=array.xspan[1]+1)
```

### Comparing `gwpy-3.0.2/gwpy/utils/__init__.py` & `gwpy-3.0.3/gwpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/decorators.py` & `gwpy-3.0.3/gwpy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/enum.py` & `gwpy-3.0.3/gwpy/utils/enum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/env.py` & `gwpy-3.0.3/gwpy/utils/env.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/lal.py` & `gwpy-3.0.3/gwpy/utils/lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/misc.py` & `gwpy-3.0.3/gwpy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/mp.py` & `gwpy-3.0.3/gwpy/utils/mp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/progress.py` & `gwpy-3.0.3/gwpy/utils/progress.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/shell.py` & `gwpy-3.0.3/gwpy/utils/shell.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/sphinx/__init__.py` & `gwpy-3.0.3/gwpy/utils/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/sphinx/epydoc.py` & `gwpy-3.0.3/gwpy/utils/sphinx/epydoc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/sphinx/ex2rst.py` & `gwpy-3.0.3/gwpy/utils/sphinx/ex2rst.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/sphinx/zenodo.py` & `gwpy-3.0.3/gwpy/utils/sphinx/zenodo.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/tests/__init__.py` & `gwpy-3.0.3/gwpy/utils/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/tests/test_decorators.py` & `gwpy-3.0.3/gwpy/utils/tests/test_decorators.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,17 +42,19 @@
 def test_return_as_error():
     """Test that `gwpy.utils.decorators.return_as` error handling works
     """
     @decorators.return_as(int)
     def myfunc(value):
         return str(value)
 
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError,
+        match="^failed to cast return from myfunc as int: ",
+    ):
         myfunc('test')
-    assert 'failed to cast return from myfunc as int: ' in str(exc.value)
 
 
 def test_deprecated_function():
     """Test that `deprecated_function` works without a message
 
     (and without any functional brackets)
     """
```

### Comparing `gwpy-3.0.2/gwpy/utils/tests/test_enum.py` & `gwpy-3.0.3/gwpy/utils/tests/test_enum.py`

 * *Files 15% similar despite different names*

```diff
@@ -64,12 +64,12 @@
         assert self.TEST_CLASS.find(
             self.TEST_CLASS.INT16.value
         ) is self.TEST_CLASS.INT16
 
     def test_find_errors(self):
         """Test :meth:`NumpyTypeEnum.find` method error handling
         """
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(
+            ValueError,
+            match=f"^'blah' is not a valid {self.TEST_CLASS.__name__}$",
+        ):
             self.TEST_CLASS.find('blah')
-        assert str(exc.value) == "'blah' is not a valid {}".format(
-            self.TEST_CLASS.__name__,
-        )
```

### Comparing `gwpy-3.0.2/gwpy/utils/tests/test_env.py` & `gwpy-3.0.3/gwpy/utils/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/tests/test_lal.py` & `gwpy-3.0.3/gwpy/utils/tests/test_lal.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,17 +101,19 @@
     ("123 m", "m", 123),
 ))
 def test_to_lal_unit(in_, out, scale):
     assert utils_lal.to_lal_unit(in_) == (lal.Unit(out), scale)
 
 
 def test_to_lal_unit_error():
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError,
+        match="^LAL has no unit corresponding to 'rad'$",
+    ):
         utils_lal.to_lal_unit('rad/s')
-    assert str(exc.value) == "LAL has no unit corresponding to 'rad'"
 
 
 @pytest.mark.parametrize(("in_", "out"), (
     ("m s^-1", "m/s"),
     ("strain", "strain"),
     ("m^1/2", "m**(1/2.)"),
     ("10^3 m", "km"),
```

### Comparing `gwpy-3.0.2/gwpy/utils/tests/test_misc.py` & `gwpy-3.0.3/gwpy/utils/tests/test_misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,18 +62,19 @@
     assert base == rounded
     assert type(base) == type(rounded)
 
 
 def test_round_to_power_error():
     """Test for an errored use case of :func:`gwpy.utils.misc.round_to_power`
     """
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError,
+        match="^'which' argument must be one of 'lower', 'upper', or None$",
+    ):
         utils_misc.round_to_power(7, which='')
-    assert str(exc.value) == (
-        "'which' argument must be one of 'lower', 'upper', or None")
 
 
 def test_unique():
     """Test for :func:`gwpy.utils.misc.unique`
     """
     a = [1, 2, 4, 3, 5, 4, 5, 3]
     assert utils_misc.unique(a) == [1, 2, 4, 3, 5]
```

### Comparing `gwpy-3.0.2/gwpy/utils/tests/test_mp.py` & `gwpy-3.0.3/gwpy/utils/tests/test_mp.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,21 +50,20 @@
         assert stdout.startswith(verbose)
 
 
 @pytest.mark.parametrize('nproc', [1, 2])
 def test_multiprocess_with_queues_errors(nproc):
     """Check that errors from child processes propagate to the parent
     """
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(ValueError, match="^math domain error$"):
         utils_mp.multiprocess_with_queues(
             nproc,
             sqrt,
             [-1, -1, -1, -1],
         )
-    assert str(exc.value) == "math domain error"
 
 
 def test_multiprocess_with_queues_raise():
     with pytest.deprecated_call():
         utils_mp.multiprocess_with_queues(
             1,
             sqrt,
```

### Comparing `gwpy-3.0.2/gwpy/utils/tests/test_shell.py` & `gwpy-3.0.3/gwpy/utils/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy/utils/tests/test_sphinx_ex2rst.py` & `gwpy-3.0.3/gwpy/utils/tests/test_sphinx_ex2rst.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.2/gwpy.egg-info/PKG-INFO` & `gwpy-3.0.3/gwpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpy
-Version: 3.0.2
+Version: 3.0.3
 Summary: A python package for gravitational-wave astrophysics
 Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/gwpy/gwpy/issues
 Project-URL: Discussion Forum, https://gwpy.slack.com
 Project-URL: Documentation, https://gwpy.github.io/docs/
 Project-URL: Source Code, https://github.com/gwpy/gwpy
```

### Comparing `gwpy-3.0.2/gwpy.egg-info/SOURCES.txt` & `gwpy-3.0.3/gwpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,18 @@
 docs/_templates/autosummary/module.rst
 docs/astro/index.rst
 docs/cli/examples.ini
 docs/cli/index.rst
 docs/detector/channel.rst
 docs/dev/release.rst
 docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+docs/external/framecpp.rst
+docs/external/framel.rst
+docs/external/lalsuite.rst
+docs/external/nds2.rst
 docs/plot/colorbars.rst
 docs/plot/colors.rst
 docs/plot/filter.rst
 docs/plot/gps.rst
 docs/plot/index.rst
 docs/plot/legend.rst
 docs/plot/log.rst
```

### Comparing `gwpy-3.0.2/gwpy.egg-info/requires.txt` & `gwpy-3.0.3/gwpy.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 python-nds2-client
 
 [conda:sys_platform != "win32"]
 python-ldas-tools-framecpp
 
 [dev]
 ciecplib
+dateparser>=1.1.2
 psycopg2
 pymysql
 pyRXP
 sqlalchemy
 uproot>=4.1.5
 
 [dev:python_version < "3.11"]
@@ -37,22 +38,22 @@
 lalsuite
 lscsoft-glue
 pycbc>=1.13.4
 python-ligo-lw>=1.7.0
 
 [docs]
 numpydoc>=0.8.0
-sphinx>=4.0.0
+Sphinx>=4.4.0
 sphinx-automodapi
 sphinx-immaterial>=0.7.3
 sphinx-panels>=0.6.0
 sphinxcontrib-programoutput
 
 [test]
 coverage[toml]>=5.0
-freezegun>=0.3.12
 pytest>=3.9.1
+pytest-freezegun
 pytest-cov>=2.4.0
 pytest-requires
 pytest-socket
 pytest-xdist
 requests-mock
```

### Comparing `gwpy-3.0.2/pyproject.toml` & `gwpy-3.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -56,38 +56,40 @@
   "version",
 ]
 
 [project.optional-dependencies]
 # test suite
 test = [
   "coverage[toml] >=5.0",
-  "freezegun >=0.3.12",
   "pytest >=3.9.1",
+  "pytest-freezegun",
   "pytest-cov >=2.4.0",
   "pytest-requires",
   "pytest-socket",
   "pytest-xdist",
   "requests-mock",
 ]
 # astronomy/cosmology calculations
 astro = [
   "inspiral-range",
 ]
 # sphinx documentation
 docs = [
   "numpydoc >=0.8.0",
-  "sphinx >=4.0.0",
+  "Sphinx >=4.4.0",
   "sphinx-automodapi",
   "sphinx-immaterial >=0.7.3",
   "sphinx-panels >=0.6.0",
   "sphinxcontrib-programoutput",
 ]
 # development environments
 dev = [
   "ciecplib",
+  # for maya to work, see https://github.com/scrapinghub/dateparser/pull/1067
+  "dateparser >=1.1.2",
   "lalsuite ; sys_platform != 'win32'",
   "lscsoft-glue ; sys_platform != 'win32'",
   "maya ; python_version < '3.11'",
   "psycopg2",
   "pycbc >=1.13.4 ; sys_platform != 'win32'",
   "pymysql",
   "pyRXP",
@@ -161,27 +163,36 @@
 ]
 xfail_strict = true
 
 # -- rstcheck
 
 [tool.rstcheck]
 ignore_directives = [
+  # matplotlib
+  "plot",
+  # sphinx
+  "include",
   # sphinx.ext.autosummary
   "autoclass",
   "autofunction",
   "automethod",
   "automodule",
   "autosummary",
-  # sphinx-automodapi
-  "automodsumm",
-  # sphinxcontrib-programoutput
-  "command-output",
   # sphinx.ext.ifconfig
   "ifconfig",
-  # matplotlib
-  "plot",
+  # sphinx-automodapi
+  "automodsumm",
+  # sphinx-immaterial
+  "md-tab-set",
   # sphinx-panels
   "tabbed",
+  # sphinxcontrib-programoutput
+  "command-output",
+]
+ignore_roles = [
+  # doxylink
+  "lal",
+  "lalframe",
 ]
 # rstcheck doesn't known about our referenced.txt which is implicitly included
 # in all pages via Sphinx's epilog option
 ignore_messages = "(Unknown target name:.*|Undefined substitution referenced: .*)"
```

### Comparing `gwpy-3.0.2/setup_utils.py` & `gwpy-3.0.3/setup_utils.py`

 * *Files identical despite different names*

