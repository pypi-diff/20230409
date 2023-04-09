# Comparing `tmp/mc3-3.1.1.tar.gz` & `tmp/mc3-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mc3-3.1.1.tar", last modified: Tue Apr  4 14:43:07 2023, max compression
+gzip compressed data, was "mc3-3.1.2.tar", last modified: Sun Apr  9 14:49:19 2023, max compression
```

## Comparing `mc3-3.1.1.tar` & `mc3-3.1.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.295116 mc3-3.1.1/
--rw-r--r--   0 pato       (501) staff       (20)      123 2023-03-30 17:50:12.000000 mc3-3.1.1/.readthedocs.yml
--rw-r--r--   0 pato       (501) staff       (20)     2943 2022-03-19 12:17:57.000000 mc3-3.1.1/CONTRIBUTING.md
--rw-r--r--   0 pato       (501) staff       (20)     1085 2022-03-19 12:17:57.000000 mc3-3.1.1/LICENSE
--rw-r--r--   0 pato       (501) staff       (20)      402 2022-03-19 12:17:57.000000 mc3-3.1.1/MANIFEST.in
--rw-r--r--   0 pato       (501) staff       (20)      991 2022-03-19 12:17:57.000000 mc3-3.1.1/Makefile
--rw-r--r--   0 pato       (501) staff       (20)     2422 2023-04-04 14:43:07.294997 mc3-3.1.1/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1779 2023-04-04 14:34:51.000000 mc3-3.1.1/README.md
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.285335 mc3-3.1.1/docs/
--rw-r--r--   0 pato       (501) staff       (20)     7657 2022-03-19 12:17:57.000000 mc3-3.1.1/docs/Makefile
--rw-r--r--   0 pato       (501) staff       (20)    62757 2023-03-30 17:50:12.000000 mc3-3.1.1/docs/api.rst
--rw-r--r--   0 pato       (501) staff       (20)    11541 2022-03-19 12:17:57.000000 mc3-3.1.1/docs/conf.py
--rw-r--r--   0 pato       (501) staff       (20)     2970 2022-03-19 12:17:57.000000 mc3-3.1.1/docs/contributing.rst
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.287553 mc3-3.1.1/docs/figures/
--rw-r--r--   0 pato       (501) staff       (20)    32125 2022-03-19 12:17:57.000000 mc3-3.1.1/docs/figures/quad_bestfit.png
--rw-r--r--   0 pato       (501) staff       (20)    34319 2022-03-19 12:17:57.000000 mc3-3.1.1/docs/figures/quad_fitting.png
--rw-r--r--   0 pato       (501) staff       (20)    46027 2023-03-30 13:26:40.000000 mc3-3.1.1/docs/figures/quad_hist.png
--rw-r--r--   0 pato       (501) staff       (20)   242288 2023-03-30 13:26:40.000000 mc3-3.1.1/docs/figures/quad_pairwise.png
--rw-r--r--   0 pato       (501) staff       (20)   211712 2023-03-30 13:26:40.000000 mc3-3.1.1/docs/figures/quad_trace.png
--rw-r--r--   0 pato       (501) staff       (20)    48970 2022-03-19 12:17:57.000000 mc3-3.1.1/docs/figures/rms-vs-binsize.png
--rw-r--r--   0 pato       (501) staff       (20)     8854 2023-03-30 13:26:40.000000 mc3-3.1.1/docs/fit_tutorial.rst
--rw-r--r--   0 pato       (501) staff       (20)     6881 2023-03-30 13:26:40.000000 mc3-3.1.1/docs/get_started.rst
--rw-r--r--   0 pato       (501) staff       (20)     4370 2023-04-04 14:34:51.000000 mc3-3.1.1/docs/index.rst
--rw-r--r--   0 pato       (501) staff       (20)     1140 2023-03-30 13:26:40.000000 mc3-3.1.1/docs/license.rst
--rw-r--r--   0 pato       (501) staff       (20)     7243 2022-03-19 12:17:57.000000 mc3-3.1.1/docs/make.bat
--rw-r--r--   0 pato       (501) staff       (20)    28030 2023-03-30 13:26:40.000000 mc3-3.1.1/docs/mcmc_tutorial.rst
--rw-r--r--   0 pato       (501) staff       (20)     1691 2022-03-19 12:17:57.000000 mc3-3.1.1/docs/references.rst
--rw-r--r--   0 pato       (501) staff       (20)     1333 2022-03-19 12:17:57.000000 mc3-3.1.1/docs/time_averaging.rst
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.288464 mc3-3.1.1/examples/
--rw-r--r--   0 pato       (501) staff       (20)     1650 2023-03-30 13:26:40.000000 mc3-3.1.1/examples/get_started.py
--rw-r--r--   0 pato       (501) staff       (20)     2243 2022-03-19 12:17:57.000000 mc3-3.1.1/examples/ns_tutorial.py
--rw-r--r--   0 pato       (501) staff       (20)     1556 2022-03-19 12:17:57.000000 mc3-3.1.1/examples/timeavg.py
--rw-r--r--   0 pato       (501) staff       (20)     2792 2023-03-30 13:26:40.000000 mc3-3.1.1/examples/tutorial.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.290141 mc3-3.1.1/mc3/
--rw-r--r--   0 pato       (501) staff       (20)      688 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    10937 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/__main__.py
--rw-r--r--   0 pato       (501) staff       (20)    13086 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/chain.py
--rw-r--r--   0 pato       (501) staff       (20)     9288 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/fit_driver.py
--rw-r--r--   0 pato       (501) staff       (20)    13642 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/mcmc_driver.py
--rw-r--r--   0 pato       (501) staff       (20)     6544 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/ns_driver.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.291409 mc3-3.1.1/mc3/plots/
--rw-r--r--   0 pato       (501) staff       (20)      604 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/plots/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     5594 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/plots/colors.py
--rw-r--r--   0 pato       (501) staff       (20)    10671 2023-03-30 17:50:12.000000 mc3-3.1.1/mc3/plots/plot_functions.py
--rw-r--r--   0 pato       (501) staff       (20)    39082 2023-03-30 17:50:12.000000 mc3-3.1.1/mc3/plots/posterior.py
--rw-r--r--   0 pato       (501) staff       (20)    15233 2023-03-30 13:16:39.000000 mc3-3.1.1/mc3/sampler.py
--rw-r--r--   0 pato       (501) staff       (20)    24594 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/sampler_driver.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.292535 mc3-3.1.1/mc3/stats/
--rw-r--r--   0 pato       (501) staff       (20)      638 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/stats/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     2674 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/stats/gelman.py
--rw-r--r--   0 pato       (501) staff       (20)      811 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/stats/prayer.py
--rw-r--r--   0 pato       (501) staff       (20)    35522 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/stats/stats.py
--rw-r--r--   0 pato       (501) staff       (20)     1589 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/stats/time_averaging.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.292900 mc3-3.1.1/mc3/utils/
--rw-r--r--   0 pato       (501) staff       (20)      529 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/utils/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     7119 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/utils/log.py
--rw-r--r--   0 pato       (501) staff       (20)    13722 2023-03-30 13:26:40.000000 mc3-3.1.1/mc3/utils/utils.py
--rw-r--r--   0 pato       (501) staff       (20)      275 2023-04-04 14:34:51.000000 mc3-3.1.1/mc3/version.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.290756 mc3-3.1.1/mc3.egg-info/
--rw-r--r--   0 pato       (501) staff       (20)     2422 2023-04-04 14:43:07.000000 mc3-3.1.1/mc3.egg-info/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1460 2023-04-04 14:43:07.000000 mc3-3.1.1/mc3.egg-info/SOURCES.txt
--rw-r--r--   0 pato       (501) staff       (20)        1 2023-04-04 14:43:07.000000 mc3-3.1.1/mc3.egg-info/dependency_links.txt
--rw-r--r--   0 pato       (501) staff       (20)       43 2023-04-04 14:43:07.000000 mc3-3.1.1/mc3.egg-info/entry_points.txt
--rw-r--r--   0 pato       (501) staff       (20)       45 2023-04-04 14:43:07.000000 mc3-3.1.1/mc3.egg-info/requires.txt
--rw-r--r--   0 pato       (501) staff       (20)        4 2023-04-04 14:43:07.000000 mc3-3.1.1/mc3.egg-info/top_level.txt
--rw-r--r--   0 pato       (501) staff       (20)      144 2022-03-19 12:17:57.000000 mc3-3.1.1/pyproject.toml
--rw-r--r--   0 pato       (501) staff       (20)      150 2022-03-19 12:17:57.000000 mc3-3.1.1/pytest.ini
--rw-r--r--   0 pato       (501) staff       (20)       57 2023-03-30 17:50:12.000000 mc3-3.1.1/requirements.txt
--rw-r--r--   0 pato       (501) staff       (20)       38 2023-04-04 14:43:07.295154 mc3-3.1.1/setup.cfg
--rw-r--r--   0 pato       (501) staff       (20)     1721 2023-03-30 17:50:12.000000 mc3-3.1.1/setup.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.293435 mc3-3.1.1/src_c/
--rw-r--r--   0 pato       (501) staff       (20)     3973 2023-03-30 13:26:40.000000 mc3-3.1.1/src_c/_binarray.c
--rw-r--r--   0 pato       (501) staff       (20)     7667 2023-03-30 13:26:40.000000 mc3-3.1.1/src_c/_chisq.c
--rw-r--r--   0 pato       (501) staff       (20)    10514 2023-03-30 13:26:40.000000 mc3-3.1.1/src_c/_dwt.c
--rw-r--r--   0 pato       (501) staff       (20)     6902 2023-03-30 13:26:40.000000 mc3-3.1.1/src_c/_time_averaging.c
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.293918 mc3-3.1.1/src_c/include/
--rw-r--r--   0 pato       (501) staff       (20)      522 2023-03-30 13:26:40.000000 mc3-3.1.1/src_c/include/ind.h
--rw-r--r--   0 pato       (501) staff       (20)     6632 2023-03-30 13:26:40.000000 mc3-3.1.1/src_c/include/stats.h
--rw-r--r--   0 pato       (501) staff       (20)     4185 2023-03-30 13:26:40.000000 mc3-3.1.1/src_c/include/wavelet.h
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-04 14:43:07.294818 mc3-3.1.1/tests/
--rw-r--r--   0 pato       (501) staff       (20)     5592 2023-03-30 13:26:40.000000 mc3-3.1.1/tests/test_dynesty.py
--rw-r--r--   0 pato       (501) staff       (20)     3988 2023-03-30 13:26:40.000000 mc3-3.1.1/tests/test_fit.py
--rw-r--r--   0 pato       (501) staff       (20)     2281 2023-03-30 13:26:40.000000 mc3-3.1.1/tests/test_logging.py
--rw-r--r--   0 pato       (501) staff       (20)    15975 2023-03-30 13:26:40.000000 mc3-3.1.1/tests/test_mcmc.py
--rw-r--r--   0 pato       (501) staff       (20)     3790 2023-03-30 13:26:40.000000 mc3-3.1.1/tests/test_plots.py
--rw-r--r--   0 pato       (501) staff       (20)    14911 2023-03-30 13:26:40.000000 mc3-3.1.1/tests/test_stats.py
--rw-r--r--   0 pato       (501) staff       (20)     8937 2023-03-30 13:26:40.000000 mc3-3.1.1/tests/test_utils.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.118392 mc3-3.1.2/
+-rw-r--r--   0 pato       (501) staff       (20)      123 2023-03-30 17:50:12.000000 mc3-3.1.2/.readthedocs.yml
+-rw-r--r--   0 pato       (501) staff       (20)     2943 2022-03-19 12:17:57.000000 mc3-3.1.2/CONTRIBUTING.md
+-rw-r--r--   0 pato       (501) staff       (20)     1085 2022-03-19 12:17:57.000000 mc3-3.1.2/LICENSE
+-rw-r--r--   0 pato       (501) staff       (20)      402 2022-03-19 12:17:57.000000 mc3-3.1.2/MANIFEST.in
+-rw-r--r--   0 pato       (501) staff       (20)      991 2022-03-19 12:17:57.000000 mc3-3.1.2/Makefile
+-rw-r--r--   0 pato       (501) staff       (20)     2422 2023-04-09 14:49:19.118268 mc3-3.1.2/PKG-INFO
+-rw-r--r--   0 pato       (501) staff       (20)     1779 2023-04-04 14:34:51.000000 mc3-3.1.2/README.md
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.108868 mc3-3.1.2/docs/
+-rw-r--r--   0 pato       (501) staff       (20)     7657 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/Makefile
+-rw-r--r--   0 pato       (501) staff       (20)    62757 2023-03-30 17:50:12.000000 mc3-3.1.2/docs/api.rst
+-rw-r--r--   0 pato       (501) staff       (20)    11541 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/conf.py
+-rw-r--r--   0 pato       (501) staff       (20)     2970 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/contributing.rst
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.110961 mc3-3.1.2/docs/figures/
+-rw-r--r--   0 pato       (501) staff       (20)    32125 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/figures/quad_bestfit.png
+-rw-r--r--   0 pato       (501) staff       (20)    34319 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/figures/quad_fitting.png
+-rw-r--r--   0 pato       (501) staff       (20)    46027 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/figures/quad_hist.png
+-rw-r--r--   0 pato       (501) staff       (20)   242288 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/figures/quad_pairwise.png
+-rw-r--r--   0 pato       (501) staff       (20)   211712 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/figures/quad_trace.png
+-rw-r--r--   0 pato       (501) staff       (20)    48970 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/figures/rms-vs-binsize.png
+-rw-r--r--   0 pato       (501) staff       (20)     8854 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/fit_tutorial.rst
+-rw-r--r--   0 pato       (501) staff       (20)     6915 2023-04-09 14:48:51.000000 mc3-3.1.2/docs/get_started.rst
+-rw-r--r--   0 pato       (501) staff       (20)     4370 2023-04-04 14:34:51.000000 mc3-3.1.2/docs/index.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1140 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/license.rst
+-rw-r--r--   0 pato       (501) staff       (20)     7243 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/make.bat
+-rw-r--r--   0 pato       (501) staff       (20)    28030 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/mcmc_tutorial.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1691 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/references.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1333 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/time_averaging.rst
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.111862 mc3-3.1.2/examples/
+-rw-r--r--   0 pato       (501) staff       (20)     1650 2023-03-30 13:26:40.000000 mc3-3.1.2/examples/get_started.py
+-rw-r--r--   0 pato       (501) staff       (20)     2243 2022-03-19 12:17:57.000000 mc3-3.1.2/examples/ns_tutorial.py
+-rw-r--r--   0 pato       (501) staff       (20)     1556 2022-03-19 12:17:57.000000 mc3-3.1.2/examples/timeavg.py
+-rw-r--r--   0 pato       (501) staff       (20)     2792 2023-03-30 13:26:40.000000 mc3-3.1.2/examples/tutorial.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.113476 mc3-3.1.2/mc3/
+-rw-r--r--   0 pato       (501) staff       (20)      688 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    10937 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/__main__.py
+-rw-r--r--   0 pato       (501) staff       (20)    13086 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/chain.py
+-rw-r--r--   0 pato       (501) staff       (20)     9288 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/fit_driver.py
+-rw-r--r--   0 pato       (501) staff       (20)    13642 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/mcmc_driver.py
+-rw-r--r--   0 pato       (501) staff       (20)     6544 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/ns_driver.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.114900 mc3-3.1.2/mc3/plots/
+-rw-r--r--   0 pato       (501) staff       (20)      604 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/plots/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     5594 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/plots/colors.py
+-rw-r--r--   0 pato       (501) staff       (20)    10671 2023-03-30 17:50:12.000000 mc3-3.1.2/mc3/plots/plot_functions.py
+-rw-r--r--   0 pato       (501) staff       (20)    39119 2023-04-09 14:48:51.000000 mc3-3.1.2/mc3/plots/posterior.py
+-rw-r--r--   0 pato       (501) staff       (20)    15233 2023-03-30 13:16:39.000000 mc3-3.1.2/mc3/sampler.py
+-rw-r--r--   0 pato       (501) staff       (20)    24594 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/sampler_driver.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.115976 mc3-3.1.2/mc3/stats/
+-rw-r--r--   0 pato       (501) staff       (20)      638 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/stats/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     2674 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/stats/gelman.py
+-rw-r--r--   0 pato       (501) staff       (20)      811 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/stats/prayer.py
+-rw-r--r--   0 pato       (501) staff       (20)    35522 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/stats/stats.py
+-rw-r--r--   0 pato       (501) staff       (20)     1589 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/stats/time_averaging.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.116365 mc3-3.1.2/mc3/utils/
+-rw-r--r--   0 pato       (501) staff       (20)      529 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/utils/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     7119 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/utils/log.py
+-rw-r--r--   0 pato       (501) staff       (20)    13722 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/utils/utils.py
+-rw-r--r--   0 pato       (501) staff       (20)      275 2023-04-09 14:48:51.000000 mc3-3.1.2/mc3/version.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.114228 mc3-3.1.2/mc3.egg-info/
+-rw-r--r--   0 pato       (501) staff       (20)     2422 2023-04-09 14:49:18.000000 mc3-3.1.2/mc3.egg-info/PKG-INFO
+-rw-r--r--   0 pato       (501) staff       (20)     1460 2023-04-09 14:49:19.000000 mc3-3.1.2/mc3.egg-info/SOURCES.txt
+-rw-r--r--   0 pato       (501) staff       (20)        1 2023-04-09 14:49:18.000000 mc3-3.1.2/mc3.egg-info/dependency_links.txt
+-rw-r--r--   0 pato       (501) staff       (20)       43 2023-04-09 14:49:18.000000 mc3-3.1.2/mc3.egg-info/entry_points.txt
+-rw-r--r--   0 pato       (501) staff       (20)       45 2023-04-09 14:49:18.000000 mc3-3.1.2/mc3.egg-info/requires.txt
+-rw-r--r--   0 pato       (501) staff       (20)        4 2023-04-09 14:49:18.000000 mc3-3.1.2/mc3.egg-info/top_level.txt
+-rw-r--r--   0 pato       (501) staff       (20)      144 2022-03-19 12:17:57.000000 mc3-3.1.2/pyproject.toml
+-rw-r--r--   0 pato       (501) staff       (20)      150 2022-03-19 12:17:57.000000 mc3-3.1.2/pytest.ini
+-rw-r--r--   0 pato       (501) staff       (20)       57 2023-03-30 17:50:12.000000 mc3-3.1.2/requirements.txt
+-rw-r--r--   0 pato       (501) staff       (20)       38 2023-04-09 14:49:19.118433 mc3-3.1.2/setup.cfg
+-rw-r--r--   0 pato       (501) staff       (20)     1721 2023-03-30 17:50:12.000000 mc3-3.1.2/setup.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.116858 mc3-3.1.2/src_c/
+-rw-r--r--   0 pato       (501) staff       (20)     3973 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/_binarray.c
+-rw-r--r--   0 pato       (501) staff       (20)     7667 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/_chisq.c
+-rw-r--r--   0 pato       (501) staff       (20)    10514 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/_dwt.c
+-rw-r--r--   0 pato       (501) staff       (20)     6902 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/_time_averaging.c
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.117215 mc3-3.1.2/src_c/include/
+-rw-r--r--   0 pato       (501) staff       (20)      522 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/include/ind.h
+-rw-r--r--   0 pato       (501) staff       (20)     6632 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/include/stats.h
+-rw-r--r--   0 pato       (501) staff       (20)     4185 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/include/wavelet.h
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.118071 mc3-3.1.2/tests/
+-rw-r--r--   0 pato       (501) staff       (20)     5592 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_dynesty.py
+-rw-r--r--   0 pato       (501) staff       (20)     3988 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_fit.py
+-rw-r--r--   0 pato       (501) staff       (20)     2281 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_logging.py
+-rw-r--r--   0 pato       (501) staff       (20)    15975 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_mcmc.py
+-rw-r--r--   0 pato       (501) staff       (20)     3790 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_plots.py
+-rw-r--r--   0 pato       (501) staff       (20)    14911 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_stats.py
+-rw-r--r--   0 pato       (501) staff       (20)     8937 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_utils.py
```

### Comparing `mc3-3.1.1/CONTRIBUTING.md` & `mc3-3.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/LICENSE` & `mc3-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/Makefile` & `mc3-3.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/PKG-INFO` & `mc3-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mc3
-Version: 3.1.1
+Version: 3.1.2
 Summary: Multi-core Markov-chain Monte Carlo package.
 Home-page: https://github.com/pcubillos/mc3
 Author: Patricio Cubillos
 Author-email: patricio.cubillos@oeaw.ac.at
 License: MIT
 Description: # mc3: Multi-core Markov-chain Monte Carlo
         > A Python implementation of the Markov-chain Monte Carlo algorithm.
```

### Comparing `mc3-3.1.1/README.md` & `mc3-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/Makefile` & `mc3-3.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/api.rst` & `mc3-3.1.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/conf.py` & `mc3-3.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/contributing.rst` & `mc3-3.1.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/figures/quad_bestfit.png` & `mc3-3.1.2/docs/figures/quad_bestfit.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/figures/quad_fitting.png` & `mc3-3.1.2/docs/figures/quad_fitting.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/figures/quad_hist.png` & `mc3-3.1.2/docs/figures/quad_hist.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/figures/quad_pairwise.png` & `mc3-3.1.2/docs/figures/quad_pairwise.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/figures/quad_trace.png` & `mc3-3.1.2/docs/figures/quad_trace.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/figures/rms-vs-binsize.png` & `mc3-3.1.2/docs/figures/rms-vs-binsize.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/fit_tutorial.rst` & `mc3-3.1.2/docs/fit_tutorial.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/get_started.rst` & `mc3-3.1.2/docs/get_started.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 Getting Started
 ===============
 
 System Requirements
 -------------------
 
 ``mc3`` is compatible with Python 3.6+, and has been `tested
-<https://travis-ci.com/pcubillos/mc3>`_ to work on Unix/Linux and
+<https://github.com/pcubillos/mc3/actions/workflows/python-package.yml>`_ to work on Unix/Linux and
 OS X machines, with the following software:
 
-* Numpy >= 1.22.3
+* Numpy >= 1.19.5
 * Scipy >= 1.9.3
-* Matplotlib >= 3.5.1
+* Matplotlib >= 3.3.4
 
 ``mc3`` may work with previous versions of these software;
 however, we do not guarantee nor provide support for that.
 
 
 Install
 -------
```

### Comparing `mc3-3.1.1/docs/index.rst` & `mc3-3.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/license.rst` & `mc3-3.1.2/docs/license.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/make.bat` & `mc3-3.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/mcmc_tutorial.rst` & `mc3-3.1.2/docs/mcmc_tutorial.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/references.rst` & `mc3-3.1.2/docs/references.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/docs/time_averaging.rst` & `mc3-3.1.2/docs/time_averaging.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/examples/get_started.py` & `mc3-3.1.2/examples/get_started.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/examples/ns_tutorial.py` & `mc3-3.1.2/examples/ns_tutorial.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/examples/timeavg.py` & `mc3-3.1.2/examples/timeavg.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/examples/tutorial.py` & `mc3-3.1.2/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/__init__.py` & `mc3-3.1.2/mc3/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/__main__.py` & `mc3-3.1.2/mc3/__main__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/chain.py` & `mc3-3.1.2/mc3/chain.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/fit_driver.py` & `mc3-3.1.2/mc3/fit_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/mcmc_driver.py` & `mc3-3.1.2/mc3/mcmc_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/ns_driver.py` & `mc3-3.1.2/mc3/ns_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/plots/__init__.py` & `mc3-3.1.2/mc3/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/plots/colors.py` & `mc3-3.1.2/mc3/plots/colors.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/plots/plot_functions.py` & `mc3-3.1.2/mc3/plots/plot_functions.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/plots/posterior.py` & `mc3-3.1.2/mc3/plots/posterior.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,14 +223,15 @@
                 hist[irow,icol],
                 colors=colors, levels=levels,
                 origin='lower', extent=extent,
             )
             edge_color = to_rgba(theme.color, alpha=0.65)
             for c in cont.collections:
                 c.set_edgecolor(edge_color)
+                c.set_linewidth(0.1)
             cont.collections[0].set_edgecolor((1,1,1,0))
             if estimates[icol] is not None:
                 ax.axvline(
                     estimates[icol],
                     dashes=(9,2), lw=linewidth, color=theme.dark_color,
                 )
             if estimates[irow+1] is not None:
```

### Comparing `mc3-3.1.1/mc3/sampler.py` & `mc3-3.1.2/mc3/sampler.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/sampler_driver.py` & `mc3-3.1.2/mc3/sampler_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/stats/__init__.py` & `mc3-3.1.2/mc3/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/stats/gelman.py` & `mc3-3.1.2/mc3/stats/gelman.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/stats/prayer.py` & `mc3-3.1.2/mc3/stats/prayer.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/stats/stats.py` & `mc3-3.1.2/mc3/stats/stats.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/stats/time_averaging.py` & `mc3-3.1.2/mc3/stats/time_averaging.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/utils/__init__.py` & `mc3-3.1.2/mc3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/utils/log.py` & `mc3-3.1.2/mc3/utils/log.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3/utils/utils.py` & `mc3-3.1.2/mc3/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/mc3.egg-info/PKG-INFO` & `mc3-3.1.2/mc3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mc3
-Version: 3.1.1
+Version: 3.1.2
 Summary: Multi-core Markov-chain Monte Carlo package.
 Home-page: https://github.com/pcubillos/mc3
 Author: Patricio Cubillos
 Author-email: patricio.cubillos@oeaw.ac.at
 License: MIT
 Description: # mc3: Multi-core Markov-chain Monte Carlo
         > A Python implementation of the Markov-chain Monte Carlo algorithm.
```

### Comparing `mc3-3.1.1/mc3.egg-info/SOURCES.txt` & `mc3-3.1.2/mc3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/setup.py` & `mc3-3.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/src_c/_binarray.c` & `mc3-3.1.2/src_c/_binarray.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/src_c/_chisq.c` & `mc3-3.1.2/src_c/_chisq.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/src_c/_dwt.c` & `mc3-3.1.2/src_c/_dwt.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/src_c/_time_averaging.c` & `mc3-3.1.2/src_c/_time_averaging.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/src_c/include/ind.h` & `mc3-3.1.2/src_c/include/ind.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/src_c/include/stats.h` & `mc3-3.1.2/src_c/include/stats.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/src_c/include/wavelet.h` & `mc3-3.1.2/src_c/include/wavelet.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/tests/test_dynesty.py` & `mc3-3.1.2/tests/test_dynesty.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/tests/test_fit.py` & `mc3-3.1.2/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/tests/test_logging.py` & `mc3-3.1.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/tests/test_mcmc.py` & `mc3-3.1.2/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/tests/test_plots.py` & `mc3-3.1.2/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/tests/test_stats.py` & `mc3-3.1.2/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.1/tests/test_utils.py` & `mc3-3.1.2/tests/test_utils.py`

 * *Files identical despite different names*

