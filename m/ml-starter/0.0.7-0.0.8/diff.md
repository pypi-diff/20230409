# Comparing `tmp/ml-starter-0.0.7.tar.gz` & `tmp/ml-starter-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.7.tar", last modified: Fri Apr  7 22:47:01 2023, max compression
+gzip compressed data, was "ml-starter-0.0.8.tar", last modified: Sun Apr  9 00:07:51 2023, max compression
```

## Comparing `ml-starter-0.0.7.tar` & `ml-starter-0.0.8.tar`

### file list

```diff
@@ -1,145 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.902388 ml-starter-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-07 22:46:49.000000 ml-starter-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-07 22:47:01.902388 ml-starter-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-07 22:46:49.000000 ml-starter-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.870387 ml-starter-0.0.7/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/__version__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.874387 ml-starter-0.0.7/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    23716 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.874387 ml-starter-0.0.7/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.874387 ml-starter-0.0.7/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.878388 ml-starter-0.0.7/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.878388 ml-starter-0.0.7/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.882387 ml-starter-0.0.7/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.882387 ml-starter-0.0.7/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.882387 ml-starter-0.0.7/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17502 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.886387 ml-starter-0.0.7/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.886387 ml-starter-0.0.7/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.886387 ml-starter-0.0.7/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.890388 ml-starter-0.0.7/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.890388 ml-starter-0.0.7/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.894388 ml-starter-0.0.7/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.894388 ml-starter-0.0.7/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/cpu_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.898388 ml-starter-0.0.7/ml/trainers/mixins/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.902388 ml-starter-0.0.7/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.902388 ml-starter-0.0.7/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-07 22:46:49.000000 ml-starter-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 22:46:49.000000 ml-starter-0.0.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 22:46:49.000000 ml-starter-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-07 22:47:01.906388 ml-starter-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-07 22:46:49.000000 ml-starter-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.707039 ml-starter-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 00:07:35.000000 ml-starter-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-09 00:07:51.707039 ml-starter-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-09 00:07:35.000000 ml-starter-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.683039 ml-starter-0.0.8/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/__version__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.683039 ml-starter-0.0.8/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.683039 ml-starter-0.0.8/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.687039 ml-starter-0.0.8/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.687039 ml-starter-0.0.8/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.687039 ml-starter-0.0.8/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.691039 ml-starter-0.0.8/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.691039 ml-starter-0.0.8/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/mp_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.691039 ml-starter-0.0.8/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17584 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.695039 ml-starter-0.0.8/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.695039 ml-starter-0.0.8/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.695039 ml-starter-0.0.8/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.695039 ml-starter-0.0.8/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.695039 ml-starter-0.0.8/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.699039 ml-starter-0.0.8/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/ddp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.699039 ml-starter-0.0.8/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/cpu_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.699039 ml-starter-0.0.8/ml/trainers/mixins/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.703039 ml-starter-0.0.8/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.707039 ml-starter-0.0.8/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-09 00:07:35.000000 ml-starter-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-09 00:07:35.000000 ml-starter-0.0.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-09 00:07:35.000000 ml-starter-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 00:07:51.707039 ml-starter-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 00:07:35.000000 ml-starter-0.0.8/setup.py
```

### Comparing `ml-starter-0.0.7/PKG-INFO` & `ml-starter-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.7
+Version: 0.0.8
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.7/README.md` & `ml-starter-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/api.py` & `ml-starter-0.0.8/ml/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "cast_init_type",
     "cast_norm_type",
     "cast_reduce_type",
     "ChunkSampler",
     "ClippifyDataset",
     "collate_non_null",
     "collate",
+    "CollateMode",
     "colorize",
     "conf_field",
     "configure_logging",
     "Environment",
     "format_timedelta",
     "from_args",
     "get_activation",
@@ -72,24 +73,27 @@
     "load_model_and_task",
     "Loss",
     "meta_to_empty_func",
     "MultiIterDataset",
     "NormType",
     "open_atomic",
     "Output",
+    "pad_all",
+    "pad_sequence",
     "Phase",
     "reduce",
     "register_logger",
     "register_lr_scheduler",
     "register_model",
     "register_optimizer",
     "register_task",
     "register_trainer",
     "ReinforcementLearningTask",
     "ReinforcementLearningTaskConfig",
+    "stage_environment",
     "State",
     "StreamingDataset",
     "SupervisedLearningTask",
     "SupervisedLearningTaskConfig",
     "SyncEnvironmentWorker",
     "SyncWorkerPool",
     "test_dataset",
@@ -134,15 +138,15 @@
     get_norm_linear,
 )
 from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
 from ml.tasks.base import BaseTask, BaseTaskConfig
 from ml.tasks.datasets import transforms
 from ml.tasks.datasets.async_iterable import AsyncIterableDataset
 from ml.tasks.datasets.clippify import ClippifyDataset
-from ml.tasks.datasets.collate import collate, collate_non_null
+from ml.tasks.datasets.collate import CollateMode, collate, collate_non_null, pad_all, pad_sequence
 from ml.tasks.datasets.multi_iter import MultiIterDataset
 from ml.tasks.datasets.samplers import ChunkSampler
 from ml.tasks.datasets.streaming import StreamingDataset
 from ml.tasks.datasets.utils import test_dataset
 from ml.tasks.datasets.video_file import VideoFileDataset
 from ml.tasks.environments.base import Environment
 from ml.tasks.environments.worker import (
@@ -175,9 +179,10 @@
     get_world_size_optional,
     is_distributed,
     is_master,
 )
 from ml.utils.io import load_model_and_task
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
+from ml.utils.staging import stage_environment
 from ml.utils.timer import Timer, timeout
 from ml.utils.video import READERS as VIDEO_READERS, WRITERS as VIDEO_WRITERS
```

### Comparing `ml-starter-0.0.7/ml/core/config.py` & `ml-starter-0.0.8/ml/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
             config: The config to resolve
         """
 
 
 class BaseObject(Generic[BaseConfigT]):
     """Defines the base class for all objects."""
 
+    __constants__ = ["config"]
+
     def __init__(self, config: BaseConfigT) -> None:
         self.config: BaseConfigT = config
 
 
 class BaseObjectWithPointers(BaseObject[BaseConfigT], Generic[BaseConfigT]):
     """Defines the base class for all objects with pointers to other objects."""
```

### Comparing `ml-starter-0.0.7/ml/core/env.py` & `ml-starter-0.0.8/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/core/registry.py` & `ml-starter-0.0.8/ml/core/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-import datetime
 import functools
-import hashlib
 import importlib.util
 import inspect
 import json
 import logging
-import os
-import shutil
 import sys
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Generic, Iterator, TypeVar, cast
-from uuid import uuid4
 
 from omegaconf import DictConfig, ListConfig, OmegaConf
 from omegaconf.basecontainer import BaseContainer
 
 from ml.core.config import BaseConfig, BaseObject, BaseObjectWithPointers
-from ml.core.env import get_project_root, get_stage_dir
+from ml.core.env import get_project_root
 from ml.utils.colors import colorize
-from ml.utils.paths import get_relative_path, is_relative_to
+from ml.utils.paths import get_relative_path
 from ml.utils.timer import Timer
 
 if TYPE_CHECKING:
     from ml.loggers.base import BaseLogger, BaseLoggerConfig
     from ml.lr_schedulers.base import BaseLRScheduler, BaseLRSchedulerConfig
     from ml.models.base import BaseModel, BaseModelConfig
     from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
@@ -40,31 +35,23 @@
 # Special key in the config, cooresponding to the reserved keyword in the
 # BaseConfig, which is used to reference the object to construct.
 NAME_KEY = "name"
 
 # This points to the root directory location for the package.
 ROOT_DIR: Path = Path(__file__).parent.parent.resolve()
 
-# Date format for staging environments.
-DATE_FORMAT = "%Y-%m-%d"
-
 # Maximum number of days to keep a staging directory around. This should
 # correspond to the maximum number of days that an experiment could run.
 MAX_STAGING_DAYS = 31
 
 
 @functools.lru_cache
-def project_root() -> Path | None:
-    return get_project_root()
-
-
-@functools.lru_cache
 def base_dirs() -> list[Path]:
     base_dirs = [ROOT_DIR]
-    project_root_dir = project_root()
+    project_root_dir = get_project_root()
     if project_root_dir is not None:
         base_dirs.append(project_root_dir)
     return base_dirs
 
 
 def get_name(key: str, config: BaseContainer) -> str:
     if not isinstance(config, DictConfig):
@@ -73,70 +60,14 @@
         raise ValueError(f"Malformed {key} config; missing expected key {NAME_KEY}")
     name = config[NAME_KEY]
     if not isinstance(name, str):
         raise ValueError(f"Expected {key} name to be a string, got {name}")
     return name
 
 
-def stage_environment() -> Path:
-    """Stages the current environment to a root directory.
-
-    Returns:
-        The stage environment path
-    """
-
-    stage_dir = get_stage_dir()
-
-    with Timer("getting files to stage"):
-        fpaths: list[Path] = []
-        for module in sys.modules.values():
-            if (fpath_str := getattr(module, "__file__", None)) is None:
-                continue
-            for base_dir in base_dirs():
-                fpath = Path(fpath_str).resolve()
-                if is_relative_to(fpath, base_dir):
-                    fpaths.append(fpath)
-                    break
-
-    assert fpaths, "Couldn't find any file paths to stage!"
-
-    with Timer("computing hash of current environment"):
-        hashobj = hashlib.md5()
-        for fpath in fpaths:
-            with open(fpath, "rb") as f:
-                while data := f.read(65536):
-                    hashobj.update(data)
-        hashval = hashobj.hexdigest()
-
-    date_str = datetime.datetime.now().strftime(DATE_FORMAT)
-    out_dir = stage_dir / f"{date_str}-{hashval[:10]}"
-    if not out_dir.exists():
-        with Timer("copying files to staging directory"):
-            tmp_dir = stage_dir / ".tmp" / str(uuid4())
-            if tmp_dir.parent.exists():
-                shutil.rmtree(tmp_dir.parent)
-            tmp_dir.mkdir(exist_ok=False, parents=True)
-            for fpath in fpaths:
-                new_fpath = tmp_dir / get_relative_path(fpath, base_dirs(), True)
-                new_fpath.parent.mkdir(exist_ok=True, parents=True)
-                shutil.copyfile(fpath, new_fpath)
-            tmp_dir.rename(out_dir)
-            tmp_dir.parent.rmdir()
-
-    with Timer("removing old directories"):
-        cur_time = datetime.datetime.now()
-        for dpath in stage_dir.iterdir():
-            dir_age = cur_time - datetime.datetime.fromtimestamp(os.stat(dpath).st_mtime)
-            if dir_age > datetime.timedelta(days=14):
-                logger.info("Removing old staging directory %s", dpath)
-                shutil.rmtree(dpath)
-
-    return out_dir
-
-
 class register_base(ABC, Generic[Entry, Config]):  # pylint: disable=invalid-name
     """Defines the base registry type.
 
     Usage:
 
     ```
     @register("my_thing", dataclass=MyThingConfig)
```

### Comparing `ml-starter-0.0.7/ml/core/state.py` & `ml-starter-0.0.8/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/loggers/base.py` & `ml-starter-0.0.8/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/loggers/meter.py` & `ml-starter-0.0.8/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/loggers/multi.py` & `ml-starter-0.0.8/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/loggers/stdout.py` & `ml-starter-0.0.8/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/loggers/tensorboard.py` & `ml-starter-0.0.8/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/lr_schedulers/base.py` & `ml-starter-0.0.8/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.8/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.8/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/lr_schedulers/linear.py` & `ml-starter-0.0.8/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.8/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.8/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/models/activations.py` & `ml-starter-0.0.8/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/models/base.py` & `ml-starter-0.0.8/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/models/init.py` & `ml-starter-0.0.8/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/models/norms.py` & `ml-starter-0.0.8/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/optimizers/adam.py` & `ml-starter-0.0.8/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/optimizers/adamw.py` & `ml-starter-0.0.8/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/optimizers/adan.py` & `ml-starter-0.0.8/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/optimizers/base.py` & `ml-starter-0.0.8/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/optimizers/sgd.py` & `ml-starter-0.0.8/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/optimizers/shampoo.py` & `ml-starter-0.0.8/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/scripts/cli.py` & `ml-starter-0.0.8/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/scripts/compiler.py` & `ml-starter-0.0.8/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/scripts/stage.py` & `ml-starter-0.0.8/ml/scripts/stage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import logging
 
 from omegaconf import DictConfig, OmegaConf
 
-from ml.core.registry import stage_environment
+from ml.core.env import get_project_root, get_stage_dir
+from ml.utils.staging import stage_environment
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def stage_main(config: DictConfig) -> None:
     """Stages the current configuration.
 
     Args:
         config: The configuration object.
+
+    Raises:
+        RuntimeError: If the project root is not set.
     """
 
     # Stages the currently-imported files.
-    out_dir = stage_environment()
+    project_root = get_project_root()
+    if project_root is None:
+        raise RuntimeError("Project root is not set.")
+    out_dir = stage_environment(project_root, get_stage_dir())
     logger.info("Staged environment to %s", out_dir)
 
     # Stages the raw config.
     config_dir = out_dir / "configs"
     config_dir.mkdir(exist_ok=True, parents=True)
     config_id = len(list(config_dir.glob("config_*.yaml")))
     config_path = config_dir / f"config_{config_id}.yaml"
```

### Comparing `ml-starter-0.0.7/ml/scripts/train.py` & `ml-starter-0.0.8/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/base.py` & `ml-starter-0.0.8/ml/tasks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,17 @@
 
         Returns:
             The single loss with shape (N), where N is the number of losses,
             and the loss names, a list of length N.
         """
 
         if isinstance(loss, Tensor):
-            if loss.ndim <= 1:
+            if loss.ndim == 0:
+                return loss.unsqueeze(0), ["loss"]
+            if loss.ndim == 1:
                 return loss, ["loss"]
             return reduce(loss, self.__final_loss_reduce_type).unsqueeze(0), ["loss"]
         assert isinstance(loss, dict), f"Loss should be a scalar or dictionary, not {type(loss)}"
         keys, values = (list(i) for i in zip(*sorted(loss.items())))
         losses = [reduce(v, self.__final_loss_reduce_type) for v in values]
         single_loss = torch.stack(losses, dim=0)
         return single_loss, keys
```

### Comparing `ml-starter-0.0.7/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.8/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.8/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/datasets/collate.py` & `ml-starter-0.0.8/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.8/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.8/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.8/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.8/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.8/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/datasets/utils.py` & `ml-starter-0.0.8/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.8/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/environments/base.py` & `ml-starter-0.0.8/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/environments/utils.py` & `ml-starter-0.0.8/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/environments/worker.py` & `ml-starter-0.0.8/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/losses/reduce.py` & `ml-starter-0.0.8/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/rl/base.py` & `ml-starter-0.0.8/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/rl/replay.py` & `ml-starter-0.0.8/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/tasks/sl/base.py` & `ml-starter-0.0.8/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/base.py` & `ml-starter-0.0.8/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/ddp.py` & `ml-starter-0.0.8/ml/trainers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.8/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/device/auto.py` & `ml-starter-0.0.8/ml/trainers/mixins/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/device/base.py` & `ml-starter-0.0.8/ml/trainers/mixins/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/device/cpu.py` & `ml-starter-0.0.8/ml/trainers/mixins/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/device/gpu.py` & `ml-starter-0.0.8/ml/trainers/mixins/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/device/metal.py` & `ml-starter-0.0.8/ml/trainers/mixins/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.8/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.8/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.8/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.8/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.8/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/rl.py` & `ml-starter-0.0.8/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/sl.py` & `ml-starter-0.0.8/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/trainers/slurm.py` & `ml-starter-0.0.8/ml/trainers/slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 from typing import Callable, Generic, TypeVar
 
 from omegaconf import II, MISSING, OmegaConf
 from torch import nn
 from torch.optim import Optimizer
 
 from ml.core.config import conf_field
-from ml.core.env import get_distributed_backend, is_torch_compiled
-from ml.core.registry import Objects, stage_environment
+from ml.core.env import ProjectRoot, get_distributed_backend, get_stage_dir, is_torch_compiled
+from ml.core.registry import Objects
 from ml.core.state import State
 from ml.lr_schedulers.base import SchedulerAdapter
 from ml.scripts.train import train_main
 from ml.trainers.base import ModelT, TaskT
 from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfig
 from ml.utils.distributed import (
     get_master_addr,
@@ -48,14 +48,15 @@
     is_master,
     set_init_method,
     set_master_addr,
     set_rank,
     set_world_size,
 )
 from ml.utils.logging import configure_logging
+from ml.utils.staging import stage_environment
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 SBATCH_TEMPLATE: str = """
 #!/bin/bash
 #SBATCH --job-name={job_name}
 #SBATCH --partition={partition}
@@ -69,14 +70,15 @@
 #SBATCH --gres={gres}
 #SBATCH --gpu-bind={gpu_bind}
 #SBATCH --output={output_path}
 #SBATCH --error={error_path}
 #SBATCH --open-mode=append
 {extra_sbatch_lines}
 
+export PROJECT_ROOT={project_root}
 export PYTHONPATH={pythonpath}
 export MASTER_PORT={master_port}
 
 # Set some debugging flags.
 export TORCH_DISTRIBUTED_DEBUG=DETAIL
 export TORCH_SHOW_CPP_STACKTRACES=1
 export NCCL_DEBUG=1
@@ -89,15 +91,15 @@
 # Runs the training command.
 srun \\
     --nodes={num_nodes} \\
     --ntasks-per-node={tasks_per_node} \\
     --cpus-per-task={cpus_per_task} \\
     --gres={gres} \\
     --gpu-bind={gpu_bind} \\
-    python {stage_dir}/ml/trainers/slurm.py {config_path}
+    python -m ml.trainers.slurm {config_path}
 
 echo ""
 """.strip()
 
 
 def get_random_port() -> int:
     return (hash(time.time()) + random.randint(0, 100000)) % (65_535 - 10_000) + 10_000
@@ -179,15 +181,19 @@
 
         # Writes all Slurm stuff (including logs) to this folder.
         slurm_log_dir = self.exp_dir / "logs"
         slurm_log_dir.mkdir(exist_ok=True, parents=True)
         sbatch_path = self.exp_dir / "sbatch.sh"
 
         # Stages all files to a new directory.
-        stage_dir = stage_environment()
+        project_root = ProjectRoot.get()
+        if project_root is None:
+            raise ValueError("Project root not found; cannot stage files")
+        stage_dir = stage_environment(project_root, get_stage_dir())
+        new_project_root = stage_dir / ProjectRoot.get().name
 
         # Gets the python path with the new output directory.
         python_path_parts = [str(stage_dir)] + os.environ.get("PYTHONPATH", "").split(":")
         python_path = ":".join(p for p in python_path_parts if p)
 
         # Comment miscellaneous stuff here.
         comments: list[str] = []
@@ -209,14 +215,15 @@
             tasks_per_node=tasks_per_node,
             cpus_per_task=cpus_per_task,
             gres=gres,
             gpu_bind=gpu_bind,
             output_path=slurm_log_dir / "slurm_out.txt",
             error_path=slurm_log_dir / "slurm_err.%j.txt",
             extra_sbatch_lines="\n".join(f"#SBATCH {line}" for line in sbatch_lines),
+            project_root=new_project_root,
             pythonpath=python_path,
             master_port=self.config.master_port,
             config_path=self.exp_dir / "config.yaml",
             lock_file_path=self.exp_dir / ".lock_running",
             stage_dir=stage_dir,
         )
```

### Comparing `ml-starter-0.0.7/ml/trainers/vanilla.py` & `ml-starter-0.0.8/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/argparse.py` & `ml-starter-0.0.8/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/atomic.py` & `ml-starter-0.0.8/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/augmentation.py` & `ml-starter-0.0.8/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/caching.py` & `ml-starter-0.0.8/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/call_train.py` & `ml-starter-0.0.8/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/cli.py` & `ml-starter-0.0.8/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/colors.py` & `ml-starter-0.0.8/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/compiler.py` & `ml-starter-0.0.8/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/data.py` & `ml-starter-0.0.8/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/datetime.py` & `ml-starter-0.0.8/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/distributed.py` & `ml-starter-0.0.8/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/io.py` & `ml-starter-0.0.8/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/large_models.py` & `ml-starter-0.0.8/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/logging.py` & `ml-starter-0.0.8/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/meter.py` & `ml-starter-0.0.8/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/timer.py` & `ml-starter-0.0.8/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml/utils/video.py` & `ml-starter-0.0.8/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.8/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.7
+Version: 0.0.8
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.7/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.8/ml_starter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 ml/lr_schedulers/linear.py
 ml/lr_schedulers/linear_no_decay.py
 ml/lr_schedulers/scripts/__init__.py
 ml/lr_schedulers/scripts/plot.py
 ml/models/__init__.py
 ml/models/activations.py
 ml/models/base.py
+ml/models/embeddings.py
 ml/models/init.py
 ml/models/norms.py
 ml/optimizers/__init__.py
 ml/optimizers/adam.py
 ml/optimizers/adamw.py
 ml/optimizers/adan.py
 ml/optimizers/base.py
@@ -110,14 +111,15 @@
 ml/utils/io.py
 ml/utils/large_models.py
 ml/utils/logging.py
 ml/utils/meter.py
 ml/utils/networking.py
 ml/utils/paths.py
 ml/utils/random.py
+ml/utils/staging.py
 ml/utils/timer.py
 ml/utils/video.py
 ml_starter.egg-info/PKG-INFO
 ml_starter.egg-info/SOURCES.txt
 ml_starter.egg-info/dependency_links.txt
 ml_starter.egg-info/entry_points.txt
 ml_starter.egg-info/requires.txt
```

### Comparing `ml-starter-0.0.7/pyproject.toml` & `ml-starter-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.7/setup.py` & `ml-starter-0.0.8/setup.py`

 * *Files identical despite different names*

