# Comparing `tmp/pyFileFixity-3.0.7.tar.gz` & `tmp/pyFileFixity-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFileFixity-3.0.7.tar", last modified: Fri Mar 31 00:07:31 2023, max compression
+gzip compressed data, was "pyFileFixity-3.0.8.tar", last modified: Fri Mar 31 00:34:54 2023, max compression
```

## Comparing `pyFileFixity-3.0.7.tar` & `pyFileFixity-3.0.8.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:31.275707 pyFileFixity-3.0.7/
--rw-rw-rw-   0        0        0      603 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/.coveragerc
--rw-rw-rw-   0        0        0     1084 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/LICENSE
--rw-rw-rw-   0        0        0      507 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1380 2022-12-09 04:21:15.000000 pyFileFixity-3.0.7/Makefile
--rw-rw-rw-   0        0        0    61817 2023-03-31 00:07:31.276705 pyFileFixity-3.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    58868 2022-12-09 04:20:36.000000 pyFileFixity-3.0.7/README.rst
--rw-rw-rw-   0        0        0    50832 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/TODO.md
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:30.728770 pyFileFixity-3.0.7/pyFileFixity/
--rw-rw-rw-   0        0        0      336 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/__init__.py
--rw-rw-rw-   0        0        0     8048 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/easy_profiler.py
--rw-rw-rw-   0        0        0     1026 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/ecc_specification.txt
--rw-rw-rw-   0        0        0     8026 2023-03-30 23:55:42.000000 pyFileFixity-3.0.7/pyFileFixity/ecc_speedtest.py
--rw-rw-rw-   0        0        0    17951 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/filetamper.py
--rw-rw-rw-   0        0        0    59856 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/header_ecc.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:30.800578 pyFileFixity-3.0.7/pyFileFixity/lib/
--rw-rw-rw-   0        0        0        2 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/__init__.py
--rw-rw-rw-   0        0        0     1357 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/_compat.py
--rw-rw-rw-   0        0        0    20261 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/aux_funcs.py
--rw-rw-rw-   0        0        0    16447 2023-03-30 21:18:38.000000 pyFileFixity-3.0.7/pyFileFixity/lib/eccman.py
--rw-rw-rw-   0        0        0     3385 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/hasher.py
--rw-rw-rw-   0        0        0    14183 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/md5py.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:30.809554 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/
--rw-rw-rw-   0        0        0        1 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:30.820524 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/memory_profiler/
--rw-rw-rw-   0        0        0        1 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/memory_profiler/__init__.py
--rw-rw-rw-   0        0        0    28865 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/memory_profiler/memory_profiler.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:30.832493 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pprofile/
--rw-rw-rw-   0        0        0        1 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pprofile/__init__.py
--rw-rw-rw-   0        0        0    29125 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pprofile/pprofile.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:30.854436 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pyinstrument/
--rw-rw-rw-   0        0        0       30 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pyinstrument/__init__.py
--rw-rw-rw-   0        0        0     4960 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pyinstrument/__main__.py
--rw-rw-rw-   0        0        0     2503 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pyinstrument/middleware.py
--rw-rw-rw-   0        0        0    13448 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pyinstrument/profiler.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:30.902400 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/
--rw-rw-rw-   0        0        0        1 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/__init__.py
--rw-rw-rw-   0        0        0     5261 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/debug.py
--rw-rw-rw-   0        0        0     6535 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/functionprofiler.py
--rw-rw-rw-   0        0        0     2365 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/kthread.py
--rw-rw-rw-   0        0        0    18471 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/memory_profiler.py
--rw-rw-rw-   0        0        0     4813 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/profilebrowser.py
--rw-rw-rw-   0        0        0    24812 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/profilehooks.py
--rw-rw-rw-   0        0        0    15436 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pycallgraph.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:30.980191 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/
--rw-rw-rw-   0        0        0      314 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/__init__.py
--rw-rw-rw-   0        0        0    90345 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/asizeof.py
--rw-rw-rw-   0        0        0     1974 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/charts.py
--rw-rw-rw-   0        0        0    19665 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/classtracker.py
--rw-rw-rw-   0        0        0    27011 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/classtracker_stats.py
--rw-rw-rw-   0        0        0     2464 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/garbagegraph.py
--rw-rw-rw-   0        0        0     1544 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/metadata.py
--rw-rw-rw-   0        0        0     3414 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/mprofile.py
--rw-rw-rw-   0        0        0     8459 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/muppy.py
--rw-rw-rw-   0        0        0     8562 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/process.py
--rw-rw-rw-   0        0        0    15213 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/refbrowser.py
--rw-rw-rw-   0        0        0    11959 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/refgraph.py
--rw-rw-rw-   0        0        0    10351 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/summary.py
--rw-rw-rw-   0        0        0     9788 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/tracker.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:31.008115 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/util/
--rw-rw-rw-   0        0        0        0 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/util/__init__.py
--rw-rw-rw-   0        0        0    63021 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/util/bottle2.py
--rw-rw-rw-   0        0        0    63069 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/util/bottle3.py
--rw-rw-rw-   0        0        0     1689 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/util/compat.py
--rw-rw-rw-   0        0        0     1865 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/util/stringutils.py
--rw-rw-rw-   0        0        0    10247 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/web.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:31.066959 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/
--rw-rw-rw-   0        0        0       65 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/__init__.py
--rw-rw-rw-   0        0        0     3042 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/_meliaejson.py
--rw-rw-rw-   0        0        0     5580 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/coldshotadapter.py
--rw-rw-rw-   0        0        0     2694 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/homedirectory.py
--rw-rw-rw-   0        0        0    11133 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/listviews.py
--rw-rw-rw-   0        0        0      231 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/macshim.py
--rw-rw-rw-   0        0        0     5979 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/meliaeadapter.py
--rw-rw-rw-   0        0        0    20210 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/meliaeloader.py
--rw-rw-rw-   0        0        0     2826 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/pstatsadapter.py
--rw-rw-rw-   0        0        0    11445 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/pstatsloader.py
--rw-rw-rw-   0        0        0    32046 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/runsnake.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:31.075936 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/squaremap/
--rw-rw-rw-   0        0        0       72 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/squaremap/__init__.py
--rw-rw-rw-   0        0        0    21515 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/squaremap/squaremap.py
--rw-rw-rw-   0        0        0    30098 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/six.py
--rw-rw-rw-   0        0        0     2927 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/lib/tee.py
--rw-rw-rw-   0        0        0    27284 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/repair_ecc.py
--rw-rw-rw-   0        0        0    36267 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/replication_repair.py
--rw-rw-rw-   0        0        0    26772 2022-12-09 03:28:39.000000 pyFileFixity-3.0.7/pyFileFixity/resiliency_tester.py
--rw-rw-rw-   0        0        0     1946 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/resiliency_tester_config.txt
--rw-rw-rw-   0        0        0    36643 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/rfigc.py
--rw-rw-rw-   0        0        0    68880 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/structural_adaptive_ecc.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:31.140070 pyFileFixity-3.0.7/pyFileFixity/tests/
--rw-rw-rw-   0        0        0        1 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/__init__.py
--rw-rw-rw-   0        0        0     6590 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/aux_tests.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:31.166000 pyFileFixity-3.0.7/pyFileFixity/tests/files/
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:31.171983 pyFileFixity-3.0.7/pyFileFixity/tests/files/Sub2/
--rw-rw-rw-   0        0        0        6 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/files/Sub2/testsub2.txt
--rw-rw-rw-   0        0        0    67254 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/files/alice.pdf
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:31.180960 pyFileFixity-3.0.7/pyFileFixity/tests/files/sub/
--rw-rw-rw-   0        0        0     2048 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/files/sub/Snark.zip
--rw-rw-rw-   0        0        0      253 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/files/sub/testsub.txt
--rw-rw-rw-   0        0        0        8 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/files/testaa.txt
--rw-rw-rw-   0        0        0    19719 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/files/tux.jpg
--rw-rw-rw-   0        0        0     3667 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/files/tuxsmall.jpg
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:31.270720 pyFileFixity-3.0.7/pyFileFixity/tests/results/
--rw-rw-rw-   0        0        0     2050 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/resiliency_tester_config_easy.cfg
--rw-rw-rw-   0        0        0     1627 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/resiliency_tester_config_hard.cfg
--rw-rw-rw-   0        0        0     1614 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_header_ecc_test_algo.db
--rw-rw-rw-   0        0        0     6473 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_header_ecc_test_dir.db
--rw-rw-rw-   0        0        0     1614 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_header_ecc_test_one_file.db
--rw-rw-rw-   0        0        0     1614 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_header_ecc_test_one_file_tamper.db
--rw-rw-rw-   0        0        0     6473 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_repair_ecc_check.db
--rw-rw-rw-   0        0        0    47542 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_repair_ecc_sa_check.db
--rw-rw-rw-   0        0        0      689 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_rfigc_test_dir.csv
--rw-rw-rw-   0        0        0      131 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_rfigc_test_error_file.log
--rw-rw-rw-   0        0        0      161 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_rfigc_test_one_file.csv
--rw-rw-rw-   0        0        0      686 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_rfigc_test_update_append.csv
--rw-rw-rw-   0        0        0      164 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_rfigc_test_update_remove.csv
--rw-rw-rw-   0        0        0     2883 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_algo.db
--rw-rw-rw-   0        0        0    47542 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_dir.db
--rw-rw-rw-   0        0        0     2883 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file.db
--rw-rw-rw-   0        0        0     2883 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file_tamper.db
--rw-rw-rw-   0        0        0     6323 2022-12-09 03:19:46.000000 pyFileFixity-3.0.7/pyFileFixity/tests/test_aux_funcs.py
--rw-rw-rw-   0        0        0     6916 2022-12-09 03:04:26.000000 pyFileFixity-3.0.7/pyFileFixity/tests/test_eccman.py
--rw-rw-rw-   0        0        0     1713 2022-12-09 03:05:18.000000 pyFileFixity-3.0.7/pyFileFixity/tests/test_hasher.py
--rw-rw-rw-   0        0        0     8111 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/test_header_ecc.py
--rw-rw-rw-   0        0        0     8229 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/test_repair_ecc.py
--rw-rw-rw-   0        0        0    12627 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/test_replication_repair.py
--rw-rw-rw-   0        0        0     8511 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/test_resiliency_tester.py
--rw-rw-rw-   0        0        0     6448 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/test_rfigc.py
--rw-rw-rw-   0        0        0    10510 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/test_structural_adaptive_ecc.py
--rw-rw-rw-   0        0        0     2240 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/pyFileFixity/tests/test_tee.py
-drwxrwxrwx   0        0        0        0 2023-03-31 00:07:30.750711 pyFileFixity-3.0.7/pyFileFixity.egg-info/
--rw-rw-rw-   0        0        0    61817 2023-03-31 00:07:28.000000 pyFileFixity-3.0.7/pyFileFixity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5350 2023-03-31 00:07:30.000000 pyFileFixity-3.0.7/pyFileFixity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 00:07:28.000000 pyFileFixity-3.0.7/pyFileFixity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-31 00:07:28.000000 pyFileFixity-3.0.7/pyFileFixity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-03-31 00:07:31.279695 pyFileFixity-3.0.7/setup.cfg
--rw-rw-rw-   0        0        0     8908 2023-03-30 22:37:27.000000 pyFileFixity-3.0.7/setup.py
--rw-rw-rw-   0        0        0     1382 2022-12-09 02:48:03.000000 pyFileFixity-3.0.7/tox.ini
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.527896 pyFileFixity-3.0.8/
+-rw-rw-rw-   0        0        0      603 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/.coveragerc
+-rw-rw-rw-   0        0        0     1084 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/LICENSE
+-rw-rw-rw-   0        0        0      507 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1380 2022-12-09 04:21:15.000000 pyFileFixity-3.0.8/Makefile
+-rw-rw-rw-   0        0        0    63279 2023-03-31 00:34:54.527896 pyFileFixity-3.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    60307 2023-03-31 00:31:51.000000 pyFileFixity-3.0.8/README.rst
+-rw-rw-rw-   0        0        0    50832 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/TODO.md
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.065741 pyFileFixity-3.0.8/pyFileFixity/
+-rw-rw-rw-   0        0        0      336 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/__init__.py
+-rw-rw-rw-   0        0        0     8048 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/easy_profiler.py
+-rw-rw-rw-   0        0        0     1026 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/ecc_specification.txt
+-rw-rw-rw-   0        0        0     8026 2023-03-30 23:55:42.000000 pyFileFixity-3.0.8/pyFileFixity/ecc_speedtest.py
+-rw-rw-rw-   0        0        0    17951 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/filetamper.py
+-rw-rw-rw-   0        0        0    59856 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/header_ecc.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.121593 pyFileFixity-3.0.8/pyFileFixity/lib/
+-rw-rw-rw-   0        0        0        2 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/__init__.py
+-rw-rw-rw-   0        0        0     1357 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/_compat.py
+-rw-rw-rw-   0        0        0    20261 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/aux_funcs.py
+-rw-rw-rw-   0        0        0    16447 2023-03-30 21:18:38.000000 pyFileFixity-3.0.8/pyFileFixity/lib/eccman.py
+-rw-rw-rw-   0        0        0     3385 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/hasher.py
+-rw-rw-rw-   0        0        0    14183 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/md5py.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.128574 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/
+-rw-rw-rw-   0        0        0        1 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.140540 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/memory_profiler/
+-rw-rw-rw-   0        0        0        1 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/memory_profiler/__init__.py
+-rw-rw-rw-   0        0        0    28865 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/memory_profiler/memory_profiler.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.152511 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pprofile/
+-rw-rw-rw-   0        0        0        1 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pprofile/__init__.py
+-rw-rw-rw-   0        0        0    29125 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pprofile/pprofile.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.169463 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pyinstrument/
+-rw-rw-rw-   0        0        0       30 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pyinstrument/__init__.py
+-rw-rw-rw-   0        0        0     4960 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pyinstrument/__main__.py
+-rw-rw-rw-   0        0        0     2503 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pyinstrument/middleware.py
+-rw-rw-rw-   0        0        0    13448 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pyinstrument/profiler.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.214343 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/
+-rw-rw-rw-   0        0        0        1 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/__init__.py
+-rw-rw-rw-   0        0        0     5261 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/debug.py
+-rw-rw-rw-   0        0        0     6535 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/functionprofiler.py
+-rw-rw-rw-   0        0        0     2365 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/kthread.py
+-rw-rw-rw-   0        0        0    18471 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/memory_profiler.py
+-rw-rw-rw-   0        0        0     4813 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/profilebrowser.py
+-rw-rw-rw-   0        0        0    24812 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/profilehooks.py
+-rw-rw-rw-   0        0        0    15436 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pycallgraph.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.279171 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/
+-rw-rw-rw-   0        0        0      314 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/__init__.py
+-rw-rw-rw-   0        0        0    90345 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/asizeof.py
+-rw-rw-rw-   0        0        0     1974 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/charts.py
+-rw-rw-rw-   0        0        0    19665 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/classtracker.py
+-rw-rw-rw-   0        0        0    27011 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/classtracker_stats.py
+-rw-rw-rw-   0        0        0     2464 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/garbagegraph.py
+-rw-rw-rw-   0        0        0     1544 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/metadata.py
+-rw-rw-rw-   0        0        0     3414 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/mprofile.py
+-rw-rw-rw-   0        0        0     8459 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/muppy.py
+-rw-rw-rw-   0        0        0     8562 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/process.py
+-rw-rw-rw-   0        0        0    15213 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/refbrowser.py
+-rw-rw-rw-   0        0        0    11959 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/refgraph.py
+-rw-rw-rw-   0        0        0    10351 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/summary.py
+-rw-rw-rw-   0        0        0     9788 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/tracker.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.303497 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/util/
+-rw-rw-rw-   0        0        0        0 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/util/__init__.py
+-rw-rw-rw-   0        0        0    63021 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/util/bottle2.py
+-rw-rw-rw-   0        0        0    63069 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/util/bottle3.py
+-rw-rw-rw-   0        0        0     1689 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/util/compat.py
+-rw-rw-rw-   0        0        0     1865 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/util/stringutils.py
+-rw-rw-rw-   0        0        0    10247 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/web.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.355359 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/
+-rw-rw-rw-   0        0        0       65 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/__init__.py
+-rw-rw-rw-   0        0        0     3042 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/_meliaejson.py
+-rw-rw-rw-   0        0        0     5580 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/coldshotadapter.py
+-rw-rw-rw-   0        0        0     2694 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/homedirectory.py
+-rw-rw-rw-   0        0        0    11133 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/listviews.py
+-rw-rw-rw-   0        0        0      231 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/macshim.py
+-rw-rw-rw-   0        0        0     5979 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/meliaeadapter.py
+-rw-rw-rw-   0        0        0    20210 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/meliaeloader.py
+-rw-rw-rw-   0        0        0     2826 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/pstatsadapter.py
+-rw-rw-rw-   0        0        0    11445 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/pstatsloader.py
+-rw-rw-rw-   0        0        0    32046 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/runsnake.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.367327 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/squaremap/
+-rw-rw-rw-   0        0        0       72 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/squaremap/__init__.py
+-rw-rw-rw-   0        0        0    21515 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/squaremap/squaremap.py
+-rw-rw-rw-   0        0        0    30098 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/six.py
+-rw-rw-rw-   0        0        0     2927 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/lib/tee.py
+-rw-rw-rw-   0        0        0    27284 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/repair_ecc.py
+-rw-rw-rw-   0        0        0    36267 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/replication_repair.py
+-rw-rw-rw-   0        0        0    26772 2022-12-09 03:28:39.000000 pyFileFixity-3.0.8/pyFileFixity/resiliency_tester.py
+-rw-rw-rw-   0        0        0     1946 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/resiliency_tester_config.txt
+-rw-rw-rw-   0        0        0    36643 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/rfigc.py
+-rw-rw-rw-   0        0        0    68880 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/structural_adaptive_ecc.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.421183 pyFileFixity-3.0.8/pyFileFixity/tests/
+-rw-rw-rw-   0        0        0        1 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/__init__.py
+-rw-rw-rw-   0        0        0     6590 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/aux_tests.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.438137 pyFileFixity-3.0.8/pyFileFixity/tests/files/
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.442126 pyFileFixity-3.0.8/pyFileFixity/tests/files/Sub2/
+-rw-rw-rw-   0        0        0        6 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/files/Sub2/testsub2.txt
+-rw-rw-rw-   0        0        0    67254 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/files/alice.pdf
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.450105 pyFileFixity-3.0.8/pyFileFixity/tests/files/sub/
+-rw-rw-rw-   0        0        0     2048 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/files/sub/Snark.zip
+-rw-rw-rw-   0        0        0      253 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/files/sub/testsub.txt
+-rw-rw-rw-   0        0        0        8 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/files/testaa.txt
+-rw-rw-rw-   0        0        0    19719 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/files/tux.jpg
+-rw-rw-rw-   0        0        0     3667 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/files/tuxsmall.jpg
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.524904 pyFileFixity-3.0.8/pyFileFixity/tests/results/
+-rw-rw-rw-   0        0        0     2050 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/resiliency_tester_config_easy.cfg
+-rw-rw-rw-   0        0        0     1627 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/resiliency_tester_config_hard.cfg
+-rw-rw-rw-   0        0        0     1614 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_header_ecc_test_algo.db
+-rw-rw-rw-   0        0        0     6473 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_header_ecc_test_dir.db
+-rw-rw-rw-   0        0        0     1614 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_header_ecc_test_one_file.db
+-rw-rw-rw-   0        0        0     1614 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_header_ecc_test_one_file_tamper.db
+-rw-rw-rw-   0        0        0     6473 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_repair_ecc_check.db
+-rw-rw-rw-   0        0        0    47542 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_repair_ecc_sa_check.db
+-rw-rw-rw-   0        0        0      689 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_rfigc_test_dir.csv
+-rw-rw-rw-   0        0        0      131 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_rfigc_test_error_file.log
+-rw-rw-rw-   0        0        0      161 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_rfigc_test_one_file.csv
+-rw-rw-rw-   0        0        0      686 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_rfigc_test_update_append.csv
+-rw-rw-rw-   0        0        0      164 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_rfigc_test_update_remove.csv
+-rw-rw-rw-   0        0        0     2883 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_algo.db
+-rw-rw-rw-   0        0        0    47542 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_dir.db
+-rw-rw-rw-   0        0        0     2883 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file.db
+-rw-rw-rw-   0        0        0     2883 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file_tamper.db
+-rw-rw-rw-   0        0        0     6323 2022-12-09 03:19:46.000000 pyFileFixity-3.0.8/pyFileFixity/tests/test_aux_funcs.py
+-rw-rw-rw-   0        0        0     6916 2022-12-09 03:04:26.000000 pyFileFixity-3.0.8/pyFileFixity/tests/test_eccman.py
+-rw-rw-rw-   0        0        0     1713 2022-12-09 03:05:18.000000 pyFileFixity-3.0.8/pyFileFixity/tests/test_hasher.py
+-rw-rw-rw-   0        0        0     8111 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/test_header_ecc.py
+-rw-rw-rw-   0        0        0     8229 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/test_repair_ecc.py
+-rw-rw-rw-   0        0        0    12627 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/test_replication_repair.py
+-rw-rw-rw-   0        0        0     8511 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/test_resiliency_tester.py
+-rw-rw-rw-   0        0        0     6448 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/test_rfigc.py
+-rw-rw-rw-   0        0        0    10510 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/test_structural_adaptive_ecc.py
+-rw-rw-rw-   0        0        0     2240 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/pyFileFixity/tests/test_tee.py
+drwxrwxrwx   0        0        0        0 2023-03-31 00:34:54.083692 pyFileFixity-3.0.8/pyFileFixity.egg-info/
+-rw-rw-rw-   0        0        0    63279 2023-03-31 00:34:52.000000 pyFileFixity-3.0.8/pyFileFixity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5350 2023-03-31 00:34:53.000000 pyFileFixity-3.0.8/pyFileFixity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-31 00:34:52.000000 pyFileFixity-3.0.8/pyFileFixity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-03-31 00:34:52.000000 pyFileFixity-3.0.8/pyFileFixity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-03-31 00:34:54.530887 pyFileFixity-3.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     8908 2023-03-30 22:37:27.000000 pyFileFixity-3.0.8/setup.py
+-rw-rw-rw-   0        0        0     1382 2022-12-09 02:48:03.000000 pyFileFixity-3.0.8/tox.ini
```

### Comparing `pyFileFixity-3.0.7/.coveragerc` & `pyFileFixity-3.0.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/LICENSE` & `pyFileFixity-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/Makefile` & `pyFileFixity-3.0.8/Makefile`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/PKG-INFO` & `pyFileFixity-3.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFileFixity
-Version: 3.0.7
+Version: 3.0.8
 Summary: Helping file fixity (long term storage of data) via redundant error correcting codes and hash auditing.
 Home-page: https://github.com/lrq3000/pyFileFixity
 Author: Stephen Larroque
 Author-email: LRQ3000@gmail.com
 Maintainer: Stephen Larroque
 Maintainer-email: LRQ3000@gmail.com
 License: MIT License
@@ -43,17 +43,21 @@
 pyFileFixity
 ============
 
 |PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
 
 |Build-Status| |Coverage|
 
-This project aims to provide a set of open source, cross-platform, easy
+pyFileFixity provides a suite of open source, cross-platform, easy
 to use and easy to maintain (readable code) to protect and manage data
-for long term storage. The project is done in pure-Python to meet those criteria.
+for long term storage/archival, and also test the performance of any data protection algorithms.
+
+The project is done in pure-Python to meet those criteria,
+although cythonized extensions are available for core routines to speed up encoding/decoding,
+but always with a pure python specification available so as to allow long term replication.
 
 Here is an example of what pyFileFixity can do:
 
 |Example|
 
 On the left, this is the original image.
 
@@ -142,28 +146,28 @@
 
 ``resiliency_tester.py -i "your_folder" -o "test_folder" -c "resiliency_tester_config.txt" -m 3 -l "testlog.txt" -f``
 
 - To get more options for any tool, use ``--help``.
 
 - DEPRECATED (because Gooey is not maintained anymore it seems): To use the GUI with any tool, use ``--gui`` and do not supply any other argument, eg: ``python rfigc.py --gui``.
 
-- You can also use `PyPy <http://pypy.org/>`_ to hugely speedup the processing time of any tool here.
+- You can also use `PyPy <http://pypy.org/>`_ or Cython to hugely speedup the processing time of any tool here.
 
 The problem of long term storage
 --------------------------------
 
-Why are data corrupted with time? Entropy, my friend, entropy.
+Why are data corrupted with time? One sole reason: entropy.
 Entropy refers to the universal tendency for systems to become
-less ordered over time. Corruption is exactly that: a disorder
+less ordered over time. Data corruption is exactly that: a disorder
 in bits order. In other words: *the Universe hates your data*.
 
 Long term storage is thus a very difficult topic: it's like fighting with
 death (in this case, the death of data). Indeed, because of entropy,
 data will eventually fade away because of various silent errors such as
-bit rot. pyFileFixity aims to provide tools to detect any data
+bit rot or cosmic rays. pyFileFixity aims to provide tools to detect any data
 corruption, but also fight data corruption by providing repairing tools.
 
 The only solution is to use a principle of engineering that is long
 known and which makes bridges safe: add some **redundancy**.
 
 There are only 2 ways to add redundancy:
 
@@ -216,14 +220,23 @@
 different kinds of error correction codes to protect and repair files.
 
 Also, the ecc file specification is made to be simple and resilient to
 corruption, so that you can process it by your own means if you want to,
 without having to study for hours how the code works (contrary to PAR2
 format).
 
+In practice, both approaches are not exclusive, and the best is to
+combine them: protect the most precious data with error correction codes,
+then duplicate them across multiple storage mediums. Hence, this suite of
+data protection tools, just like any other such suite, is not sufficient to
+guarantee your data is protected, you must have an active data curation strategy
+which includes regularly checking your data and replacing copies that are damaged.
+
+For a primer on storage mediums and data protection strategies, see `this post I wrote <https://web.archive.org/web/20220529125543/https://superuser.com/questions/374609/what-medium-should-be-used-for-long-term-high-volume-data-storage-archival/873260>`_.
+
 Why not just use RAID ?
 -----------------------
 
 RAID is clearly insufficient for long-term data storage, and in fact it
 was primarily meant as a cheap way to get more storage (RAID0) or more
 availability (RAID1) of data, not for archiving data, even on a medium
 timescale:
@@ -683,18 +696,28 @@
    thus the generated ECC won't be compatible with algo 1 to 3.
    But do not be scared, the ECC will work just the same.
 
 Cython implementation
 ---------------------
 
 This section describes how to use the Cython implementation. However,
-you should first try PyPy, as it did give 10x to 100x speedup over
-Cython in our case.
+you should first try PyPy, as it may give great performances too.
+
+Simply follow the instruction to install the `reedsolo <https://github.com/tomerfiliba/reedsolomon/releases/tag/v2.0.5>`_ module with
+the cythonized module:
+
+.. code:: sh
+    
+    pip install --upgrade reedsolo --install-option="--cythonize" --verbose
+
+Then make sure to use ``ecc_algo=3`` in all your ``eccman`` calls, and you
+are then good to go, the cythonized module ``creedsolo`` will always be used
+for both encoding and decoding transparently.
 
-THIS SECTION ISÂ OLD AND DEPRECATED, because the Cython compilation is now
+THE REST OF THIS SECTION ISÂ OLD AND DEPRECATED, because the Cython compilation is now
 done directly in the Reed-Solomon submodules, instead of here, so you
 should not need to worry about it, just pip install with the requirements.txt
 and you should be set. The information below is left for historical purposes:
 
 A speedy Cython implementation of the Reed-Solomon library is included.
 It should provide C-speed for all scripts (as long as you use
 --ecc\_algo 1 or 2, not 3 nor 4). It is not needed, since a pure-python
```

### Comparing `pyFileFixity-3.0.7/README.rst` & `pyFileFixity-3.0.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 pyFileFixity
 ============
 
 |PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
 
 |Build-Status| |Coverage|
 
-This project aims to provide a set of open source, cross-platform, easy
+pyFileFixity provides a suite of open source, cross-platform, easy
 to use and easy to maintain (readable code) to protect and manage data
-for long term storage. The project is done in pure-Python to meet those criteria.
+for long term storage/archival, and also test the performance of any data protection algorithms.
+
+The project is done in pure-Python to meet those criteria,
+although cythonized extensions are available for core routines to speed up encoding/decoding,
+but always with a pure python specification available so as to allow long term replication.
 
 Here is an example of what pyFileFixity can do:
 
 |Example|
 
 On the left, this is the original image.
 
@@ -100,28 +104,28 @@
 
 ``resiliency_tester.py -i "your_folder" -o "test_folder" -c "resiliency_tester_config.txt" -m 3 -l "testlog.txt" -f``
 
 - To get more options for any tool, use ``--help``.
 
 - DEPRECATED (because Gooey is not maintained anymore it seems): To use the GUI with any tool, use ``--gui`` and do not supply any other argument, eg: ``python rfigc.py --gui``.
 
-- You can also use `PyPy <http://pypy.org/>`_ to hugely speedup the processing time of any tool here.
+- You can also use `PyPy <http://pypy.org/>`_ or Cython to hugely speedup the processing time of any tool here.
 
 The problem of long term storage
 --------------------------------
 
-Why are data corrupted with time? Entropy, my friend, entropy.
+Why are data corrupted with time? One sole reason: entropy.
 Entropy refers to the universal tendency for systems to become
-less ordered over time. Corruption is exactly that: a disorder
+less ordered over time. Data corruption is exactly that: a disorder
 in bits order. In other words: *the Universe hates your data*.
 
 Long term storage is thus a very difficult topic: it's like fighting with
 death (in this case, the death of data). Indeed, because of entropy,
 data will eventually fade away because of various silent errors such as
-bit rot. pyFileFixity aims to provide tools to detect any data
+bit rot or cosmic rays. pyFileFixity aims to provide tools to detect any data
 corruption, but also fight data corruption by providing repairing tools.
 
 The only solution is to use a principle of engineering that is long
 known and which makes bridges safe: add some **redundancy**.
 
 There are only 2 ways to add redundancy:
 
@@ -174,14 +178,23 @@
 different kinds of error correction codes to protect and repair files.
 
 Also, the ecc file specification is made to be simple and resilient to
 corruption, so that you can process it by your own means if you want to,
 without having to study for hours how the code works (contrary to PAR2
 format).
 
+In practice, both approaches are not exclusive, and the best is to
+combine them: protect the most precious data with error correction codes,
+then duplicate them across multiple storage mediums. Hence, this suite of
+data protection tools, just like any other such suite, is not sufficient to
+guarantee your data is protected, you must have an active data curation strategy
+which includes regularly checking your data and replacing copies that are damaged.
+
+For a primer on storage mediums and data protection strategies, see `this post I wrote <https://web.archive.org/web/20220529125543/https://superuser.com/questions/374609/what-medium-should-be-used-for-long-term-high-volume-data-storage-archival/873260>`_.
+
 Why not just use RAID ?
 -----------------------
 
 RAID is clearly insufficient for long-term data storage, and in fact it
 was primarily meant as a cheap way to get more storage (RAID0) or more
 availability (RAID1) of data, not for archiving data, even on a medium
 timescale:
@@ -641,18 +654,28 @@
    thus the generated ECC won't be compatible with algo 1 to 3.
    But do not be scared, the ECC will work just the same.
 
 Cython implementation
 ---------------------
 
 This section describes how to use the Cython implementation. However,
-you should first try PyPy, as it did give 10x to 100x speedup over
-Cython in our case.
+you should first try PyPy, as it may give great performances too.
+
+Simply follow the instruction to install the `reedsolo <https://github.com/tomerfiliba/reedsolomon/releases/tag/v2.0.5>`_ module with
+the cythonized module:
+
+.. code:: sh
+    
+    pip install --upgrade reedsolo --install-option="--cythonize" --verbose
+
+Then make sure to use ``ecc_algo=3`` in all your ``eccman`` calls, and you
+are then good to go, the cythonized module ``creedsolo`` will always be used
+for both encoding and decoding transparently.
 
-THIS SECTION IS OLD AND DEPRECATED, because the Cython compilation is now
+THE REST OF THIS SECTION IS OLD AND DEPRECATED, because the Cython compilation is now
 done directly in the Reed-Solomon submodules, instead of here, so you
 should not need to worry about it, just pip install with the requirements.txt
 and you should be set. The information below is left for historical purposes:
 
 A speedy Cython implementation of the Reed-Solomon library is included.
 It should provide C-speed for all scripts (as long as you use
 --ecc\_algo 1 or 2, not 3 nor 4). It is not needed, since a pure-python
```

### Comparing `pyFileFixity-3.0.7/TODO.md` & `pyFileFixity-3.0.8/TODO.md`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/easy_profiler.py` & `pyFileFixity-3.0.8/pyFileFixity/easy_profiler.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/ecc_specification.txt` & `pyFileFixity-3.0.8/pyFileFixity/ecc_specification.txt`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/ecc_speedtest.py` & `pyFileFixity-3.0.8/pyFileFixity/ecc_speedtest.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/filetamper.py` & `pyFileFixity-3.0.8/pyFileFixity/filetamper.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/header_ecc.py` & `pyFileFixity-3.0.8/pyFileFixity/header_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/_compat.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/_compat.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/aux_funcs.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/aux_funcs.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/eccman.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/eccman.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/hasher.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/hasher.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/md5py.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/md5py.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/memory_profiler/memory_profiler.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/memory_profiler/memory_profiler.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pprofile/pprofile.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pprofile/pprofile.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pyinstrument/__main__.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pyinstrument/__main__.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pyinstrument/middleware.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pyinstrument/middleware.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/pyinstrument/profiler.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/pyinstrument/profiler.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/debug.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/debug.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/functionprofiler.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/functionprofiler.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/kthread.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/kthread.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/memory_profiler.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/memory_profiler.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/profilebrowser.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/profilebrowser.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/profilehooks.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/profilehooks.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pycallgraph.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pycallgraph.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/asizeof.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/charts.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/charts.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/classtracker.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/classtracker.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/classtracker_stats.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/classtracker_stats.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/garbagegraph.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/garbagegraph.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/metadata.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/metadata.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/mprofile.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/mprofile.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/muppy.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/muppy.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/process.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/process.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/refbrowser.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/refbrowser.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/refgraph.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/refgraph.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/summary.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/summary.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/tracker.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/tracker.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/util/bottle2.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/util/bottle2.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/util/bottle3.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/util/bottle3.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/util/compat.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/util/compat.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/util/stringutils.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/util/stringutils.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/pympler/web.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/pympler/web.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/_meliaejson.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/_meliaejson.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/coldshotadapter.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/coldshotadapter.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/homedirectory.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/homedirectory.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/listviews.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/listviews.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/meliaeadapter.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/meliaeadapter.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/meliaeloader.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/meliaeloader.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/pstatsadapter.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/pstatsadapter.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/pstatsloader.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/pstatsloader.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/runsnake.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/runsnake.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/profilers/visual/runsnakerun/squaremap/squaremap.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/profilers/visual/runsnakerun/squaremap/squaremap.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/six.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/six.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/lib/tee.py` & `pyFileFixity-3.0.8/pyFileFixity/lib/tee.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/repair_ecc.py` & `pyFileFixity-3.0.8/pyFileFixity/repair_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/replication_repair.py` & `pyFileFixity-3.0.8/pyFileFixity/replication_repair.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/resiliency_tester.py` & `pyFileFixity-3.0.8/pyFileFixity/resiliency_tester.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/resiliency_tester_config.txt` & `pyFileFixity-3.0.8/pyFileFixity/resiliency_tester_config.txt`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/rfigc.py` & `pyFileFixity-3.0.8/pyFileFixity/rfigc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/structural_adaptive_ecc.py` & `pyFileFixity-3.0.8/pyFileFixity/structural_adaptive_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/aux_tests.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/aux_tests.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/files/alice.pdf` & `pyFileFixity-3.0.8/pyFileFixity/tests/files/alice.pdf`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/files/sub/Snark.zip` & `pyFileFixity-3.0.8/pyFileFixity/tests/files/sub/Snark.zip`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/files/tux.jpg` & `pyFileFixity-3.0.8/pyFileFixity/tests/files/tux.jpg`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/files/tuxsmall.jpg` & `pyFileFixity-3.0.8/pyFileFixity/tests/files/tuxsmall.jpg`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/resiliency_tester_config_easy.cfg` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/resiliency_tester_config_easy.cfg`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/resiliency_tester_config_hard.cfg` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/resiliency_tester_config_hard.cfg`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_header_ecc_test_algo.db` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_header_ecc_test_algo.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_header_ecc_test_dir.db` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_header_ecc_test_dir.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_header_ecc_test_one_file.db` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_header_ecc_test_one_file.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_header_ecc_test_one_file_tamper.db` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_header_ecc_test_one_file_tamper.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_repair_ecc_check.db` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_repair_ecc_check.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_repair_ecc_sa_check.db` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_repair_ecc_sa_check.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_rfigc_test_dir.csv` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_rfigc_test_dir.csv`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_rfigc_test_update_append.csv` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_rfigc_test_update_append.csv`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_algo.db` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_algo.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_dir.db` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_dir.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file.db` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file_tamper.db` & `pyFileFixity-3.0.8/pyFileFixity/tests/results/test_structural_adaptive_ecc_test_one_file_tamper.db`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/test_aux_funcs.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/test_aux_funcs.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/test_eccman.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/test_eccman.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/test_hasher.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/test_hasher.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/test_header_ecc.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/test_header_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/test_repair_ecc.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/test_repair_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/test_replication_repair.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/test_replication_repair.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/test_resiliency_tester.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/test_resiliency_tester.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/test_rfigc.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/test_rfigc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/test_structural_adaptive_ecc.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/test_structural_adaptive_ecc.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity/tests/test_tee.py` & `pyFileFixity-3.0.8/pyFileFixity/tests/test_tee.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/pyFileFixity.egg-info/PKG-INFO` & `pyFileFixity-3.0.8/pyFileFixity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFileFixity
-Version: 3.0.7
+Version: 3.0.8
 Summary: Helping file fixity (long term storage of data) via redundant error correcting codes and hash auditing.
 Home-page: https://github.com/lrq3000/pyFileFixity
 Author: Stephen Larroque
 Author-email: LRQ3000@gmail.com
 Maintainer: Stephen Larroque
 Maintainer-email: LRQ3000@gmail.com
 License: MIT License
@@ -43,17 +43,21 @@
 pyFileFixity
 ============
 
 |PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
 
 |Build-Status| |Coverage|
 
-This project aims to provide a set of open source, cross-platform, easy
+pyFileFixity provides a suite of open source, cross-platform, easy
 to use and easy to maintain (readable code) to protect and manage data
-for long term storage. The project is done in pure-Python to meet those criteria.
+for long term storage/archival, and also test the performance of any data protection algorithms.
+
+The project is done in pure-Python to meet those criteria,
+although cythonized extensions are available for core routines to speed up encoding/decoding,
+but always with a pure python specification available so as to allow long term replication.
 
 Here is an example of what pyFileFixity can do:
 
 |Example|
 
 On the left, this is the original image.
 
@@ -142,28 +146,28 @@
 
 ``resiliency_tester.py -i "your_folder" -o "test_folder" -c "resiliency_tester_config.txt" -m 3 -l "testlog.txt" -f``
 
 - To get more options for any tool, use ``--help``.
 
 - DEPRECATED (because Gooey is not maintained anymore it seems): To use the GUI with any tool, use ``--gui`` and do not supply any other argument, eg: ``python rfigc.py --gui``.
 
-- You can also use `PyPy <http://pypy.org/>`_ to hugely speedup the processing time of any tool here.
+- You can also use `PyPy <http://pypy.org/>`_ or Cython to hugely speedup the processing time of any tool here.
 
 The problem of long term storage
 --------------------------------
 
-Why are data corrupted with time? Entropy, my friend, entropy.
+Why are data corrupted with time? One sole reason: entropy.
 Entropy refers to the universal tendency for systems to become
-less ordered over time. Corruption is exactly that: a disorder
+less ordered over time. Data corruption is exactly that: a disorder
 in bits order. In other words: *the Universe hates your data*.
 
 Long term storage is thus a very difficult topic: it's like fighting with
 death (in this case, the death of data). Indeed, because of entropy,
 data will eventually fade away because of various silent errors such as
-bit rot. pyFileFixity aims to provide tools to detect any data
+bit rot or cosmic rays. pyFileFixity aims to provide tools to detect any data
 corruption, but also fight data corruption by providing repairing tools.
 
 The only solution is to use a principle of engineering that is long
 known and which makes bridges safe: add some **redundancy**.
 
 There are only 2 ways to add redundancy:
 
@@ -216,14 +220,23 @@
 different kinds of error correction codes to protect and repair files.
 
 Also, the ecc file specification is made to be simple and resilient to
 corruption, so that you can process it by your own means if you want to,
 without having to study for hours how the code works (contrary to PAR2
 format).
 
+In practice, both approaches are not exclusive, and the best is to
+combine them: protect the most precious data with error correction codes,
+then duplicate them across multiple storage mediums. Hence, this suite of
+data protection tools, just like any other such suite, is not sufficient to
+guarantee your data is protected, you must have an active data curation strategy
+which includes regularly checking your data and replacing copies that are damaged.
+
+For a primer on storage mediums and data protection strategies, see `this post I wrote <https://web.archive.org/web/20220529125543/https://superuser.com/questions/374609/what-medium-should-be-used-for-long-term-high-volume-data-storage-archival/873260>`_.
+
 Why not just use RAID ?
 -----------------------
 
 RAID is clearly insufficient for long-term data storage, and in fact it
 was primarily meant as a cheap way to get more storage (RAID0) or more
 availability (RAID1) of data, not for archiving data, even on a medium
 timescale:
@@ -683,18 +696,28 @@
    thus the generated ECC won't be compatible with algo 1 to 3.
    But do not be scared, the ECC will work just the same.
 
 Cython implementation
 ---------------------
 
 This section describes how to use the Cython implementation. However,
-you should first try PyPy, as it did give 10x to 100x speedup over
-Cython in our case.
+you should first try PyPy, as it may give great performances too.
+
+Simply follow the instruction to install the `reedsolo <https://github.com/tomerfiliba/reedsolomon/releases/tag/v2.0.5>`_ module with
+the cythonized module:
+
+.. code:: sh
+    
+    pip install --upgrade reedsolo --install-option="--cythonize" --verbose
+
+Then make sure to use ``ecc_algo=3`` in all your ``eccman`` calls, and you
+are then good to go, the cythonized module ``creedsolo`` will always be used
+for both encoding and decoding transparently.
 
-THIS SECTION ISÂ OLD AND DEPRECATED, because the Cython compilation is now
+THE REST OF THIS SECTION ISÂ OLD AND DEPRECATED, because the Cython compilation is now
 done directly in the Reed-Solomon submodules, instead of here, so you
 should not need to worry about it, just pip install with the requirements.txt
 and you should be set. The information below is left for historical purposes:
 
 A speedy Cython implementation of the Reed-Solomon library is included.
 It should provide C-speed for all scripts (as long as you use
 --ecc\_algo 1 or 2, not 3 nor 4). It is not needed, since a pure-python
```

### Comparing `pyFileFixity-3.0.7/pyFileFixity.egg-info/SOURCES.txt` & `pyFileFixity-3.0.8/pyFileFixity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/setup.py` & `pyFileFixity-3.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `pyFileFixity-3.0.7/tox.ini` & `pyFileFixity-3.0.8/tox.ini`

 * *Files identical despite different names*

