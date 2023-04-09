# Comparing `tmp/popgym-1.0.1.tar.gz` & `tmp/popgym-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popgym-1.0.1.tar", last modified: Sat Mar 11 19:22:25 2023, max compression
+gzip compressed data, was "popgym-1.0.2.tar", last modified: Sun Apr  9 17:17:30 2023, max compression
```

## Comparing `popgym-1.0.1.tar` & `popgym-1.0.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.130166 popgym-1.0.1/
--rw-r--r--   0 smorad     (501) staff       (20)     1069 2023-01-26 13:50:44.000000 popgym-1.0.1/LICENSE.md
--rw-r--r--   0 smorad     (501) staff       (20)     7567 2023-03-11 19:22:25.130236 popgym-1.0.1/PKG-INFO
--rw-r--r--   0 smorad     (501) staff       (20)     7240 2023-03-11 17:40:45.000000 popgym-1.0.1/README.md
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.119984 popgym-1.0.1/popgym/
--rw-r--r--   0 smorad     (501) staff       (20)       73 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/__init__.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.120727 popgym-1.0.1/popgym/baselines/
--rw-r--r--   0 smorad     (501) staff       (20)       85 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/__init__.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.121591 popgym-1.0.1/popgym/baselines/models/
--rw-r--r--   0 smorad     (501) staff       (20)        0 2023-03-08 13:39:50.000000 popgym-1.0.1/popgym/baselines/models/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)      992 2022-09-22 16:05:05.000000 popgym-1.0.1/popgym/baselines/models/aggregations.py
--rw-r--r--   0 smorad     (501) staff       (20)     9855 2022-09-22 16:05:05.000000 popgym-1.0.1/popgym/baselines/models/embeddings.py
--rw-r--r--   0 smorad     (501) staff       (20)     1834 2023-01-26 13:50:44.000000 popgym-1.0.1/popgym/baselines/models/fwp.py
--rw-r--r--   0 smorad     (501) staff       (20)     2046 2022-09-22 16:05:05.000000 popgym-1.0.1/popgym/baselines/models/indrnn.py
--rw-r--r--   0 smorad     (501) staff       (20)     2450 2022-09-22 16:05:05.000000 popgym-1.0.1/popgym/baselines/models/linear_attention.py
--rw-r--r--   0 smorad     (501) staff       (20)    10069 2022-09-27 16:44:40.000000 popgym-1.0.1/popgym/baselines/models/lmu.py
--rw-r--r--   0 smorad     (501) staff       (20)    60700 2022-10-08 11:28:47.000000 popgym-1.0.1/popgym/baselines/models/s4d.py
--rw-r--r--   0 smorad     (501) staff       (20)     7318 2023-01-26 13:50:44.000000 popgym-1.0.1/popgym/baselines/ppo.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.123526 popgym-1.0.1/popgym/baselines/ray_models/
--rw-r--r--   0 smorad     (501) staff       (20)        0 2023-03-08 13:39:50.000000 popgym-1.0.1/popgym/baselines/ray_models/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)    12303 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/base_model.py
--rw-r--r--   0 smorad     (501) staff       (20)     5407 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_diffnc.py
--rw-r--r--   0 smorad     (501) staff       (20)     2367 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_elman.py
--rw-r--r--   0 smorad     (501) staff       (20)     2343 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_frameconv.py
--rw-r--r--   0 smorad     (501) staff       (20)     3689 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_framestack.py
--rw-r--r--   0 smorad     (501) staff       (20)     3543 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_fwp.py
--rw-r--r--   0 smorad     (501) staff       (20)     2493 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_gru.py
--rw-r--r--   0 smorad     (501) staff       (20)     2359 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_indrnn.py
--rw-r--r--   0 smorad     (501) staff       (20)     3772 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_linear_attention.py
--rw-r--r--   0 smorad     (501) staff       (20)     2269 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_lmu.py
--rw-r--r--   0 smorad     (501) staff       (20)     2617 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_lstm.py
--rw-r--r--   0 smorad     (501) staff       (20)     1441 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_mlp.py
--rw-r--r--   0 smorad     (501) staff       (20)     2704 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/baselines/ray_models/ray_s4d.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.124189 popgym-1.0.1/popgym/core/
--rw-r--r--   0 smorad     (501) staff       (20)       56 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/core/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     9714 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/core/deck.py
--rw-r--r--   0 smorad     (501) staff       (20)      863 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/core/env.py
--rw-r--r--   0 smorad     (501) staff       (20)     5507 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/core/maze.py
--rw-r--r--   0 smorad     (501) staff       (20)      590 2023-01-26 13:50:44.000000 popgym-1.0.1/popgym/core/observability.py
--rw-r--r--   0 smorad     (501) staff       (20)      785 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/core/wrapper.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.126114 popgym-1.0.1/popgym/envs/
--rw-r--r--   0 smorad     (501) staff       (20)     9092 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/envs/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     3594 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/envs/autoencode.py
--rw-r--r--   0 smorad     (501) staff       (20)     5123 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/envs/battleship.py
--rw-r--r--   0 smorad     (501) staff       (20)     6837 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/envs/concentration.py
--rw-r--r--   0 smorad     (501) staff       (20)     5489 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/envs/count_recall.py
--rw-r--r--   0 smorad     (501) staff       (20)     3526 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/envs/higher_lower.py
--rw-r--r--   0 smorad     (501) staff       (20)     2072 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/envs/labyrinth_escape.py
--rw-r--r--   0 smorad     (501) staff       (20)     2419 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/envs/labyrinth_explore.py
--rw-r--r--   0 smorad     (501) staff       (20)     4742 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/envs/minesweeper.py
--rw-r--r--   0 smorad     (501) staff       (20)     2357 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/envs/multiarmed_bandit.py
--rw-r--r--   0 smorad     (501) staff       (20)     1625 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/envs/noisy_stateless_cartpole.py
--rw-r--r--   0 smorad     (501) staff       (20)     1597 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/envs/noisy_stateless_pendulum.py
--rw-r--r--   0 smorad     (501) staff       (20)     2465 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/envs/repeat_first.py
--rw-r--r--   0 smorad     (501) staff       (20)     3060 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/envs/repeat_previous.py
--rw-r--r--   0 smorad     (501) staff       (20)     2860 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/envs/stateless_cartpole.py
--rw-r--r--   0 smorad     (501) staff       (20)     2622 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/envs/stateless_pendulum.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.126331 popgym-1.0.1/popgym/util/
--rw-r--r--   0 smorad     (501) staff       (20)       33 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/util/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     6140 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/util/benchmark.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.126877 popgym-1.0.1/popgym/wrappers/
--rw-r--r--   0 smorad     (501) staff       (20)      313 2023-03-11 17:40:45.000000 popgym-1.0.1/popgym/wrappers/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     3459 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/wrappers/antialias.py
--rw-r--r--   0 smorad     (501) staff       (20)     3008 2023-03-09 21:24:36.000000 popgym-1.0.1/popgym/wrappers/flatten.py
--rw-r--r--   0 smorad     (501) staff       (20)     2109 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/wrappers/markovian.py
--rw-r--r--   0 smorad     (501) staff       (20)     5570 2023-03-08 15:29:35.000000 popgym-1.0.1/popgym/wrappers/previous_action.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.120518 popgym-1.0.1/popgym.egg-info/
--rw-r--r--   0 smorad     (501) staff       (20)     7567 2023-03-11 19:22:25.000000 popgym-1.0.1/popgym.egg-info/PKG-INFO
--rw-r--r--   0 smorad     (501) staff       (20)     2488 2023-03-11 19:22:25.000000 popgym-1.0.1/popgym.egg-info/SOURCES.txt
--rw-r--r--   0 smorad     (501) staff       (20)        1 2023-03-11 19:22:25.000000 popgym-1.0.1/popgym.egg-info/dependency_links.txt
--rw-r--r--   0 smorad     (501) staff       (20)       89 2023-03-11 19:22:25.000000 popgym-1.0.1/popgym.egg-info/requires.txt
--rw-r--r--   0 smorad     (501) staff       (20)       13 2023-03-11 19:22:25.000000 popgym-1.0.1/popgym.egg-info/top_level.txt
--rw-r--r--   0 smorad     (501) staff       (20)       80 2023-01-26 13:50:44.000000 popgym-1.0.1/pyproject.toml
--rw-r--r--   0 smorad     (501) staff       (20)      638 2023-03-11 19:22:25.130518 popgym-1.0.1/setup.cfg
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-03-11 19:22:25.130011 popgym-1.0.1/tests/
--rw-r--r--   0 smorad     (501) staff       (20)        0 2022-09-22 16:05:05.000000 popgym-1.0.1/tests/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     3391 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/base_env_test.py
--rw-r--r--   0 smorad     (501) staff       (20)      907 2022-09-22 16:05:05.000000 popgym-1.0.1/tests/compute_framerate.py
--rw-r--r--   0 smorad     (501) staff       (20)      351 2022-09-22 16:05:05.000000 popgym-1.0.1/tests/notest_bipedal_walker.py
--rw-r--r--   0 smorad     (501) staff       (20)     1013 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/test_autoencode.py
--rw-r--r--   0 smorad     (501) staff       (20)      217 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/test_bandits.py
--rw-r--r--   0 smorad     (501) staff       (20)     3216 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/test_battleship.py
--rw-r--r--   0 smorad     (501) staff       (20)     4160 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/test_concentration.py
--rw-r--r--   0 smorad     (501) staff       (20)     1602 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/test_count_recall.py
--rw-r--r--   0 smorad     (501) staff       (20)     2091 2022-09-22 16:05:05.000000 popgym-1.0.1/tests/test_deck.py
--rw-r--r--   0 smorad     (501) staff       (20)      267 2023-03-11 17:40:45.000000 popgym-1.0.1/tests/test_envs.py
--rw-r--r--   0 smorad     (501) staff       (20)      909 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/test_higher_lower.py
--rw-r--r--   0 smorad     (501) staff       (20)     1435 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/test_labyrinth_escape.py
--rw-r--r--   0 smorad     (501) staff       (20)     1822 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/test_labyrinth_explore.py
--rw-r--r--   0 smorad     (501) staff       (20)     1570 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/test_minesweeper.py
--rw-r--r--   0 smorad     (501) staff       (20)      972 2023-03-08 15:29:35.000000 popgym-1.0.1/tests/test_multiarmed_bandit.py
--rw-r--r--   0 smorad     (501) staff       (20)        0 2022-09-22 16:05:05.000000 popgym-1.0.1/tests/test_nonstationary_bandit.py
--rw-r--r--   0 smorad     (501) staff       (20)      674 2023-03-11 17:40:45.000000 popgym-1.0.1/tests/test_repeat_first.py
--rw-r--r--   0 smorad     (501) staff       (20)     1936 2023-03-11 17:40:45.000000 popgym-1.0.1/tests/test_repeat_previous.py
--rw-r--r--   0 smorad     (501) staff       (20)     3660 2023-03-11 17:40:45.000000 popgym-1.0.1/tests/test_wrappers.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.196375 popgym-1.0.2/
+-rw-r--r--   0 smorad     (501) staff       (20)     1069 2023-01-26 13:50:44.000000 popgym-1.0.2/LICENSE.md
+-rw-r--r--   0 smorad     (501) staff       (20)     7729 2023-04-09 17:17:30.196493 popgym-1.0.2/PKG-INFO
+-rw-r--r--   0 smorad     (501) staff       (20)     7375 2023-04-09 16:55:40.000000 popgym-1.0.2/README.md
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.180017 popgym-1.0.2/popgym/
+-rw-r--r--   0 smorad     (501) staff       (20)       73 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/__init__.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.181192 popgym-1.0.2/popgym/baselines/
+-rw-r--r--   0 smorad     (501) staff       (20)       85 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/__init__.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.182964 popgym-1.0.2/popgym/baselines/models/
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2023-03-08 13:39:50.000000 popgym-1.0.2/popgym/baselines/models/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)      992 2022-09-22 16:05:05.000000 popgym-1.0.2/popgym/baselines/models/aggregations.py
+-rw-r--r--   0 smorad     (501) staff       (20)     9855 2022-09-22 16:05:05.000000 popgym-1.0.2/popgym/baselines/models/embeddings.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1834 2023-01-26 13:50:44.000000 popgym-1.0.2/popgym/baselines/models/fwp.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2046 2022-09-22 16:05:05.000000 popgym-1.0.2/popgym/baselines/models/indrnn.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2450 2022-09-22 16:05:05.000000 popgym-1.0.2/popgym/baselines/models/linear_attention.py
+-rw-r--r--   0 smorad     (501) staff       (20)    10069 2022-09-27 16:44:40.000000 popgym-1.0.2/popgym/baselines/models/lmu.py
+-rw-r--r--   0 smorad     (501) staff       (20)    60700 2022-10-08 11:28:47.000000 popgym-1.0.2/popgym/baselines/models/s4d.py
+-rw-r--r--   0 smorad     (501) staff       (20)     7318 2023-01-26 13:50:44.000000 popgym-1.0.2/popgym/baselines/ppo.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.186283 popgym-1.0.2/popgym/baselines/ray_models/
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2023-03-08 13:39:50.000000 popgym-1.0.2/popgym/baselines/ray_models/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)    12303 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/base_model.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5407 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_diffnc.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2367 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_elman.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2343 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_frameconv.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3689 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_framestack.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3543 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_fwp.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2493 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_gru.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2359 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_indrnn.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3772 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_linear_attention.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2269 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_lmu.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2617 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_lstm.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1441 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_mlp.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2704 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_s4d.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.187461 popgym-1.0.2/popgym/core/
+-rw-r--r--   0 smorad     (501) staff       (20)       56 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/core/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     9714 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/core/deck.py
+-rw-r--r--   0 smorad     (501) staff       (20)      863 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/core/env.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5507 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/core/maze.py
+-rw-r--r--   0 smorad     (501) staff       (20)      590 2023-01-26 13:50:44.000000 popgym-1.0.2/popgym/core/observability.py
+-rw-r--r--   0 smorad     (501) staff       (20)      785 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/core/wrapper.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.190517 popgym-1.0.2/popgym/envs/
+-rw-r--r--   0 smorad     (501) staff       (20)     9576 2023-04-09 16:59:46.000000 popgym-1.0.2/popgym/envs/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3594 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/autoencode.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5123 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/battleship.py
+-rw-r--r--   0 smorad     (501) staff       (20)     6837 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/concentration.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5489 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/count_recall.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3526 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/higher_lower.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2072 2023-04-09 16:52:16.000000 popgym-1.0.2/popgym/envs/labyrinth_escape.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2419 2023-04-09 16:52:13.000000 popgym-1.0.2/popgym/envs/labyrinth_explore.py
+-rw-r--r--   0 smorad     (501) staff       (20)     4742 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/envs/minesweeper.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2357 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/envs/multiarmed_bandit.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1625 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/envs/noisy_stateless_cartpole.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1597 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/envs/noisy_stateless_pendulum.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2465 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/repeat_first.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3060 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/repeat_previous.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2860 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/stateless_cartpole.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2622 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/stateless_pendulum.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.190824 popgym-1.0.2/popgym/util/
+-rw-r--r--   0 smorad     (501) staff       (20)       33 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/util/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     6140 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/util/benchmark.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.192227 popgym-1.0.2/popgym/wrappers/
+-rw-r--r--   0 smorad     (501) staff       (20)      313 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/wrappers/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3459 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/wrappers/antialias.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3008 2023-03-09 21:24:36.000000 popgym-1.0.2/popgym/wrappers/flatten.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2109 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/wrappers/markovian.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5570 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/wrappers/previous_action.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.180790 popgym-1.0.2/popgym.egg-info/
+-rw-r--r--   0 smorad     (501) staff       (20)     7729 2023-04-09 17:17:30.000000 popgym-1.0.2/popgym.egg-info/PKG-INFO
+-rw-r--r--   0 smorad     (501) staff       (20)     2488 2023-04-09 17:17:30.000000 popgym-1.0.2/popgym.egg-info/SOURCES.txt
+-rw-r--r--   0 smorad     (501) staff       (20)        1 2023-04-09 17:17:30.000000 popgym-1.0.2/popgym.egg-info/dependency_links.txt
+-rw-r--r--   0 smorad     (501) staff       (20)      103 2023-04-09 17:17:30.000000 popgym-1.0.2/popgym.egg-info/requires.txt
+-rw-r--r--   0 smorad     (501) staff       (20)       13 2023-04-09 17:17:30.000000 popgym-1.0.2/popgym.egg-info/top_level.txt
+-rw-r--r--   0 smorad     (501) staff       (20)       80 2023-01-26 13:50:44.000000 popgym-1.0.2/pyproject.toml
+-rw-r--r--   0 smorad     (501) staff       (20)      652 2023-04-09 17:17:30.196885 popgym-1.0.2/setup.cfg
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.196203 popgym-1.0.2/tests/
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2022-09-22 16:05:05.000000 popgym-1.0.2/tests/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3391 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/base_env_test.py
+-rw-r--r--   0 smorad     (501) staff       (20)      907 2022-09-22 16:05:05.000000 popgym-1.0.2/tests/compute_framerate.py
+-rw-r--r--   0 smorad     (501) staff       (20)      351 2022-09-22 16:05:05.000000 popgym-1.0.2/tests/notest_bipedal_walker.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1013 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_autoencode.py
+-rw-r--r--   0 smorad     (501) staff       (20)      217 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_bandits.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3216 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_battleship.py
+-rw-r--r--   0 smorad     (501) staff       (20)     4160 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_concentration.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1602 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_count_recall.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2091 2022-09-22 16:05:05.000000 popgym-1.0.2/tests/test_deck.py
+-rw-r--r--   0 smorad     (501) staff       (20)      267 2023-03-11 17:40:45.000000 popgym-1.0.2/tests/test_envs.py
+-rw-r--r--   0 smorad     (501) staff       (20)      909 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_higher_lower.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1637 2023-04-09 16:58:11.000000 popgym-1.0.2/tests/test_labyrinth_escape.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2068 2023-04-09 16:58:11.000000 popgym-1.0.2/tests/test_labyrinth_explore.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1570 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_minesweeper.py
+-rw-r--r--   0 smorad     (501) staff       (20)      972 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_multiarmed_bandit.py
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2022-09-22 16:05:05.000000 popgym-1.0.2/tests/test_nonstationary_bandit.py
+-rw-r--r--   0 smorad     (501) staff       (20)      674 2023-03-11 17:40:45.000000 popgym-1.0.2/tests/test_repeat_first.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1936 2023-03-11 17:40:45.000000 popgym-1.0.2/tests/test_repeat_previous.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3660 2023-03-11 17:40:45.000000 popgym-1.0.2/tests/test_wrappers.py
```

### Comparing `popgym-1.0.1/LICENSE.md` & `popgym-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/PKG-INFO` & `popgym-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: popgym
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of partially-observable procedural gym environments
 Author: Steven Morad
 License: MIT
 Keywords: gym,gymnasium,pomdp,partially observable,reinforcement learning,rl
 Description-Content-Type: text/markdown
+Provides-Extra: navigation
 Provides-Extra: baselines
 License-File: LICENSE.md
 
 # POPGym: Partially Observable Process Gym
 ![tests](https://github.com/smorad/popgym/actions/workflows/python-app.yml/badge.svg)
 [![codecov](https://codecov.io/gh/smorad/popgym/branch/master/graph/badge.svg?token=I47IDFZXSV)](https://codecov.io/gh/smorad/popgym)
 
 POPGym is designed to benchmark memory in deep reinforcement learning. It contains a set of [environments](#popgym-environments) and a collection of [memory model baselines](#popgym-baselines). The full paper is available on [OpenReview](https://openreview.net/forum?id=chDrutUTs0K). Please see the [documentation](https://popgym.readthedocs.io/en/latest/) for advanced installation instructions and examples. 
 
 ## Quickstart Install
 
 ```python
-pip install popgym # environments only
+pip install popgym # base environments only, only requires numpy and gymnasium
+pip install "popgym[navigation]" # also include navigation environments, which require mazelib
 pip install "popgym[baselines]" # environments and memory baselines
 ```
 
 ## POPGym Environments
 
 POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Openai Gym](https://github.com/openai/gym) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
```

### Comparing `popgym-1.0.1/README.md` & `popgym-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 [![codecov](https://codecov.io/gh/smorad/popgym/branch/master/graph/badge.svg?token=I47IDFZXSV)](https://codecov.io/gh/smorad/popgym)
 
 POPGym is designed to benchmark memory in deep reinforcement learning. It contains a set of [environments](#popgym-environments) and a collection of [memory model baselines](#popgym-baselines). The full paper is available on [OpenReview](https://openreview.net/forum?id=chDrutUTs0K). Please see the [documentation](https://popgym.readthedocs.io/en/latest/) for advanced installation instructions and examples. 
 
 ## Quickstart Install
 
 ```python
-pip install popgym # environments only
+pip install popgym # base environments only, only requires numpy and gymnasium
+pip install "popgym[navigation]" # also include navigation environments, which require mazelib
 pip install "popgym[baselines]" # environments and memory baselines
 ```
 
 ## POPGym Environments
 
 POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Openai Gym](https://github.com/openai/gym) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
```

### Comparing `popgym-1.0.1/popgym/baselines/models/aggregations.py` & `popgym-1.0.2/popgym/baselines/models/aggregations.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/models/embeddings.py` & `popgym-1.0.2/popgym/baselines/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/models/fwp.py` & `popgym-1.0.2/popgym/baselines/models/fwp.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/models/indrnn.py` & `popgym-1.0.2/popgym/baselines/models/indrnn.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/models/linear_attention.py` & `popgym-1.0.2/popgym/baselines/models/linear_attention.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/models/lmu.py` & `popgym-1.0.2/popgym/baselines/models/lmu.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/models/s4d.py` & `popgym-1.0.2/popgym/baselines/models/s4d.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ppo.py` & `popgym-1.0.2/popgym/baselines/ppo.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/base_model.py` & `popgym-1.0.2/popgym/baselines/ray_models/base_model.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_diffnc.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_diffnc.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_elman.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_elman.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_frameconv.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_frameconv.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_framestack.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_framestack.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_fwp.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_fwp.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_gru.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_gru.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_indrnn.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_indrnn.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_linear_attention.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_linear_attention.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_lmu.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_lmu.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_lstm.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_lstm.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_mlp.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_mlp.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/baselines/ray_models/ray_s4d.py` & `popgym-1.0.2/popgym/baselines/ray_models/ray_s4d.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/core/deck.py` & `popgym-1.0.2/popgym/core/deck.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/core/env.py` & `popgym-1.0.2/popgym/core/env.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/core/maze.py` & `popgym-1.0.2/popgym/core/maze.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/core/observability.py` & `popgym-1.0.2/popgym/core/observability.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/core/wrapper.py` & `popgym-1.0.2/popgym/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/__init__.py` & `popgym-1.0.2/popgym/envs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Collection of POPGym environments
 """
 
 import inspect
+from importlib import find_loader
 from typing import Any, Dict
 
 import gymnasium as gym
 
 from popgym.envs.autoencode import (
     Autoencode,
     AutoencodeEasy,
@@ -32,26 +33,14 @@
 )
 from popgym.envs.higher_lower import (
     HigherLower,
     HigherLowerEasy,
     HigherLowerHard,
     HigherLowerMedium,
 )
-from popgym.envs.labyrinth_escape import (
-    LabyrinthEscape,
-    LabyrinthEscapeEasy,
-    LabyrinthEscapeHard,
-    LabyrinthEscapeMedium,
-)
-from popgym.envs.labyrinth_explore import (
-    LabyrinthExplore,
-    LabyrinthExploreEasy,
-    LabyrinthExploreHard,
-    LabyrinthExploreMedium,
-)
 from popgym.envs.minesweeper import (
     MineSweeper,
     MineSweeperEasy,
     MineSweeperHard,
     MineSweeperMedium,
 )
 from popgym.envs.multiarmed_bandit import (
@@ -240,33 +229,59 @@
 }
 
 ALL_GAME = {**GAME_EASY, **GAME_MEDIUM, **GAME_HARD}
 
 #
 # Navigation envs
 #
-NAVIGATION: Dict[gym.Env, Dict[str, Any]] = {
-    LabyrinthExplore: {"id": "popgym-LabyrinthExplore-v0"},
-    LabyrinthEscape: {"id": "popgym-LabyrinthEscape-v0"},
-}
-
-NAVIGATION_EASY: Dict[gym.Env, Dict[str, Any]] = {
-    LabyrinthExploreEasy: {"id": "popgym-LabyrinthExploreEasy-v0"},
-    LabyrinthEscapeEasy: {"id": "popgym-LabyrinthEscapeEasy-v0"},
-}
-
-NAVIGATION_MEDIUM: Dict[gym.Env, Dict[str, Any]] = {
-    LabyrinthExploreMedium: {"id": "popgym-LabyrinthExploreMedium-v0"},
-    LabyrinthEscapeMedium: {"id": "popgym-LabyrinthEscapeMedium-v0"},
-}
-
-NAVIGATION_HARD: Dict[gym.Env, Dict[str, Any]] = {
-    LabyrinthExploreHard: {"id": "popgym-LabyrinthExploreHard-v0"},
-    LabyrinthEscapeHard: {"id": "popgym-LabyrinthEscapeHard-v0"},
-}
+def has_mazelib():  # noqa: E302
+    """Check if mazelib is installed"""
+    return find_loader("mazelib") is not None
+
+
+if has_mazelib():
+    # mazelib can somtimes be a headache to install
+    # mazes are also a poor test of memory
+    from popgym.envs.labyrinth_escape import (
+        LabyrinthEscape,
+        LabyrinthEscapeEasy,
+        LabyrinthEscapeHard,
+        LabyrinthEscapeMedium,
+    )
+    from popgym.envs.labyrinth_explore import (
+        LabyrinthExplore,
+        LabyrinthExploreEasy,
+        LabyrinthExploreHard,
+        LabyrinthExploreMedium,
+    )
+
+    NAVIGATION: Dict[gym.Env, Dict[str, Any]] = {
+        LabyrinthExplore: {"id": "popgym-LabyrinthExplore-v0"},
+        LabyrinthEscape: {"id": "popgym-LabyrinthEscape-v0"},
+    }
+
+    NAVIGATION_EASY: Dict[gym.Env, Dict[str, Any]] = {
+        LabyrinthExploreEasy: {"id": "popgym-LabyrinthExploreEasy-v0"},
+        LabyrinthEscapeEasy: {"id": "popgym-LabyrinthEscapeEasy-v0"},
+    }
+
+    NAVIGATION_MEDIUM: Dict[gym.Env, Dict[str, Any]] = {
+        LabyrinthExploreMedium: {"id": "popgym-LabyrinthExploreMedium-v0"},
+        LabyrinthEscapeMedium: {"id": "popgym-LabyrinthEscapeMedium-v0"},
+    }
+
+    NAVIGATION_HARD: Dict[gym.Env, Dict[str, Any]] = {
+        LabyrinthExploreHard: {"id": "popgym-LabyrinthExploreHard-v0"},
+        LabyrinthEscapeHard: {"id": "popgym-LabyrinthEscapeHard-v0"},
+    }
+else:
+    NAVIGATION = {}
+    NAVIGATION_EASY = {}
+    NAVIGATION_MEDIUM = {}
+    NAVIGATION_HARD = {}
 
 ALL_NAVIGATION = {
     **NAVIGATION_EASY,
     **NAVIGATION_MEDIUM,
     **NAVIGATION_HARD,
 }
```

### Comparing `popgym-1.0.1/popgym/envs/autoencode.py` & `popgym-1.0.2/popgym/envs/autoencode.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/battleship.py` & `popgym-1.0.2/popgym/envs/battleship.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/concentration.py` & `popgym-1.0.2/popgym/envs/concentration.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/count_recall.py` & `popgym-1.0.2/popgym/envs/count_recall.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/higher_lower.py` & `popgym-1.0.2/popgym/envs/higher_lower.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/labyrinth_escape.py` & `popgym-1.0.2/popgym/envs/labyrinth_escape.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/labyrinth_explore.py` & `popgym-1.0.2/popgym/envs/labyrinth_explore.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/minesweeper.py` & `popgym-1.0.2/popgym/envs/minesweeper.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/multiarmed_bandit.py` & `popgym-1.0.2/popgym/envs/multiarmed_bandit.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/noisy_stateless_cartpole.py` & `popgym-1.0.2/popgym/envs/noisy_stateless_cartpole.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/noisy_stateless_pendulum.py` & `popgym-1.0.2/popgym/envs/noisy_stateless_pendulum.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/repeat_first.py` & `popgym-1.0.2/popgym/envs/repeat_first.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/repeat_previous.py` & `popgym-1.0.2/popgym/envs/repeat_previous.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/stateless_cartpole.py` & `popgym-1.0.2/popgym/envs/stateless_cartpole.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/envs/stateless_pendulum.py` & `popgym-1.0.2/popgym/envs/stateless_pendulum.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/util/benchmark.py` & `popgym-1.0.2/popgym/util/benchmark.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/wrappers/antialias.py` & `popgym-1.0.2/popgym/wrappers/antialias.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/wrappers/flatten.py` & `popgym-1.0.2/popgym/wrappers/flatten.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/wrappers/markovian.py` & `popgym-1.0.2/popgym/wrappers/markovian.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym/wrappers/previous_action.py` & `popgym-1.0.2/popgym/wrappers/previous_action.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/popgym.egg-info/PKG-INFO` & `popgym-1.0.2/popgym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: popgym
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of partially-observable procedural gym environments
 Author: Steven Morad
 License: MIT
 Keywords: gym,gymnasium,pomdp,partially observable,reinforcement learning,rl
 Description-Content-Type: text/markdown
+Provides-Extra: navigation
 Provides-Extra: baselines
 License-File: LICENSE.md
 
 # POPGym: Partially Observable Process Gym
 ![tests](https://github.com/smorad/popgym/actions/workflows/python-app.yml/badge.svg)
 [![codecov](https://codecov.io/gh/smorad/popgym/branch/master/graph/badge.svg?token=I47IDFZXSV)](https://codecov.io/gh/smorad/popgym)
 
 POPGym is designed to benchmark memory in deep reinforcement learning. It contains a set of [environments](#popgym-environments) and a collection of [memory model baselines](#popgym-baselines). The full paper is available on [OpenReview](https://openreview.net/forum?id=chDrutUTs0K). Please see the [documentation](https://popgym.readthedocs.io/en/latest/) for advanced installation instructions and examples. 
 
 ## Quickstart Install
 
 ```python
-pip install popgym # environments only
+pip install popgym # base environments only, only requires numpy and gymnasium
+pip install "popgym[navigation]" # also include navigation environments, which require mazelib
 pip install "popgym[baselines]" # environments and memory baselines
 ```
 
 ## POPGym Environments
 
 POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Openai Gym](https://github.com/openai/gym) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
```

### Comparing `popgym-1.0.1/popgym.egg-info/SOURCES.txt` & `popgym-1.0.2/popgym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/setup.cfg` & `popgym-1.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [metadata]
 name = popgym
 description = A collection of partially-observable procedural gym environments
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Steven Morad
-version = 1.0.1
+version = 1.0.2
 license = MIT
 readme = README.md
 requires-python = >=3.7 <=3.10 # Remove 3.10 limit when mazelib fixes its build process
 keywords = gym, gymnasium, pomdp, partially observable, reinforcement learning, rl
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	gymnasium
-	mazelib
 
 [options.extras_require]
+navigation = 
+	mazelib
 baselines = 
 	torch
 	opt_einsum
 	wandb
 	dnc
 	einops
 	ray[rllib]==2.3.0
```

### Comparing `popgym-1.0.1/tests/base_env_test.py` & `popgym-1.0.2/tests/base_env_test.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/compute_framerate.py` & `popgym-1.0.2/tests/compute_framerate.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_autoencode.py` & `popgym-1.0.2/tests/test_autoencode.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_battleship.py` & `popgym-1.0.2/tests/test_battleship.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_concentration.py` & `popgym-1.0.2/tests/test_concentration.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_count_recall.py` & `popgym-1.0.2/tests/test_count_recall.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_deck.py` & `popgym-1.0.2/tests/test_deck.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_higher_lower.py` & `popgym-1.0.2/tests/test_higher_lower.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_labyrinth_escape.py` & `popgym-1.0.2/tests/test_labyrinth_escape.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 import unittest
 
-from popgym.envs.labyrinth_escape import LabyrinthEscape
+from popgym.envs import has_mazelib
 
+if has_mazelib():
+    from popgym.envs.labyrinth_escape import LabyrinthEscape
 
-class TestLabyrinthEscape(unittest.TestCase):
-    def test_step(self):
-        e = LabyrinthEscape()
-        e.reset()
-        for i in range(1000):
-            _, _, terminated, truncated, _ = e.step(e.action_space.sample())
-            if terminated or truncated:
-                e.reset()
-
-    def test_tostring(self):
-        e = LabyrinthEscape((6, 6))
-        e.reset()
-        e.tostring()
-
-    def test_goal(self):
-        e = LabyrinthEscape((6, 6))
-        terminated = truncated = False
-        e.reset()
-        for i in range(5):
-            while not (terminated or truncated):
+    class TestLabyrinthEscape(unittest.TestCase):
+        def test_step(self):
+            e = LabyrinthEscape()
+            e.reset()
+            for i in range(1000):
                 _, _, terminated, truncated, _ = e.step(e.action_space.sample())
-            self.assertTrue(e.curr_step < e.max_episode_length)
+                if terminated or truncated:
+                    e.reset()
+
+        def test_tostring(self):
+            e = LabyrinthEscape((6, 6))
             e.reset()
+            e.tostring()
+
+        def test_goal(self):
+            e = LabyrinthEscape((6, 6))
+            terminated = truncated = False
+            e.reset()
+            for i in range(5):
+                while not (terminated or truncated):
+                    _, _, terminated, truncated, _ = e.step(e.action_space.sample())
+                self.assertTrue(e.curr_step < e.max_episode_length)
+                e.reset()
 
-    def test_known(self):
-        e = LabyrinthEscape((8, 8))
-        e.reset(seed=1)
-        left, right, _, down = 0, 1, 2, 3
-        actions = [down] * 5 + [left] * 2 + [down] * 2 + [right] * 6 + [down] * 1
-        done = False
-        cum_rew = 0
-        for action in actions:
-            self.assertFalse(done)
-            obs, reward, terminated, truncated, info = e.step(action)
-            cum_rew += reward
-
-        self.assertTrue(terminated)
-        self.assertFalse(truncated)
-        expected = 1.0 + len(actions) * e.neg_reward_scale
-        self.assertAlmostEqual(cum_rew, expected)
+        def test_known(self):
+            e = LabyrinthEscape((8, 8))
+            e.reset(seed=1)
+            left, right, _, down = 0, 1, 2, 3
+            actions = [down] * 5 + [left] * 2 + [down] * 2 + [right] * 6 + [down] * 1
+            done = False
+            cum_rew = 0
+            for action in actions:
+                self.assertFalse(done)
+                obs, reward, terminated, truncated, info = e.step(action)
+                cum_rew += reward
+
+            self.assertTrue(terminated)
+            self.assertFalse(truncated)
+            expected = 1.0 + len(actions) * e.neg_reward_scale
+            self.assertAlmostEqual(cum_rew, expected)
```

### Comparing `popgym-1.0.1/tests/test_labyrinth_explore.py` & `popgym-1.0.2/tests/test_labyrinth_explore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 import unittest
 
 import numpy as np
 
-from popgym.envs.labyrinth_explore import LabyrinthExplore
+from popgym.envs import has_mazelib
 
+if has_mazelib():
+    from popgym.envs.labyrinth_explore import LabyrinthExplore
 
-class TestLabyrinthExplore(unittest.TestCase):
-    def test_step(self):
-        e = LabyrinthExplore()
-        obs, _ = e.reset()
-        self.assertEqual(obs.dtype, np.int32)
-        terminated = truncated = False
-        for i in range(1000):
-            obs, _, terminated, truncated, _ = e.step(e.action_space.sample())
+    class TestLabyrinthExplore(unittest.TestCase):
+        def test_step(self):
+            e = LabyrinthExplore()
+            obs, _ = e.reset()
             self.assertEqual(obs.dtype, np.int32)
-            if terminated or truncated:
-                obs = e.reset()
+            terminated = truncated = False
+            for i in range(1000):
+                obs, _, terminated, truncated, _ = e.step(e.action_space.sample())
                 self.assertEqual(obs.dtype, np.int32)
-
-    def test_noclip(self):
-        e = LabyrinthExplore()
-        terminated = truncated = False
-        e.reset()
-        for i in range(5):
-            while not (terminated or truncated):
-                _, _, terminated, truncated, _ = e.step(e.action_space.sample())
-
-            visit_mask = e.explored == 1
-            obstacle_mask = e.maze.grid == 1
-            self.assertFalse(np.any(visit_mask * obstacle_mask == 1))
+                if terminated or truncated:
+                    obs = e.reset()
+                    self.assertEqual(obs.dtype, np.int32)
+
+        def test_noclip(self):
+            e = LabyrinthExplore()
+            terminated = truncated = False
             e.reset()
-
-    def test_known(self):
-        e = LabyrinthExplore((6, 6))
-        e.reset(seed=0)
-        left, right, up, down = 0, 1, 2, 3
-        actions = (
-            [left] * 5
-            + [up] * 2
-            + [right] * 2
-            + [left] * 2
-            + [down] * 2
-            + [right] * 4
-            + [up] * 4
-            + [left] * 4
-        )
-        terminated = truncated = False
-        cum_rew = 0
-        for action in actions:
-            self.assertFalse(terminated or truncated)
-            obs, reward, terminated, truncated, info = e.step(action)
-            cum_rew += reward
-
-        self.assertTrue(terminated)
-        self.assertFalse(truncated)
-        expected = 1.0 + 8 * e.neg_reward_scale
-        self.assertAlmostEqual(cum_rew, expected)
+            for i in range(5):
+                while not (terminated or truncated):
+                    _, _, terminated, truncated, _ = e.step(e.action_space.sample())
+
+                visit_mask = e.explored == 1
+                obstacle_mask = e.maze.grid == 1
+                self.assertFalse(np.any(visit_mask * obstacle_mask == 1))
+                e.reset()
+
+        def test_known(self):
+            e = LabyrinthExplore((6, 6))
+            e.reset(seed=0)
+            left, right, up, down = 0, 1, 2, 3
+            actions = (
+                [left] * 5
+                + [up] * 2
+                + [right] * 2
+                + [left] * 2
+                + [down] * 2
+                + [right] * 4
+                + [up] * 4
+                + [left] * 4
+            )
+            terminated = truncated = False
+            cum_rew = 0
+            for action in actions:
+                self.assertFalse(terminated or truncated)
+                obs, reward, terminated, truncated, info = e.step(action)
+                cum_rew += reward
+
+            self.assertTrue(terminated)
+            self.assertFalse(truncated)
+            expected = 1.0 + 8 * e.neg_reward_scale
+            self.assertAlmostEqual(cum_rew, expected)
```

### Comparing `popgym-1.0.1/tests/test_minesweeper.py` & `popgym-1.0.2/tests/test_minesweeper.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_multiarmed_bandit.py` & `popgym-1.0.2/tests/test_multiarmed_bandit.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_repeat_first.py` & `popgym-1.0.2/tests/test_repeat_first.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_repeat_previous.py` & `popgym-1.0.2/tests/test_repeat_previous.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.1/tests/test_wrappers.py` & `popgym-1.0.2/tests/test_wrappers.py`

 * *Files identical despite different names*

