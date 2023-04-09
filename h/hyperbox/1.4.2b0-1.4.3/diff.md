# Comparing `tmp/hyperbox-1.4.2b0.tar.gz` & `tmp/hyperbox-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hyperbox-1.4.2b0.tar", last modified: Tue Mar 28 02:30:31 2023, max compression
+gzip compressed data, was "hyperbox-1.4.3.tar", last modified: Sun Apr  9 00:45:11 2023, max compression
```

## Comparing `hyperbox-1.4.2b0.tar` & `hyperbox-1.4.3.tar`

### file list

```diff
@@ -1,310 +1,310 @@
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/
--rw-r-----   0 xihe     (34831) nvidia    (1001)     1084 2021-11-02 13:12:50.000000 hyperbox-1.4.2b0/LICENSE
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       41 2022-04-18 11:26:40.000000 hyperbox-1.4.2b0/MANIFEST.in
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      246 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/PKG-INFO
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     5805 2022-12-10 14:17:32.000000 hyperbox-1.4.2b0/README.md
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:29.000000 hyperbox-1.4.2b0/hyperbox/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2021-12-26 06:45:17.000000 hyperbox-1.4.2b0/hyperbox/__init__.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/callbacks/
--rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.2b0/hyperbox/callbacks/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     8638 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/callbacks/wandb_callbacks.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/__init__.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/callbacks/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      847 2022-04-18 06:52:44.000000 hyperbox-1.4.2b0/hyperbox/configs/callbacks/default.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/callbacks/none.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      728 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/callbacks/wandb.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     1398 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/config.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/datamodule/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      289 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/datamodule/cifar100_datamodule.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      285 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/datamodule/cifar10_datamodule.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      298 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/datamodule/fakedata_datamodule.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      189 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/datamodule/imagenet_dali_datamodule.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      238 2022-07-29 05:50:40.000000 hyperbox-1.4.2b0/hyperbox/configs/datamodule/imagenet_datamodule.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      161 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/datamodule/medmnist_datamodule.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      182 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/datamodule/mnist_datamodule.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/datamodule/transforms/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      285 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/datamodule/transforms/cifar.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/engine/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-04-18 06:49:41.000000 hyperbox-1.4.2b0/hyperbox/configs/engine/none.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/experiment/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      776 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/experiment/example_bnnas.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      670 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/experiment/example_classify.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      731 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/experiment/example_darts_nas.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     1631 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/experiment/example_full.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      881 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/experiment/example_nasbench.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      862 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/experiment/example_ofa_nas.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      532 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/experiment/example_random_nas.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      977 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/experiment/example_repnas.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      729 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/experiment/example_simple.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/hparams_search/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     1944 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/hparams_search/mnist_optuna.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/hydra/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      770 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/hydra/default.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      489 2022-01-16 07:12:46.000000 hyperbox-1.4.2b0/hyperbox/configs/lite.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/logger/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      234 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/logger/comet.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      163 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/logger/csv.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      175 2022-02-04 13:07:58.000000 hyperbox-1.4.2b0/hyperbox/configs/logger/many_loggers.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      219 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/logger/mlflow.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      333 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/logger/neptune.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      253 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/logger/tensorboard.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      406 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/logger/wandb.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/model/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      274 2022-07-08 15:14:53.000000 hyperbox-1.4.2b0/hyperbox/configs/model/classify_model.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      247 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/darts_model.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/model/loss_cfg/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       35 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/loss_cfg/cross_entropy.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       91 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/loss_cfg/cross_entropy_labelsmooth.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/model/metric_cfg/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      100 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/metric_cfg/accuracy.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      170 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mnist_model.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       47 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/darts_multiple_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       39 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/darts_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      281 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/ea_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      297 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/enas_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      426 2022-04-29 10:58:27.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/evolution_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       61 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/fairdarts_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       57 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/fairnas_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      146 2022-05-03 12:24:07.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/fewshot_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       40 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/onehot_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       48 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/random_multiple_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       55 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/random_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       40 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/mutator_cfg/repnas_mutator.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      242 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/nasbench_model.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      257 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/bn_nas.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      256 2022-07-08 15:15:02.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/darts_network.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      141 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/enas_macro.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      133 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/enas_micro.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       43 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/finegrained_resnet.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      216 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/mobilenet2d_nas.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      218 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/mobilenet3d_nas.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      119 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/nasbench201.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      141 2022-04-16 12:28:50.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/nasbench_mbnet.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      354 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/ofa_mbv3.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      220 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/repnas_network.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       63 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/network_cfg/torch_network.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      244 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/ofa_model.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/model/optimizer_cfg/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       96 2022-02-14 08:07:22.000000 hyperbox-1.4.2b0/hyperbox/configs/model/optimizer_cfg/adadelta.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       61 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/optimizer_cfg/adam.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       58 2022-02-15 04:29:56.000000 hyperbox-1.4.2b0/hyperbox/configs/model/optimizer_cfg/adamw.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       53 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/optimizer_cfg/asam.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      113 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/optimizer_cfg/lamb.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      111 2022-02-14 08:02:59.000000 hyperbox-1.4.2b0/hyperbox/configs/model/optimizer_cfg/rmsprop.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       52 2022-02-15 04:29:33.000000 hyperbox-1.4.2b0/hyperbox/configs/model/optimizer_cfg/sam.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       74 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/optimizer_cfg/sgd.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      247 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/random_model.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      442 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/repnas_model.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      295 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/resnet18.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/model/scheduler_cfg/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       92 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/scheduler_cfg/CosineAnnealingLR.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       75 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/scheduler_cfg/ExponentialLR.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      104 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/scheduler_cfg/MultiStepLR.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      201 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/scheduler_cfg/ReducedLRonPlateau.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      346 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/configs/model/scheduler_cfg/warmup_scheduler.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/paths/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      609 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/paths/default.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/configs/trainer/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      407 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/trainer/ddp.yaml
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      334 2022-08-05 13:07:27.000000 hyperbox-1.4.2b0/hyperbox/configs/trainer/default.yaml
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/datamodules/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      300 2021-12-24 08:24:04.000000 hyperbox-1.4.2b0/hyperbox/datamodules/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     6420 2022-08-04 13:13:55.000000 hyperbox-1.4.2b0/hyperbox/datamodules/cifar_datamodule.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/datamodules/datasets/
--rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.2b0/hyperbox/datamodules/datasets/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     2642 2021-12-24 08:24:04.000000 hyperbox-1.4.2b0/hyperbox/datamodules/distributed_sampler_wrapper.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     4216 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/datamodules/fakedata_datamodule.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     9518 2022-08-04 14:34:56.000000 hyperbox-1.4.2b0/hyperbox/datamodules/imagenet_dali_datamodule.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     4850 2023-02-21 06:36:50.000000 hyperbox-1.4.2b0/hyperbox/datamodules/imagenet_datamodule.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    11646 2022-01-27 08:35:53.000000 hyperbox-1.4.2b0/hyperbox/datamodules/medmnist_datamodule.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     3600 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/datamodules/mnist_datamodule.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/datamodules/transforms/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      612 2021-11-10 06:57:09.000000 hyperbox-1.4.2b0/hyperbox/datamodules/transforms/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     5038 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/datamodules/transforms/albumentation_transforms.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)    11812 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/datamodules/transforms/autoaugment.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     1057 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/datamodules/transforms/base_transforms.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     2287 2021-07-21 12:32:16.000000 hyperbox-1.4.2b0/hyperbox/datamodules/transforms/custom_transforms.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     1303 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/datamodules/transforms/cutout.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     4215 2021-11-10 06:57:09.000000 hyperbox-1.4.2b0/hyperbox/datamodules/transforms/torch_transforms.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/engine/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-04-17 07:31:21.000000 hyperbox-1.4.2b0/hyperbox/engine/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      344 2022-04-18 08:25:25.000000 hyperbox-1.4.2b0/hyperbox/engine/base_engine.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/losses/
--rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.2b0/hyperbox/losses/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     1064 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/losses/ce_labelsmooth_loss.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     3827 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/losses/focal_loss.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)      594 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/losses/kd_loss.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/models/
--rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.2b0/hyperbox/models/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    12795 2022-05-03 07:07:08.000000 hyperbox-1.4.2b0/hyperbox/models/base_model.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     5040 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/models/classify_model.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    10617 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/models/darts_model.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     5026 2021-10-28 11:38:49.000000 hyperbox-1.4.2b0/hyperbox/models/ea_model.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     4864 2022-01-14 05:07:52.000000 hyperbox-1.4.2b0/hyperbox/models/mnist_model.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     5052 2022-04-04 13:49:53.000000 hyperbox-1.4.2b0/hyperbox/models/nasbench_model.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)    15958 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/models/ofa_model.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     5113 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/models/random_model.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox/mutables/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      535 2022-08-24 11:41:08.000000 hyperbox-1.4.2b0/hyperbox/mutables/__init__.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/mutables/layers/
--rw-r-----   0 xihe     (34831) nvidia    (1001)       23 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/mutables/layers/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     6261 2022-08-08 11:13:05.000000 hyperbox-1.4.2b0/hyperbox/mutables/layers/layers2d.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     1081 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/mutables/masker.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/
--rw-r-----   0 xihe     (34831) nvidia    (1001)      212 2023-03-28 02:26:22.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     1725 2022-08-08 12:33:18.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/base_module.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     4370 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/batchnorm.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    16635 2023-03-26 10:30:23.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/conv.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     2277 2023-03-27 06:47:32.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/embedding.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     3393 2023-03-27 14:10:07.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/groupnorm.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     4216 2023-03-27 08:42:55.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/layernorm.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     4610 2023-03-27 08:42:21.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/linear.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    17277 2023-03-27 13:06:30.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/multihead_attention.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)      639 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/mutables/ops/utils.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    23468 2023-03-27 09:47:37.000000 hyperbox-1.4.2b0/hyperbox/mutables/spaces.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/mutator/
--rw-r-----   0 xihe     (34831) nvidia    (1001)      646 2022-04-29 02:56:54.000000 hyperbox-1.4.2b0/hyperbox/mutator/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     6885 2022-04-27 12:40:56.000000 hyperbox-1.4.2b0/hyperbox/mutator/base_mutator.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     6373 2022-04-27 13:36:28.000000 hyperbox-1.4.2b0/hyperbox/mutator/darts_multiple_mutator.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     5780 2022-04-27 13:36:28.000000 hyperbox-1.4.2b0/hyperbox/mutator/darts_mutator.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    10786 2023-02-21 06:36:50.000000 hyperbox-1.4.2b0/hyperbox/mutator/default_mutator.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    20789 2023-03-26 10:30:23.000000 hyperbox-1.4.2b0/hyperbox/mutator/ea_mutator.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)    10885 2022-04-27 13:36:28.000000 hyperbox-1.4.2b0/hyperbox/mutator/enas_mutator.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    19266 2023-02-21 06:36:50.000000 hyperbox-1.4.2b0/hyperbox/mutator/evolution_mutator.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     8837 2022-05-09 13:46:33.000000 hyperbox-1.4.2b0/hyperbox/mutator/fairnas_mutator.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     5978 2022-05-03 13:25:30.000000 hyperbox-1.4.2b0/hyperbox/mutator/fewshot_mutator.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     2663 2022-04-27 13:36:28.000000 hyperbox-1.4.2b0/hyperbox/mutator/fixed_mutator.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     4055 2021-08-22 15:08:45.000000 hyperbox-1.4.2b0/hyperbox/mutator/hete_mutator.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     1573 2022-04-27 13:36:28.000000 hyperbox-1.4.2b0/hyperbox/mutator/onehot_mutator.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)    17999 2022-04-27 13:36:28.000000 hyperbox-1.4.2b0/hyperbox/mutator/proxyless_mutator.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     2043 2022-04-27 16:36:46.000000 hyperbox-1.4.2b0/hyperbox/mutator/random_multiple_mutator.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     1733 2022-04-27 13:36:28.000000 hyperbox-1.4.2b0/hyperbox/mutator/random_mutator.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     6298 2022-04-27 13:36:28.000000 hyperbox-1.4.2b0/hyperbox/mutator/repnas_mutator.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     2548 2022-04-27 13:45:23.000000 hyperbox-1.4.2b0/hyperbox/mutator/sequential_mutator.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     3754 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/mutator/utils.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2021-12-24 08:24:04.000000 hyperbox-1.4.2b0/hyperbox/networks/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     8314 2023-03-27 02:17:23.000000 hyperbox-1.4.2b0/hyperbox/networks/base_nas_network.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/bnnas/
--rw-r-----   0 xihe     (34831) nvidia    (1001)       46 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/bnnas/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     2446 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/bnnas/bn_blocks.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     6141 2023-03-28 02:24:18.000000 hyperbox-1.4.2b0/hyperbox/networks/bnnas/bn_net.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     3807 2022-04-27 13:51:38.000000 hyperbox-1.4.2b0/hyperbox/networks/bnnas/ea_search.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/darts/
--rw-r-----   0 xihe     (34831) nvidia    (1001)       30 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/darts/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    11739 2022-01-14 05:07:53.000000 hyperbox-1.4.2b0/hyperbox/networks/darts/darts_network.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     6546 2022-01-14 05:07:53.000000 hyperbox-1.4.2b0/hyperbox/networks/darts/darts_ops.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/enas/
--rw-r-----   0 xihe     (34831) nvidia    (1001)       29 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/enas/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)    12277 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/enas/enas_network.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     5666 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/enas/enas_ops.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/gpt/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       20 2023-03-27 13:33:03.000000 hyperbox-1.4.2b0/hyperbox/networks/gpt/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     8892 2023-03-27 13:33:19.000000 hyperbox-1.4.2b0/hyperbox/networks/gpt/gpt2.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/mobilenet/
--rw-r-----   0 xihe     (34831) nvidia    (1001)       72 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/mobilenet/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     6534 2023-02-26 03:44:28.000000 hyperbox-1.4.2b0/hyperbox/networks/mobilenet/mobile3d_net.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    12881 2023-02-28 03:01:43.000000 hyperbox-1.4.2b0/hyperbox/networks/mobilenet/mobile3d_ops.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     6138 2023-02-27 12:03:40.000000 hyperbox-1.4.2b0/hyperbox/networks/mobilenet/mobile_net.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    12923 2023-02-28 03:01:49.000000 hyperbox-1.4.2b0/hyperbox/networks/mobilenet/mobile_ops.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     2287 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/mobilenet/mobile_utils.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-04-19 11:16:04.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     2070 2022-04-19 14:19:00.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/base_ops.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      203 2022-04-19 11:24:57.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      246 2022-04-19 11:25:01.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/constants.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     2503 2022-04-19 12:52:32.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/db_gen.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     3826 2022-04-19 12:32:02.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/graph_util.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     3696 2022-04-19 12:33:05.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/model.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     2486 2022-04-19 12:32:07.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/query.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     5913 2022-04-19 14:01:43.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/graph_util.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     5641 2022-04-19 14:38:25.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/model_spec.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    13515 2022-04-20 07:03:30.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench101/nasbench101.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench201/
--rw-r-----   0 xihe     (34831) nvidia    (1001)       44 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench201/__init__.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench201/db_gen/
--rw-r-----   0 xihe     (34831) nvidia    (1001)      208 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench201/db_gen/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)      187 2022-04-25 03:54:27.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench201/db_gen/constants.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     5448 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench201/db_gen/db_gen.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     6116 2021-11-02 13:12:51.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench201/db_gen/model.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     2826 2021-12-14 14:39:48.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench201/db_gen/query.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    14733 2022-04-27 12:56:52.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench201/nasbench201.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench301/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       44 2021-12-02 14:46:53.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench301/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     9879 2021-12-02 14:56:45.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench301/nasbench301_network.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     3127 2021-12-07 08:08:09.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench301/utils.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench_mbnet/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-04-16 11:38:03.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench_mbnet/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     6224 2022-05-13 12:39:34.000000 hyperbox-1.4.2b0/hyperbox/networks/nasbench_mbnet/network.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     3936 2022-01-14 05:07:53.000000 hyperbox-1.4.2b0/hyperbox/networks/network_ema.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/ofa/
--rw-r-----   0 xihe     (34831) nvidia    (1001)       38 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/networks/ofa/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    10939 2023-02-28 03:16:55.000000 hyperbox-1.4.2b0/hyperbox/networks/ofa/ofa_mbv3.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    15429 2022-01-24 07:01:45.000000 hyperbox-1.4.2b0/hyperbox/networks/pytorch_modules.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/repnas/
--rw-r-----   0 xihe     (34831) nvidia    (1001)       31 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/networks/repnas/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     9632 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/networks/repnas/rep_ops.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     6555 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/networks/repnas/repnas_spos.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     2826 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/networks/repnas/utils.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/resnet/
--rw-r-----   0 xihe     (34831) nvidia    (1001)       21 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/networks/resnet/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    13514 2023-02-26 03:44:28.000000 hyperbox-1.4.2b0/hyperbox/networks/resnet/resnet.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/rnn/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2023-02-23 03:27:40.000000 hyperbox-1.4.2b0/hyperbox/networks/rnn/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      851 2023-02-23 03:29:24.000000 hyperbox-1.4.2b0/hyperbox/networks/rnn/genotypes.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     5117 2023-02-23 03:29:08.000000 hyperbox-1.4.2b0/hyperbox/networks/rnn/rnn.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     2955 2023-02-23 03:28:22.000000 hyperbox-1.4.2b0/hyperbox/networks/rnn/utils.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/spos/
--rw-r-----   0 xihe     (34831) nvidia    (1001)       54 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/networks/spos/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     4525 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/networks/spos/shuffle_blocks.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     4431 2022-04-16 11:39:32.000000 hyperbox-1.4.2b0/hyperbox/networks/spos/spos_net.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     8572 2022-05-07 08:19:13.000000 hyperbox-1.4.2b0/hyperbox/networks/utils.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/networks/vit/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       18 2022-12-12 14:26:49.000000 hyperbox-1.4.2b0/hyperbox/networks/vit/__init__.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    12574 2023-02-22 13:51:59.000000 hyperbox-1.4.2b0/hyperbox/networks/vit/vit.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/optimizers/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2021-12-24 08:24:04.000000 hyperbox-1.4.2b0/hyperbox/optimizers/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     4620 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/optimizers/lamb.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     2237 2021-11-10 06:57:09.000000 hyperbox-1.4.2b0/hyperbox/optimizers/sam.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     1588 2022-08-05 13:07:28.000000 hyperbox-1.4.2b0/hyperbox/run.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/schedulers/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2021-07-17 14:40:04.000000 hyperbox-1.4.2b0/hyperbox/schedulers/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     4497 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/schedulers/warmup_scheduler.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     4824 2022-04-18 09:10:04.000000 hyperbox-1.4.2b0/hyperbox/train.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/hyperbox/utils/
--rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.2b0/hyperbox/utils/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     2767 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/utils/average_meter.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     5499 2022-04-29 06:58:11.000000 hyperbox-1.4.2b0/hyperbox/utils/calc_model_size.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     1431 2023-02-21 06:36:50.000000 hyperbox-1.4.2b0/hyperbox/utils/logger.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     1495 2021-12-24 08:24:04.000000 hyperbox-1.4.2b0/hyperbox/utils/metrics.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)    11196 2023-03-28 02:29:20.000000 hyperbox-1.4.2b0/hyperbox/utils/utils.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     2989 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/hyperbox/utils/visualize_darts_cell.py
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     1780 2022-04-16 12:18:22.000000 hyperbox-1.4.2b0/hyperbox/utils/visualize_mbconv_net.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:30.000000 hyperbox-1.4.2b0/hyperbox.egg-info/
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      246 2023-03-28 02:30:29.000000 hyperbox-1.4.2b0/hyperbox.egg-info/PKG-INFO
--rw-r--r--   0 xihe     (34831) nvidia    (1001)     9950 2023-03-28 02:30:29.000000 hyperbox-1.4.2b0/hyperbox.egg-info/SOURCES.txt
--rw-r--r--   0 xihe     (34831) nvidia    (1001)        1 2023-03-28 02:30:29.000000 hyperbox-1.4.2b0/hyperbox.egg-info/dependency_links.txt
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      347 2023-03-28 02:30:29.000000 hyperbox-1.4.2b0/hyperbox.egg-info/requires.txt
--rw-r--r--   0 xihe     (34831) nvidia    (1001)       15 2023-03-28 02:30:29.000000 hyperbox-1.4.2b0/hyperbox.egg-info/top_level.txt
--rw-r-----   0 xihe     (34831) nvidia    (1001)      764 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/setup.cfg
--rw-r--r--   0 xihe     (34831) nvidia    (1001)      640 2023-03-28 02:29:42.000000 hyperbox-1.4.2b0/setup.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/tests/
--rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.2b0/tests/__init__.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/tests/helpers/
--rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.2b0/tests/helpers/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)      953 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/tests/helpers/module_available.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)      330 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/tests/helpers/run_command.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     3544 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/tests/helpers/runif.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/tests/smoke/
--rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:30.000000 hyperbox-1.4.2b0/tests/smoke/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     2665 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/tests/smoke/test_commands.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     1140 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/tests/smoke/test_mixed_precision.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)      978 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/tests/smoke/test_sweeps.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)     1027 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/tests/smoke/test_wandb.py
-drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-03-28 02:30:31.000000 hyperbox-1.4.2b0/tests/unit/
--rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:30.000000 hyperbox-1.4.2b0/tests/unit/__init__.py
--rw-r-----   0 xihe     (34831) nvidia    (1001)      600 2021-11-02 13:12:52.000000 hyperbox-1.4.2b0/tests/unit/test_sth.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.478577 hyperbox-1.4.3/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     1084 2021-11-02 13:12:50.000000 hyperbox-1.4.3/LICENSE
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       41 2022-04-18 11:26:40.000000 hyperbox-1.4.3/MANIFEST.in
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      188 2023-04-09 00:45:11.479577 hyperbox-1.4.3/PKG-INFO
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     5802 2023-03-29 11:10:24.000000 hyperbox-1.4.3/README.md
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.020562 hyperbox-1.4.3/hyperbox/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2021-12-26 06:45:17.000000 hyperbox-1.4.3/hyperbox/__init__.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.089559 hyperbox-1.4.3/hyperbox/callbacks/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.3/hyperbox/callbacks/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     8638 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/callbacks/wandb_callbacks.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.100562 hyperbox-1.4.3/hyperbox/configs/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/__init__.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.135562 hyperbox-1.4.3/hyperbox/configs/callbacks/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      847 2022-04-18 06:52:44.000000 hyperbox-1.4.3/hyperbox/configs/callbacks/default.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/callbacks/none.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      728 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/callbacks/wandb.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     1398 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/config.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.175562 hyperbox-1.4.3/hyperbox/configs/datamodule/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      289 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/datamodule/cifar100_datamodule.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      285 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/datamodule/cifar10_datamodule.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      298 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/datamodule/fakedata_datamodule.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      189 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/datamodule/imagenet_dali_datamodule.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      238 2022-07-29 05:50:40.000000 hyperbox-1.4.3/hyperbox/configs/datamodule/imagenet_datamodule.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      161 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/datamodule/medmnist_datamodule.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      182 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/datamodule/mnist_datamodule.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.197560 hyperbox-1.4.3/hyperbox/configs/datamodule/transforms/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      285 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/datamodule/transforms/cifar.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.219560 hyperbox-1.4.3/hyperbox/configs/engine/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-04-18 06:49:41.000000 hyperbox-1.4.3/hyperbox/configs/engine/none.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.261562 hyperbox-1.4.3/hyperbox/configs/experiment/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      776 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/experiment/example_bnnas.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      670 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/experiment/example_classify.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      731 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/experiment/example_darts_nas.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     1631 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/experiment/example_full.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      881 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/experiment/example_nasbench.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      862 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/experiment/example_ofa_nas.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      532 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/experiment/example_random_nas.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      977 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/experiment/example_repnas.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      729 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/experiment/example_simple.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.274561 hyperbox-1.4.3/hyperbox/configs/hparams_search/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     1944 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/hparams_search/mnist_optuna.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.290561 hyperbox-1.4.3/hyperbox/configs/hydra/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      770 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/hydra/default.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      489 2022-01-16 07:12:46.000000 hyperbox-1.4.3/hyperbox/configs/lite.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.353562 hyperbox-1.4.3/hyperbox/configs/logger/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      234 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/logger/comet.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      163 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/logger/csv.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      175 2022-02-04 13:07:58.000000 hyperbox-1.4.3/hyperbox/configs/logger/many_loggers.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      219 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/logger/mlflow.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      333 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/logger/neptune.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      253 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/logger/tensorboard.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      406 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/logger/wandb.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.376563 hyperbox-1.4.3/hyperbox/configs/model/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      274 2022-07-08 15:14:53.000000 hyperbox-1.4.3/hyperbox/configs/model/classify_model.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      247 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/darts_model.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.381564 hyperbox-1.4.3/hyperbox/configs/model/loss_cfg/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       35 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/loss_cfg/cross_entropy.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       91 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/loss_cfg/cross_entropy_labelsmooth.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.385562 hyperbox-1.4.3/hyperbox/configs/model/metric_cfg/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      100 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/metric_cfg/accuracy.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      170 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mnist_model.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.455564 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       47 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/darts_multiple_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       39 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/darts_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      281 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/ea_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      297 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/enas_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      426 2022-04-29 10:58:27.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/evolution_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       61 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/fairdarts_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       57 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/fairnas_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      146 2022-05-03 12:24:07.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/fewshot_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       40 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/onehot_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       48 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/random_multiple_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       55 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/random_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       40 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/mutator_cfg/repnas_mutator.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      242 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/nasbench_model.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.511564 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      257 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/bn_nas.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      256 2022-07-08 15:15:02.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/darts_network.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      141 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/enas_macro.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      133 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/enas_micro.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       43 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/finegrained_resnet.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      216 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/mobilenet2d_nas.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      218 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/mobilenet3d_nas.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      119 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/nasbench201.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      141 2022-04-16 12:28:50.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/nasbench_mbnet.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      354 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/ofa_mbv3.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      220 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/repnas_network.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       63 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/network_cfg/torch_network.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      244 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/ofa_model.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.556567 hyperbox-1.4.3/hyperbox/configs/model/optimizer_cfg/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       96 2022-02-14 08:07:22.000000 hyperbox-1.4.3/hyperbox/configs/model/optimizer_cfg/adadelta.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       61 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/optimizer_cfg/adam.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       58 2022-02-15 04:29:56.000000 hyperbox-1.4.3/hyperbox/configs/model/optimizer_cfg/adamw.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       53 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/optimizer_cfg/asam.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      113 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/optimizer_cfg/lamb.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      111 2022-02-14 08:02:59.000000 hyperbox-1.4.3/hyperbox/configs/model/optimizer_cfg/rmsprop.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       52 2022-02-15 04:29:33.000000 hyperbox-1.4.3/hyperbox/configs/model/optimizer_cfg/sam.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       74 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/optimizer_cfg/sgd.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      247 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/random_model.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      442 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/repnas_model.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      295 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/resnet18.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.580566 hyperbox-1.4.3/hyperbox/configs/model/scheduler_cfg/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       92 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/scheduler_cfg/CosineAnnealingLR.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       75 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/scheduler_cfg/ExponentialLR.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      104 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/scheduler_cfg/MultiStepLR.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      201 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/scheduler_cfg/ReducedLRonPlateau.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      346 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/configs/model/scheduler_cfg/warmup_scheduler.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.583565 hyperbox-1.4.3/hyperbox/configs/paths/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      609 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/paths/default.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.589565 hyperbox-1.4.3/hyperbox/configs/trainer/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      407 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/trainer/ddp.yaml
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      334 2022-08-05 13:07:27.000000 hyperbox-1.4.3/hyperbox/configs/trainer/default.yaml
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.640567 hyperbox-1.4.3/hyperbox/datamodules/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      300 2021-12-24 08:24:04.000000 hyperbox-1.4.3/hyperbox/datamodules/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     6420 2022-08-04 13:13:55.000000 hyperbox-1.4.3/hyperbox/datamodules/cifar_datamodule.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.673565 hyperbox-1.4.3/hyperbox/datamodules/datasets/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.3/hyperbox/datamodules/datasets/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     2642 2021-12-24 08:24:04.000000 hyperbox-1.4.3/hyperbox/datamodules/distributed_sampler_wrapper.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     4216 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/datamodules/fakedata_datamodule.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     9518 2022-08-04 14:34:56.000000 hyperbox-1.4.3/hyperbox/datamodules/imagenet_dali_datamodule.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     4850 2023-02-21 06:36:50.000000 hyperbox-1.4.3/hyperbox/datamodules/imagenet_datamodule.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    11646 2022-01-27 08:35:53.000000 hyperbox-1.4.3/hyperbox/datamodules/medmnist_datamodule.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     3600 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/datamodules/mnist_datamodule.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.719567 hyperbox-1.4.3/hyperbox/datamodules/transforms/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      612 2021-11-10 06:57:09.000000 hyperbox-1.4.3/hyperbox/datamodules/transforms/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     5038 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/datamodules/transforms/albumentation_transforms.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)    11812 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/datamodules/transforms/autoaugment.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     1057 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/datamodules/transforms/base_transforms.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     2287 2021-07-21 12:32:16.000000 hyperbox-1.4.3/hyperbox/datamodules/transforms/custom_transforms.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     1303 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/datamodules/transforms/cutout.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     4215 2021-11-10 06:57:09.000000 hyperbox-1.4.3/hyperbox/datamodules/transforms/torch_transforms.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.737568 hyperbox-1.4.3/hyperbox/engine/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-04-17 07:31:21.000000 hyperbox-1.4.3/hyperbox/engine/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      344 2022-04-18 08:25:25.000000 hyperbox-1.4.3/hyperbox/engine/base_engine.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.757569 hyperbox-1.4.3/hyperbox/losses/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.3/hyperbox/losses/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     1064 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/losses/ce_labelsmooth_loss.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     3827 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/losses/focal_loss.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      594 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/losses/kd_loss.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.801566 hyperbox-1.4.3/hyperbox/models/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.3/hyperbox/models/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    12795 2022-05-03 07:07:08.000000 hyperbox-1.4.3/hyperbox/models/base_model.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     5040 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/models/classify_model.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    10617 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/models/darts_model.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     5026 2021-10-28 11:38:49.000000 hyperbox-1.4.3/hyperbox/models/ea_model.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     4864 2022-01-14 05:07:52.000000 hyperbox-1.4.3/hyperbox/models/mnist_model.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     5052 2022-04-04 13:49:53.000000 hyperbox-1.4.3/hyperbox/models/nasbench_model.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)    15958 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/models/ofa_model.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     5113 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/models/random_model.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.823570 hyperbox-1.4.3/hyperbox/mutables/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      535 2022-08-24 11:41:08.000000 hyperbox-1.4.3/hyperbox/mutables/__init__.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.841566 hyperbox-1.4.3/hyperbox/mutables/layers/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)       23 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/mutables/layers/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     5883 2023-03-31 05:37:34.000000 hyperbox-1.4.3/hyperbox/mutables/layers/layers2d.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     1081 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/mutables/masker.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.889569 hyperbox-1.4.3/hyperbox/mutables/ops/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      212 2023-03-28 02:26:22.000000 hyperbox-1.4.3/hyperbox/mutables/ops/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     1860 2023-03-31 05:35:23.000000 hyperbox-1.4.3/hyperbox/mutables/ops/base_module.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     4370 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/mutables/ops/batchnorm.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    19145 2023-04-04 13:35:30.000000 hyperbox-1.4.3/hyperbox/mutables/ops/conv.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     2505 2023-04-01 02:25:09.000000 hyperbox-1.4.3/hyperbox/mutables/ops/embedding.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     3816 2023-04-01 02:19:45.000000 hyperbox-1.4.3/hyperbox/mutables/ops/groupnorm.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     4662 2023-04-01 02:22:24.000000 hyperbox-1.4.3/hyperbox/mutables/ops/layernorm.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     4610 2023-03-27 08:42:21.000000 hyperbox-1.4.3/hyperbox/mutables/ops/linear.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    24161 2023-04-01 02:30:53.000000 hyperbox-1.4.3/hyperbox/mutables/ops/multihead_attention.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      639 2023-03-30 06:21:11.000000 hyperbox-1.4.3/hyperbox/mutables/ops/utils.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    23822 2023-03-30 08:12:44.000000 hyperbox-1.4.3/hyperbox/mutables/spaces.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.955570 hyperbox-1.4.3/hyperbox/mutator/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      646 2022-04-29 02:56:54.000000 hyperbox-1.4.3/hyperbox/mutator/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     6885 2022-04-27 12:40:56.000000 hyperbox-1.4.3/hyperbox/mutator/base_mutator.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     6373 2022-04-27 13:36:28.000000 hyperbox-1.4.3/hyperbox/mutator/darts_multiple_mutator.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     5780 2022-04-27 13:36:28.000000 hyperbox-1.4.3/hyperbox/mutator/darts_mutator.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    10786 2023-02-21 06:36:50.000000 hyperbox-1.4.3/hyperbox/mutator/default_mutator.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    20789 2023-03-26 10:30:23.000000 hyperbox-1.4.3/hyperbox/mutator/ea_mutator.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)    10885 2022-04-27 13:36:28.000000 hyperbox-1.4.3/hyperbox/mutator/enas_mutator.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    19266 2023-02-21 06:36:50.000000 hyperbox-1.4.3/hyperbox/mutator/evolution_mutator.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     8837 2022-05-09 13:46:33.000000 hyperbox-1.4.3/hyperbox/mutator/fairnas_mutator.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     5978 2022-05-03 13:25:30.000000 hyperbox-1.4.3/hyperbox/mutator/fewshot_mutator.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     2663 2022-04-27 13:36:28.000000 hyperbox-1.4.3/hyperbox/mutator/fixed_mutator.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     4055 2021-08-22 15:08:45.000000 hyperbox-1.4.3/hyperbox/mutator/hete_mutator.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     1573 2022-04-27 13:36:28.000000 hyperbox-1.4.3/hyperbox/mutator/onehot_mutator.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)    17999 2022-04-27 13:36:28.000000 hyperbox-1.4.3/hyperbox/mutator/proxyless_mutator.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     2043 2022-04-27 16:36:46.000000 hyperbox-1.4.3/hyperbox/mutator/random_multiple_mutator.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     1733 2022-04-27 13:36:28.000000 hyperbox-1.4.3/hyperbox/mutator/random_mutator.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     6298 2022-04-27 13:36:28.000000 hyperbox-1.4.3/hyperbox/mutator/repnas_mutator.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     2548 2022-04-27 13:45:23.000000 hyperbox-1.4.3/hyperbox/mutator/sequential_mutator.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     3754 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/mutator/utils.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.972569 hyperbox-1.4.3/hyperbox/networks/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2021-12-24 08:24:04.000000 hyperbox-1.4.3/hyperbox/networks/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     8506 2023-03-28 06:01:06.000000 hyperbox-1.4.3/hyperbox/networks/base_nas_network.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.001570 hyperbox-1.4.3/hyperbox/networks/bnnas/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)       46 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/bnnas/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     2446 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/bnnas/bn_blocks.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     6141 2023-03-28 02:24:18.000000 hyperbox-1.4.3/hyperbox/networks/bnnas/bn_net.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     3807 2022-04-27 13:51:38.000000 hyperbox-1.4.3/hyperbox/networks/bnnas/ea_search.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.058572 hyperbox-1.4.3/hyperbox/networks/darts/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)       30 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/darts/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    11739 2023-04-07 11:08:33.000000 hyperbox-1.4.3/hyperbox/networks/darts/darts_network.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     6546 2022-01-14 05:07:53.000000 hyperbox-1.4.3/hyperbox/networks/darts/darts_ops.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.084569 hyperbox-1.4.3/hyperbox/networks/enas/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)       29 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/enas/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)    12277 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/enas/enas_network.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     5666 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/enas/enas_ops.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.106571 hyperbox-1.4.3/hyperbox/networks/gpt/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       20 2023-03-27 13:33:03.000000 hyperbox-1.4.3/hyperbox/networks/gpt/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     8892 2023-03-27 13:33:19.000000 hyperbox-1.4.3/hyperbox/networks/gpt/gpt2.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.139570 hyperbox-1.4.3/hyperbox/networks/mobilenet/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)       72 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/mobilenet/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     6534 2023-02-26 03:44:28.000000 hyperbox-1.4.3/hyperbox/networks/mobilenet/mobile3d_net.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    12881 2023-02-28 03:01:43.000000 hyperbox-1.4.3/hyperbox/networks/mobilenet/mobile3d_ops.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     6138 2023-04-07 14:42:42.000000 hyperbox-1.4.3/hyperbox/networks/mobilenet/mobile_net.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    12923 2023-02-28 03:01:49.000000 hyperbox-1.4.3/hyperbox/networks/mobilenet/mobile_ops.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     2287 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/mobilenet/mobile_utils.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.167571 hyperbox-1.4.3/hyperbox/networks/nasbench101/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-04-19 11:16:04.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     2070 2022-04-19 14:19:00.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/base_ops.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.211570 hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      203 2022-04-19 11:24:57.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      246 2022-04-19 11:25:01.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/constants.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     2503 2022-04-19 12:52:32.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/db_gen.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     3826 2022-04-19 12:32:02.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/graph_util.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     3696 2022-04-19 12:33:05.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/model.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     2486 2022-04-19 12:32:07.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/query.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     5913 2022-04-19 14:01:43.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/graph_util.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     5641 2022-04-19 14:38:25.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/model_spec.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    13515 2022-04-20 07:03:30.000000 hyperbox-1.4.3/hyperbox/networks/nasbench101/nasbench101.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.230572 hyperbox-1.4.3/hyperbox/networks/nasbench201/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)       44 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/nasbench201/__init__.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.249572 hyperbox-1.4.3/hyperbox/networks/nasbench201/db_gen/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      208 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/nasbench201/db_gen/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      187 2022-04-25 03:54:27.000000 hyperbox-1.4.3/hyperbox/networks/nasbench201/db_gen/constants.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     5448 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/nasbench201/db_gen/db_gen.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     6116 2021-11-02 13:12:51.000000 hyperbox-1.4.3/hyperbox/networks/nasbench201/db_gen/model.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     2826 2021-12-14 14:39:48.000000 hyperbox-1.4.3/hyperbox/networks/nasbench201/db_gen/query.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    14733 2022-04-27 12:56:52.000000 hyperbox-1.4.3/hyperbox/networks/nasbench201/nasbench201.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.274571 hyperbox-1.4.3/hyperbox/networks/nasbench301/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       44 2021-12-02 14:46:53.000000 hyperbox-1.4.3/hyperbox/networks/nasbench301/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     9879 2021-12-02 14:56:45.000000 hyperbox-1.4.3/hyperbox/networks/nasbench301/nasbench301_network.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     3127 2021-12-07 08:08:09.000000 hyperbox-1.4.3/hyperbox/networks/nasbench301/utils.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.280573 hyperbox-1.4.3/hyperbox/networks/nasbench_mbnet/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2022-04-16 11:38:03.000000 hyperbox-1.4.3/hyperbox/networks/nasbench_mbnet/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     6224 2022-05-13 12:39:34.000000 hyperbox-1.4.3/hyperbox/networks/nasbench_mbnet/network.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     3936 2022-01-14 05:07:53.000000 hyperbox-1.4.3/hyperbox/networks/network_ema.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.288570 hyperbox-1.4.3/hyperbox/networks/ofa/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)       38 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/networks/ofa/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    14644 2023-04-01 02:06:14.000000 hyperbox-1.4.3/hyperbox/networks/ofa/ofa_mbv3.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    15429 2022-01-24 07:01:45.000000 hyperbox-1.4.3/hyperbox/networks/pytorch_modules.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.302571 hyperbox-1.4.3/hyperbox/networks/repnas/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)       31 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/networks/repnas/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     9632 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/networks/repnas/rep_ops.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     6555 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/networks/repnas/repnas_spos.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     2826 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/networks/repnas/utils.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.319571 hyperbox-1.4.3/hyperbox/networks/resnet/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)       21 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/networks/resnet/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    13514 2023-02-26 03:44:28.000000 hyperbox-1.4.3/hyperbox/networks/resnet/resnet.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.351574 hyperbox-1.4.3/hyperbox/networks/rnn/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2023-02-23 03:27:40.000000 hyperbox-1.4.3/hyperbox/networks/rnn/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      851 2023-02-23 03:29:24.000000 hyperbox-1.4.3/hyperbox/networks/rnn/genotypes.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     5117 2023-02-23 03:29:08.000000 hyperbox-1.4.3/hyperbox/networks/rnn/rnn.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     2955 2023-02-23 03:28:22.000000 hyperbox-1.4.3/hyperbox/networks/rnn/utils.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.362574 hyperbox-1.4.3/hyperbox/networks/spos/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)       54 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/networks/spos/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     4525 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/networks/spos/shuffle_blocks.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     4431 2022-04-16 11:39:32.000000 hyperbox-1.4.3/hyperbox/networks/spos/spos_net.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     8572 2022-05-07 08:19:13.000000 hyperbox-1.4.3/hyperbox/networks/utils.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.385572 hyperbox-1.4.3/hyperbox/networks/vit/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       18 2022-12-12 14:26:49.000000 hyperbox-1.4.3/hyperbox/networks/vit/__init__.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    13299 2023-04-09 00:42:13.000000 hyperbox-1.4.3/hyperbox/networks/vit/vit.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.395572 hyperbox-1.4.3/hyperbox/optimizers/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2021-12-24 08:24:04.000000 hyperbox-1.4.3/hyperbox/optimizers/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     4620 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/optimizers/lamb.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     2237 2021-11-10 06:57:09.000000 hyperbox-1.4.3/hyperbox/optimizers/sam.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     1588 2022-08-05 13:07:28.000000 hyperbox-1.4.3/hyperbox/run.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.401582 hyperbox-1.4.3/hyperbox/schedulers/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        0 2021-07-17 14:40:04.000000 hyperbox-1.4.3/hyperbox/schedulers/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     4497 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/schedulers/warmup_scheduler.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     4824 2022-04-18 09:10:04.000000 hyperbox-1.4.3/hyperbox/train.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.426575 hyperbox-1.4.3/hyperbox/utils/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.3/hyperbox/utils/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     2767 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/utils/average_meter.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     7602 2023-04-01 02:35:32.000000 hyperbox-1.4.3/hyperbox/utils/calc_model_size.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     1431 2023-02-21 06:36:50.000000 hyperbox-1.4.3/hyperbox/utils/logger.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     1495 2021-12-24 08:24:04.000000 hyperbox-1.4.3/hyperbox/utils/metrics.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)    11196 2023-03-31 05:36:02.000000 hyperbox-1.4.3/hyperbox/utils/utils.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     2989 2021-11-02 13:12:52.000000 hyperbox-1.4.3/hyperbox/utils/visualize_darts_cell.py
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     1780 2022-04-16 12:18:22.000000 hyperbox-1.4.3/hyperbox/utils/visualize_mbconv_net.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:10.057561 hyperbox-1.4.3/hyperbox.egg-info/
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      188 2023-04-09 00:45:09.000000 hyperbox-1.4.3/hyperbox.egg-info/PKG-INFO
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)     9950 2023-04-09 00:45:09.000000 hyperbox-1.4.3/hyperbox.egg-info/SOURCES.txt
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)        1 2023-04-09 00:45:09.000000 hyperbox-1.4.3/hyperbox.egg-info/dependency_links.txt
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      347 2023-04-09 00:45:09.000000 hyperbox-1.4.3/hyperbox.egg-info/requires.txt
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)       15 2023-04-09 00:45:09.000000 hyperbox-1.4.3/hyperbox.egg-info/top_level.txt
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      764 2023-04-09 00:45:11.482580 hyperbox-1.4.3/setup.cfg
+-rw-r--r--   0 xihe     (34831) nvidia    (1001)      638 2023-03-31 05:45:01.000000 hyperbox-1.4.3/setup.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.430574 hyperbox-1.4.3/tests/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.3/tests/__init__.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.453574 hyperbox-1.4.3/tests/helpers/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:29.000000 hyperbox-1.4.3/tests/helpers/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      953 2021-11-02 13:12:52.000000 hyperbox-1.4.3/tests/helpers/module_available.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      330 2021-11-02 13:12:52.000000 hyperbox-1.4.3/tests/helpers/run_command.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     3544 2021-11-02 13:12:52.000000 hyperbox-1.4.3/tests/helpers/runif.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.470573 hyperbox-1.4.3/tests/smoke/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:30.000000 hyperbox-1.4.3/tests/smoke/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     2665 2021-11-02 13:12:52.000000 hyperbox-1.4.3/tests/smoke/test_commands.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     1140 2021-11-02 13:12:52.000000 hyperbox-1.4.3/tests/smoke/test_mixed_precision.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      978 2021-11-02 13:12:52.000000 hyperbox-1.4.3/tests/smoke/test_sweeps.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)     1027 2021-11-02 13:12:52.000000 hyperbox-1.4.3/tests/smoke/test_wandb.py
+drwxr-xr-x   0 xihe     (34831) nvidia    (1001)        0 2023-04-09 00:45:11.475581 hyperbox-1.4.3/tests/unit/
+-rw-r-----   0 xihe     (34831) nvidia    (1001)        0 2021-06-14 05:38:30.000000 hyperbox-1.4.3/tests/unit/__init__.py
+-rw-r-----   0 xihe     (34831) nvidia    (1001)      600 2021-11-02 13:12:52.000000 hyperbox-1.4.3/tests/unit/test_sth.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hyperbox-1.4.2b0/LICENSE` & `hyperbox-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/README.md` & `hyperbox-1.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 pip install hyperbox
 ```
 - install via `github`
 
 ```
 git clone https://github.com/marsggbo/hyperbox
 cd hyperbox
+pip install -r requirements.txt
 python setup.py develop
-python install -r requirements.txt
 ```
 
 </details>
 
 <details>
 <summary><b> Quick Start </b></summary>
```

#### html2text {}

```diff
@@ -1,55 +1,54 @@
   # Hyperbox [Hyperbox] [Python] [PyTorch] [Lightning] [Config:_hydra] [Code
  style:_black]  A clean and scalable template to kickstart your AutoML project
                                   ðâ¡ð¥
                      *Currently uses dev version of Hydra.
                        Suggestions are always welcome!*
 You can refer to [Wiki](https://github.com/marsggbo/hyperbox/wiki) for more
 details.  Install - install via `pip` ``` pip install hyperbox ``` - install
-via `github` ``` git clone https://github.com/marsggbo/hyperbox cd hyperbox
-python setup.py develop python install -r requirements.txt ```   Quick Start
-``` python -m hyperbox.run experiment=example_random_nas
-+trainer.fast_dev_run=True ```   Hyperbox Mutables (Searchable `nn.Module`)
-[image] - Code implementation for Figure (left) ```python import torch.nn as nn
-from hyperbox . mutables . spaces import OperationSpace op1 = nn.Conv2d
-(in_channels=3, out_channels=16, kernel_size=3, stride =1, padding=1) op2 =
-nn.Conv2d(in_channels=3, out_channels=16, kernel_size=5, stride =1, padding=2)
-op3 = nn.Conv2d(in_channels=3, out_channels=16, kernel_size=7, stride =1,
-padding=3) ops = OperationSpace(candidates=[op1, op2, op3], key=âconv_opâ,
-mask=[1, 0, 0]) ``` Code implementation for Figure (middle) ```python import
-torch from hyperbox.mutables.spaces import InputSpace in1 = torch.rand(2, 64)
-in2 = torch.rand(2, 32) in3 = torch.rand(2, 16) inputs = [in1, in2, in3]
-skipconnect = InputSpace(n_candidates=3, n_chosen=1, key=âscâ, mask=[0, 1,
-0]) out = skipconnect([ in1 , in2 , in3 ]) assert out is in2 >>> True ``` -
-Code implementation for Figure (right) ```python from hyperbox.mutables.ops
-import Conv2d, Linear from hyperbox.mutables.spaces import ValueSpace #
-convolution ks = ValueSpace([3, 5, 7], key=âkernelSizeâ, mask=[0, 1, 0])
-cout = ValueSpace([16, 32, 64], key=âchannelOutâ, mask=[0, 1, 0]) conv =
-Conv2d(3 , cout , ks , stride =1, padding=2, bias=False ) print([x.shape for x
-in conv.parameters()]) >>> [torch.Size([32, 3, 5, 5])] # linear cout =
-ValueSpace([10, 100], key=âchannelOut1â) isBias = ValueSpace([0, 1],
-key=âbiasâ) # 0: False, 1: True linear = Linear(10, cout , bias=isBias)
-print([x.shape for x in linear.parameters()]) >>> [ torch . Size ([100 , 10]) ,
-torch . Size ([100]) ] ```   Hyperbox Mutator (Search Algorithms) - Random
-Search Algorithm `RandomMutator` ```python from hyperbox.mutator import
-RandomMutator from hyperbox.networks.ofa import OFAMobileNetV3 net =
-OFAMobileNetV3() rm = RandomMutator(net) rm.reset() # search a subnet arch:
-dict = rm._cache # arch of a subnet print(arch) subnet = OFAMobileNetV3
-(mask=arch) # initialize a subnet, which has smaller parameters than `net` ```
-the model arch is saved in `rm._cache`   Hyperbox Wikis - [Wiki for
-hyperbox.config](https://github.com/marsggbo/hyperbox/wiki/Customize-Config) -
-[Wiki for hyperbox.mutables](https://github.com/marsggbo/hyperbox/wiki/
-Customize-Mutable) - [Wiki for hyperbox.engine](https://github.com/marsggbo/
-hyperbox/wiki/Customize-Engine) - [Wiki for hyperbox.mutator](https://
-github.com/marsggbo/hyperbox/wiki/Customize-Mutator) - [Wiki for
-hyperbox.models](https://github.com/marsggbo/hyperbox/wiki/Customize-Models) -
-[Wiki for hyperbox.networks](https://github.com/marsggbo/hyperbox/wiki/
-Customize-NAS-Network) - [Wiki for Hydra](https://github.com/marsggbo/hyperbox/
-wiki/Hydra-Q&A) - [Wiki for Hyperbox App](https://github.com/marsggbo/hyperbox/
-wiki/Hyperbox-App:-Start-a-new-project) - [Miscellaneous](https://github.com/
-marsggbo/hyperbox/wiki/Miscellaneous-(tricks)) - [Q&A](https://github.com/
-marsggbo/hyperbox/wiki/Q&A) - [Usage](https://github.com/marsggbo/hyperbox/
-wiki/Usages)  ## Thanks [![](https://shields.io/badge/-NNI-
-017F2F?style=flat&logo=github&labelColor=303030)](https://github.com/microsoft/
-nni/tree/v1.7) [![](https://shields.io/badge/-Lightning--Hydra--Template-
-017F2F?style=flat&logo=github&labelColor=303030)](https://github.com/ashleve/
-lightning-hydra-template)
+via `github` ``` git clone https://github.com/marsggbo/hyperbox cd hyperbox pip
+install -r requirements.txt python setup.py develop ```   Quick Start ```
+python -m hyperbox.run experiment=example_random_nas +trainer.fast_dev_run=True
+```   Hyperbox Mutables (Searchable `nn.Module`) [image] - Code implementation
+for Figure (left) ```python import torch.nn as nn from hyperbox . mutables .
+spaces import OperationSpace op1 = nn.Conv2d(in_channels=3, out_channels=16,
+kernel_size=3, stride =1, padding=1) op2 = nn.Conv2d(in_channels=3,
+out_channels=16, kernel_size=5, stride =1, padding=2) op3 = nn.Conv2d
+(in_channels=3, out_channels=16, kernel_size=7, stride =1, padding=3) ops =
+OperationSpace(candidates=[op1, op2, op3], key=âconv_opâ, mask=[1, 0, 0])
+``` Code implementation for Figure (middle) ```python import torch from
+hyperbox.mutables.spaces import InputSpace in1 = torch.rand(2, 64) in2 =
+torch.rand(2, 32) in3 = torch.rand(2, 16) inputs = [in1, in2, in3] skipconnect
+= InputSpace(n_candidates=3, n_chosen=1, key=âscâ, mask=[0, 1, 0]) out =
+skipconnect([ in1 , in2 , in3 ]) assert out is in2 >>> True ``` - Code
+implementation for Figure (right) ```python from hyperbox.mutables.ops import
+Conv2d, Linear from hyperbox.mutables.spaces import ValueSpace # convolution ks
+= ValueSpace([3, 5, 7], key=âkernelSizeâ, mask=[0, 1, 0]) cout = ValueSpace
+([16, 32, 64], key=âchannelOutâ, mask=[0, 1, 0]) conv = Conv2d(3 , cout ,
+ks , stride =1, padding=2, bias=False ) print([x.shape for x in conv.parameters
+()]) >>> [torch.Size([32, 3, 5, 5])] # linear cout = ValueSpace([10, 100],
+key=âchannelOut1â) isBias = ValueSpace([0, 1], key=âbiasâ) # 0: False,
+1: True linear = Linear(10, cout , bias=isBias) print([x.shape for x in
+linear.parameters()]) >>> [ torch . Size ([100 , 10]) , torch . Size ([100]) ]
+```   Hyperbox Mutator (Search Algorithms) - Random Search Algorithm
+`RandomMutator` ```python from hyperbox.mutator import RandomMutator from
+hyperbox.networks.ofa import OFAMobileNetV3 net = OFAMobileNetV3() rm =
+RandomMutator(net) rm.reset() # search a subnet arch: dict = rm._cache # arch
+of a subnet print(arch) subnet = OFAMobileNetV3(mask=arch) # initialize a
+subnet, which has smaller parameters than `net` ``` the model arch is saved in
+`rm._cache`   Hyperbox Wikis - [Wiki for hyperbox.config](https://github.com/
+marsggbo/hyperbox/wiki/Customize-Config) - [Wiki for hyperbox.mutables](https:/
+/github.com/marsggbo/hyperbox/wiki/Customize-Mutable) - [Wiki for
+hyperbox.engine](https://github.com/marsggbo/hyperbox/wiki/Customize-Engine) -
+[Wiki for hyperbox.mutator](https://github.com/marsggbo/hyperbox/wiki/
+Customize-Mutator) - [Wiki for hyperbox.models](https://github.com/marsggbo/
+hyperbox/wiki/Customize-Models) - [Wiki for hyperbox.networks](https://
+github.com/marsggbo/hyperbox/wiki/Customize-NAS-Network) - [Wiki for Hydra]
+(https://github.com/marsggbo/hyperbox/wiki/Hydra-Q&A) - [Wiki for Hyperbox App]
+(https://github.com/marsggbo/hyperbox/wiki/Hyperbox-App:-Start-a-new-project) -
+[Miscellaneous](https://github.com/marsggbo/hyperbox/wiki/Miscellaneous-
+(tricks)) - [Q&A](https://github.com/marsggbo/hyperbox/wiki/Q&A) - [Usage]
+(https://github.com/marsggbo/hyperbox/wiki/Usages)  ## Thanks [![](https://
+shields.io/badge/-NNI-017F2F?style=flat&logo=github&labelColor=303030)](https:/
+/github.com/microsoft/nni/tree/v1.7) [![](https://shields.io/badge/-Lightning--
+Hydra--Template-017F2F?style=flat&logo=github&labelColor=303030)](https://
+github.com/ashleve/lightning-hydra-template)
```

### Comparing `hyperbox-1.4.2b0/hyperbox/callbacks/wandb_callbacks.py` & `hyperbox-1.4.3/hyperbox/callbacks/wandb_callbacks.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/callbacks/default.yaml` & `hyperbox-1.4.3/hyperbox/configs/callbacks/default.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/callbacks/wandb.yaml` & `hyperbox-1.4.3/hyperbox/configs/callbacks/wandb.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/config.yaml` & `hyperbox-1.4.3/hyperbox/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/experiment/example_bnnas.yaml` & `hyperbox-1.4.3/hyperbox/configs/experiment/example_bnnas.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/experiment/example_classify.yaml` & `hyperbox-1.4.3/hyperbox/configs/experiment/example_classify.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/experiment/example_darts_nas.yaml` & `hyperbox-1.4.3/hyperbox/configs/experiment/example_darts_nas.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/experiment/example_full.yaml` & `hyperbox-1.4.3/hyperbox/configs/experiment/example_full.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/experiment/example_nasbench.yaml` & `hyperbox-1.4.3/hyperbox/configs/experiment/example_nasbench.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/experiment/example_ofa_nas.yaml` & `hyperbox-1.4.3/hyperbox/configs/experiment/example_ofa_nas.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/experiment/example_random_nas.yaml` & `hyperbox-1.4.3/hyperbox/configs/experiment/example_random_nas.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/experiment/example_repnas.yaml` & `hyperbox-1.4.3/hyperbox/configs/experiment/example_repnas.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/experiment/example_simple.yaml` & `hyperbox-1.4.3/hyperbox/configs/experiment/example_simple.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/hparams_search/mnist_optuna.yaml` & `hyperbox-1.4.3/hyperbox/configs/hparams_search/mnist_optuna.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/hydra/default.yaml` & `hyperbox-1.4.3/hyperbox/configs/hydra/default.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/configs/paths/default.yaml` & `hyperbox-1.4.3/hyperbox/configs/paths/default.yaml`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/cifar_datamodule.py` & `hyperbox-1.4.3/hyperbox/datamodules/cifar_datamodule.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/distributed_sampler_wrapper.py` & `hyperbox-1.4.3/hyperbox/datamodules/distributed_sampler_wrapper.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/fakedata_datamodule.py` & `hyperbox-1.4.3/hyperbox/datamodules/fakedata_datamodule.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/imagenet_dali_datamodule.py` & `hyperbox-1.4.3/hyperbox/datamodules/imagenet_dali_datamodule.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/imagenet_datamodule.py` & `hyperbox-1.4.3/hyperbox/datamodules/imagenet_datamodule.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/medmnist_datamodule.py` & `hyperbox-1.4.3/hyperbox/datamodules/medmnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/mnist_datamodule.py` & `hyperbox-1.4.3/hyperbox/datamodules/mnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/transforms/__init__.py` & `hyperbox-1.4.3/hyperbox/datamodules/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/transforms/albumentation_transforms.py` & `hyperbox-1.4.3/hyperbox/datamodules/transforms/albumentation_transforms.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/transforms/autoaugment.py` & `hyperbox-1.4.3/hyperbox/datamodules/transforms/autoaugment.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/transforms/base_transforms.py` & `hyperbox-1.4.3/hyperbox/datamodules/transforms/base_transforms.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/transforms/custom_transforms.py` & `hyperbox-1.4.3/hyperbox/datamodules/transforms/custom_transforms.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/transforms/cutout.py` & `hyperbox-1.4.3/hyperbox/datamodules/transforms/cutout.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/datamodules/transforms/torch_transforms.py` & `hyperbox-1.4.3/hyperbox/datamodules/transforms/torch_transforms.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/losses/ce_labelsmooth_loss.py` & `hyperbox-1.4.3/hyperbox/losses/ce_labelsmooth_loss.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/losses/focal_loss.py` & `hyperbox-1.4.3/hyperbox/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/losses/kd_loss.py` & `hyperbox-1.4.3/hyperbox/losses/kd_loss.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/models/base_model.py` & `hyperbox-1.4.3/hyperbox/models/base_model.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/models/classify_model.py` & `hyperbox-1.4.3/hyperbox/models/classify_model.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/models/darts_model.py` & `hyperbox-1.4.3/hyperbox/models/darts_model.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/models/ea_model.py` & `hyperbox-1.4.3/hyperbox/models/ea_model.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/models/mnist_model.py` & `hyperbox-1.4.3/hyperbox/models/mnist_model.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/models/nasbench_model.py` & `hyperbox-1.4.3/hyperbox/models/nasbench_model.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/models/ofa_model.py` & `hyperbox-1.4.3/hyperbox/models/ofa_model.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/models/random_model.py` & `hyperbox-1.4.3/hyperbox/models/random_model.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/__init__.py` & `hyperbox-1.4.3/hyperbox/mutables/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/layers/layers2d.py` & `hyperbox-1.4.3/hyperbox/mutables/layers/layers2d.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,24 +56,15 @@
         prefix=None
     ):
         super(SELayer, self).__init__()
 
         self.reduction = SELayer.REDUCTION if reduction is None else reduction
 
         if isinstance(channel, ValueSpace):
-            num_mid = []
-            for c in channel.candidates:
-                num_mid.append(
-                    make_divisible(c // self.reduction, divisor=self.CHANNEL_DIVISIBLE)
-                )
-            if prefix is None:
-                key = channel.key + '_subSE_mc'
-            else:
-                key = prefix + '_subSE_mc'
-            num_mid = ValueSpace(num_mid, key=key)
+            num_mid = channel * self.reduction
         else:
             num_mid = make_divisible(channel // self.reduction, divisor=self.CHANNEL_DIVISIBLE)
 
         self.fc = nn.Sequential(OrderedDict([
             ('reduce', ops.Conv2d(channel, num_mid, 1, 1, 0, bias=True)),
             ('relu', nn.ReLU(inplace=True)),
             ('expand', ops.Conv2d(num_mid, channel, 1, 1, 0, bias=True)),
@@ -102,36 +93,27 @@
         prefix=None, # prefix for key of ValueSpace
     ):
         flag = isinstance(in_channels, ValueSpace) and isinstance(expand_ratio, ValueSpace)
         assert not flag, "in_channels and expand_ratio cannot both be ValueSpace"
         super(MBConvLayer, self).__init__()
 
         # build modules
-        if isinstance(in_channels, ValueSpace):
-            middle_channels = []
-            for c in in_channels.candidates:
-                middle_channels.append(
-                    make_divisible(round(c * self.expand_ratio), self.CHANNEL_DIVISIBLE)
-                )
-            if prefix is None:
-                key = in_channels.key + '_subMB_mc'
-            else:
-                key = prefix + '_subMB_mc'
-            middle_channels = ValueSpace(middle_channels, key=key)
-        elif isinstance(expand_ratio, ValueSpace):
-            middle_channels = []
-            for e in expand_ratio.candidates:
-                middle_channels.append(
-                    make_divisible(round(self.in_channels * e), self.CHANNEL_DIVISIBLE)
-                )
-            if prefix is None:
-                key = expand_ratio.key + '_subMB_mc'
-            else:
-                key = prefix + '_subMB_mc'
-            middle_channels = ValueSpace(middle_channels, key=key)
+        if isinstance(in_channels, ValueSpace) and not isinstance(expand_ratio, ValueSpace):
+            middle_channels = self.expand_ratio * in_channels
+        elif isinstance(expand_ratio, ValueSpace) and not isinstance(in_channels, ValueSpace):
+            middle_channels = expand_ratio * self.in_channels
+        # Todo: support in_channels and expand_ratio both be ValueSpace
+        # elif isinstance(in_channels, ValueSpace) and isinstance(expand_ratio, ValueSpace):
+        #     in_channels_candidates = in_channels.candidates_original
+        #     expand_ratio_candidates = expand_ratio.candidates_original
+        #     middle_channels_candidates = []
+        #     for i, c in enumerate(in_channels_candidates):
+        #         for j, r in enumerate(expand_ratio_candidates):
+        #             middle_channels_candidates.append(c * r)
+        #     middle_channels = ValueSpace(middle_channels_candidates, key=prefix + '_subMBConv_mc')  
         else:
             middle_channels = make_divisible(
                 round(self.in_channels * self.expand_ratio), self.CHANNEL_DIVISIBLE)
         if (isinstance(expand_ratio, ValueSpace) and expand_ratio.max_value==1) or self.expand_ratio== 1:
             self.inverted_bottleneck = None
         else:
             self.inverted_bottleneck = nn.Sequential(OrderedDict([
```

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/masker.py` & `hyperbox-1.4.3/hyperbox/mutables/masker.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/ops/base_module.py` & `hyperbox-1.4.3/hyperbox/mutables/ops/base_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         # The decorator @hparams_wrapper can automatically save all input arguments to
         # ``hparams`` attribute
         self.value_spaces = self.getValueSpaces(self.hparams)
 
     def getValueSpaces(self, kwargs):
         value_spaces = nn.ModuleDict()
         for key, value in kwargs.items():
+            if key in ['weight', 'bias']:
+                if hasattr(self, key): delattr(self, key)
+                key = '_' + key
             if isinstance(value, ValueSpace):
                 value_spaces[key] = value
                 if value.index is not None:
                     _v = value.candidates_original[value.index]
                 elif len(value.mask) != 0:
                     if isinstance(value.mask, torch.Tensor):
                         index = value.mask.clone().detach().cpu().numpy().argmax()
```

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/ops/batchnorm.py` & `hyperbox-1.4.3/hyperbox/mutables/ops/batchnorm.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/ops/conv.py` & `hyperbox-1.4.3/hyperbox/mutables/ops/conv.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,1040 +1,1197 @@
 00000000: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
 00000010: 706f 7274 2055 6e69 6f6e 2c20 4f70 7469  port Union, Opti
-00000020: 6f6e 616c 2c20 5365 740d 0a0d 0a69 6d70  onal, Set....imp
-00000030: 6f72 7420 746f 7263 680d 0a69 6d70 6f72  ort torch..impor
-00000040: 7420 746f 7263 682e 6e6e 2061 7320 6e6e  t torch.nn as nn
-00000050: 0d0a 696d 706f 7274 2074 6f72 6368 2e6e  ..import torch.n
-00000060: 6e2e 6675 6e63 7469 6f6e 616c 2061 7320  n.functional as 
-00000070: 460d 0a66 726f 6d20 746f 7263 682e 6e6e  F..from torch.nn
-00000080: 2e6d 6f64 756c 6573 2e63 6f6e 7620 696d  .modules.conv im
-00000090: 706f 7274 205f 436f 6e76 4e64 0d0a 6672  port _ConvNd..fr
-000000a0: 6f6d 2074 6f72 6368 2e6e 6e2e 636f 6d6d  om torch.nn.comm
-000000b0: 6f6e 5f74 7970 6573 2069 6d70 6f72 7420  on_types import 
-000000c0: 5f73 697a 655f 315f 742c 205f 7369 7a65  _size_1_t, _size
-000000d0: 5f32 5f74 2c20 5f73 697a 655f 335f 740d  _2_t, _size_3_t.
-000000e0: 0a66 726f 6d20 746f 7263 682e 6e6e 2e6d  .from torch.nn.m
-000000f0: 6f64 756c 6573 2e75 7469 6c73 2069 6d70  odules.utils imp
-00000100: 6f72 7420 5f73 696e 676c 652c 205f 7061  ort _single, _pa
-00000110: 6972 2c20 5f74 7269 706c 650d 0a66 726f  ir, _triple..fro
-00000120: 6d20 746f 7263 682e 6e6e 2e70 6172 616d  m torch.nn.param
-00000130: 6574 6572 2069 6d70 6f72 7420 5061 7261  eter import Para
-00000140: 6d65 7465 720d 0a0d 0a66 726f 6d20 6879  meter....from hy
-00000150: 7065 7262 6f78 2e6d 7574 6162 6c65 732e  perbox.mutables.
-00000160: 7370 6163 6573 2069 6d70 6f72 7420 5661  spaces import Va
-00000170: 6c75 6553 7061 6365 0d0a 6672 6f6d 2068  lueSpace..from h
-00000180: 7970 6572 626f 782e 6d75 7461 626c 6573  yperbox.mutables
-00000190: 2e6f 7073 2e62 6173 655f 6d6f 6475 6c65  .ops.base_module
-000001a0: 2069 6d70 6f72 7420 4669 6e65 6772 6169   import Finegrai
-000001b0: 6e65 644d 6f64 756c 650d 0a66 726f 6d20  nedModule..from 
-000001c0: 6879 7065 7262 6f78 2e6d 7574 6162 6c65  hyperbox.mutable
-000001d0: 732e 6f70 732e 7574 696c 7320 696d 706f  s.ops.utils impo
-000001e0: 7274 2073 7562 5f66 696c 7465 725f 7374  rt sub_filter_st
-000001f0: 6172 745f 656e 642c 2069 735f 7365 6172  art_end, is_sear
-00000200: 6368 6162 6c65 0d0a 0d0a 0d0a 5f5f 616c  chable......__al
-00000210: 6c5f 5f20 3d20 5b0d 0a20 2020 2027 4261  l__ = [..    'Ba
-00000220: 7365 436f 6e76 4e64 272c 0d0a 2020 2020  seConvNd',..    
-00000230: 2743 6f6e 7631 6427 2c0d 0a20 2020 2027  'Conv1d',..    '
-00000240: 436f 6e76 3264 272c 0d0a 2020 2020 2743  Conv2d',..    'C
-00000250: 6f6e 7633 6427 0d0a 5d0d 0a0d 0a0d 0a63  onv3d'..]......c
-00000260: 6c61 7373 2042 6173 6543 6f6e 764e 6428  lass BaseConvNd(
-00000270: 5f43 6f6e 764e 642c 2046 696e 6567 7261  _ConvNd, Finegra
-00000280: 696e 6564 4d6f 6475 6c65 293a 0d0a 2020  inedModule):..  
-00000290: 2020 4b45 524e 454c 5f54 5241 4e53 464f    KERNEL_TRANSFO
-000002a0: 524d 5f4d 4f44 4520 3d20 3120 2320 4e6f  RM_MODE = 1 # No
-000002b0: 6e65 206f 7220 3120 6f72 206f 7468 6572  ne or 1 or other
-000002c0: 2073 6574 7469 6e67 730d 0a0d 0a20 2020   settings....   
-000002d0: 2064 6566 205f 5f69 6e69 745f 5f28 0d0a   def __init__(..
-000002e0: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-000002f0: 2020 2020 2020 2069 6e5f 6368 616e 6e65         in_channe
-00000300: 6c73 3a20 696e 742c 0d0a 2020 2020 2020  ls: int,..      
-00000310: 2020 6f75 745f 6368 616e 6e65 6c73 3a20    out_channels: 
-00000320: 696e 742c 0d0a 2020 2020 2020 2020 6b65  int,..        ke
-00000330: 726e 656c 5f73 697a 653a 2055 6e69 6f6e  rnel_size: Union
-00000340: 5b69 6e74 2c20 7475 706c 652c 2056 616c  [int, tuple, Val
-00000350: 7565 5370 6163 655d 2c0d 0a20 2020 2020  ueSpace],..     
-00000360: 2020 2073 7472 6964 653a 2055 6e69 6f6e     stride: Union
-00000370: 5b69 6e74 2c20 7475 706c 652c 2056 616c  [int, tuple, Val
-00000380: 7565 5370 6163 655d 2c0d 0a20 2020 2020  ueSpace],..     
-00000390: 2020 2070 6164 6469 6e67 3a20 556e 696f     padding: Unio
-000003a0: 6e5b 7374 722c 2069 6e74 2c20 7475 706c  n[str, int, tupl
-000003b0: 652c 2056 616c 7565 5370 6163 655d 2c0d  e, ValueSpace],.
-000003c0: 0a20 2020 2020 2020 2064 696c 6174 696f  .        dilatio
-000003d0: 6e3a 2055 6e69 6f6e 5b69 6e74 2c20 7475  n: Union[int, tu
-000003e0: 706c 652c 2056 616c 7565 5370 6163 655d  ple, ValueSpace]
-000003f0: 2c0d 0a20 2020 2020 2020 2067 726f 7570  ,..        group
-00000400: 733a 2055 6e69 6f6e 5b69 6e74 2c20 7475  s: Union[int, tu
-00000410: 706c 652c 2056 616c 7565 5370 6163 655d  ple, ValueSpace]
-00000420: 2c0d 0a20 2020 2020 2020 2062 6961 733a  ,..        bias:
-00000430: 2062 6f6f 6c2c 0d0a 2020 2020 2020 2020   bool,..        
-00000440: 7061 6464 696e 675f 6d6f 6465 3a20 7374  padding_mode: st
-00000450: 7220 3d20 277a 6572 6f73 272c 0d0a 2020  r = 'zeros',..  
-00000460: 2020 2020 2020 6175 746f 5f70 6164 6469        auto_paddi
-00000470: 6e67 3a20 626f 6f6c 203d 2046 616c 7365  ng: bool = False
-00000480: 2c0d 0a20 2020 2020 2020 202a 6172 6773  ,..        *args
-00000490: 2c0d 0a20 2020 2020 2020 202a 2a6b 7761  ,..        **kwa
-000004a0: 7267 730d 0a20 2020 2029 3a0d 0a20 2020  rgs..    ):..   
-000004b0: 2020 2020 2027 2727 4261 7365 2043 6f6e       '''Base Con
-000004c0: 7620 4d6f 6475 6c65 0d0a 2020 2020 2020  v Module..      
-000004d0: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-000004e0: 2020 2020 2061 7574 6f5f 7061 6464 696e       auto_paddin
-000004f0: 673a 2069 6620 7365 7420 746f 2074 7275  g: if set to tru
-00000500: 652c 2077 696c 6c20 7365 7420 6120 7072  e, will set a pr
-00000510: 6f70 6572 2070 6164 6469 6e67 2073 697a  oper padding siz
-00000520: 6520 746f 206d 616b 6520 6f75 7470 7574  e to make output
-00000530: 2073 697a 6520 7361 6d65 2061 7320 7468   size same as th
-00000540: 6520 696e 7075 7420 7369 7a65 2e0d 0a20  e input size... 
-00000550: 2020 2020 2020 2020 2020 2020 2020 2046                 F
-00000560: 6f72 2065 7861 6d70 6c65 2c20 6966 206b  or example, if k
-00000570: 6572 6e65 6c20 7369 7a65 2069 7320 332c  ernel size is 3,
-00000580: 2074 6865 2070 6164 6469 6e67 2073 697a   the padding siz
-00000590: 6520 6973 2031 3b0d 0a20 2020 2020 2020  e is 1;..       
-000005a0: 2020 2020 2020 2020 2069 6620 6b65 726e           if kern
-000005b0: 656c 5f73 697a 6520 6973 2028 332c 3729  el_size is (3,7)
-000005c0: 2c20 7468 6520 7061 6464 696e 6720 7369  , the padding si
-000005d0: 7a65 2069 7320 2831 2c20 3329 0d0a 2020  ze is (1, 3)..  
-000005e0: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
-000005f0: 2020 2073 656c 662e 636f 6e76 5f64 696d     self.conv_dim
-00000600: 203d 2073 656c 662e 5f5f 636c 6173 735f   = self.__class_
-00000610: 5f2e 5f5f 6e61 6d65 5f5f 5b2d 323a 5d0d  _.__name__[-2:].
-00000620: 0a20 2020 2020 2020 2023 2066 6972 7374  .        # first
-00000630: 2069 6e69 7469 616c 697a 6520 6279 2046   initialize by F
-00000640: 696e 6567 7261 696e 6564 4d6f 6475 6c65  inegrainedModule
-00000650: 0d0a 2020 2020 2020 2020 4669 6e65 6772  ..        Finegr
-00000660: 6169 6e65 644d 6f64 756c 652e 5f5f 696e  ainedModule.__in
-00000670: 6974 5f5f 2873 656c 6629 0d0a 2020 2020  it__(self)..    
-00000680: 2020 2020 636f 6e76 5f6b 7761 7267 7320      conv_kwargs 
-00000690: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-000006a0: 206b 6579 3a20 6765 7461 7474 7228 7365   key: getattr(se
-000006b0: 6c66 2c20 6b65 792c 204e 6f6e 6529 2066  lf, key, None) f
-000006c0: 6f72 206b 6579 2069 6e20 5b0d 0a20 2020  or key in [..   
-000006d0: 2020 2020 2020 2020 2020 2020 2027 696e               'in
-000006e0: 5f63 6861 6e6e 656c 7327 2c20 276f 7574  _channels', 'out
-000006f0: 5f63 6861 6e6e 656c 7327 2c20 276b 6572  _channels', 'ker
-00000700: 6e65 6c5f 7369 7a65 272c 0d0a 2020 2020  nel_size',..    
-00000710: 2020 2020 2020 2020 2020 2020 2773 7472              'str
-00000720: 6964 6527 2c20 2770 6164 6469 6e67 272c  ide', 'padding',
-00000730: 2027 6469 6c61 7469 6f6e 272c 2027 6772   'dilation', 'gr
-00000740: 6f75 7073 272c 2027 6269 6173 270d 0a20  oups', 'bias'.. 
-00000750: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00000760: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
-00000770: 2020 2020 2073 656c 662e 696e 6974 5f6f       self.init_o
-00000780: 7073 282a 2a63 6f6e 765f 6b77 6172 6773  ps(**conv_kwargs
-00000790: 290d 0a20 2020 2020 2020 2023 2074 6865  )..        # the
-000007a0: 6e20 696e 6974 6961 6c69 7a65 6420 6279  n initialized by
-000007b0: 205f 436f 6e76 4e64 0d0a 2020 2020 2020   _ConvNd..      
-000007c0: 2020 5f43 6f6e 764e 642e 5f5f 696e 6974    _ConvNd.__init
-000007d0: 5f5f 280d 0a20 2020 2020 2020 2020 2020  __(..           
-000007e0: 2073 656c 662c 2073 656c 662e 696e 5f63   self, self.in_c
-000007f0: 6861 6e6e 656c 732c 2073 656c 662e 6f75  hannels, self.ou
-00000800: 745f 6368 616e 6e65 6c73 2c20 7365 6c66  t_channels, self
-00000810: 2e6b 6572 6e65 6c5f 7369 7a65 2c20 7365  .kernel_size, se
-00000820: 6c66 2e73 7472 6964 652c 2073 656c 662e  lf.stride, self.
-00000830: 7061 6464 696e 672c 0d0a 2020 2020 2020  padding,..      
-00000840: 2020 2020 2020 7365 6c66 2e64 696c 6174        self.dilat
-00000850: 696f 6e2c 2046 616c 7365 2c20 7365 6c66  ion, False, self
-00000860: 2e6f 7574 7075 745f 7061 6464 696e 672c  .output_padding,
-00000870: 2073 656c 662e 6772 6f75 7073 2c20 5472   self.groups, Tr
-00000880: 7565 2c20 7365 6c66 2e70 6164 6469 6e67  ue, self.padding
-00000890: 5f6d 6f64 6529 0d0a 2020 2020 2020 2020  _mode)..        
-000008a0: 6966 206e 6f74 2062 6961 733a 0d0a 2020  if not bias:..  
-000008b0: 2020 2020 2020 2020 2020 6465 6c20 7365            del se
-000008c0: 6c66 2e62 6961 730d 0a20 2020 2020 2020  lf.bias..       
-000008d0: 2020 2020 2073 656c 662e 7265 6769 7374       self.regist
-000008e0: 6572 5f70 6172 616d 6574 6572 2827 6269  er_parameter('bi
-000008f0: 6173 272c 204e 6f6e 6529 0d0a 2020 2020  as', None)..    
-00000900: 2020 2020 7365 6c66 2e69 735f 7365 6172      self.is_sear
-00000910: 6368 203d 2073 656c 662e 6973 5365 6172  ch = self.isSear
-00000920: 6368 436f 6e76 2829 0d0a 0d0a 2020 2020  chConv()....    
-00000930: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00000940: 6528 6b65 726e 656c 5f73 697a 652c 2056  e(kernel_size, V
-00000950: 616c 7565 5370 6163 6529 2061 6e64 205c  alueSpace) and \
-00000960: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000970: 6c66 2e4b 4552 4e45 4c5f 5452 414e 5346  lf.KERNEL_TRANSF
-00000980: 4f52 4d5f 4d4f 4445 2069 7320 6e6f 7420  ORM_MODE is not 
-00000990: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-000009a0: 2020 2023 2072 6567 6973 7465 7220 7363     # register sc
-000009b0: 616c 696e 6720 7061 7261 6d65 7465 7273  aling parameters
-000009c0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000009d0: 3774 6f35 5f6d 6174 7269 782c 2035 746f  7to5_matrix, 5to
-000009e0: 335f 6d61 7472 6978 0d0a 2020 2020 2020  3_matrix..      
-000009f0: 2020 2020 2020 7363 616c 655f 7061 7261        scale_para
-00000a00: 6d73 203d 207b 7d0d 0a20 2020 2020 2020  ms = {}..       
-00000a10: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00000a20: 6e67 6528 6c65 6e28 6b65 726e 656c 5f73  nge(len(kernel_s
-00000a30: 697a 6529 202d 2031 293a 0d0a 2020 2020  ize) - 1):..    
-00000a40: 2020 2020 2020 2020 2020 2020 6b73 5f73              ks_s
-00000a50: 6d61 6c6c 203d 206b 6572 6e65 6c5f 7369  mall = kernel_si
-00000a60: 7a65 5b69 5d0d 0a20 2020 2020 2020 2020  ze[i]..         
-00000a70: 2020 2020 2020 206b 735f 6c61 7267 6572         ks_larger
-00000a80: 203d 206b 6572 6e65 6c5f 7369 7a65 5b69   = kernel_size[i
-00000a90: 202b 2031 5d0d 0a20 2020 2020 2020 2020   + 1]..         
-00000aa0: 2020 2020 2020 2070 6172 616d 5f6e 616d         param_nam
-00000ab0: 6520 3d20 2725 6474 6f25 6427 2025 2028  e = '%dto%d' % (
-00000ac0: 6b73 5f6c 6172 6765 722c 206b 735f 736d  ks_larger, ks_sm
-00000ad0: 616c 6c29 0d0a 2020 2020 2020 2020 2020  all)..          
-00000ae0: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-00000af0: 7469 6f6e 2050 7941 7267 756d 656e 744c  tion PyArgumentL
-00000b00: 6973 740d 0a20 2020 2020 2020 2020 2020  ist..           
-00000b10: 2020 2020 2073 6361 6c65 5f70 6172 616d       scale_param
-00000b20: 735b 2725 735f 6d61 7472 6978 2720 2520  s['%s_matrix' % 
-00000b30: 7061 7261 6d5f 6e61 6d65 5d20 3d20 5061  param_name] = Pa
-00000b40: 7261 6d65 7465 7228 746f 7263 682e 6579  rameter(torch.ey
-00000b50: 6528 6b73 5f73 6d61 6c6c 202a 2a20 3229  e(ks_small ** 2)
-00000b60: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00000b70: 6f72 206e 616d 652c 2070 6172 616d 2069  or name, param i
-00000b80: 6e20 7363 616c 655f 7061 7261 6d73 2e69  n scale_params.i
-00000b90: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00000ba0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00000bb0: 6769 7374 6572 5f70 6172 616d 6574 6572  gister_parameter
-00000bc0: 286e 616d 652c 2070 6172 616d 290d 0a0d  (name, param)...
-00000bd0: 0a20 2020 2064 6566 2069 6e69 745f 6f70  .    def init_op
-00000be0: 7328 7365 6c66 2c20 2a61 7267 732c 202a  s(self, *args, *
-00000bf0: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
-00000c00: 2020 2027 2727 4765 6e65 7261 7465 2043     '''Generate C
-00000c10: 6f6e 7620 6f70 6572 6174 696f 6e27 2727  onv operation'''
-00000c20: 0d0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
-00000c30: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-00000c40: 726f 720d 0a0d 0a20 2020 2064 6566 2069  ror....    def i
-00000c50: 7353 6561 7263 6843 6f6e 7628 7365 6c66  sSearchConv(self
-00000c60: 293a 0d0a 2020 2020 2020 2020 2727 2753  ):..        '''S
-00000c70: 6561 7263 6820 666c 6167 0d0a 2020 2020  earch flag..    
-00000c80: 2020 2020 5375 7070 6f72 7465 6420 6172      Supported ar
-00000c90: 6775 6d65 6e74 730d 0a20 2020 2020 2020  guments..       
-00000ca0: 2020 2020 202d 2073 6561 7263 685f 696e       - search_in
-00000cb0: 5f63 6861 6e6e 656c 0d0a 2020 2020 2020  _channel..      
-00000cc0: 2020 2020 2020 2d20 7365 6172 6368 5f6f        - search_o
-00000cd0: 7574 5f63 6861 6e6e 656c 0d0a 2020 2020  ut_channel..    
-00000ce0: 2020 2020 2020 2020 2d20 7365 6172 6368          - search
-00000cf0: 5f6b 6572 6e65 6c5f 7369 7a65 0d0a 2020  _kernel_size..  
-00000d00: 2020 2020 2020 2020 2020 2d20 7365 6172            - sear
-00000d10: 6368 5f73 7472 6964 650d 0a20 2020 2020  ch_stride..     
-00000d20: 2020 2020 2020 202d 2073 6561 7263 685f         - search_
-00000d30: 6469 6c61 7469 6f6e 0d0a 2020 2020 2020  dilation..      
-00000d40: 2020 2020 2020 2d20 7365 6172 6368 5f67        - search_g
-00000d50: 726f 7570 730d 0a20 2020 2020 2020 2027  roups..        '
-00000d60: 2727 0d0a 2020 2020 2020 2020 7365 6c66  ''..        self
-00000d70: 2e73 6561 7263 685f 696e 5f63 6861 6e6e  .search_in_chann
-00000d80: 656c 203d 2046 616c 7365 0d0a 2020 2020  el = False..    
-00000d90: 2020 2020 7365 6c66 2e73 6561 7263 685f      self.search_
-00000da0: 6f75 745f 6368 616e 6e65 6c20 3d20 4661  out_channel = Fa
-00000db0: 6c73 650d 0a20 2020 2020 2020 2073 656c  lse..        sel
-00000dc0: 662e 7365 6172 6368 5f6b 6572 6e65 6c5f  f.search_kernel_
-00000dd0: 7369 7a65 203d 2046 616c 7365 0d0a 2020  size = False..  
-00000de0: 2020 2020 2020 7365 6c66 2e73 6561 7263        self.searc
-00000df0: 685f 7374 7269 6465 203d 2046 616c 7365  h_stride = False
-00000e00: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00000e10: 6561 7263 685f 6469 6c61 7469 6f6e 203d  earch_dilation =
-00000e20: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00000e30: 7365 6c66 2e73 6561 7263 685f 6772 6f75  self.search_grou
-00000e40: 7073 203d 2046 616c 7365 0d0a 2020 2020  ps = False..    
-00000e50: 2020 2020 2320 7365 6c66 2e73 6561 7263      # self.searc
-00000e60: 685f 6269 6173 203d 2046 616c 7365 0d0a  h_bias = False..
-00000e70: 0d0a 2020 2020 2020 2020 6966 2061 6c6c  ..        if all
-00000e80: 285b 6e6f 7420 7673 2e69 735f 7365 6172  ([not vs.is_sear
-00000e90: 6368 2066 6f72 2076 7320 696e 2073 656c  ch for vs in sel
-00000ea0: 662e 7661 6c75 655f 7370 6163 6573 2e76  f.value_spaces.v
-00000eb0: 616c 7565 7328 295d 293a 0d0a 2020 2020  alues()]):..    
-00000ec0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00000ed0: 616c 7365 0d0a 0d0a 2020 2020 2020 2020  alse....        
-00000ee0: 6966 2020 6973 5f73 6561 7263 6861 626c  if  is_searchabl
-00000ef0: 6528 6765 7461 7474 7228 7365 6c66 2e76  e(getattr(self.v
-00000f00: 616c 7565 5f73 7061 6365 732c 2027 696e  alue_spaces, 'in
-00000f10: 5f63 6861 6e6e 656c 7327 2c20 4e6f 6e65  _channels', None
-00000f20: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00000f30: 2073 656c 662e 7365 6172 6368 5f69 6e5f   self.search_in_
-00000f40: 6368 616e 6e65 6c20 3d20 5472 7565 0d0a  channel = True..
-00000f50: 2020 2020 2020 2020 6966 2020 6973 5f73          if  is_s
-00000f60: 6561 7263 6861 626c 6528 6765 7461 7474  earchable(getatt
-00000f70: 7228 7365 6c66 2e76 616c 7565 5f73 7061  r(self.value_spa
-00000f80: 6365 732c 2027 6f75 745f 6368 616e 6e65  ces, 'out_channe
-00000f90: 6c73 272c 204e 6f6e 6529 293a 0d0a 2020  ls', None)):..  
-00000fa0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00000fb0: 6561 7263 685f 6f75 745f 6368 616e 6e65  earch_out_channe
-00000fc0: 6c20 3d20 5472 7565 0d0a 2020 2020 2020  l = True..      
-00000fd0: 2020 6966 2020 6973 5f73 6561 7263 6861    if  is_searcha
-00000fe0: 626c 6528 6765 7461 7474 7228 7365 6c66  ble(getattr(self
-00000ff0: 2e76 616c 7565 5f73 7061 6365 732c 2027  .value_spaces, '
-00001000: 6b65 726e 656c 5f73 697a 6527 2c20 4e6f  kernel_size', No
-00001010: 6e65 2929 3a0d 0a20 2020 2020 2020 2020  ne)):..         
-00001020: 2020 206b 6572 6e65 6c5f 6361 6e64 6964     kernel_candid
-00001030: 6174 6573 203d 2073 656c 662e 7661 6c75  ates = self.valu
-00001040: 655f 7370 6163 6573 5b27 6b65 726e 656c  e_spaces['kernel
-00001050: 5f73 697a 6527 5d2e 6361 6e64 6964 6174  _size'].candidat
-00001060: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
-00001070: 6d61 785f 6b20 3d20 7365 6c66 2e6b 6572  max_k = self.ker
-00001080: 6e65 6c5f 7369 7a65 0d0a 2020 2020 2020  nel_size..      
-00001090: 2020 2020 2020 2320 546f 646f 3a20 e4b8        # Todo: ..
-000010a0: 8e60 7472 616e 7366 6f72 6d5f 6b65 726e  .`transform_kern
-000010b0: 656c 5f73 697a 6560 e690 ade9 858d e4bd  el_size`........
-000010c0: bfe7 94a8 efbc 8ce7 9bae e589 8de6 9caa  ................
-000010d0: e4bd bfe7 94a8 0d0a 2020 2020 2020 2020  ........        
-000010e0: 2020 2020 7365 6c66 2e73 6561 7263 685f      self.search_
-000010f0: 6b65 726e 656c 5f73 697a 6520 3d20 5472  kernel_size = Tr
-00001100: 7565 0d0a 2020 2020 2020 2020 6966 2020  ue..        if  
-00001110: 6973 5f73 6561 7263 6861 626c 6528 6765  is_searchable(ge
-00001120: 7461 7474 7228 7365 6c66 2e76 616c 7565  tattr(self.value
-00001130: 5f73 7061 6365 732c 2027 7374 7269 6465  _spaces, 'stride
-00001140: 272c 204e 6f6e 6529 293a 0d0a 2020 2020  ', None)):..    
-00001150: 2020 2020 2020 2020 7365 6c66 2e73 6561          self.sea
-00001160: 7263 685f 7374 7269 6465 203d 2054 7275  rch_stride = Tru
-00001170: 650d 0a20 2020 2020 2020 2069 6620 2069  e..        if  i
-00001180: 735f 7365 6172 6368 6162 6c65 2867 6574  s_searchable(get
-00001190: 6174 7472 2873 656c 662e 7661 6c75 655f  attr(self.value_
-000011a0: 7370 6163 6573 2c20 2764 696c 6174 696f  spaces, 'dilatio
-000011b0: 6e27 2c20 4e6f 6e65 2929 3a0d 0a20 2020  n', None)):..   
-000011c0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000011d0: 6172 6368 5f64 696c 6174 696f 6e20 3d20  arch_dilation = 
-000011e0: 5472 7565 0d0a 2020 2020 2020 2020 6966  True..        if
-000011f0: 2020 6973 5f73 6561 7263 6861 626c 6528    is_searchable(
-00001200: 6765 7461 7474 7228 7365 6c66 2e76 616c  getattr(self.val
-00001210: 7565 5f73 7061 6365 732c 2027 6772 6f75  ue_spaces, 'grou
-00001220: 7073 272c 204e 6f6e 6529 293a 0d0a 2020  ps', None)):..  
-00001230: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00001240: 6561 7263 685f 6772 6f75 7073 203d 2054  earch_groups = T
-00001250: 7275 650d 0a20 2020 2020 2020 2023 2069  rue..        # i
-00001260: 6620 2069 735f 7365 6172 6368 6162 6c65  f  is_searchable
-00001270: 2867 6574 6174 7472 2873 656c 662e 7661  (getattr(self.va
-00001280: 6c75 655f 7370 6163 6573 2c20 2762 6961  lue_spaces, 'bia
-00001290: 7327 2c20 4e6f 6e65 2929 3a0d 0a20 2020  s', None)):..   
-000012a0: 2020 2020 2023 2020 2020 2073 656c 662e       #     self.
-000012b0: 7365 6172 6368 5f62 6961 7320 3d20 5472  search_bias = Tr
-000012c0: 7565 0d0a 0d0a 2020 2020 2020 2020 7265  ue....        re
-000012d0: 7475 726e 2054 7275 650d 0a0d 0a20 2020  turn True....   
-000012e0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-000012f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001300: 2323 2323 2323 2323 2323 2323 0d0a 2020  ############..  
-00001310: 2020 2320 666f 7277 6172 6420 696d 706c    # forward impl
-00001320: 656d 656e 7461 7469 6f6e 0d0a 2020 2020  ementation..    
-00001330: 2320 2d20 666f 7277 6172 645f 636f 6e76  # - forward_conv
-00001340: 0d0a 2020 2020 2320 2020 2d20 7472 616e  ..    #   - tran
-00001350: 7366 6f72 6d5f 6b65 726e 656c 5f73 697a  sform_kernel_siz
-00001360: 650d 0a20 2020 2023 2323 2323 2323 2323  e..    #########
-00001370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001390: 2323 0d0a 0d0a 2020 2020 6465 6620 666f  ##....    def fo
-000013a0: 7277 6172 6428 7365 6c66 2c20 7829 3a0d  rward(self, x):.
-000013b0: 0a20 2020 2020 2020 206f 7574 203d 204e  .        out = N
-000013c0: 6f6e 650d 0a20 2020 2020 2020 2069 6620  one..        if 
-000013d0: 6e6f 7420 7365 6c66 2e69 735f 7365 6172  not self.is_sear
-000013e0: 6368 3a0d 0a20 2020 2020 2020 2020 2020  ch:..           
-000013f0: 2070 6164 6469 6e67 203d 2073 656c 662e   padding = self.
-00001400: 7061 6464 696e 670d 0a20 2020 2020 2020  padding..       
-00001410: 2020 2020 2069 6620 7365 6c66 2e61 7574       if self.aut
-00001420: 6f5f 7061 6464 696e 673a 0d0a 2020 2020  o_padding:..    
-00001430: 2020 2020 2020 2020 2020 2020 6b65 726e              kern
-00001440: 656c 5f73 697a 6520 3d20 7365 6c66 2e77  el_size = self.w
-00001450: 6569 6768 742e 7368 6170 655b 323a 5d0d  eight.shape[2:].
-00001460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001470: 2070 6164 6469 6e67 203d 205b 5d0d 0a20   padding = [].. 
-00001480: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00001490: 6f72 206b 2069 6e20 6b65 726e 656c 5f73  or k in kernel_s
-000014a0: 697a 653a 0d0a 2020 2020 2020 2020 2020  ize:..          
-000014b0: 2020 2020 2020 2020 2020 7061 6464 696e            paddin
-000014c0: 672e 6170 7065 6e64 286b 2f2f 3229 0d0a  g.append(k//2)..
-000014d0: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
-000014e0: 3d20 7365 6c66 2e63 6f6e 7628 782c 2073  = self.conv(x, s
-000014f0: 656c 662e 7765 6967 6874 2c20 7365 6c66  elf.weight, self
-00001500: 2e62 6961 732c 2073 656c 662e 7374 7269  .bias, self.stri
-00001510: 6465 2c0d 0a20 2020 2020 2020 2020 2020  de,..           
-00001520: 2020 2020 2070 6164 6469 6e67 2c20 7365       padding, se
-00001530: 6c66 2e64 696c 6174 696f 6e2c 2073 656c  lf.dilation, sel
-00001540: 662e 6772 6f75 7073 290d 0a20 2020 2020  f.groups)..     
-00001550: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00001560: 2020 2020 2020 6f75 7420 3d20 7365 6c66        out = self
-00001570: 2e66 6f72 7761 7264 5f63 6f6e 7628 7829  .forward_conv(x)
-00001580: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001590: 206f 7574 0d0a 0d0a 2020 2020 6465 6620   out....    def 
-000015a0: 666f 7277 6172 645f 636f 6e76 2873 656c  forward_conv(sel
-000015b0: 662c 2078 293a 0d0a 2020 2020 2020 2020  f, x):..        
-000015c0: 6669 6c74 6572 7320 3d20 7365 6c66 2e77  filters = self.w
-000015d0: 6569 6768 742e 636f 6e74 6967 756f 7573  eight.contiguous
-000015e0: 2829 0d0a 2020 2020 2020 2020 6269 6173  ()..        bias
-000015f0: 203d 2073 656c 662e 6269 6173 0d0a 2020   = self.bias..  
-00001600: 2020 2020 2020 696e 5f63 6861 6e6e 656c        in_channel
-00001610: 7320 3d20 7365 6c66 2e69 6e5f 6368 616e  s = self.in_chan
-00001620: 6e65 6c73 0d0a 2020 2020 2020 2020 6f75  nels..        ou
-00001630: 745f 6368 616e 6e65 6c73 203d 2073 656c  t_channels = sel
-00001640: 662e 6f75 745f 6368 616e 6e65 6c73 0d0a  f.out_channels..
-00001650: 2020 2020 2020 2020 7374 7269 6465 203d          stride =
-00001660: 2073 656c 662e 7661 6c75 655f 7370 6163   self.value_spac
-00001670: 6573 5b27 7374 7269 6465 275d 2e76 616c  es['stride'].val
-00001680: 7565 2069 6620 7365 6c66 2e73 6561 7263  ue if self.searc
-00001690: 685f 7374 7269 6465 2065 6c73 6520 7365  h_stride else se
-000016a0: 6c66 2e73 7472 6964 650d 0a20 2020 2020  lf.stride..     
-000016b0: 2020 2067 726f 7570 7320 3d20 7365 6c66     groups = self
-000016c0: 2e76 616c 7565 5f73 7061 6365 735b 2767  .value_spaces['g
-000016d0: 726f 7570 7327 5d2e 7661 6c75 6520 6966  roups'].value if
-000016e0: 2073 656c 662e 7365 6172 6368 5f67 726f   self.search_gro
-000016f0: 7570 7320 656c 7365 2073 656c 662e 6772  ups else self.gr
-00001700: 6f75 7073 0d0a 2020 2020 2020 2020 6469  oups..        di
-00001710: 6c61 7469 6f6e 203d 2073 656c 662e 7661  lation = self.va
-00001720: 6c75 655f 7370 6163 6573 5b27 6469 6c61  lue_spaces['dila
-00001730: 7469 6f6e 275d 2e76 616c 7565 2069 6620  tion'].value if 
-00001740: 7365 6c66 2e73 6561 7263 685f 6469 6c61  self.search_dila
-00001750: 7469 6f6e 2065 6c73 6520 7365 6c66 2e64  tion else self.d
-00001760: 696c 6174 696f 6e0d 0a20 2020 2020 2020  ilation..       
-00001770: 2070 6164 6469 6e67 203d 2073 656c 662e   padding = self.
-00001780: 7061 6464 696e 670d 0a0d 0a20 2020 2020  padding....     
-00001790: 2020 2069 6620 7365 6c66 2e73 6561 7263     if self.searc
-000017a0: 685f 696e 5f63 6861 6e6e 656c 3a0d 0a20  h_in_channel:.. 
-000017b0: 2020 2020 2020 2020 2020 2069 6e5f 6368             in_ch
-000017c0: 616e 6e65 6c73 203d 2073 656c 662e 7661  annels = self.va
-000017d0: 6c75 655f 7370 6163 6573 5b27 696e 5f63  lue_spaces['in_c
-000017e0: 6861 6e6e 656c 7327 5d2e 7661 6c75 650d  hannels'].value.
-000017f0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-00001800: 7465 7273 203d 2066 696c 7465 7273 5b3a  ters = filters[:
-00001810: 2c20 3a69 6e5f 6368 616e 6e65 6c73 2c20  , :in_channels, 
-00001820: 2e2e 2e5d 0d0a 2020 2020 2020 2020 6966  ...]..        if
-00001830: 2073 656c 662e 7365 6172 6368 5f6f 7574   self.search_out
-00001840: 5f63 6861 6e6e 656c 3a0d 0a20 2020 2020  _channel:..     
-00001850: 2020 2020 2020 206f 7574 5f63 6861 6e6e         out_chann
-00001860: 656c 7320 3d20 7365 6c66 2e76 616c 7565  els = self.value
-00001870: 5f73 7061 6365 735b 276f 7574 5f63 6861  _spaces['out_cha
-00001880: 6e6e 656c 7327 5d2e 7661 6c75 650d 0a20  nnels'].value.. 
-00001890: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000018a0: 6c66 2e62 6961 7320 6973 206e 6f74 204e  lf.bias is not N
-000018b0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000018c0: 2020 2020 2020 6269 6173 203d 2062 6961        bias = bia
-000018d0: 735b 3a6f 7574 5f63 6861 6e6e 656c 735d  s[:out_channels]
-000018e0: 0d0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
-000018f0: 6c74 6572 7320 3d20 6669 6c74 6572 735b  lters = filters[
-00001900: 3a6f 7574 5f63 6861 6e6e 656c 732c 202e  :out_channels, .
-00001910: 2e2e 5d0d 0a20 2020 2020 2020 2069 6620  ..]..        if 
-00001920: 7365 6c66 2e73 6561 7263 685f 6b65 726e  self.search_kern
-00001930: 656c 5f73 697a 653a 0d0a 2020 2020 2020  el_size:..      
-00001940: 2020 2020 2020 6669 6c74 6572 7320 3d20        filters = 
-00001950: 7365 6c66 2e74 7261 6e73 666f 726d 5f6b  self.transform_k
-00001960: 6572 6e65 6c5f 7369 7a65 2866 696c 7465  ernel_size(filte
-00001970: 7273 290d 0a20 2020 2020 2020 2069 6620  rs)..        if 
-00001980: 7365 6c66 2e73 6561 7263 685f 6772 6f75  self.search_grou
-00001990: 7073 3a0d 0a20 2020 2020 2020 2020 2020  ps:..           
-000019a0: 2066 696c 7465 7273 203d 2073 656c 662e   filters = self.
-000019b0: 6765 745f 6669 6c74 6572 735f 6279 5f67  get_filters_by_g
-000019c0: 726f 7570 7328 6669 6c74 6572 732c 2069  roups(filters, i
-000019d0: 6e5f 6368 616e 6e65 6c73 2c20 6772 6f75  n_channels, grou
-000019e0: 7073 292e 636f 6e74 6967 756f 7573 2829  ps).contiguous()
-000019f0: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00001a00: 662e 6175 746f 5f70 6164 6469 6e67 3a0d  f.auto_padding:.
-00001a10: 0a20 2020 2020 2020 2020 2020 206b 6572  .            ker
-00001a20: 6e65 6c5f 7369 7a65 203d 2066 696c 7465  nel_size = filte
-00001a30: 7273 2e73 6861 7065 5b32 3a5d 0d0a 2020  rs.shape[2:]..  
-00001a40: 2020 2020 2020 2020 2020 7061 6464 696e            paddin
-00001a50: 6720 3d20 5b5d 0d0a 2020 2020 2020 2020  g = []..        
-00001a60: 2020 2020 666f 7220 6b20 696e 206b 6572      for k in ker
-00001a70: 6e65 6c5f 7369 7a65 3a0d 0a20 2020 2020  nel_size:..     
-00001a80: 2020 2020 2020 2020 2020 2070 6164 6469             paddi
-00001a90: 6e67 2e61 7070 656e 6428 6b2f 2f32 290d  ng.append(k//2).
-00001aa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001ab0: 7365 6c66 2e63 6f6e 7628 782c 2066 696c  self.conv(x, fil
-00001ac0: 7465 7273 2c20 6269 6173 2c20 7374 7269  ters, bias, stri
-00001ad0: 6465 2c20 7061 6464 696e 672c 2064 696c  de, padding, dil
-00001ae0: 6174 696f 6e2c 2067 726f 7570 7329 0d0a  ation, groups)..
-00001af0: 0d0a 2020 2020 6465 6620 6765 745f 6669  ..    def get_fi
-00001b00: 6c74 6572 735f 6279 5f67 726f 7570 7328  lters_by_groups(
-00001b10: 7365 6c66 2c20 6669 6c74 6572 732c 2069  self, filters, i
-00001b20: 6e5f 6368 616e 6e65 6c73 2c20 6772 6f75  n_channels, grou
-00001b30: 7073 293a 0d0a 2020 2020 2020 2020 2727  ps):..        ''
-00001b40: 2747 6574 2066 696c 7465 7273 2077 6865  'Get filters whe
-00001b50: 6e20 7365 6172 6368 696e 6720 666f 7220  n searching for 
-00001b60: 236f 6620 6772 6f75 7073 2727 270d 0a20  #of groups'''.. 
-00001b70: 2020 2020 2020 2073 7562 5f66 696c 7465         sub_filte
-00001b80: 7273 203d 2074 6f72 6368 2e63 6875 6e6b  rs = torch.chunk
-00001b90: 2866 696c 7465 7273 2c20 6772 6f75 7073  (filters, groups
-00001ba0: 2c20 6469 6d3d 3029 0d0a 2020 2020 2020  , dim=0)..      
-00001bb0: 2020 7375 625f 696e 5f63 6861 6e6e 656c    sub_in_channel
-00001bc0: 7320 3d20 696e 5f63 6861 6e6e 656c 7320  s = in_channels 
-00001bd0: 2f2f 2067 726f 7570 730d 0a20 2020 2020  // groups..     
-00001be0: 2020 2073 7562 5f72 6174 696f 203d 2066     sub_ratio = f
-00001bf0: 696c 7465 7273 2e73 697a 6528 3129 202f  ilters.size(1) /
-00001c00: 2f20 7375 625f 696e 5f63 6861 6e6e 656c  / sub_in_channel
-00001c10: 730d 0a0d 0a20 2020 2020 2020 2066 696c  s....        fil
-00001c20: 7465 725f 6372 6f70 7320 3d20 5b5d 0d0a  ter_crops = []..
-00001c30: 2020 2020 2020 2020 666f 7220 692c 2073          for i, s
-00001c40: 7562 5f66 696c 7465 7220 696e 2065 6e75  ub_filter in enu
-00001c50: 6d65 7261 7465 2873 7562 5f66 696c 7465  merate(sub_filte
-00001c60: 7273 293a 0d0a 2020 2020 2020 2020 2020  rs):..          
-00001c70: 2020 7061 7274 5f69 6420 3d20 6920 2520    part_id = i % 
-00001c80: 7375 625f 7261 7469 6f0d 0a20 2020 2020  sub_ratio..     
-00001c90: 2020 2020 2020 2073 7461 7274 203d 2070         start = p
-00001ca0: 6172 745f 6964 202a 2073 7562 5f69 6e5f  art_id * sub_in_
-00001cb0: 6368 616e 6e65 6c73 0d0a 2020 2020 2020  channels..      
-00001cc0: 2020 2020 2020 6669 6c74 6572 5f63 726f        filter_cro
-00001cd0: 7073 2e61 7070 656e 6428 7375 625f 6669  ps.append(sub_fi
-00001ce0: 6c74 6572 5b3a 2c20 7374 6172 743a 7374  lter[:, start:st
-00001cf0: 6172 7420 2b20 7375 625f 696e 5f63 6861  art + sub_in_cha
-00001d00: 6e6e 656c 732c 203a 2c20 3a5d 290d 0a20  nnels, :, :]).. 
-00001d10: 2020 2020 2020 2066 696c 7465 7273 203d         filters =
-00001d20: 2074 6f72 6368 2e63 6174 2866 696c 7465   torch.cat(filte
-00001d30: 725f 6372 6f70 732c 2064 696d 3d30 290d  r_crops, dim=0).
-00001d40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001d50: 6669 6c74 6572 730d 0a0d 0a20 2020 2064  filters....    d
-00001d60: 6566 2074 7261 6e73 666f 726d 5f6b 6572  ef transform_ker
-00001d70: 6e65 6c5f 7369 7a65 2873 656c 662c 2066  nel_size(self, f
-00001d80: 696c 7465 7273 293a 0d0a 2020 2020 2020  ilters):..      
-00001d90: 2020 2320 546f 646f 3a20 7375 7070 6f72    # Todo: suppor
-00001da0: 7420 6469 6666 6572 656e 7420 7479 7065  t different type
-00001db0: 7320 6f66 206b 6572 6e65 6c20 7369 7a65  s of kernel size
-00001dc0: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
-00001dd0: 6d65 7468 6f64 7320 6279 2060 7472 616e  methods by `tran
-00001de0: 7366 6f72 6d5f 6b65 726e 656c 5f73 697a  sform_kernel_siz
-00001df0: 6560 2066 756e 6374 696f 6e0d 0a20 2020  e` function..   
-00001e00: 2020 2020 2073 7562 5f6b 6572 6e65 6c5f       sub_kernel_
-00001e10: 7369 7a65 203d 2073 656c 662e 7661 6c75  size = self.valu
-00001e20: 655f 7370 6163 6573 5b27 6b65 726e 656c  e_spaces['kernel
-00001e30: 5f73 697a 6527 5d2e 7661 6c75 650d 0a20  _size'].value.. 
-00001e40: 2020 2020 2020 2073 7461 7274 2c20 656e         start, en
-00001e50: 6420 3d20 7375 625f 6669 6c74 6572 5f73  d = sub_filter_s
-00001e60: 7461 7274 5f65 6e64 2873 656c 662e 6b65  tart_end(self.ke
-00001e70: 726e 656c 5f73 697a 652c 2073 7562 5f6b  rnel_size, sub_k
-00001e80: 6572 6e65 6c5f 7369 7a65 290d 0a20 2020  ernel_size)..   
-00001e90: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-00001ea0: 765f 6469 6d3d 3d27 3164 273a 2066 696c  v_dim=='1d': fil
-00001eb0: 7465 7273 203d 2066 696c 7465 7273 5b3a  ters = filters[:
-00001ec0: 2c20 3a2c 2073 7461 7274 3a65 6e64 5d0d  , :, start:end].
-00001ed0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00001ee0: 2e63 6f6e 765f 6469 6d3d 3d27 3264 273a  .conv_dim=='2d':
-00001ef0: 2066 696c 7465 7273 203d 2066 696c 7465   filters = filte
-00001f00: 7273 5b3a 2c20 3a2c 2073 7461 7274 3a65  rs[:, :, start:e
-00001f10: 6e64 2c20 7374 6172 743a 656e 645d 0d0a  nd, start:end]..
-00001f20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00001f30: 636f 6e76 5f64 696d 3d3d 2733 6427 3a20  conv_dim=='3d': 
-00001f40: 6669 6c74 6572 7320 3d20 6669 6c74 6572  filters = filter
-00001f50: 735b 3a2c 203a 2c20 7374 6172 743a 656e  s[:, :, start:en
-00001f60: 642c 2073 7461 7274 3a65 6e64 2c20 7374  d, start:end, st
-00001f70: 6172 743a 656e 645d 0d0a 2020 2020 2020  art:end]..      
-00001f80: 2020 7265 7475 726e 2066 696c 7465 7273    return filters
-00001f90: 0d0a 0d0a 2020 2020 6465 6620 736f 7274  ....    def sort
-00001fa0: 5f77 6569 6768 745f 6269 6173 2873 656c  _weight_bias(sel
-00001fb0: 662c 206d 6f64 756c 6529 3a0d 0a20 2020  f, module):..   
-00001fc0: 2020 2020 2069 6620 7365 6c66 2e73 6561       if self.sea
-00001fd0: 7263 685f 696e 5f63 6861 6e6e 656c 3a0d  rch_in_channel:.
-00001fe0: 0a20 2020 2020 2020 2020 2020 2076 6320  .            vc 
-00001ff0: 3d20 7365 6c66 2e76 616c 7565 5f73 7061  = self.value_spa
-00002000: 6365 735b 2769 6e5f 6368 616e 6e65 6c73  ces['in_channels
-00002010: 275d 0d0a 2020 2020 2020 2020 2020 2020  ']..            
-00002020: 6d6f 6475 6c65 2e77 6569 6768 742e 6461  module.weight.da
-00002030: 7461 203d 2074 6f72 6368 2e69 6e64 6578  ta = torch.index
-00002040: 5f73 656c 6563 7428 6d6f 6475 6c65 2e77  _select(module.w
-00002050: 6569 6768 742e 6461 7461 2c20 312c 2076  eight.data, 1, v
-00002060: 632e 736f 7274 4964 7829 0d0a 2020 2020  c.sortIdx)..    
-00002070: 2020 2020 6966 2073 656c 662e 7365 6172      if self.sear
-00002080: 6368 5f6f 7574 5f63 6861 6e6e 656c 3a0d  ch_out_channel:.
-00002090: 0a20 2020 2020 2020 2020 2020 2076 6320  .            vc 
-000020a0: 3d20 7365 6c66 2e76 616c 7565 5f73 7061  = self.value_spa
-000020b0: 6365 735b 276f 7574 5f63 6861 6e6e 656c  ces['out_channel
-000020c0: 7327 5d0d 0a20 2020 2020 2020 2020 2020  s']..           
-000020d0: 206d 6f64 756c 652e 7765 6967 6874 2e64   module.weight.d
-000020e0: 6174 6120 3d20 746f 7263 682e 696e 6465  ata = torch.inde
-000020f0: 785f 7365 6c65 6374 286d 6f64 756c 652e  x_select(module.
-00002100: 7765 6967 6874 2e64 6174 612c 2030 2c20  weight.data, 0, 
-00002110: 7663 2e73 6f72 7449 6478 290d 0a20 2020  vc.sortIdx)..   
-00002120: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00002130: 2e62 6961 7320 6973 206e 6f74 204e 6f6e  .bias is not Non
-00002140: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002150: 2020 2020 6d6f 6475 6c65 2e62 6961 732e      module.bias.
-00002160: 6461 7461 203d 2074 6f72 6368 2e69 6e64  data = torch.ind
-00002170: 6578 5f73 656c 6563 7428 6d6f 6475 6c65  ex_select(module
-00002180: 2e62 6961 732e 6461 7461 2c20 302c 2076  .bias.data, 0, v
-00002190: 632e 736f 7274 4964 7829 0d0a 0d0a 2020  c.sortIdx)....  
-000021a0: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
-000021b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000021c0: 2323 2323 2323 2323 2323 2323 230d 0a20  #############.. 
-000021d0: 2020 2023 2070 726f 7065 7274 790d 0a20     # property.. 
-000021e0: 2020 2023 2323 2323 2323 2323 2323 2323     #############
-000021f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002200: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-00002210: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00002220: 0a20 2020 2064 6566 2070 6172 616d 7328  .    def params(
-00002230: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00002240: 2727 2754 6865 206e 756d 6265 7220 6f66  '''The number of
-00002250: 2074 6865 2074 7261 696e 6162 6c65 2070   the trainable p
-00002260: 6172 616d 6574 6572 7327 2727 0d0a 2020  arameters'''..  
-00002270: 2020 2020 2020 2320 636f 6e76 0d0a 2020        # conv..  
-00002280: 2020 2020 2020 7765 6967 6874 203d 2073        weight = s
-00002290: 656c 662e 7765 6967 6874 0d0a 2020 2020  elf.weight..    
-000022a0: 2020 2020 6269 6173 203d 2073 656c 662e      bias = self.
-000022b0: 6269 6173 0d0a 0d0a 2020 2020 2020 2020  bias....        
-000022c0: 6966 2073 656c 662e 7365 6172 6368 5f69  if self.search_i
-000022d0: 6e5f 6368 616e 6e65 6c3a 0d0a 2020 2020  n_channel:..    
-000022e0: 2020 2020 2020 2020 696e 5f63 6861 6e6e          in_chann
-000022f0: 656c 7320 3d20 7365 6c66 2e76 616c 7565  els = self.value
-00002300: 5f73 7061 6365 735b 2769 6e5f 6368 616e  _spaces['in_chan
-00002310: 6e65 6c73 275d 2e76 616c 7565 0d0a 2020  nels'].value..  
-00002320: 2020 2020 2020 2020 2020 7765 6967 6874            weight
-00002330: 203d 2077 6569 6768 745b 3a2c 203a 696e   = weight[:, :in
-00002340: 5f63 6861 6e6e 656c 732c 202e 2e2e 5d0d  _channels, ...].
-00002350: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00002360: 2e73 6561 7263 685f 6f75 745f 6368 616e  .search_out_chan
-00002370: 6e65 6c3a 0d0a 2020 2020 2020 2020 2020  nel:..          
-00002380: 2020 6f75 745f 6368 616e 6e65 6c73 203d    out_channels =
-00002390: 2073 656c 662e 7661 6c75 655f 7370 6163   self.value_spac
-000023a0: 6573 5b27 6f75 745f 6368 616e 6e65 6c73  es['out_channels
-000023b0: 275d 2e76 616c 7565 0d0a 2020 2020 2020  '].value..      
-000023c0: 2020 2020 2020 7765 6967 6874 203d 2077        weight = w
-000023d0: 6569 6768 745b 3a6f 7574 5f63 6861 6e6e  eight[:out_chann
-000023e0: 656c 732c 203a 2c20 2e2e 2e5d 0d0a 2020  els, :, ...]..  
-000023f0: 2020 2020 2020 2020 2020 6966 2062 6961            if bia
-00002400: 7320 6973 206e 6f74 204e 6f6e 653a 2062  s is not None: b
-00002410: 6961 7320 3d20 6269 6173 5b3a 6f75 745f  ias = bias[:out_
-00002420: 6368 616e 6e65 6c73 5d0d 0a20 2020 2020  channels]..     
-00002430: 2020 2069 6620 7365 6c66 2e73 6561 7263     if self.searc
-00002440: 685f 6b65 726e 656c 5f73 697a 653a 0d0a  h_kernel_size:..
-00002450: 2020 2020 2020 2020 2020 2020 6b65 726e              kern
-00002460: 656c 5f73 697a 6520 3d20 7365 6c66 2e76  el_size = self.v
-00002470: 616c 7565 5f73 7061 6365 735b 276b 6572  alue_spaces['ker
-00002480: 6e65 6c5f 7369 7a65 275d 2e76 616c 7565  nel_size'].value
-00002490: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-000024a0: 6172 742c 2065 6e64 203d 2073 7562 5f66  art, end = sub_f
-000024b0: 696c 7465 725f 7374 6172 745f 656e 6428  ilter_start_end(
-000024c0: 7365 6c66 2e6b 6572 6e65 6c5f 7369 7a65  self.kernel_size
-000024d0: 2c20 6b65 726e 656c 5f73 697a 6529 0d0a  , kernel_size)..
-000024e0: 2020 2020 2020 2020 2020 2020 7368 6170              shap
-000024f0: 655f 7369 7a65 203d 206c 656e 2877 6569  e_size = len(wei
-00002500: 6768 742e 7368 6170 6529 0d0a 2020 2020  ght.shape)..    
-00002510: 2020 2020 2020 2020 6966 2073 6861 7065          if shape
-00002520: 5f73 697a 6520 3d3d 2033 3a0d 0a20 2020  _size == 3:..   
-00002530: 2020 2020 2020 2020 2020 2020 2023 2031               # 1
-00002540: 4420 636f 6e76 0d0a 2020 2020 2020 2020  D conv..        
-00002550: 2020 2020 2020 2020 7765 6967 6874 203d          weight =
-00002560: 2077 6569 6768 745b 3a2c 203a 2c20 7374   weight[:, :, st
-00002570: 6172 743a 656e 645d 0d0a 2020 2020 2020  art:end]..      
-00002580: 2020 2020 2020 656c 6966 2073 6861 7065        elif shape
-00002590: 5f73 697a 6520 3d3d 2034 3a0d 0a20 2020  _size == 4:..   
-000025a0: 2020 2020 2020 2020 2020 2020 2023 2032               # 2
-000025b0: 4420 636f 6e76 0d0a 2020 2020 2020 2020  D conv..        
-000025c0: 2020 2020 2020 2020 7765 6967 6874 203d          weight =
-000025d0: 2077 6569 6768 745b 3a2c 203a 2c20 7374   weight[:, :, st
-000025e0: 6172 743a 656e 642c 2073 7461 7274 3a65  art:end, start:e
-000025f0: 6e64 5d0d 0a20 2020 2020 2020 2020 2020  nd]..           
-00002600: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00002610: 2020 2020 2020 2020 2320 3344 2063 6f6e          # 3D con
-00002620: 760d 0a20 2020 2020 2020 2020 2020 2020  v..             
-00002630: 2020 2077 6569 6768 7420 3d20 7765 6967     weight = weig
-00002640: 6874 5b3a 2c20 3a2c 2073 7461 7274 3a65  ht[:, :, start:e
-00002650: 6e64 2c20 7374 6172 743a 656e 642c 2073  nd, start:end, s
-00002660: 7461 7274 3a65 6e64 5d0d 0a20 2020 2020  tart:end]..     
-00002670: 2020 2070 6172 616d 6574 6572 7320 3d20     parameters = 
-00002680: 5b77 6569 6768 742c 2062 6961 735d 0d0a  [weight, bias]..
-00002690: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-000026a0: 2073 756d 285b 702e 6e75 6d65 6c28 2920   sum([p.numel() 
-000026b0: 666f 7220 7020 696e 2070 6172 616d 6574  for p in paramet
-000026c0: 6572 7320 6966 2070 2069 7320 6e6f 7420  ers if p is not 
-000026d0: 4e6f 6e65 5d29 0d0a 2020 2020 2020 2020  None])..        
-000026e0: 7265 7475 726e 2070 6172 616d 730d 0a0d  return params...
-000026f0: 0a0d 0a63 6c61 7373 2043 6f6e 7631 6428  ...class Conv1d(
-00002700: 4261 7365 436f 6e76 4e64 293a 0d0a 2020  BaseConvNd):..  
-00002710: 2020 6465 6620 5f5f 696e 6974 5f5f 280d    def __init__(.
-00002720: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
-00002730: 2020 2020 2020 2020 696e 5f63 6861 6e6e          in_chann
-00002740: 656c 733a 2069 6e74 2c0d 0a20 2020 2020  els: int,..     
-00002750: 2020 206f 7574 5f63 6861 6e6e 656c 733a     out_channels:
-00002760: 2069 6e74 2c0d 0a20 2020 2020 2020 206b   int,..        k
-00002770: 6572 6e65 6c5f 7369 7a65 3a20 556e 696f  ernel_size: Unio
-00002780: 6e5b 5f73 697a 655f 315f 742c 2056 616c  n[_size_1_t, Val
-00002790: 7565 5370 6163 655d 2c0d 0a20 2020 2020  ueSpace],..     
-000027a0: 2020 2073 7472 6964 653a 2055 6e69 6f6e     stride: Union
-000027b0: 5b5f 7369 7a65 5f31 5f74 2c20 5661 6c75  [_size_1_t, Valu
-000027c0: 6553 7061 6365 5d20 3d20 312c 0d0a 2020  eSpace] = 1,..  
-000027d0: 2020 2020 2020 7061 6464 696e 673a 2055        padding: U
-000027e0: 6e69 6f6e 5b73 7472 2c20 5f73 697a 655f  nion[str, _size_
-000027f0: 315f 742c 2056 616c 7565 5370 6163 655d  1_t, ValueSpace]
-00002800: 203d 2030 2c0d 0a20 2020 2020 2020 2064   = 0,..        d
-00002810: 696c 6174 696f 6e3a 2055 6e69 6f6e 5b5f  ilation: Union[_
-00002820: 7369 7a65 5f31 5f74 2c20 5661 6c75 6553  size_1_t, ValueS
-00002830: 7061 6365 5d20 3d20 312c 0d0a 2020 2020  pace] = 1,..    
-00002840: 2020 2020 6772 6f75 7073 3a20 556e 696f      groups: Unio
-00002850: 6e5b 696e 742c 2056 616c 7565 5370 6163  n[int, ValueSpac
-00002860: 655d 203d 2031 2c0d 0a20 2020 2020 2020  e] = 1,..       
-00002870: 2062 6961 733a 2062 6f6f 6c20 3d20 5472   bias: bool = Tr
-00002880: 7565 2c0d 0a20 2020 2020 2020 2070 6164  ue,..        pad
-00002890: 6469 6e67 5f6d 6f64 653a 2073 7472 203d  ding_mode: str =
-000028a0: 2027 7a65 726f 7327 2c0d 0a20 2020 2020   'zeros',..     
-000028b0: 2020 2061 7574 6f5f 7061 6464 696e 673a     auto_padding:
-000028c0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-000028d0: 2020 2020 2020 2020 2a61 7267 732c 202a          *args, *
-000028e0: 2a6b 7761 7267 730d 0a20 2020 2029 3a0d  *kwargs..    ):.
-000028f0: 0a20 2020 2020 2020 2073 7570 6572 2843  .        super(C
-00002900: 6f6e 7631 642c 2073 656c 6629 2e5f 5f69  onv1d, self).__i
-00002910: 6e69 745f 5f28 0d0a 2020 2020 2020 2020  nit__(..        
-00002920: 2020 2020 696e 5f63 6861 6e6e 656c 732c      in_channels,
-00002930: 206f 7574 5f63 6861 6e6e 656c 732c 206b   out_channels, k
-00002940: 6572 6e65 6c5f 7369 7a65 2c20 7374 7269  ernel_size, stri
-00002950: 6465 2c20 7061 6464 696e 672c 0d0a 2020  de, padding,..  
-00002960: 2020 2020 2020 2020 2020 6469 6c61 7469            dilati
-00002970: 6f6e 2c20 6772 6f75 7073 2c20 6269 6173  on, groups, bias
-00002980: 2c20 7061 6464 696e 675f 6d6f 6465 2c20  , padding_mode, 
-00002990: 6175 746f 5f70 6164 6469 6e67 290d 0a0d  auto_padding)...
-000029a0: 0a20 2020 2064 6566 2069 6e69 745f 6f70  .    def init_op
-000029b0: 7328 0d0a 2020 2020 2020 2020 7365 6c66  s(..        self
-000029c0: 2c0d 0a20 2020 2020 2020 2069 6e5f 6368  ,..        in_ch
-000029d0: 616e 6e65 6c73 3a20 696e 742c 0d0a 2020  annels: int,..  
-000029e0: 2020 2020 2020 6f75 745f 6368 616e 6e65        out_channe
-000029f0: 6c73 3a20 696e 742c 0d0a 2020 2020 2020  ls: int,..      
-00002a00: 2020 6b65 726e 656c 5f73 697a 653a 205f    kernel_size: _
-00002a10: 7369 7a65 5f31 5f74 2c0d 0a20 2020 2020  size_1_t,..     
-00002a20: 2020 2073 7472 6964 653a 205f 7369 7a65     stride: _size
-00002a30: 5f31 5f74 203d 2031 2c0d 0a20 2020 2020  _1_t = 1,..     
-00002a40: 2020 2070 6164 6469 6e67 3a20 556e 696f     padding: Unio
-00002a50: 6e5b 7374 722c 205f 7369 7a65 5f31 5f74  n[str, _size_1_t
-00002a60: 5d20 3d20 302c 0d0a 2020 2020 2020 2020  ] = 0,..        
-00002a70: 6469 6c61 7469 6f6e 3a20 5f73 697a 655f  dilation: _size_
-00002a80: 315f 7420 3d20 312c 0d0a 2020 2020 2020  1_t = 1,..      
-00002a90: 2020 6772 6f75 7073 3a20 696e 7420 3d20    groups: int = 
-00002aa0: 312c 0d0a 2020 2020 2020 2020 6269 6173  1,..        bias
-00002ab0: 3a20 626f 6f6c 203d 2054 7275 650d 0a20  : bool = True.. 
-00002ac0: 2020 2029 3a0d 0a20 2020 2020 2020 2027     ):..        '
-00002ad0: 2727 4765 6e65 7261 7465 2043 6f6e 7620  ''Generate Conv 
-00002ae0: 6f70 6572 6174 696f 6e27 2727 0d0a 2020  operation'''..  
-00002af0: 2020 2020 2020 7365 6c66 2e6b 6572 6e65        self.kerne
-00002b00: 6c5f 7369 7a65 203d 205f 7369 6e67 6c65  l_size = _single
-00002b10: 286b 6572 6e65 6c5f 7369 7a65 290d 0a20  (kernel_size).. 
-00002b20: 2020 2020 2020 2073 656c 662e 7374 7269         self.stri
-00002b30: 6465 203d 205f 7369 6e67 6c65 2873 7472  de = _single(str
-00002b40: 6964 6529 0d0a 2020 2020 2020 2020 7365  ide)..        se
-00002b50: 6c66 2e70 6164 6469 6e67 203d 2070 6164  lf.padding = pad
-00002b60: 6469 6e67 2069 6620 6973 696e 7374 616e  ding if isinstan
-00002b70: 6365 2870 6164 6469 6e67 2c20 7374 7229  ce(padding, str)
-00002b80: 2065 6c73 6520 5f73 696e 676c 6528 7061   else _single(pa
-00002b90: 6464 696e 6729 0d0a 2020 2020 2020 2020  dding)..        
-00002ba0: 7365 6c66 2e64 696c 6174 696f 6e20 3d20  self.dilation = 
-00002bb0: 5f73 696e 676c 6528 6469 6c61 7469 6f6e  _single(dilation
-00002bc0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00002bd0: 6f75 7470 7574 5f70 6164 6469 6e67 203d  output_padding =
-00002be0: 205f 7369 6e67 6c65 2830 290d 0a20 2020   _single(0)..   
-00002bf0: 2020 2020 2073 656c 662e 636f 6e76 203d       self.conv =
-00002c00: 2046 2e63 6f6e 7631 640d 0a0d 0a0d 0a63   F.conv1d......c
-00002c10: 6c61 7373 2043 6f6e 7632 6428 4261 7365  lass Conv2d(Base
-00002c20: 436f 6e76 4e64 293a 0d0a 2020 2020 6465  ConvNd):..    de
-00002c30: 6620 5f5f 696e 6974 5f5f 280d 0a20 2020  f __init__(..   
-00002c40: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
-00002c50: 2020 2020 696e 5f63 6861 6e6e 656c 733a      in_channels:
-00002c60: 2069 6e74 2c0d 0a20 2020 2020 2020 206f   int,..        o
-00002c70: 7574 5f63 6861 6e6e 656c 733a 2069 6e74  ut_channels: int
-00002c80: 2c0d 0a20 2020 2020 2020 206b 6572 6e65  ,..        kerne
-00002c90: 6c5f 7369 7a65 3a20 556e 696f 6e5b 696e  l_size: Union[in
-00002ca0: 742c 2074 7570 6c65 5d2c 0d0a 2020 2020  t, tuple],..    
-00002cb0: 2020 2020 7374 7269 6465 3a20 556e 696f      stride: Unio
-00002cc0: 6e5b 696e 742c 2074 7570 6c65 5d20 3d20  n[int, tuple] = 
-00002cd0: 312c 0d0a 2020 2020 2020 2020 7061 6464  1,..        padd
-00002ce0: 696e 673a 2055 6e69 6f6e 5b73 7472 2c20  ing: Union[str, 
-00002cf0: 696e 742c 2074 7570 6c65 5d20 3d20 302c  int, tuple] = 0,
-00002d00: 0d0a 2020 2020 2020 2020 6469 6c61 7469  ..        dilati
-00002d10: 6f6e 3a20 556e 696f 6e5b 696e 742c 2074  on: Union[int, t
-00002d20: 7570 6c65 5d20 3d20 312c 0d0a 2020 2020  uple] = 1,..    
-00002d30: 2020 2020 6772 6f75 7073 3a20 696e 7420      groups: int 
-00002d40: 3d20 312c 0d0a 2020 2020 2020 2020 6269  = 1,..        bi
-00002d50: 6173 3a20 626f 6f6c 203d 2054 7275 652c  as: bool = True,
-00002d60: 0d0a 2020 2020 2020 2020 7061 6464 696e  ..        paddin
-00002d70: 675f 6d6f 6465 3a20 7374 7220 3d20 277a  g_mode: str = 'z
-00002d80: 6572 6f73 272c 0d0a 2020 2020 2020 2020  eros',..        
-00002d90: 6175 746f 5f70 6164 6469 6e67 3a20 626f  auto_padding: bo
-00002da0: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
-00002db0: 2020 2020 202a 6172 6773 2c20 2a2a 6b77       *args, **kw
-00002dc0: 6172 6773 0d0a 2020 2020 2020 2020 293a  args..        ):
-00002dd0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-00002de0: 436f 6e76 3264 2c20 7365 6c66 292e 5f5f  Conv2d, self).__
-00002df0: 696e 6974 5f5f 280d 0a20 2020 2020 2020  init__(..       
-00002e00: 2020 2020 2069 6e5f 6368 616e 6e65 6c73       in_channels
-00002e10: 2c20 6f75 745f 6368 616e 6e65 6c73 2c20  , out_channels, 
-00002e20: 6b65 726e 656c 5f73 697a 652c 2073 7472  kernel_size, str
-00002e30: 6964 652c 2070 6164 6469 6e67 2c0d 0a20  ide, padding,.. 
-00002e40: 2020 2020 2020 2020 2020 2064 696c 6174             dilat
-00002e50: 696f 6e2c 2067 726f 7570 732c 2062 6961  ion, groups, bia
-00002e60: 732c 2070 6164 6469 6e67 5f6d 6f64 652c  s, padding_mode,
-00002e70: 2061 7574 6f5f 7061 6464 696e 6729 0d0a   auto_padding)..
-00002e80: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00002e90: 662e 7365 6172 6368 5f6b 6572 6e65 6c5f  f.search_kernel_
-00002ea0: 7369 7a65 2061 6e64 2073 656c 662e 4b45  size and self.KE
-00002eb0: 524e 454c 5f54 5241 4e53 464f 524d 5f4d  RNEL_TRANSFORM_M
-00002ec0: 4f44 4520 6973 206e 6f74 204e 6f6e 653a  ODE is not None:
-00002ed0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00002ee0: 6c66 2e69 6e69 745f 6b65 726e 656c 5f74  lf.init_kernel_t
-00002ef0: 7261 6e73 666f 726d 5f6d 6174 7269 7828  ransform_matrix(
-00002f00: 290d 0a0d 0a20 2020 2064 6566 2069 6e69  )....    def ini
-00002f10: 745f 6b65 726e 656c 5f74 7261 6e73 666f  t_kernel_transfo
-00002f20: 726d 5f6d 6174 7269 7828 7365 6c66 293a  rm_matrix(self):
-00002f30: 0d0a 2020 2020 2020 2020 6b65 726e 656c  ..        kernel
-00002f40: 5f73 697a 6520 3d20 7365 6c66 2e76 616c  _size = self.val
-00002f50: 7565 5f73 7061 6365 735b 276b 6572 6e65  ue_spaces['kerne
-00002f60: 6c5f 7369 7a65 275d 2e63 616e 6469 6461  l_size'].candida
-00002f70: 7465 735f 6f72 6967 696e 616c 0d0a 2020  tes_original..  
-00002f80: 2020 2020 2020 2320 7265 6769 7374 6572        # register
-00002f90: 2073 6361 6c69 6e67 2070 6172 616d 6574   scaling paramet
-00002fa0: 6572 730d 0a20 2020 2020 2020 2023 2037  ers..        # 7
-00002fb0: 746f 355f 6d61 7472 6978 2c20 3574 6f33  to5_matrix, 5to3
-00002fc0: 5f6d 6174 7269 780d 0a20 2020 2020 2020  _matrix..       
-00002fd0: 2073 6361 6c65 5f70 6172 616d 7320 3d20   scale_params = 
-00002fe0: 7b7d 0d0a 2020 2020 2020 2020 666f 7220  {}..        for 
-00002ff0: 6920 696e 2072 616e 6765 286c 656e 286b  i in range(len(k
-00003000: 6572 6e65 6c5f 7369 7a65 2920 2d20 3129  ernel_size) - 1)
-00003010: 3a0d 0a20 2020 2020 2020 2020 2020 206b  :..            k
-00003020: 735f 736d 616c 6c20 3d20 6b65 726e 656c  s_small = kernel
-00003030: 5f73 697a 655b 695d 0d0a 2020 2020 2020  _size[i]..      
-00003040: 2020 2020 2020 6b73 5f6c 6172 6765 7220        ks_larger 
-00003050: 3d20 6b65 726e 656c 5f73 697a 655b 6920  = kernel_size[i 
-00003060: 2b20 315d 0d0a 2020 2020 2020 2020 2020  + 1]..          
-00003070: 2020 7061 7261 6d5f 6e61 6d65 203d 2027    param_name = '
-00003080: 2564 746f 2564 2720 2520 286b 735f 6c61  %dto%d' % (ks_la
-00003090: 7267 6572 2c20 6b73 5f73 6d61 6c6c 290d  rger, ks_small).
-000030a0: 0a20 2020 2020 2020 2020 2020 2023 206e  .            # n
-000030b0: 6f69 6e73 7065 6374 696f 6e20 5079 4172  oinspection PyAr
-000030c0: 6775 6d65 6e74 4c69 7374 0d0a 2020 2020  gumentList..    
-000030d0: 2020 2020 2020 2020 7363 616c 655f 7061          scale_pa
-000030e0: 7261 6d73 5b27 2573 5f6d 6174 7269 7827  rams['%s_matrix'
-000030f0: 2025 2070 6172 616d 5f6e 616d 655d 203d   % param_name] =
-00003100: 2050 6172 616d 6574 6572 2874 6f72 6368   Parameter(torch
-00003110: 2e65 7965 286b 735f 736d 616c 6c20 2a2a  .eye(ks_small **
-00003120: 2032 2929 0d0a 2020 2020 2020 2020 666f   2))..        fo
-00003130: 7220 6e61 6d65 2c20 7061 7261 6d20 696e  r name, param in
-00003140: 2073 6361 6c65 5f70 6172 616d 732e 6974   scale_params.it
-00003150: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00003160: 2020 2020 7365 6c66 2e72 6567 6973 7465      self.registe
-00003170: 725f 7061 7261 6d65 7465 7228 6e61 6d65  r_parameter(name
-00003180: 2c20 7061 7261 6d29 0d0a 0d0a 2020 2020  , param)....    
-00003190: 6465 6620 696e 6974 5f6f 7073 280d 0a20  def init_ops(.. 
-000031a0: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-000031b0: 2020 2020 2020 696e 5f63 6861 6e6e 656c        in_channel
-000031c0: 733a 2069 6e74 2c0d 0a20 2020 2020 2020  s: int,..       
-000031d0: 206f 7574 5f63 6861 6e6e 656c 733a 2069   out_channels: i
-000031e0: 6e74 2c0d 0a20 2020 2020 2020 206b 6572  nt,..        ker
-000031f0: 6e65 6c5f 7369 7a65 3a20 5f73 697a 655f  nel_size: _size_
-00003200: 325f 742c 0d0a 2020 2020 2020 2020 7374  2_t,..        st
-00003210: 7269 6465 3a20 5f73 697a 655f 325f 7420  ride: _size_2_t 
-00003220: 3d20 312c 0d0a 2020 2020 2020 2020 7061  = 1,..        pa
-00003230: 6464 696e 673a 2055 6e69 6f6e 5b73 7472  dding: Union[str
-00003240: 2c20 5f73 697a 655f 325f 745d 203d 2030  , _size_2_t] = 0
-00003250: 2c0d 0a20 2020 2020 2020 2064 696c 6174  ,..        dilat
-00003260: 696f 6e3a 205f 7369 7a65 5f32 5f74 203d  ion: _size_2_t =
-00003270: 2031 2c0d 0a20 2020 2020 2020 2067 726f   1,..        gro
-00003280: 7570 733a 2069 6e74 203d 2031 2c0d 0a20  ups: int = 1,.. 
-00003290: 2020 2020 2020 2062 6961 733a 2062 6f6f         bias: boo
-000032a0: 6c20 3d20 5472 7565 2c0d 0a20 2020 2029  l = True,..    )
-000032b0: 3a0d 0a20 2020 2020 2020 2027 2727 4765  :..        '''Ge
-000032c0: 6e65 7261 7465 2043 6f6e 7620 6f70 6572  nerate Conv oper
-000032d0: 6174 696f 6e27 2727 0d0a 2020 2020 2020  ation'''..      
-000032e0: 2020 7365 6c66 2e6b 6572 6e65 6c5f 7369    self.kernel_si
-000032f0: 7a65 203d 205f 7061 6972 286b 6572 6e65  ze = _pair(kerne
-00003300: 6c5f 7369 7a65 290d 0a20 2020 2020 2020  l_size)..       
-00003310: 2073 656c 662e 7374 7269 6465 203d 205f   self.stride = _
-00003320: 7061 6972 2873 7472 6964 6529 0d0a 2020  pair(stride)..  
-00003330: 2020 2020 2020 7365 6c66 2e70 6164 6469        self.paddi
-00003340: 6e67 203d 2070 6164 6469 6e67 2069 6620  ng = padding if 
-00003350: 6973 696e 7374 616e 6365 2870 6164 6469  isinstance(paddi
-00003360: 6e67 2c20 7374 7229 2065 6c73 6520 5f70  ng, str) else _p
-00003370: 6169 7228 7061 6464 696e 6729 0d0a 2020  air(padding)..  
-00003380: 2020 2020 2020 7365 6c66 2e64 696c 6174        self.dilat
-00003390: 696f 6e20 3d20 5f70 6169 7228 6469 6c61  ion = _pair(dila
-000033a0: 7469 6f6e 290d 0a20 2020 2020 2020 2073  tion)..        s
-000033b0: 656c 662e 6f75 7470 7574 5f70 6164 6469  elf.output_paddi
-000033c0: 6e67 203d 205f 7061 6972 2830 290d 0a20  ng = _pair(0).. 
-000033d0: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-000033e0: 203d 2046 2e63 6f6e 7632 640d 0a0d 0a20   = F.conv2d.... 
-000033f0: 2020 2064 6566 2074 7261 6e73 666f 726d     def transform
-00003400: 5f6b 6572 6e65 6c5f 7369 7a65 2873 656c  _kernel_size(sel
-00003410: 662c 2066 696c 7465 7273 293a 0d0a 2020  f, filters):..  
-00003420: 2020 2020 2020 6966 2073 656c 662e 4b45        if self.KE
-00003430: 524e 454c 5f54 5241 4e53 464f 524d 5f4d  RNEL_TRANSFORM_M
-00003440: 4f44 4520 6973 204e 6f6e 653a 0d0a 2020  ODE is None:..  
-00003450: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003460: 2073 7570 6572 2843 6f6e 7632 642c 2073   super(Conv2d, s
-00003470: 656c 6629 2e74 7261 6e73 666f 726d 5f6b  elf).transform_k
-00003480: 6572 6e65 6c5f 7369 7a65 2866 696c 7465  ernel_size(filte
-00003490: 7273 290d 0a20 2020 2020 2020 2065 6c73  rs)..        els
-000034a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000034b0: 6d61 785f 6b65 726e 656c 5f73 697a 6520  max_kernel_size 
-000034c0: 3d20 7365 6c66 2e6b 6572 6e65 6c5f 7369  = self.kernel_si
-000034d0: 7a65 0d0a 2020 2020 2020 2020 2020 2020  ze..            
-000034e0: 6966 2069 7369 6e73 7461 6e63 6528 6d61  if isinstance(ma
-000034f0: 785f 6b65 726e 656c 5f73 697a 652c 2028  x_kernel_size, (
-00003500: 7475 706c 652c 206c 6973 7429 293a 0d0a  tuple, list)):..
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 6d61 785f 6b65 726e 656c 5f73 697a 6520  max_kernel_size 
-00003530: 3d20 6d61 7828 6d61 785f 6b65 726e 656c  = max(max_kernel
-00003540: 5f73 697a 6529 0d0a 2020 2020 2020 2020  _size)..        
-00003550: 2020 2020 7375 625f 6b65 726e 656c 5f73      sub_kernel_s
-00003560: 697a 6520 3d20 7365 6c66 2e76 616c 7565  ize = self.value
-00003570: 5f73 7061 6365 735b 276b 6572 6e65 6c5f  _spaces['kernel_
-00003580: 7369 7a65 275d 2e76 616c 7565 0d0a 2020  size'].value..  
-00003590: 2020 2020 2020 2020 2020 6b73 5f73 6574            ks_set
-000035a0: 203d 2073 656c 662e 7661 6c75 655f 7370   = self.value_sp
-000035b0: 6163 6573 5b27 6b65 726e 656c 5f73 697a  aces['kernel_siz
-000035c0: 6527 5d2e 6361 6e64 6964 6174 6573 0d0a  e'].candidates..
-000035d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000035e0: 7562 5f6b 6572 6e65 6c5f 7369 7a65 203c  ub_kernel_size <
-000035f0: 206d 6178 5f6b 6572 6e65 6c5f 7369 7a65   max_kernel_size
-00003600: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003610: 2020 2073 7461 7274 5f66 696c 7465 7220     start_filter 
-00003620: 3d20 6669 6c74 6572 730d 0a20 2020 2020  = filters..     
-00003630: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00003640: 2069 6e20 7261 6e67 6528 6c65 6e28 6b73   in range(len(ks
-00003650: 5f73 6574 292d 312c 2030 2c20 2d31 293a  _set)-1, 0, -1):
-00003660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003670: 2020 2020 2020 7372 635f 6b73 203d 206b        src_ks = k
-00003680: 735f 7365 745b 695d 0d0a 2020 2020 2020  s_set[i]..      
-00003690: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000036a0: 2073 7263 5f6b 7320 3c3d 2073 7562 5f6b   src_ks <= sub_k
-000036b0: 6572 6e65 6c5f 7369 7a65 3a0d 0a20 2020  ernel_size:..   
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036d0: 2020 2020 2062 7265 616b 0d0a 2020 2020       break..    
-000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036f0: 7461 7267 6574 5f6b 7320 3d20 6b73 5f73  target_ks = ks_s
-00003700: 6574 5b69 202d 2031 5d0d 0a20 2020 2020  et[i - 1]..     
-00003710: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003720: 7461 7274 2c20 656e 6420 3d20 7375 625f  tart, end = sub_
-00003730: 6669 6c74 6572 5f73 7461 7274 5f65 6e64  filter_start_end
-00003740: 2873 7263 5f6b 732c 2074 6172 6765 745f  (src_ks, target_
-00003750: 6b73 290d 0a20 2020 2020 2020 2020 2020  ks)..           
-00003760: 2020 2020 2020 2020 205f 696e 7075 745f           _input_
-00003770: 6669 6c74 6572 203d 2073 7461 7274 5f66  filter = start_f
-00003780: 696c 7465 725b 3a2c 203a 2c20 7374 6172  ilter[:, :, star
-00003790: 743a 656e 642c 2073 7461 7274 3a65 6e64  t:end, start:end
-000037a0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000037b0: 2020 2020 2020 205f 696e 7075 745f 6669         _input_fi
-000037c0: 6c74 6572 203d 205f 696e 7075 745f 6669  lter = _input_fi
-000037d0: 6c74 6572 2e63 6f6e 7469 6775 6f75 7328  lter.contiguous(
-000037e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000037f0: 2020 2020 2020 205f 696e 7075 745f 6669         _input_fi
-00003800: 6c74 6572 203d 205f 696e 7075 745f 6669  lter = _input_fi
-00003810: 6c74 6572 2e76 6965 7728 5f69 6e70 7574  lter.view(_input
-00003820: 5f66 696c 7465 722e 7369 7a65 2830 292c  _filter.size(0),
-00003830: 205f 696e 7075 745f 6669 6c74 6572 2e73   _input_filter.s
-00003840: 697a 6528 3129 2c20 2d31 290d 0a20 2020  ize(1), -1)..   
-00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 205f 696e 7075 745f 6669 6c74 6572 203d   _input_filter =
-00003870: 205f 696e 7075 745f 6669 6c74 6572 2e76   _input_filter.v
-00003880: 6965 7728 2d31 2c20 5f69 6e70 7574 5f66  iew(-1, _input_f
-00003890: 696c 7465 722e 7369 7a65 2832 2929 0d0a  ilter.size(2))..
-000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038b0: 2020 2020 5f69 6e70 7574 5f66 696c 7465      _input_filte
-000038c0: 7220 3d20 462e 6c69 6e65 6172 280d 0a20  r = F.linear(.. 
-000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038e0: 2020 2020 2020 205f 696e 7075 745f 6669         _input_fi
-000038f0: 6c74 6572 2c20 6765 7461 7474 7228 7365  lter, getattr(se
-00003900: 6c66 2c20 2725 6474 6f25 645f 6d61 7472  lf, '%dto%d_matr
-00003910: 6978 2720 2520 2873 7263 5f6b 732c 2074  ix' % (src_ks, t
-00003920: 6172 6765 745f 6b73 2929 2c0d 0a20 2020  arget_ks)),..   
-00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003940: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-00003950: 2020 2020 2020 2020 5f69 6e70 7574 5f66          _input_f
-00003960: 696c 7465 7220 3d20 5f69 6e70 7574 5f66  ilter = _input_f
-00003970: 696c 7465 722e 7669 6577 2866 696c 7465  ilter.view(filte
-00003980: 7273 2e73 697a 6528 3029 2c20 6669 6c74  rs.size(0), filt
-00003990: 6572 732e 7369 7a65 2831 292c 2074 6172  ers.size(1), tar
-000039a0: 6765 745f 6b73 202a 2a20 3229 0d0a 2020  get_ks ** 2)..  
-000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039c0: 2020 5f69 6e70 7574 5f66 696c 7465 7220    _input_filter 
-000039d0: 3d20 5f69 6e70 7574 5f66 696c 7465 722e  = _input_filter.
-000039e0: 7669 6577 2866 696c 7465 7273 2e73 697a  view(filters.siz
-000039f0: 6528 3029 2c20 6669 6c74 6572 732e 7369  e(0), filters.si
-00003a00: 7a65 2831 292c 2074 6172 6765 745f 6b73  ze(1), target_ks
-00003a10: 2c20 7461 7267 6574 5f6b 7329 0d0a 2020  , target_ks)..  
-00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a30: 2020 7374 6172 745f 6669 6c74 6572 203d    start_filter =
-00003a40: 205f 696e 7075 745f 6669 6c74 6572 0d0a   _input_filter..
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 6669 6c74 6572 7320 3d20 7374 6172 745f  filters = start_
-00003a70: 6669 6c74 6572 0d0a 2020 2020 2020 2020  filter..        
-00003a80: 2020 2020 7265 7475 726e 2066 696c 7465      return filte
-00003a90: 7273 0d0a 0d0a 0d0a 636c 6173 7320 436f  rs......class Co
-00003aa0: 6e76 3364 2842 6173 6543 6f6e 764e 6429  nv3d(BaseConvNd)
-00003ab0: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
-00003ac0: 745f 5f28 0d0a 2020 2020 2020 2020 7365  t__(..        se
-00003ad0: 6c66 2c0d 0a20 2020 2020 2020 2069 6e5f  lf,..        in_
-00003ae0: 6368 616e 6e65 6c73 3a20 696e 742c 0d0a  channels: int,..
-00003af0: 2020 2020 2020 2020 6f75 745f 6368 616e          out_chan
-00003b00: 6e65 6c73 3a20 696e 742c 0d0a 2020 2020  nels: int,..    
-00003b10: 2020 2020 6b65 726e 656c 5f73 697a 653a      kernel_size:
-00003b20: 2055 6e69 6f6e 5b69 6e74 2c20 7475 706c   Union[int, tupl
-00003b30: 655d 2c0d 0a20 2020 2020 2020 2073 7472  e],..        str
-00003b40: 6964 653a 2055 6e69 6f6e 5b69 6e74 2c20  ide: Union[int, 
-00003b50: 7475 706c 655d 203d 2031 2c0d 0a20 2020  tuple] = 1,..   
-00003b60: 2020 2020 2070 6164 6469 6e67 3a20 556e       padding: Un
-00003b70: 696f 6e5b 7374 722c 2069 6e74 2c20 7475  ion[str, int, tu
-00003b80: 706c 655d 203d 2030 2c0d 0a20 2020 2020  ple] = 0,..     
+00000020: 6f6e 616c 2c20 5365 742c 2054 7570 6c65  onal, Set, Tuple
+00000030: 0d0a 0d0a 696d 706f 7274 2074 6f72 6368  ....import torch
+00000040: 0d0a 696d 706f 7274 2074 6f72 6368 2e6e  ..import torch.n
+00000050: 6e20 6173 206e 6e0d 0a69 6d70 6f72 7420  n as nn..import 
+00000060: 746f 7263 682e 6e6e 2e66 756e 6374 696f  torch.nn.functio
+00000070: 6e61 6c20 6173 2046 0d0a 6672 6f6d 2074  nal as F..from t
+00000080: 6f72 6368 2e6e 6e2e 6d6f 6475 6c65 732e  orch.nn.modules.
+00000090: 636f 6e76 2069 6d70 6f72 7420 5f43 6f6e  conv import _Con
+000000a0: 764e 640d 0a66 726f 6d20 746f 7263 682e  vNd..from torch.
+000000b0: 6e6e 2e63 6f6d 6d6f 6e5f 7479 7065 7320  nn.common_types 
+000000c0: 696d 706f 7274 205f 7369 7a65 5f31 5f74  import _size_1_t
+000000d0: 2c20 5f73 697a 655f 325f 742c 205f 7369  , _size_2_t, _si
+000000e0: 7a65 5f33 5f74 0d0a 6672 6f6d 2074 6f72  ze_3_t..from tor
+000000f0: 6368 2e6e 6e2e 6d6f 6475 6c65 732e 7574  ch.nn.modules.ut
+00000100: 696c 7320 696d 706f 7274 205f 7369 6e67  ils import _sing
+00000110: 6c65 2c20 5f70 6169 722c 205f 7472 6970  le, _pair, _trip
+00000120: 6c65 0d0a 6672 6f6d 2074 6f72 6368 2e6e  le..from torch.n
+00000130: 6e2e 7061 7261 6d65 7465 7220 696d 706f  n.parameter impo
+00000140: 7274 2050 6172 616d 6574 6572 0d0a 0d0a  rt Parameter....
+00000150: 6672 6f6d 2068 7970 6572 626f 782e 6d75  from hyperbox.mu
+00000160: 7461 626c 6573 2e73 7061 6365 7320 696d  tables.spaces im
+00000170: 706f 7274 2056 616c 7565 5370 6163 650d  port ValueSpace.
+00000180: 0a66 726f 6d20 6879 7065 7262 6f78 2e6d  .from hyperbox.m
+00000190: 7574 6162 6c65 732e 6f70 732e 6261 7365  utables.ops.base
+000001a0: 5f6d 6f64 756c 6520 696d 706f 7274 2046  _module import F
+000001b0: 696e 6567 7261 696e 6564 4d6f 6475 6c65  inegrainedModule
+000001c0: 0d0a 6672 6f6d 2068 7970 6572 626f 782e  ..from hyperbox.
+000001d0: 6d75 7461 626c 6573 2e6f 7073 2e75 7469  mutables.ops.uti
+000001e0: 6c73 2069 6d70 6f72 7420 7375 625f 6669  ls import sub_fi
+000001f0: 6c74 6572 5f73 7461 7274 5f65 6e64 2c20  lter_start_end, 
+00000200: 6973 5f73 6561 7263 6861 626c 650d 0a0d  is_searchable...
+00000210: 0a0d 0a5f 5f61 6c6c 5f5f 203d 205b 0d0a  ...__all__ = [..
+00000220: 2020 2020 2742 6173 6543 6f6e 764e 6427      'BaseConvNd'
+00000230: 2c0d 0a20 2020 2027 436f 6e76 3164 272c  ,..    'Conv1d',
+00000240: 0d0a 2020 2020 2743 6f6e 7632 6427 2c0d  ..    'Conv2d',.
+00000250: 0a20 2020 2027 436f 6e76 3364 270d 0a5d  .    'Conv3d'..]
+00000260: 0d0a 0d0a 0d0a 636c 6173 7320 4261 7365  ......class Base
+00000270: 436f 6e76 4e64 285f 436f 6e76 4e64 2c20  ConvNd(_ConvNd, 
+00000280: 4669 6e65 6772 6169 6e65 644d 6f64 756c  FinegrainedModul
+00000290: 6529 3a0d 0a20 2020 204b 4552 4e45 4c5f  e):..    KERNEL_
+000002a0: 5452 414e 5346 4f52 4d5f 4d4f 4445 203d  TRANSFORM_MODE =
+000002b0: 2031 2023 204e 6f6e 6520 6f72 2031 206f   1 # None or 1 o
+000002c0: 7220 6f74 6865 7220 7365 7474 696e 6773  r other settings
+000002d0: 0d0a 0d0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
+000002e0: 6974 5f5f 280d 0a20 2020 2020 2020 2073  it__(..        s
+000002f0: 656c 662c 0d0a 2020 2020 2020 2020 696e  elf,..        in
+00000300: 5f63 6861 6e6e 656c 733a 2055 6e69 6f6e  _channels: Union
+00000310: 5b69 6e74 2c20 7475 706c 652c 2056 616c  [int, tuple, Val
+00000320: 7565 5370 6163 655d 2c0d 0a20 2020 2020  ueSpace],..     
+00000330: 2020 206f 7574 5f63 6861 6e6e 656c 733a     out_channels:
+00000340: 2055 6e69 6f6e 5b69 6e74 2c20 7475 706c   Union[int, tupl
+00000350: 652c 2056 616c 7565 5370 6163 655d 2c0d  e, ValueSpace],.
+00000360: 0a20 2020 2020 2020 206b 6572 6e65 6c5f  .        kernel_
+00000370: 7369 7a65 3a20 556e 696f 6e5b 696e 742c  size: Union[int,
+00000380: 2074 7570 6c65 2c20 5661 6c75 6553 7061   tuple, ValueSpa
+00000390: 6365 5d2c 0d0a 2020 2020 2020 2020 7374  ce],..        st
+000003a0: 7269 6465 3a20 556e 696f 6e5b 696e 742c  ride: Union[int,
+000003b0: 2074 7570 6c65 2c20 5661 6c75 6553 7061   tuple, ValueSpa
+000003c0: 6365 5d2c 0d0a 2020 2020 2020 2020 7061  ce],..        pa
+000003d0: 6464 696e 673a 2055 6e69 6f6e 5b73 7472  dding: Union[str
+000003e0: 2c20 696e 742c 2074 7570 6c65 2c20 5661  , int, tuple, Va
+000003f0: 6c75 6553 7061 6365 5d2c 0d0a 2020 2020  lueSpace],..    
+00000400: 2020 2020 6469 6c61 7469 6f6e 3a20 556e      dilation: Un
+00000410: 696f 6e5b 696e 742c 2056 616c 7565 5370  ion[int, ValueSp
+00000420: 6163 655d 2c0d 0a20 2020 2020 2020 2067  ace],..        g
+00000430: 726f 7570 733a 2055 6e69 6f6e 5b69 6e74  roups: Union[int
+00000440: 2c20 5661 6c75 6553 7061 6365 5d2c 0d0a  , ValueSpace],..
+00000450: 2020 2020 2020 2020 6269 6173 3a20 626f          bias: bo
+00000460: 6f6c 2c0d 0a20 2020 2020 2020 2070 6164  ol,..        pad
+00000470: 6469 6e67 5f6d 6f64 653a 2073 7472 2c0d  ding_mode: str,.
+00000480: 0a20 2020 2020 2020 2064 6576 6963 653d  .        device=
+00000490: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2064  None,..        d
+000004a0: 7479 7065 3d4e 6f6e 652c 0d0a 2020 2020  type=None,..    
+000004b0: 2020 2020 6175 746f 5f70 6164 6469 6e67      auto_padding
+000004c0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
+000004d0: 0a20 2020 2020 2020 2074 7261 6e73 706f  .        transpo
+000004e0: 7365 643a 2062 6f6f 6c20 3d20 4661 6c73  sed: bool = Fals
+000004f0: 652c 0d0a 2020 2020 2020 2020 6f75 7470  e,..        outp
+00000500: 7574 5f70 6164 6469 6e67 3a20 5475 706c  ut_padding: Tupl
+00000510: 655b 696e 742c 202e 2e2e 5d20 3d20 302c  e[int, ...] = 0,
+00000520: 0d0a 2020 2020 2020 2020 2a2a 6b77 6172  ..        **kwar
+00000530: 6773 0d0a 2020 2020 293a 0d0a 2020 2020  gs..    ):..    
+00000540: 2020 2020 2727 2742 6173 6520 436f 6e76      '''Base Conv
+00000550: 204d 6f64 756c 650d 0a20 2020 2020 2020   Module..       
+00000560: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+00000570: 2020 2020 6175 746f 5f70 6164 6469 6e67      auto_padding
+00000580: 3a20 6966 2073 6574 2074 6f20 7472 7565  : if set to true
+00000590: 2c20 7769 6c6c 2073 6574 2061 2070 726f  , will set a pro
+000005a0: 7065 7220 7061 6464 696e 6720 7369 7a65  per padding size
+000005b0: 2074 6f20 6d61 6b65 206f 7574 7075 7420   to make output 
+000005c0: 7369 7a65 2073 616d 6520 6173 2074 6865  size same as the
+000005d0: 2069 6e70 7574 2073 697a 652e 0d0a 2020   input size...  
+000005e0: 2020 2020 2020 2020 2020 2020 2020 466f                Fo
+000005f0: 7220 6578 616d 706c 652c 2069 6620 6b65  r example, if ke
+00000600: 726e 656c 2073 697a 6520 6973 2033 2c20  rnel size is 3, 
+00000610: 7468 6520 7061 6464 696e 6720 7369 7a65  the padding size
+00000620: 2069 7320 313b 0d0a 2020 2020 2020 2020   is 1;..        
+00000630: 2020 2020 2020 2020 6966 206b 6572 6e65          if kerne
+00000640: 6c5f 7369 7a65 2069 7320 2833 2c37 292c  l_size is (3,7),
+00000650: 2074 6865 2070 6164 6469 6e67 2073 697a   the padding siz
+00000660: 6520 6973 2028 312c 2033 290d 0a20 2020  e is (1, 3)..   
+00000670: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
+00000680: 2020 7365 6c66 2e63 6f6e 765f 6469 6d20    self.conv_dim 
+00000690: 3d20 7365 6c66 2e5f 5f63 6c61 7373 5f5f  = self.__class__
+000006a0: 2e5f 5f6e 616d 655f 5f5b 2d32 5d0d 0a20  .__name__[-2].. 
+000006b0: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+000006c0: 6c66 2e63 6f6e 765f 6469 6d20 696e 205b  lf.conv_dim in [
+000006d0: 2731 272c 2027 3227 2c20 2733 275d 2c20  '1', '2', '3'], 
+000006e0: 2763 6f6e 765f 6469 6d20 6d75 7374 2062  'conv_dim must b
+000006f0: 6520 312c 2032 206f 7220 3327 0d0a 2020  e 1, 2 or 3'..  
+00000700: 2020 2020 2020 7365 6c66 2e63 6f6e 765f        self.conv_
+00000710: 6469 6d20 3d20 696e 7428 7365 6c66 2e63  dim = int(self.c
+00000720: 6f6e 765f 6469 6d29 0d0a 2020 2020 2020  onv_dim)..      
+00000730: 2020 0d0a 2020 2020 2020 2020 5f69 6e5f    ..        _in_
+00000740: 6368 616e 6e65 6c73 203d 2069 6e5f 6368  channels = in_ch
+00000750: 616e 6e65 6c73 2e6d 6178 5f76 616c 7565  annels.max_value
+00000760: 2069 6620 6973 696e 7374 616e 6365 2869   if isinstance(i
+00000770: 6e5f 6368 616e 6e65 6c73 2c20 5661 6c75  n_channels, Valu
+00000780: 6553 7061 6365 2920 656c 7365 2069 6e5f  eSpace) else in_
+00000790: 6368 616e 6e65 6c73 0d0a 2020 2020 2020  channels..      
+000007a0: 2020 5f6f 7574 5f63 6861 6e6e 656c 7320    _out_channels 
+000007b0: 3d20 6f75 745f 6368 616e 6e65 6c73 2e6d  = out_channels.m
+000007c0: 6178 5f76 616c 7565 2069 6620 6973 696e  ax_value if isin
+000007d0: 7374 616e 6365 286f 7574 5f63 6861 6e6e  stance(out_chann
+000007e0: 656c 732c 2056 616c 7565 5370 6163 6529  els, ValueSpace)
+000007f0: 2065 6c73 6520 6f75 745f 6368 616e 6e65   else out_channe
+00000800: 6c73 0d0a 2020 2020 2020 2020 5f6b 6572  ls..        _ker
+00000810: 6e65 6c5f 7369 7a65 203d 206b 6572 6e65  nel_size = kerne
+00000820: 6c5f 7369 7a65 2e6d 6178 5f76 616c 7565  l_size.max_value
+00000830: 2069 6620 6973 696e 7374 616e 6365 286b   if isinstance(k
+00000840: 6572 6e65 6c5f 7369 7a65 2c20 5661 6c75  ernel_size, Valu
+00000850: 6553 7061 6365 2920 656c 7365 206b 6572  eSpace) else ker
+00000860: 6e65 6c5f 7369 7a65 0d0a 2020 2020 2020  nel_size..      
+00000870: 2020 5f73 7472 6964 6520 3d20 7374 7269    _stride = stri
+00000880: 6465 2e6d 6178 5f76 616c 7565 2069 6620  de.max_value if 
+00000890: 6973 696e 7374 616e 6365 2873 7472 6964  isinstance(strid
+000008a0: 652c 2056 616c 7565 5370 6163 6529 2065  e, ValueSpace) e
+000008b0: 6c73 6520 7374 7269 6465 0d0a 2020 2020  lse stride..    
+000008c0: 2020 2020 5f70 6164 6469 6e67 203d 2070      _padding = p
+000008d0: 6164 6469 6e67 2e6d 6178 5f76 616c 7565  adding.max_value
+000008e0: 2069 6620 6973 696e 7374 616e 6365 2870   if isinstance(p
+000008f0: 6164 6469 6e67 2c20 5661 6c75 6553 7061  adding, ValueSpa
+00000900: 6365 2920 656c 7365 2070 6164 6469 6e67  ce) else padding
+00000910: 0d0a 2020 2020 2020 2020 5f64 696c 6174  ..        _dilat
+00000920: 696f 6e20 3d20 6469 6c61 7469 6f6e 2e6d  ion = dilation.m
+00000930: 696e 5f76 616c 7565 2069 6620 6973 696e  in_value if isin
+00000940: 7374 616e 6365 2864 696c 6174 696f 6e2c  stance(dilation,
+00000950: 2056 616c 7565 5370 6163 6529 2065 6c73   ValueSpace) els
+00000960: 6520 6469 6c61 7469 6f6e 0d0a 0d0a 2020  e dilation....  
+00000970: 2020 2020 2020 5f67 726f 7570 7320 3d20        _groups = 
+00000980: 6772 6f75 7073 0d0a 2020 2020 2020 2020  groups..        
+00000990: 6966 2069 7369 6e73 7461 6e63 6528 6772  if isinstance(gr
+000009a0: 6f75 7073 2c20 5661 6c75 6553 7061 6365  oups, ValueSpace
+000009b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000009c0: 6966 2069 7369 6e73 7461 6e63 6528 696e  if isinstance(in
+000009d0: 5f63 6861 6e6e 656c 732c 2056 616c 7565  _channels, Value
+000009e0: 5370 6163 6529 3a0d 0a20 2020 2020 2020  Space):..       
+000009f0: 2020 2020 2020 2020 2069 6620 6772 6f75           if grou
+00000a00: 7073 2069 7320 6e6f 7420 696e 5f63 6861  ps is not in_cha
+00000a10: 6e6e 656c 733a 0d0a 2020 2020 2020 2020  nnels:..        
+00000a20: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00000a30: 7428 2767 726f 7570 7320 6d75 7374 2062  t('groups must b
+00000a40: 6520 7468 6520 7361 6d65 2061 7320 696e  e the same as in
+00000a50: 5f63 6861 6e6e 656c 7320 7768 656e 2069  _channels when i
+00000a60: 6e5f 6368 616e 6e65 6c73 2069 7320 5661  n_channels is Va
+00000a70: 6c75 6553 7061 6365 2729 0d0a 2020 2020  lueSpace')..    
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 6772 6f75 7073 203d 2069 6e5f 6368 616e  groups = in_chan
+00000aa0: 6e65 6c73 0d0a 2020 2020 2020 2020 2020  nels..          
+00000ab0: 2020 2020 2020 5f67 726f 7570 7320 3d20        _groups = 
+00000ac0: 6772 6f75 7073 2e6d 6178 5f76 616c 7565  groups.max_value
+00000ad0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00000ae0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000af0: 2020 2020 205f 6772 6f75 7073 203d 2067       _groups = g
+00000b00: 726f 7570 732e 6d69 6e5f 7661 6c75 650d  roups.min_value.
+00000b10: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00000b20: 666f 726d 6174 5f61 7267 7328 5f6b 6572  format_args(_ker
+00000b30: 6e65 6c5f 7369 7a65 2c20 5f73 7472 6964  nel_size, _strid
+00000b40: 652c 205f 7061 6464 696e 672c 205f 6469  e, _padding, _di
+00000b50: 6c61 7469 6f6e 290d 0a20 2020 2020 2020  lation)..       
+00000b60: 2063 6f6e 765f 6b77 6172 6773 203d 206b   conv_kwargs = k
+00000b70: 7761 7267 730d 0a20 2020 2020 2020 2063  wargs..        c
+00000b80: 6f6e 765f 6b77 6172 6773 2e75 7064 6174  onv_kwargs.updat
+00000b90: 6528 7b0d 0a20 2020 2020 2020 2020 2020  e({..           
+00000ba0: 2027 696e 5f63 6861 6e6e 656c 7327 3a20   'in_channels': 
+00000bb0: 5f69 6e5f 6368 616e 6e65 6c73 2c0d 0a20  _in_channels,.. 
+00000bc0: 2020 2020 2020 2020 2020 2027 6f75 745f             'out_
+00000bd0: 6368 616e 6e65 6c73 273a 205f 6f75 745f  channels': _out_
+00000be0: 6368 616e 6e65 6c73 2c0d 0a20 2020 2020  channels,..     
+00000bf0: 2020 2020 2020 2027 6b65 726e 656c 5f73         'kernel_s
+00000c00: 697a 6527 3a20 7365 6c66 2e6b 6572 6e65  ize': self.kerne
+00000c10: 6c5f 7369 7a65 2c0d 0a20 2020 2020 2020  l_size,..       
+00000c20: 2020 2020 2027 7374 7269 6465 273a 2073       'stride': s
+00000c30: 656c 662e 7374 7269 6465 2c0d 0a20 2020  elf.stride,..   
+00000c40: 2020 2020 2020 2020 2027 7061 6464 696e           'paddin
+00000c50: 6727 3a20 7365 6c66 2e70 6164 6469 6e67  g': self.padding
+00000c60: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
+00000c70: 6469 6c61 7469 6f6e 273a 2073 656c 662e  dilation': self.
+00000c80: 6469 6c61 7469 6f6e 2c0d 0a20 2020 2020  dilation,..     
+00000c90: 2020 2020 2020 2027 7472 616e 7370 6f73         'transpos
+00000ca0: 6564 273a 2074 7261 6e73 706f 7365 642c  ed': transposed,
+00000cb0: 0d0a 2020 2020 2020 2020 2020 2020 276f  ..            'o
+00000cc0: 7574 7075 745f 7061 6464 696e 6727 3a20  utput_padding': 
+00000cd0: 7365 6c66 2e6f 7574 7075 745f 7061 6464  self.output_padd
+00000ce0: 696e 672c 0d0a 2020 2020 2020 2020 2020  ing,..          
+00000cf0: 2020 2767 726f 7570 7327 3a20 5f67 726f    'groups': _gro
+00000d00: 7570 732c 0d0a 2020 2020 2020 2020 2020  ups,..          
+00000d10: 2020 2762 6961 7327 3a20 6269 6173 2c0d    'bias': bias,.
+00000d20: 0a20 2020 2020 2020 2020 2020 2027 7061  .            'pa
+00000d30: 6464 696e 675f 6d6f 6465 273a 2070 6164  dding_mode': pad
+00000d40: 6469 6e67 5f6d 6f64 652c 0d0a 2020 2020  ding_mode,..    
+00000d50: 2020 2020 2020 2020 2764 6576 6963 6527          'device'
+00000d60: 3a20 6465 7669 6365 2c0d 0a20 2020 2020  : device,..     
+00000d70: 2020 2020 2020 2027 6474 7970 6527 3a20         'dtype': 
+00000d80: 6474 7970 652c 0d0a 2020 2020 2020 2020  dtype,..        
+00000d90: 7d29 0d0a 2020 2020 2020 2020 7375 7065  })..        supe
+00000da0: 7228 4261 7365 436f 6e76 4e64 2c20 7365  r(BaseConvNd, se
+00000db0: 6c66 292e 5f5f 696e 6974 5f5f 282a 2a63  lf).__init__(**c
+00000dc0: 6f6e 765f 6b77 6172 6773 290d 0a20 2020  onv_kwargs)..   
+00000dd0: 2020 2020 2073 656c 662e 6973 5f73 6561       self.is_sea
+00000de0: 7263 6820 3d20 7365 6c66 2e69 7353 6561  rch = self.isSea
+00000df0: 7263 6843 6f6e 7628 290d 0a0d 0a20 2020  rchConv()....   
+00000e00: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00000e10: 6365 286b 6572 6e65 6c5f 7369 7a65 2c20  ce(kernel_size, 
+00000e20: 5661 6c75 6553 7061 6365 2920 616e 6420  ValueSpace) and 
+00000e30: 5c0d 0a20 2020 2020 2020 2020 2020 2073  \..            s
+00000e40: 656c 662e 4b45 524e 454c 5f54 5241 4e53  elf.KERNEL_TRANS
+00000e50: 464f 524d 5f4d 4f44 4520 6973 206e 6f74  FORM_MODE is not
+00000e60: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00000e70: 2020 2020 2020 2020 7365 6c66 2e69 6e69          self.ini
+00000e80: 745f 6b65 726e 656c 5f74 7261 6e73 666f  t_kernel_transfo
+00000e90: 726d 5f6d 6174 7269 7828 290d 0a20 2020  rm_matrix()..   
+00000ea0: 200d 0a20 2020 2064 6566 2077 6569 6768   ..    def weigh
+00000eb0: 745f 7374 616e 6461 7264 697a 6174 696f  t_standardizatio
+00000ec0: 6e28 7365 6c66 2c20 7765 6967 6874 293a  n(self, weight):
+00000ed0: 0d0a 2020 2020 2020 2020 7365 6c66 2e57  ..        self.W
+00000ee0: 535f 4550 5320 3d20 3165 2d38 0d0a 2020  S_EPS = 1e-8..  
+00000ef0: 2020 2020 2020 7765 6967 6874 5f6d 6561        weight_mea
+00000f00: 6e20 3d20 280d 0a20 2020 2020 2020 2020  n = (..         
+00000f10: 2020 2077 6569 6768 742e 6d65 616e 2864     weight.mean(d
+00000f20: 696d 3d31 2c20 6b65 6570 6469 6d3d 5472  im=1, keepdim=Tr
+00000f30: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+00000f40: 202e 6d65 616e 2864 696d 3d32 2c20 6b65   .mean(dim=2, ke
+00000f50: 6570 6469 6d3d 5472 7565 290d 0a20 2020  epdim=True)..   
+00000f60: 2020 2020 2020 2020 202e 6d65 616e 2864           .mean(d
+00000f70: 696d 3d33 2c20 6b65 6570 6469 6d3d 5472  im=3, keepdim=Tr
+00000f80: 7565 290d 0a20 2020 2020 2020 2029 0d0a  ue)..        )..
+00000f90: 2020 2020 2020 2020 7765 6967 6874 203d          weight =
+00000fa0: 2077 6569 6768 7420 2d20 7765 6967 6874   weight - weight
+00000fb0: 5f6d 6561 6e0d 0a20 2020 2020 2020 2073  _mean..        s
+00000fc0: 7464 203d 2028 0d0a 2020 2020 2020 2020  td = (..        
+00000fd0: 2020 2020 7765 6967 6874 2e76 6965 7728      weight.view(
+00000fe0: 7765 6967 6874 2e73 697a 6528 3029 2c20  weight.size(0), 
+00000ff0: 2d31 292e 7374 6428 6469 6d3d 3129 2e76  -1).std(dim=1).v
+00001000: 6965 7728 2d31 2c20 312c 2031 2c20 3129  iew(-1, 1, 1, 1)
+00001010: 0d0a 2020 2020 2020 2020 2020 2020 2b20  ..            + 
+00001020: 7365 6c66 2e57 535f 4550 530d 0a20 2020  self.WS_EPS..   
+00001030: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00001040: 7765 6967 6874 203d 2077 6569 6768 7420  weight = weight 
+00001050: 2f20 7374 642e 6578 7061 6e64 5f61 7328  / std.expand_as(
+00001060: 7765 6967 6874 290d 0a20 2020 2020 2020  weight)..       
+00001070: 2072 6574 7572 6e20 7765 6967 6874 0d0a   return weight..
+00001080: 0d0a 2020 2020 6465 6620 696e 6974 5f6b  ..    def init_k
+00001090: 6572 6e65 6c5f 7472 616e 7366 6f72 6d5f  ernel_transform_
+000010a0: 6d61 7472 6978 2873 656c 6629 3a0d 0a20  matrix(self):.. 
+000010b0: 2020 2020 2020 2023 2072 6567 6973 7465         # registe
+000010c0: 7220 7363 616c 696e 6720 7061 7261 6d65  r scaling parame
+000010d0: 7465 7273 0d0a 2020 2020 2020 2020 2320  ters..        # 
+000010e0: 3774 6f35 5f6d 6174 7269 782c 2035 746f  7to5_matrix, 5to
+000010f0: 335f 6d61 7472 6978 0d0a 2020 2020 2020  3_matrix..      
+00001100: 2020 6b65 726e 656c 5f73 697a 6520 3d20    kernel_size = 
+00001110: 7365 6c66 2e76 616c 7565 5f73 7061 6365  self.value_space
+00001120: 735b 276b 6572 6e65 6c5f 7369 7a65 275d  s['kernel_size']
+00001130: 2e63 616e 6469 6461 7465 735f 6f72 6967  .candidates_orig
+00001140: 696e 616c 0d0a 2020 2020 2020 2020 7363  inal..        sc
+00001150: 616c 655f 7061 7261 6d73 203d 207b 7d0d  ale_params = {}.
+00001160: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+00001170: 6e20 7261 6e67 6528 6c65 6e28 6b65 726e  n range(len(kern
+00001180: 656c 5f73 697a 6529 202d 2031 293a 0d0a  el_size) - 1):..
+00001190: 2020 2020 2020 2020 2020 2020 6b73 5f73              ks_s
+000011a0: 6d61 6c6c 203d 206b 6572 6e65 6c5f 7369  mall = kernel_si
+000011b0: 7a65 5b69 5d0d 0a20 2020 2020 2020 2020  ze[i]..         
+000011c0: 2020 206b 735f 6c61 7267 6572 203d 206b     ks_larger = k
+000011d0: 6572 6e65 6c5f 7369 7a65 5b69 202b 2031  ernel_size[i + 1
+000011e0: 5d0d 0a20 2020 2020 2020 2020 2020 2070  ]..            p
+000011f0: 6172 616d 5f6e 616d 6520 3d20 2725 6474  aram_name = '%dt
+00001200: 6f25 6427 2025 2028 6b73 5f6c 6172 6765  o%d' % (ks_large
+00001210: 722c 206b 735f 736d 616c 6c29 0d0a 2020  r, ks_small)..  
+00001220: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00001230: 7061 7261 6d73 5b27 2573 5f6d 6174 7269  params['%s_matri
+00001240: 7827 2025 2070 6172 616d 5f6e 616d 655d  x' % param_name]
+00001250: 203d 2050 6172 616d 6574 6572 2874 6f72   = Parameter(tor
+00001260: 6368 2e65 7965 286b 735f 736d 616c 6c20  ch.eye(ks_small 
+00001270: 2a2a 2073 656c 662e 636f 6e76 5f64 696d  ** self.conv_dim
+00001280: 2929 0d0a 2020 2020 2020 2020 666f 7220  ))..        for 
+00001290: 6e61 6d65 2c20 7061 7261 6d20 696e 2073  name, param in s
+000012a0: 6361 6c65 5f70 6172 616d 732e 6974 656d  cale_params.item
+000012b0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+000012c0: 2020 7365 6c66 2e72 6567 6973 7465 725f    self.register_
+000012d0: 7061 7261 6d65 7465 7228 6e61 6d65 2c20  parameter(name, 
+000012e0: 7061 7261 6d29 0d0a 0d0a 2020 2020 6465  param)....    de
+000012f0: 6620 666f 726d 6174 5f61 7267 7328 7365  f format_args(se
+00001300: 6c66 2c20 2a61 7267 732c 202a 2a6b 7761  lf, *args, **kwa
+00001310: 7267 7329 3a0d 0a20 2020 2020 2020 2027  rgs):..        '
+00001320: 2727 4765 6e65 7261 7465 2043 6f6e 7620  ''Generate Conv 
+00001330: 6f70 6572 6174 696f 6e27 2727 0d0a 2020  operation'''..  
+00001340: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+00001350: 6d70 6c65 6d65 6e74 6564 4572 726f 720d  mplementedError.
+00001360: 0a0d 0a20 2020 2064 6566 2069 7353 6561  ...    def isSea
+00001370: 7263 6843 6f6e 7628 7365 6c66 293a 0d0a  rchConv(self):..
+00001380: 2020 2020 2020 2020 2727 2753 6561 7263          '''Searc
+00001390: 6820 666c 6167 0d0a 2020 2020 2020 2020  h flag..        
+000013a0: 5375 7070 6f72 7465 6420 6172 6775 6d65  Supported argume
+000013b0: 6e74 730d 0a20 2020 2020 2020 2020 2020  nts..           
+000013c0: 202d 2073 6561 7263 685f 696e 5f63 6861   - search_in_cha
+000013d0: 6e6e 656c 0d0a 2020 2020 2020 2020 2020  nnel..          
+000013e0: 2020 2d20 7365 6172 6368 5f6f 7574 5f63    - search_out_c
+000013f0: 6861 6e6e 656c 0d0a 2020 2020 2020 2020  hannel..        
+00001400: 2020 2020 2d20 7365 6172 6368 5f6b 6572      - search_ker
+00001410: 6e65 6c5f 7369 7a65 0d0a 2020 2020 2020  nel_size..      
+00001420: 2020 2020 2020 2d20 7365 6172 6368 5f73        - search_s
+00001430: 7472 6964 650d 0a20 2020 2020 2020 2020  tride..         
+00001440: 2020 202d 2073 6561 7263 685f 6469 6c61     - search_dila
+00001450: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+00001460: 2020 2d20 7365 6172 6368 5f67 726f 7570    - search_group
+00001470: 730d 0a20 2020 2020 2020 2027 2727 0d0a  s..        '''..
+00001480: 2020 2020 2020 2020 7365 6c66 2e73 6561          self.sea
+00001490: 7263 685f 696e 5f63 6861 6e6e 656c 203d  rch_in_channel =
+000014a0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+000014b0: 7365 6c66 2e73 6561 7263 685f 6f75 745f  self.search_out_
+000014c0: 6368 616e 6e65 6c20 3d20 4661 6c73 650d  channel = False.
+000014d0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+000014e0: 6172 6368 5f6b 6572 6e65 6c5f 7369 7a65  arch_kernel_size
+000014f0: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+00001500: 2020 7365 6c66 2e73 6561 7263 685f 7374    self.search_st
+00001510: 7269 6465 203d 2046 616c 7365 0d0a 2020  ride = False..  
+00001520: 2020 2020 2020 7365 6c66 2e73 6561 7263        self.searc
+00001530: 685f 6469 6c61 7469 6f6e 203d 2046 616c  h_dilation = Fal
+00001540: 7365 0d0a 2020 2020 2020 2020 7365 6c66  se..        self
+00001550: 2e73 6561 7263 685f 6772 6f75 7073 203d  .search_groups =
+00001560: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00001570: 2320 7365 6c66 2e73 6561 7263 685f 6269  # self.search_bi
+00001580: 6173 203d 2046 616c 7365 0d0a 0d0a 2020  as = False....  
+00001590: 2020 2020 2020 6966 2061 6c6c 285b 6e6f        if all([no
+000015a0: 7420 7673 2e69 735f 7365 6172 6368 2066  t vs.is_search f
+000015b0: 6f72 2076 7320 696e 2073 656c 662e 7661  or vs in self.va
+000015c0: 6c75 655f 7370 6163 6573 2e76 616c 7565  lue_spaces.value
+000015d0: 7328 295d 293a 0d0a 2020 2020 2020 2020  s()]):..        
+000015e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000015f0: 0d0a 0d0a 2020 2020 2020 2020 6966 2020  ....        if  
+00001600: 6973 5f73 6561 7263 6861 626c 6528 6765  is_searchable(ge
+00001610: 7461 7474 7228 7365 6c66 2e76 616c 7565  tattr(self.value
+00001620: 5f73 7061 6365 732c 2027 696e 5f63 6861  _spaces, 'in_cha
+00001630: 6e6e 656c 7327 2c20 4e6f 6e65 2929 3a0d  nnels', None)):.
+00001640: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001650: 662e 7365 6172 6368 5f69 6e5f 6368 616e  f.search_in_chan
+00001660: 6e65 6c20 3d20 5472 7565 0d0a 2020 2020  nel = True..    
+00001670: 2020 2020 6966 2020 6973 5f73 6561 7263      if  is_searc
+00001680: 6861 626c 6528 6765 7461 7474 7228 7365  hable(getattr(se
+00001690: 6c66 2e76 616c 7565 5f73 7061 6365 732c  lf.value_spaces,
+000016a0: 2027 6f75 745f 6368 616e 6e65 6c73 272c   'out_channels',
+000016b0: 204e 6f6e 6529 293a 0d0a 2020 2020 2020   None)):..      
+000016c0: 2020 2020 2020 7365 6c66 2e73 6561 7263        self.searc
+000016d0: 685f 6f75 745f 6368 616e 6e65 6c20 3d20  h_out_channel = 
+000016e0: 5472 7565 0d0a 2020 2020 2020 2020 6966  True..        if
+000016f0: 2020 6973 5f73 6561 7263 6861 626c 6528    is_searchable(
+00001700: 6765 7461 7474 7228 7365 6c66 2e76 616c  getattr(self.val
+00001710: 7565 5f73 7061 6365 732c 2027 6b65 726e  ue_spaces, 'kern
+00001720: 656c 5f73 697a 6527 2c20 4e6f 6e65 2929  el_size', None))
+00001730: 3a0d 0a20 2020 2020 2020 2020 2020 206b  :..            k
+00001740: 6572 6e65 6c5f 6361 6e64 6964 6174 6573  ernel_candidates
+00001750: 203d 2073 656c 662e 7661 6c75 655f 7370   = self.value_sp
+00001760: 6163 6573 5b27 6b65 726e 656c 5f73 697a  aces['kernel_siz
+00001770: 6527 5d2e 6361 6e64 6964 6174 6573 0d0a  e'].candidates..
+00001780: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+00001790: 6b20 3d20 7365 6c66 2e6b 6572 6e65 6c5f  k = self.kernel_
+000017a0: 7369 7a65 0d0a 2020 2020 2020 2020 2020  size..          
+000017b0: 2020 2320 546f 646f 3a20 e4b8 8e60 7472    # Todo: ...`tr
+000017c0: 616e 7366 6f72 6d5f 6b65 726e 656c 5f73  ansform_kernel_s
+000017d0: 697a 6560 e690 ade9 858d e4bd bfe7 94a8  ize`............
+000017e0: efbc 8ce7 9bae e589 8de6 9caa e4bd bfe7  ................
+000017f0: 94a8 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00001800: 7365 6c66 2e73 6561 7263 685f 6b65 726e  self.search_kern
+00001810: 656c 5f73 697a 6520 3d20 5472 7565 0d0a  el_size = True..
+00001820: 2020 2020 2020 2020 6966 2020 6973 5f73          if  is_s
+00001830: 6561 7263 6861 626c 6528 6765 7461 7474  earchable(getatt
+00001840: 7228 7365 6c66 2e76 616c 7565 5f73 7061  r(self.value_spa
+00001850: 6365 732c 2027 7374 7269 6465 272c 204e  ces, 'stride', N
+00001860: 6f6e 6529 293a 0d0a 2020 2020 2020 2020  one)):..        
+00001870: 2020 2020 7365 6c66 2e73 6561 7263 685f      self.search_
+00001880: 7374 7269 6465 203d 2054 7275 650d 0a20  stride = True.. 
+00001890: 2020 2020 2020 2069 6620 2069 735f 7365         if  is_se
+000018a0: 6172 6368 6162 6c65 2867 6574 6174 7472  archable(getattr
+000018b0: 2873 656c 662e 7661 6c75 655f 7370 6163  (self.value_spac
+000018c0: 6573 2c20 2764 696c 6174 696f 6e27 2c20  es, 'dilation', 
+000018d0: 4e6f 6e65 2929 3a0d 0a20 2020 2020 2020  None)):..       
+000018e0: 2020 2020 2073 656c 662e 7365 6172 6368       self.search
+000018f0: 5f64 696c 6174 696f 6e20 3d20 5472 7565  _dilation = True
+00001900: 0d0a 2020 2020 2020 2020 6966 2020 6973  ..        if  is
+00001910: 5f73 6561 7263 6861 626c 6528 6765 7461  _searchable(geta
+00001920: 7474 7228 7365 6c66 2e76 616c 7565 5f73  ttr(self.value_s
+00001930: 7061 6365 732c 2027 6772 6f75 7073 272c  paces, 'groups',
+00001940: 204e 6f6e 6529 293a 0d0a 2020 2020 2020   None)):..      
+00001950: 2020 2020 2020 7365 6c66 2e73 6561 7263        self.searc
+00001960: 685f 6772 6f75 7073 203d 2054 7275 650d  h_groups = True.
+00001970: 0a20 2020 2020 2020 2023 2069 6620 2069  .        # if  i
+00001980: 735f 7365 6172 6368 6162 6c65 2867 6574  s_searchable(get
+00001990: 6174 7472 2873 656c 662e 7661 6c75 655f  attr(self.value_
+000019a0: 7370 6163 6573 2c20 2762 6961 7327 2c20  spaces, 'bias', 
+000019b0: 4e6f 6e65 2929 3a0d 0a20 2020 2020 2020  None)):..       
+000019c0: 2023 2020 2020 2073 656c 662e 7365 6172   #     self.sear
+000019d0: 6368 5f62 6961 7320 3d20 5472 7565 0d0a  ch_bias = True..
+000019e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000019f0: 2054 7275 650d 0a0d 0a20 2020 2023 2323   True....    ###
+00001a00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001a10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001a20: 2323 2323 2323 2323 0d0a 2020 2020 2320  ########..    # 
+00001a30: 666f 7277 6172 6420 696d 706c 656d 656e  forward implemen
+00001a40: 7461 7469 6f6e 0d0a 2020 2020 2320 2d20  tation..    # - 
+00001a50: 666f 7277 6172 645f 636f 6e76 0d0a 2020  forward_conv..  
+00001a60: 2020 2320 2020 2d20 7472 616e 7366 6f72    #   - transfor
+00001a70: 6d5f 6b65 726e 656c 5f73 697a 650d 0a20  m_kernel_size.. 
+00001a80: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+00001a90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001aa0: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
+00001ab0: 0d0a 2020 2020 6465 6620 666f 7277 6172  ..    def forwar
+00001ac0: 6428 7365 6c66 2c20 7829 3a0d 0a20 2020  d(self, x):..   
+00001ad0: 2020 2020 206f 7574 203d 204e 6f6e 650d       out = None.
+00001ae0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00001af0: 7365 6c66 2e69 735f 7365 6172 6368 3a0d  self.is_search:.
+00001b00: 0a20 2020 2020 2020 2020 2020 2070 6164  .            pad
+00001b10: 6469 6e67 203d 2073 656c 662e 7061 6464  ding = self.padd
+00001b20: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
+00001b30: 2069 6620 7365 6c66 2e61 7574 6f5f 7061   if self.auto_pa
+00001b40: 6464 696e 673a 0d0a 2020 2020 2020 2020  dding:..        
+00001b50: 2020 2020 2020 2020 6b65 726e 656c 5f73          kernel_s
+00001b60: 697a 6520 3d20 7365 6c66 2e77 6569 6768  ize = self.weigh
+00001b70: 742e 7368 6170 655b 323a 5d0d 0a20 2020  t.shape[2:]..   
+00001b80: 2020 2020 2020 2020 2020 2020 2070 6164               pad
+00001b90: 6469 6e67 203d 205b 5d0d 0a20 2020 2020  ding = []..     
+00001ba0: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+00001bb0: 2069 6e20 6b65 726e 656c 5f73 697a 653a   in kernel_size:
+00001bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001bd0: 2020 2020 2020 7061 6464 696e 672e 6170        padding.ap
+00001be0: 7065 6e64 286b 2f2f 3229 0d0a 2020 2020  pend(k//2)..    
+00001bf0: 2020 2020 2020 2020 6f75 7420 3d20 7365          out = se
+00001c00: 6c66 2e63 6f6e 7628 782c 2073 656c 662e  lf.conv(x, self.
+00001c10: 7765 6967 6874 2c20 7365 6c66 2e62 6961  weight, self.bia
+00001c20: 732c 2073 656c 662e 7374 7269 6465 2c0d  s, self.stride,.
+00001c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c40: 2070 6164 6469 6e67 2c20 7365 6c66 2e64   padding, self.d
+00001c50: 696c 6174 696f 6e2c 2073 656c 662e 6772  ilation, self.gr
+00001c60: 6f75 7073 290d 0a20 2020 2020 2020 2065  oups)..        e
+00001c70: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00001c80: 2020 6f75 7420 3d20 7365 6c66 2e66 6f72    out = self.for
+00001c90: 7761 7264 5f63 6f6e 7628 7829 0d0a 2020  ward_conv(x)..  
+00001ca0: 2020 2020 2020 7265 7475 726e 206f 7574        return out
+00001cb0: 0d0a 0d0a 2020 2020 6465 6620 666f 7277  ....    def forw
+00001cc0: 6172 645f 636f 6e76 2873 656c 662c 2078  ard_conv(self, x
+00001cd0: 293a 0d0a 2020 2020 2020 2020 6669 6c74  ):..        filt
+00001ce0: 6572 7320 3d20 7365 6c66 2e77 6569 6768  ers = self.weigh
+00001cf0: 742e 636f 6e74 6967 756f 7573 2829 0d0a  t.contiguous()..
+00001d00: 2020 2020 2020 2020 6269 6173 203d 2073          bias = s
+00001d10: 656c 662e 6269 6173 0d0a 2020 2020 2020  elf.bias..      
+00001d20: 2020 696e 5f63 6861 6e6e 656c 7320 3d20    in_channels = 
+00001d30: 7365 6c66 2e69 6e5f 6368 616e 6e65 6c73  self.in_channels
+00001d40: 0d0a 2020 2020 2020 2020 6f75 745f 6368  ..        out_ch
+00001d50: 616e 6e65 6c73 203d 2073 656c 662e 6f75  annels = self.ou
+00001d60: 745f 6368 616e 6e65 6c73 0d0a 2020 2020  t_channels..    
+00001d70: 2020 2020 7374 7269 6465 203d 2073 656c      stride = sel
+00001d80: 662e 7661 6c75 655f 7370 6163 6573 5b27  f.value_spaces['
+00001d90: 7374 7269 6465 275d 2e76 616c 7565 2069  stride'].value i
+00001da0: 6620 7365 6c66 2e73 6561 7263 685f 7374  f self.search_st
+00001db0: 7269 6465 2065 6c73 6520 7365 6c66 2e73  ride else self.s
+00001dc0: 7472 6964 650d 0a20 2020 2020 2020 2067  tride..        g
+00001dd0: 726f 7570 7320 3d20 7365 6c66 2e76 616c  roups = self.val
+00001de0: 7565 5f73 7061 6365 735b 2767 726f 7570  ue_spaces['group
+00001df0: 7327 5d2e 7661 6c75 6520 6966 2073 656c  s'].value if sel
+00001e00: 662e 7365 6172 6368 5f67 726f 7570 7320  f.search_groups 
+00001e10: 656c 7365 2073 656c 662e 6772 6f75 7073  else self.groups
+00001e20: 0d0a 2020 2020 2020 2020 6469 6c61 7469  ..        dilati
+00001e30: 6f6e 203d 2073 656c 662e 7661 6c75 655f  on = self.value_
+00001e40: 7370 6163 6573 5b27 6469 6c61 7469 6f6e  spaces['dilation
+00001e50: 275d 2e76 616c 7565 2069 6620 7365 6c66  '].value if self
+00001e60: 2e73 6561 7263 685f 6469 6c61 7469 6f6e  .search_dilation
+00001e70: 2065 6c73 6520 7365 6c66 2e64 696c 6174   else self.dilat
+00001e80: 696f 6e0d 0a20 2020 2020 2020 2070 6164  ion..        pad
+00001e90: 6469 6e67 203d 2073 656c 662e 7061 6464  ding = self.padd
+00001ea0: 696e 670d 0a0d 0a20 2020 2020 2020 2069  ing....        i
+00001eb0: 6620 7365 6c66 2e73 6561 7263 685f 696e  f self.search_in
+00001ec0: 5f63 6861 6e6e 656c 3a0d 0a20 2020 2020  _channel:..     
+00001ed0: 2020 2020 2020 2069 6e5f 6368 616e 6e65         in_channe
+00001ee0: 6c73 203d 2073 656c 662e 7661 6c75 655f  ls = self.value_
+00001ef0: 7370 6163 6573 5b27 696e 5f63 6861 6e6e  spaces['in_chann
+00001f00: 656c 7327 5d2e 7661 6c75 650d 0a20 2020  els'].value..   
+00001f10: 2020 2020 2020 2020 2066 696c 7465 7273           filters
+00001f20: 203d 2066 696c 7465 7273 5b3a 2c20 3a69   = filters[:, :i
+00001f30: 6e5f 6368 616e 6e65 6c73 2c20 2e2e 2e5d  n_channels, ...]
+00001f40: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00001f50: 662e 7365 6172 6368 5f6f 7574 5f63 6861  f.search_out_cha
+00001f60: 6e6e 656c 3a0d 0a20 2020 2020 2020 2020  nnel:..         
+00001f70: 2020 206f 7574 5f63 6861 6e6e 656c 7320     out_channels 
+00001f80: 3d20 7365 6c66 2e76 616c 7565 5f73 7061  = self.value_spa
+00001f90: 6365 735b 276f 7574 5f63 6861 6e6e 656c  ces['out_channel
+00001fa0: 7327 5d2e 7661 6c75 650d 0a20 2020 2020  s'].value..     
+00001fb0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00001fc0: 6961 7320 6973 206e 6f74 204e 6f6e 653a  ias is not None:
+00001fd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001fe0: 2020 6269 6173 203d 2062 6961 735b 3a6f    bias = bias[:o
+00001ff0: 7574 5f63 6861 6e6e 656c 735d 0d0a 2020  ut_channels]..  
+00002000: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
+00002010: 7320 3d20 6669 6c74 6572 735b 3a6f 7574  s = filters[:out
+00002020: 5f63 6861 6e6e 656c 732c 202e 2e2e 5d0d  _channels, ...].
+00002030: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00002040: 2e73 6561 7263 685f 6b65 726e 656c 5f73  .search_kernel_s
+00002050: 697a 653a 0d0a 2020 2020 2020 2020 2020  ize:..          
+00002060: 2020 6669 6c74 6572 7320 3d20 7365 6c66    filters = self
+00002070: 2e74 7261 6e73 666f 726d 5f6b 6572 6e65  .transform_kerne
+00002080: 6c5f 7369 7a65 2866 696c 7465 7273 290d  l_size(filters).
+00002090: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000020a0: 2e73 6561 7263 685f 6772 6f75 7073 2061  .search_groups a
+000020b0: 6e64 206e 6f74 2073 656c 662e 7365 6172  nd not self.sear
+000020c0: 6368 5f69 6e5f 6368 616e 6e65 6c3a 0d0a  ch_in_channel:..
+000020d0: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+000020e0: 6572 7320 3d20 7365 6c66 2e67 6574 5f66  ers = self.get_f
+000020f0: 696c 7465 7273 5f62 795f 6772 6f75 7073  ilters_by_groups
+00002100: 2866 696c 7465 7273 2c20 696e 5f63 6861  (filters, in_cha
+00002110: 6e6e 656c 732c 2067 726f 7570 7329 2e63  nnels, groups).c
+00002120: 6f6e 7469 6775 6f75 7328 290d 0a20 2020  ontiguous()..   
+00002130: 2020 2020 2069 6620 7365 6c66 2e61 7574       if self.aut
+00002140: 6f5f 7061 6464 696e 673a 0d0a 2020 2020  o_padding:..    
+00002150: 2020 2020 2020 2020 6b65 726e 656c 5f73          kernel_s
+00002160: 697a 6520 3d20 6669 6c74 6572 732e 7368  ize = filters.sh
+00002170: 6170 655b 323a 5d0d 0a20 2020 2020 2020  ape[2:]..       
+00002180: 2020 2020 2070 6164 6469 6e67 203d 205b       padding = [
+00002190: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
+000021a0: 6f72 206b 2069 6e20 6b65 726e 656c 5f73  or k in kernel_s
+000021b0: 697a 653a 0d0a 2020 2020 2020 2020 2020  ize:..          
+000021c0: 2020 2020 2020 7061 6464 696e 672e 6170        padding.ap
+000021d0: 7065 6e64 286b 2f2f 3229 0d0a 2020 2020  pend(k//2)..    
+000021e0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000021f0: 636f 6e76 2878 2c20 6669 6c74 6572 732c  conv(x, filters,
+00002200: 2062 6961 732c 2073 7472 6964 652c 2070   bias, stride, p
+00002210: 6164 6469 6e67 2c20 6469 6c61 7469 6f6e  adding, dilation
+00002220: 2c20 6772 6f75 7073 290d 0a0d 0a20 2020  , groups)....   
+00002230: 2064 6566 2067 6574 5f66 696c 7465 7273   def get_filters
+00002240: 5f62 795f 6772 6f75 7073 2873 656c 662c  _by_groups(self,
+00002250: 2066 696c 7465 7273 2c20 696e 5f63 6861   filters, in_cha
+00002260: 6e6e 656c 732c 2067 726f 7570 7329 3a0d  nnels, groups):.
+00002270: 0a20 2020 2020 2020 2027 2727 4765 7420  .        '''Get 
+00002280: 6669 6c74 6572 7320 7768 656e 2073 6561  filters when sea
+00002290: 7263 6869 6e67 2066 6f72 2023 6f66 2067  rching for #of g
+000022a0: 726f 7570 7327 2727 0d0a 2020 2020 2020  roups'''..      
+000022b0: 2020 6966 2067 726f 7570 7320 3d3d 2031    if groups == 1
+000022c0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000022d0: 6574 7572 6e20 6669 6c74 6572 730d 0a20  eturn filters.. 
+000022e0: 2020 2020 2020 2073 7562 5f69 6e5f 6368         sub_in_ch
+000022f0: 616e 6e65 6c73 203d 2069 6e5f 6368 616e  annels = in_chan
+00002300: 6e65 6c73 202f 2f20 6772 6f75 7073 0d0a  nels // groups..
+00002310: 2020 2020 2020 2020 7375 625f 7261 7469          sub_rati
+00002320: 6f20 3d20 6669 6c74 6572 732e 7369 7a65  o = filters.size
+00002330: 2831 2920 2f2f 2073 7562 5f69 6e5f 6368  (1) // sub_in_ch
+00002340: 616e 6e65 6c73 0d0a 0d0a 2020 2020 2020  annels....      
+00002350: 2020 6669 6c74 6572 5f63 726f 7073 203d    filter_crops =
+00002360: 205b 5d0d 0a20 2020 2020 2020 2073 7562   []..        sub
+00002370: 5f66 696c 7465 7273 203d 2074 6f72 6368  _filters = torch
+00002380: 2e63 6875 6e6b 2866 696c 7465 7273 2c20  .chunk(filters, 
+00002390: 6772 6f75 7073 2c20 6469 6d3d 3029 0d0a  groups, dim=0)..
+000023a0: 2020 2020 2020 2020 666f 7220 692c 2073          for i, s
+000023b0: 7562 5f66 696c 7465 7220 696e 2065 6e75  ub_filter in enu
+000023c0: 6d65 7261 7465 2873 7562 5f66 696c 7465  merate(sub_filte
+000023d0: 7273 293a 0d0a 2020 2020 2020 2020 2020  rs):..          
+000023e0: 2020 7061 7274 5f69 6420 3d20 6920 2520    part_id = i % 
+000023f0: 7375 625f 7261 7469 6f0d 0a20 2020 2020  sub_ratio..     
+00002400: 2020 2020 2020 2073 7461 7274 203d 2070         start = p
+00002410: 6172 745f 6964 202a 2073 7562 5f69 6e5f  art_id * sub_in_
+00002420: 6368 616e 6e65 6c73 0d0a 2020 2020 2020  channels..      
+00002430: 2020 2020 2020 6669 6c74 6572 5f63 726f        filter_cro
+00002440: 7073 2e61 7070 656e 6428 7375 625f 6669  ps.append(sub_fi
+00002450: 6c74 6572 5b3a 2c20 7374 6172 743a 7374  lter[:, start:st
+00002460: 6172 7420 2b20 7375 625f 696e 5f63 6861  art + sub_in_cha
+00002470: 6e6e 656c 732c 203a 2c20 3a5d 290d 0a20  nnels, :, :]).. 
+00002480: 2020 2020 2020 2066 696c 7465 7273 203d         filters =
+00002490: 2074 6f72 6368 2e63 6174 2866 696c 7465   torch.cat(filte
+000024a0: 725f 6372 6f70 732c 2064 696d 3d30 290d  r_crops, dim=0).
+000024b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000024c0: 6669 6c74 6572 730d 0a0d 0a20 2020 2064  filters....    d
+000024d0: 6566 2074 7261 6e73 666f 726d 5f6b 6572  ef transform_ker
+000024e0: 6e65 6c5f 7369 7a65 2873 656c 662c 2066  nel_size(self, f
+000024f0: 696c 7465 7273 293a 2020 2020 2020 2020  ilters):        
+00002500: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00002510: 662e 4b45 524e 454c 5f54 5241 4e53 464f  f.KERNEL_TRANSFO
+00002520: 524d 5f4d 4f44 4520 6973 204e 6f6e 653a  RM_MODE is None:
+00002530: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00002540: 7072 696e 7428 2776 616e 696c 6c61 2074  print('vanilla t
+00002550: 7261 6e73 666f 726d 5f6b 6572 6e65 6c5f  ransform_kernel_
+00002560: 7369 7a65 2729 0d0a 2020 2020 2020 2020  size')..        
+00002570: 2020 2020 7375 625f 6b65 726e 656c 5f73      sub_kernel_s
+00002580: 697a 6520 3d20 7365 6c66 2e76 616c 7565  ize = self.value
+00002590: 5f73 7061 6365 735b 276b 6572 6e65 6c5f  _spaces['kernel_
+000025a0: 7369 7a65 275d 2e76 616c 7565 0d0a 2020  size'].value..  
+000025b0: 2020 2020 2020 2020 2020 7374 6172 742c            start,
+000025c0: 2065 6e64 203d 2073 7562 5f66 696c 7465   end = sub_filte
+000025d0: 725f 7374 6172 745f 656e 6428 7365 6c66  r_start_end(self
+000025e0: 2e6b 6572 6e65 6c5f 7369 7a65 2c20 7375  .kernel_size, su
+000025f0: 625f 6b65 726e 656c 5f73 697a 6529 0d0a  b_kernel_size)..
+00002600: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00002610: 656c 662e 636f 6e76 5f64 696d 3d3d 313a  elf.conv_dim==1:
+00002620: 2066 696c 7465 7273 203d 2066 696c 7465   filters = filte
+00002630: 7273 5b3a 2c20 3a2c 2073 7461 7274 3a65  rs[:, :, start:e
+00002640: 6e64 5d0d 0a20 2020 2020 2020 2020 2020  nd]..           
+00002650: 2069 6620 7365 6c66 2e63 6f6e 765f 6469   if self.conv_di
+00002660: 6d3d 3d32 3a20 6669 6c74 6572 7320 3d20  m==2: filters = 
+00002670: 6669 6c74 6572 735b 3a2c 203a 2c20 7374  filters[:, :, st
+00002680: 6172 743a 656e 642c 2073 7461 7274 3a65  art:end, start:e
+00002690: 6e64 5d0d 0a20 2020 2020 2020 2020 2020  nd]..           
+000026a0: 2069 6620 7365 6c66 2e63 6f6e 765f 6469   if self.conv_di
+000026b0: 6d3d 3d33 3a20 6669 6c74 6572 7320 3d20  m==3: filters = 
+000026c0: 6669 6c74 6572 735b 3a2c 203a 2c20 7374  filters[:, :, st
+000026d0: 6172 743a 656e 642c 2073 7461 7274 3a65  art:end, start:e
+000026e0: 6e64 2c20 7374 6172 743a 656e 645d 0d0a  nd, start:end]..
+000026f0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00002700: 2020 2020 2020 2020 2020 206d 6178 5f6b             max_k
+00002710: 6572 6e65 6c5f 7369 7a65 203d 2073 656c  ernel_size = sel
+00002720: 662e 6b65 726e 656c 5f73 697a 650d 0a20  f.kernel_size.. 
+00002730: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00002740: 696e 7374 616e 6365 286d 6178 5f6b 6572  instance(max_ker
+00002750: 6e65 6c5f 7369 7a65 2c20 2874 7570 6c65  nel_size, (tuple
+00002760: 2c20 6c69 7374 2929 3a0d 0a20 2020 2020  , list)):..     
+00002770: 2020 2020 2020 2020 2020 206d 6178 5f6b             max_k
+00002780: 6572 6e65 6c5f 7369 7a65 203d 206d 6178  ernel_size = max
+00002790: 286d 6178 5f6b 6572 6e65 6c5f 7369 7a65  (max_kernel_size
+000027a0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+000027b0: 7562 5f6b 6572 6e65 6c5f 7369 7a65 203d  ub_kernel_size =
+000027c0: 2073 656c 662e 7661 6c75 655f 7370 6163   self.value_spac
+000027d0: 6573 5b27 6b65 726e 656c 5f73 697a 6527  es['kernel_size'
+000027e0: 5d2e 7661 6c75 650d 0a20 2020 2020 2020  ].value..       
+000027f0: 2020 2020 206b 735f 7365 7420 3d20 7365       ks_set = se
+00002800: 6c66 2e76 616c 7565 5f73 7061 6365 735b  lf.value_spaces[
+00002810: 276b 6572 6e65 6c5f 7369 7a65 275d 2e63  'kernel_size'].c
+00002820: 616e 6469 6461 7465 730d 0a20 2020 2020  andidates..     
+00002830: 2020 2020 2020 2069 6620 7375 625f 6b65         if sub_ke
+00002840: 726e 656c 5f73 697a 6520 3c20 6d61 785f  rnel_size < max_
+00002850: 6b65 726e 656c 5f73 697a 653a 0d0a 2020  kernel_size:..  
+00002860: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00002870: 6172 745f 6669 6c74 6572 203d 2066 696c  art_filter = fil
+00002880: 7465 7273 0d0a 2020 2020 2020 2020 2020  ters..          
+00002890: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+000028a0: 616e 6765 286c 656e 286b 735f 7365 7429  ange(len(ks_set)
+000028b0: 2d31 2c20 302c 202d 3129 3a0d 0a20 2020  -1, 0, -1):..   
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2073 7263 5f6b 7320 3d20 6b73 5f73 6574   src_ks = ks_set
+000028e0: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
+000028f0: 2020 2020 2020 2020 2069 6620 7372 635f           if src_
+00002900: 6b73 203c 3d20 7375 625f 6b65 726e 656c  ks <= sub_kernel
+00002910: 5f73 697a 653a 0d0a 2020 2020 2020 2020  _size:..        
+00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002930: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
+00002940: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+00002950: 745f 6b73 203d 206b 735f 7365 745b 6920  t_ks = ks_set[i 
+00002960: 2d20 315d 0d0a 2020 2020 2020 2020 2020  - 1]..          
+00002970: 2020 2020 2020 2020 2020 7374 6172 742c            start,
+00002980: 2065 6e64 203d 2073 7562 5f66 696c 7465   end = sub_filte
+00002990: 725f 7374 6172 745f 656e 6428 7372 635f  r_start_end(src_
+000029a0: 6b73 2c20 7461 7267 6574 5f6b 7329 0d0a  ks, target_ks)..
+000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029c0: 2020 2020 6966 2073 656c 662e 636f 6e76      if self.conv
+000029d0: 5f64 696d 3d3d 313a 205f 696e 7075 745f  _dim==1: _input_
+000029e0: 6669 6c74 6572 203d 2073 7461 7274 5f66  filter = start_f
+000029f0: 696c 7465 725b 3a2c 203a 2c20 7374 6172  ilter[:, :, star
+00002a00: 743a 656e 645d 0d0a 2020 2020 2020 2020  t:end]..        
+00002a10: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00002a20: 2073 656c 662e 636f 6e76 5f64 696d 3d3d   self.conv_dim==
+00002a30: 323a 205f 696e 7075 745f 6669 6c74 6572  2: _input_filter
+00002a40: 203d 2073 7461 7274 5f66 696c 7465 725b   = start_filter[
+00002a50: 3a2c 203a 2c20 7374 6172 743a 656e 642c  :, :, start:end,
+00002a60: 2073 7461 7274 3a65 6e64 5d0d 0a20 2020   start:end]..   
+00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a80: 2065 6c69 6620 7365 6c66 2e63 6f6e 765f   elif self.conv_
+00002a90: 6469 6d3d 3d33 3a20 5f69 6e70 7574 5f66  dim==3: _input_f
+00002aa0: 696c 7465 7220 3d20 7374 6172 745f 6669  ilter = start_fi
+00002ab0: 6c74 6572 5b3a 2c20 3a2c 2073 7461 7274  lter[:, :, start
+00002ac0: 3a65 6e64 2c20 7374 6172 743a 656e 642c  :end, start:end,
+00002ad0: 2073 7461 7274 3a65 6e64 5d0d 0a20 2020   start:end]..   
+00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002af0: 205f 696e 7075 745f 6669 6c74 6572 203d   _input_filter =
+00002b00: 205f 696e 7075 745f 6669 6c74 6572 2e63   _input_filter.c
+00002b10: 6f6e 7469 6775 6f75 7328 290d 0a20 2020  ontiguous()..   
+00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b30: 205f 696e 7075 745f 6669 6c74 6572 203d   _input_filter =
+00002b40: 205f 696e 7075 745f 6669 6c74 6572 2e76   _input_filter.v
+00002b50: 6965 7728 5f69 6e70 7574 5f66 696c 7465  iew(_input_filte
+00002b60: 722e 7369 7a65 2830 292c 205f 696e 7075  r.size(0), _inpu
+00002b70: 745f 6669 6c74 6572 2e73 697a 6528 3129  t_filter.size(1)
+00002b80: 2c20 2d31 290d 0a20 2020 2020 2020 2020  , -1)..         
+00002b90: 2020 2020 2020 2020 2020 205f 696e 7075             _inpu
+00002ba0: 745f 6669 6c74 6572 203d 205f 696e 7075  t_filter = _inpu
+00002bb0: 745f 6669 6c74 6572 2e76 6965 7728 2d31  t_filter.view(-1
+00002bc0: 2c20 5f69 6e70 7574 5f66 696c 7465 722e  , _input_filter.
+00002bd0: 7369 7a65 2832 2929 0d0a 2020 2020 2020  size(2))..      
+00002be0: 2020 2020 2020 2020 2020 2020 2020 5f69                _i
+00002bf0: 6e70 7574 5f66 696c 7465 7220 3d20 462e  nput_filter = F.
+00002c00: 6c69 6e65 6172 280d 0a20 2020 2020 2020  linear(..       
+00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c20: 205f 696e 7075 745f 6669 6c74 6572 2c20   _input_filter, 
+00002c30: 6765 7461 7474 7228 7365 6c66 2c20 2725  getattr(self, '%
+00002c40: 6474 6f25 645f 6d61 7472 6978 2720 2520  dto%d_matrix' % 
+00002c50: 2873 7263 5f6b 732c 2074 6172 6765 745f  (src_ks, target_
+00002c60: 6b73 2929 2c0d 0a20 2020 2020 2020 2020  ks)),..         
+00002c70: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 2020 5f69 6e70 7574 5f66 696c 7465 7220    _input_filter 
+00002ca0: 3d20 5f69 6e70 7574 5f66 696c 7465 722e  = _input_filter.
+00002cb0: 7669 6577 2866 696c 7465 7273 2e73 697a  view(filters.siz
+00002cc0: 6528 3029 2c20 6669 6c74 6572 732e 7369  e(0), filters.si
+00002cd0: 7a65 2831 292c 2074 6172 6765 745f 6b73  ze(1), target_ks
+00002ce0: 202a 2a20 7365 6c66 2e63 6f6e 765f 6469   ** self.conv_di
+00002cf0: 6d29 0d0a 2020 2020 2020 2020 2020 2020  m)..            
+00002d00: 2020 2020 2020 2020 5f69 6e70 7574 5f66          _input_f
+00002d10: 696c 7465 7220 3d20 5f69 6e70 7574 5f66  ilter = _input_f
+00002d20: 696c 7465 722e 7669 6577 2866 696c 7465  ilter.view(filte
+00002d30: 7273 2e73 697a 6528 3029 2c20 6669 6c74  rs.size(0), filt
+00002d40: 6572 732e 7369 7a65 2831 292c 202a 285b  ers.size(1), *([
+00002d50: 7461 7267 6574 5f6b 735d 2a73 656c 662e  target_ks]*self.
+00002d60: 636f 6e76 5f64 696d 2929 0d0a 2020 2020  conv_dim))..    
+00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d80: 7374 6172 745f 6669 6c74 6572 203d 205f  start_filter = _
+00002d90: 696e 7075 745f 6669 6c74 6572 0d0a 2020  input_filter..  
+00002da0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00002db0: 6c74 6572 7320 3d20 7374 6172 745f 6669  lters = start_fi
+00002dc0: 6c74 6572 0d0a 2020 2020 2020 2020 7265  lter..        re
+00002dd0: 7475 726e 2066 696c 7465 7273 0d0a 0d0a  turn filters....
+00002de0: 2020 2020 6465 6620 736f 7274 5f77 6569      def sort_wei
+00002df0: 6768 745f 6269 6173 2873 656c 662c 206d  ght_bias(self, m
+00002e00: 6f64 756c 6529 3a0d 0a20 2020 2020 2020  odule):..       
+00002e10: 2069 6620 7365 6c66 2e73 6561 7263 685f   if self.search_
+00002e20: 696e 5f63 6861 6e6e 656c 3a0d 0a20 2020  in_channel:..   
+00002e30: 2020 2020 2020 2020 2076 6320 3d20 7365           vc = se
+00002e40: 6c66 2e76 616c 7565 5f73 7061 6365 735b  lf.value_spaces[
+00002e50: 2769 6e5f 6368 616e 6e65 6c73 275d 0d0a  'in_channels']..
+00002e60: 2020 2020 2020 2020 2020 2020 6d6f 6475              modu
+00002e70: 6c65 2e77 6569 6768 742e 6461 7461 203d  le.weight.data =
+00002e80: 2074 6f72 6368 2e69 6e64 6578 5f73 656c   torch.index_sel
+00002e90: 6563 7428 6d6f 6475 6c65 2e77 6569 6768  ect(module.weigh
+00002ea0: 742e 6461 7461 2c20 312c 2076 632e 736f  t.data, 1, vc.so
+00002eb0: 7274 4964 7829 0d0a 2020 2020 2020 2020  rtIdx)..        
+00002ec0: 6966 2073 656c 662e 7365 6172 6368 5f6f  if self.search_o
+00002ed0: 7574 5f63 6861 6e6e 656c 3a0d 0a20 2020  ut_channel:..   
+00002ee0: 2020 2020 2020 2020 2076 6320 3d20 7365           vc = se
+00002ef0: 6c66 2e76 616c 7565 5f73 7061 6365 735b  lf.value_spaces[
+00002f00: 276f 7574 5f63 6861 6e6e 656c 7327 5d0d  'out_channels'].
+00002f10: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+00002f20: 756c 652e 7765 6967 6874 2e64 6174 6120  ule.weight.data 
+00002f30: 3d20 746f 7263 682e 696e 6465 785f 7365  = torch.index_se
+00002f40: 6c65 6374 286d 6f64 756c 652e 7765 6967  lect(module.weig
+00002f50: 6874 2e64 6174 612c 2030 2c20 7663 2e73  ht.data, 0, vc.s
+00002f60: 6f72 7449 6478 290d 0a20 2020 2020 2020  ortIdx)..       
+00002f70: 2020 2020 2069 6620 7365 6c66 2e62 6961       if self.bia
+00002f80: 7320 6973 206e 6f74 204e 6f6e 653a 0d0a  s is not None:..
+00002f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fa0: 6d6f 6475 6c65 2e62 6961 732e 6461 7461  module.bias.data
+00002fb0: 203d 2074 6f72 6368 2e69 6e64 6578 5f73   = torch.index_s
+00002fc0: 656c 6563 7428 6d6f 6475 6c65 2e62 6961  elect(module.bia
+00002fd0: 732e 6461 7461 2c20 302c 2076 632e 736f  s.data, 0, vc.so
+00002fe0: 7274 4964 7829 0d0a 0d0a 2020 2020 2323  rtIdx)....    ##
+00002ff0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003010: 2323 2323 2323 2323 230d 0a20 2020 2023  #########..    #
+00003020: 2070 726f 7065 7274 790d 0a20 2020 2023   property..    #
+00003030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003050: 2323 2323 2323 2323 2323 0d0a 0d0a 2020  ##########....  
+00003060: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00003070: 2064 6566 2070 6172 616d 7328 7365 6c66   def params(self
+00003080: 293a 0d0a 2020 2020 2020 2020 2727 2754  ):..        '''T
+00003090: 6865 206e 756d 6265 7220 6f66 2074 6865  he number of the
+000030a0: 2074 7261 696e 6162 6c65 2070 6172 616d   trainable param
+000030b0: 6574 6572 7327 2727 0d0a 2020 2020 2020  eters'''..      
+000030c0: 2020 2320 636f 6e76 0d0a 2020 2020 2020    # conv..      
+000030d0: 2020 7765 6967 6874 203d 2073 656c 662e    weight = self.
+000030e0: 7765 6967 6874 0d0a 2020 2020 2020 2020  weight..        
+000030f0: 6269 6173 203d 2073 656c 662e 6269 6173  bias = self.bias
+00003100: 0d0a 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
+00003110: 656c 662e 7365 6172 6368 5f69 6e5f 6368  elf.search_in_ch
+00003120: 616e 6e65 6c3a 0d0a 2020 2020 2020 2020  annel:..        
+00003130: 2020 2020 696e 5f63 6861 6e6e 656c 7320      in_channels 
+00003140: 3d20 7365 6c66 2e76 616c 7565 5f73 7061  = self.value_spa
+00003150: 6365 735b 2769 6e5f 6368 616e 6e65 6c73  ces['in_channels
+00003160: 275d 2e76 616c 7565 0d0a 2020 2020 2020  '].value..      
+00003170: 2020 2020 2020 7765 6967 6874 203d 2077        weight = w
+00003180: 6569 6768 745b 3a2c 203a 696e 5f63 6861  eight[:, :in_cha
+00003190: 6e6e 656c 732c 202e 2e2e 5d0d 0a20 2020  nnels, ...]..   
+000031a0: 2020 2020 2069 6620 7365 6c66 2e73 6561       if self.sea
+000031b0: 7263 685f 6f75 745f 6368 616e 6e65 6c3a  rch_out_channel:
+000031c0: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
+000031d0: 745f 6368 616e 6e65 6c73 203d 2073 656c  t_channels = sel
+000031e0: 662e 7661 6c75 655f 7370 6163 6573 5b27  f.value_spaces['
+000031f0: 6f75 745f 6368 616e 6e65 6c73 275d 2e76  out_channels'].v
+00003200: 616c 7565 0d0a 2020 2020 2020 2020 2020  alue..          
+00003210: 2020 7765 6967 6874 203d 2077 6569 6768    weight = weigh
+00003220: 745b 3a6f 7574 5f63 6861 6e6e 656c 732c  t[:out_channels,
+00003230: 203a 2c20 2e2e 2e5d 0d0a 2020 2020 2020   :, ...]..      
+00003240: 2020 2020 2020 6966 2062 6961 7320 6973        if bias is
+00003250: 206e 6f74 204e 6f6e 653a 2062 6961 7320   not None: bias 
+00003260: 3d20 6269 6173 5b3a 6f75 745f 6368 616e  = bias[:out_chan
+00003270: 6e65 6c73 5d0d 0a20 2020 2020 2020 2069  nels]..        i
+00003280: 6620 7365 6c66 2e73 6561 7263 685f 6b65  f self.search_ke
+00003290: 726e 656c 5f73 697a 653a 0d0a 2020 2020  rnel_size:..    
+000032a0: 2020 2020 2020 2020 6b65 726e 656c 5f73          kernel_s
+000032b0: 697a 6520 3d20 7365 6c66 2e76 616c 7565  ize = self.value
+000032c0: 5f73 7061 6365 735b 276b 6572 6e65 6c5f  _spaces['kernel_
+000032d0: 7369 7a65 275d 2e76 616c 7565 0d0a 2020  size'].value..  
+000032e0: 2020 2020 2020 2020 2020 7374 6172 742c            start,
+000032f0: 2065 6e64 203d 2073 7562 5f66 696c 7465   end = sub_filte
+00003300: 725f 7374 6172 745f 656e 6428 7365 6c66  r_start_end(self
+00003310: 2e6b 6572 6e65 6c5f 7369 7a65 2c20 6b65  .kernel_size, ke
+00003320: 726e 656c 5f73 697a 6529 0d0a 2020 2020  rnel_size)..    
+00003330: 2020 2020 2020 2020 7368 6170 655f 7369          shape_si
+00003340: 7a65 203d 206c 656e 2877 6569 6768 742e  ze = len(weight.
+00003350: 7368 6170 6529 0d0a 2020 2020 2020 2020  shape)..        
+00003360: 2020 2020 6966 2073 6861 7065 5f73 697a      if shape_siz
+00003370: 6520 3d3d 2033 3a0d 0a20 2020 2020 2020  e == 3:..       
+00003380: 2020 2020 2020 2020 2023 2031 4420 636f           # 1D co
+00003390: 6e76 0d0a 2020 2020 2020 2020 2020 2020  nv..            
+000033a0: 2020 2020 7765 6967 6874 203d 2077 6569      weight = wei
+000033b0: 6768 745b 3a2c 203a 2c20 7374 6172 743a  ght[:, :, start:
+000033c0: 656e 645d 0d0a 2020 2020 2020 2020 2020  end]..          
+000033d0: 2020 656c 6966 2073 6861 7065 5f73 697a    elif shape_siz
+000033e0: 6520 3d3d 2034 3a0d 0a20 2020 2020 2020  e == 4:..       
+000033f0: 2020 2020 2020 2020 2023 2032 4420 636f           # 2D co
+00003400: 6e76 0d0a 2020 2020 2020 2020 2020 2020  nv..            
+00003410: 2020 2020 7765 6967 6874 203d 2077 6569      weight = wei
+00003420: 6768 745b 3a2c 203a 2c20 7374 6172 743a  ght[:, :, start:
+00003430: 656e 642c 2073 7461 7274 3a65 6e64 5d0d  end, start:end].
+00003440: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00003450: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003460: 2020 2020 2320 3344 2063 6f6e 760d 0a20      # 3D conv.. 
+00003470: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00003480: 6569 6768 7420 3d20 7765 6967 6874 5b3a  eight = weight[:
+00003490: 2c20 3a2c 2073 7461 7274 3a65 6e64 2c20  , :, start:end, 
+000034a0: 7374 6172 743a 656e 642c 2073 7461 7274  start:end, start
+000034b0: 3a65 6e64 5d0d 0a20 2020 2020 2020 2070  :end]..        p
+000034c0: 6172 616d 6574 6572 7320 3d20 5b77 6569  arameters = [wei
+000034d0: 6768 742c 2062 6961 735d 0d0a 2020 2020  ght, bias]..    
+000034e0: 2020 2020 7061 7261 6d73 203d 2073 756d      params = sum
+000034f0: 285b 702e 6e75 6d65 6c28 2920 666f 7220  ([p.numel() for 
+00003500: 7020 696e 2070 6172 616d 6574 6572 7320  p in parameters 
+00003510: 6966 2070 2069 7320 6e6f 7420 4e6f 6e65  if p is not None
+00003520: 5d29 0d0a 2020 2020 2020 2020 7265 7475  ])..        retu
+00003530: 726e 2070 6172 616d 730d 0a0d 0a0d 0a63  rn params......c
+00003540: 6c61 7373 2043 6f6e 7631 6428 4261 7365  lass Conv1d(Base
+00003550: 436f 6e76 4e64 293a 0d0a 2020 2020 6465  ConvNd):..    de
+00003560: 6620 5f5f 696e 6974 5f5f 280d 0a20 2020  f __init__(..   
+00003570: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
+00003580: 2020 2020 696e 5f63 6861 6e6e 656c 733a      in_channels:
+00003590: 2055 6e69 6f6e 5b69 6e74 2c20 7475 706c   Union[int, tupl
+000035a0: 652c 2056 616c 7565 5370 6163 655d 2c0d  e, ValueSpace],.
+000035b0: 0a20 2020 2020 2020 206f 7574 5f63 6861  .        out_cha
+000035c0: 6e6e 656c 733a 2055 6e69 6f6e 5b69 6e74  nnels: Union[int
+000035d0: 2c20 7475 706c 652c 2056 616c 7565 5370  , tuple, ValueSp
+000035e0: 6163 655d 2c0d 0a20 2020 2020 2020 206b  ace],..        k
+000035f0: 6572 6e65 6c5f 7369 7a65 3a20 556e 696f  ernel_size: Unio
+00003600: 6e5b 5f73 697a 655f 315f 742c 2056 616c  n[_size_1_t, Val
+00003610: 7565 5370 6163 655d 2c0d 0a20 2020 2020  ueSpace],..     
+00003620: 2020 2073 7472 6964 653a 2055 6e69 6f6e     stride: Union
+00003630: 5b5f 7369 7a65 5f31 5f74 2c20 5661 6c75  [_size_1_t, Valu
+00003640: 6553 7061 6365 5d20 3d20 312c 0d0a 2020  eSpace] = 1,..  
+00003650: 2020 2020 2020 7061 6464 696e 673a 2055        padding: U
+00003660: 6e69 6f6e 5b73 7472 2c20 5f73 697a 655f  nion[str, _size_
+00003670: 315f 742c 2056 616c 7565 5370 6163 655d  1_t, ValueSpace]
+00003680: 203d 2030 2c0d 0a20 2020 2020 2020 2064   = 0,..        d
+00003690: 696c 6174 696f 6e3a 2055 6e69 6f6e 5b5f  ilation: Union[_
+000036a0: 7369 7a65 5f31 5f74 2c20 5661 6c75 6553  size_1_t, ValueS
+000036b0: 7061 6365 5d20 3d20 312c 0d0a 2020 2020  pace] = 1,..    
+000036c0: 2020 2020 6772 6f75 7073 3a20 556e 696f      groups: Unio
+000036d0: 6e5b 696e 742c 2056 616c 7565 5370 6163  n[int, ValueSpac
+000036e0: 655d 203d 2031 2c0d 0a20 2020 2020 2020  e] = 1,..       
+000036f0: 2062 6961 733a 2062 6f6f 6c20 3d20 5472   bias: bool = Tr
+00003700: 7565 2c0d 0a20 2020 2020 2020 2070 6164  ue,..        pad
+00003710: 6469 6e67 5f6d 6f64 653a 2073 7472 203d  ding_mode: str =
+00003720: 2027 7a65 726f 7327 2c0d 0a20 2020 2020   'zeros',..     
+00003730: 2020 2064 6576 6963 653d 4e6f 6e65 2c0d     device=None,.
+00003740: 0a20 2020 2020 2020 2064 7479 7065 3d4e  .        dtype=N
+00003750: 6f6e 652c 0d0a 2020 2020 2020 2020 6175  one,..        au
+00003760: 746f 5f70 6164 6469 6e67 3a20 626f 6f6c  to_padding: bool
+00003770: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
+00003780: 2020 202a 2a6b 7761 7267 730d 0a20 2020     **kwargs..   
+00003790: 2029 3a0d 0a20 2020 2020 2020 2073 7570   ):..        sup
+000037a0: 6572 2843 6f6e 7631 642c 2073 656c 6629  er(Conv1d, self)
+000037b0: 2e5f 5f69 6e69 745f 5f28 696e 5f63 6861  .__init__(in_cha
+000037c0: 6e6e 656c 732c 206f 7574 5f63 6861 6e6e  nnels, out_chann
+000037d0: 656c 732c 206b 6572 6e65 6c5f 7369 7a65  els, kernel_size
+000037e0: 2c20 7374 7269 6465 2c20 7061 6464 696e  , stride, paddin
+000037f0: 672c 0d0a 2020 2020 2020 2020 2020 2020  g,..            
+00003800: 6469 6c61 7469 6f6e 2c20 6772 6f75 7073  dilation, groups
+00003810: 2c20 6269 6173 2c20 7061 6464 696e 675f  , bias, padding_
+00003820: 6d6f 6465 2c20 6465 7669 6365 2c20 6474  mode, device, dt
+00003830: 7970 652c 2061 7574 6f5f 7061 6464 696e  ype, auto_paddin
+00003840: 672c 202a 2a6b 7761 7267 7329 0d0a 0d0a  g, **kwargs)....
+00003850: 2020 2020 6465 6620 666f 726d 6174 5f61      def format_a
+00003860: 7267 7328 0d0a 2020 2020 2020 2020 7365  rgs(..        se
+00003870: 6c66 2c0d 0a20 2020 2020 2020 206b 6572  lf,..        ker
+00003880: 6e65 6c5f 7369 7a65 3a20 5f73 697a 655f  nel_size: _size_
+00003890: 315f 742c 0d0a 2020 2020 2020 2020 7374  1_t,..        st
+000038a0: 7269 6465 3a20 5f73 697a 655f 315f 7420  ride: _size_1_t 
+000038b0: 3d20 312c 0d0a 2020 2020 2020 2020 7061  = 1,..        pa
+000038c0: 6464 696e 673a 2055 6e69 6f6e 5b73 7472  dding: Union[str
+000038d0: 2c20 5f73 697a 655f 315f 745d 203d 2030  , _size_1_t] = 0
+000038e0: 2c0d 0a20 2020 2020 2020 2064 696c 6174  ,..        dilat
+000038f0: 696f 6e3a 205f 7369 7a65 5f31 5f74 203d  ion: _size_1_t =
+00003900: 2031 2c0d 0a20 2020 2029 3a0d 0a20 2020   1,..    ):..   
+00003910: 2020 2020 2027 2727 4765 6e65 7261 7465       '''Generate
+00003920: 2043 6f6e 7620 6f70 6572 6174 696f 6e27   Conv operation'
+00003930: 2727 0d0a 2020 2020 2020 2020 7365 6c66  ''..        self
+00003940: 2e6b 6572 6e65 6c5f 7369 7a65 203d 205f  .kernel_size = _
+00003950: 7369 6e67 6c65 286b 6572 6e65 6c5f 7369  single(kernel_si
+00003960: 7a65 290d 0a20 2020 2020 2020 2073 656c  ze)..        sel
+00003970: 662e 7374 7269 6465 203d 205f 7369 6e67  f.stride = _sing
+00003980: 6c65 2873 7472 6964 6529 0d0a 2020 2020  le(stride)..    
+00003990: 2020 2020 7365 6c66 2e70 6164 6469 6e67      self.padding
+000039a0: 203d 2070 6164 6469 6e67 2069 6620 6973   = padding if is
+000039b0: 696e 7374 616e 6365 2870 6164 6469 6e67  instance(padding
+000039c0: 2c20 7374 7229 2065 6c73 6520 5f73 696e  , str) else _sin
+000039d0: 676c 6528 7061 6464 696e 6729 0d0a 2020  gle(padding)..  
+000039e0: 2020 2020 2020 7365 6c66 2e64 696c 6174        self.dilat
+000039f0: 696f 6e20 3d20 5f73 696e 676c 6528 6469  ion = _single(di
+00003a00: 6c61 7469 6f6e 290d 0a20 2020 2020 2020  lation)..       
+00003a10: 2073 656c 662e 6f75 7470 7574 5f70 6164   self.output_pad
+00003a20: 6469 6e67 203d 205f 7369 6e67 6c65 2830  ding = _single(0
+00003a30: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003a40: 636f 6e76 203d 2046 2e63 6f6e 7631 640d  conv = F.conv1d.
+00003a50: 0a0d 0a0d 0a63 6c61 7373 2043 6f6e 7632  .....class Conv2
+00003a60: 6428 4261 7365 436f 6e76 4e64 293a 0d0a  d(BaseConvNd):..
+00003a70: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00003a80: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
+00003a90: 0d0a 2020 2020 2020 2020 696e 5f63 6861  ..        in_cha
+00003aa0: 6e6e 656c 733a 2055 6e69 6f6e 5b69 6e74  nnels: Union[int
+00003ab0: 2c20 7475 706c 652c 2056 616c 7565 5370  , tuple, ValueSp
+00003ac0: 6163 655d 2c0d 0a20 2020 2020 2020 206f  ace],..        o
+00003ad0: 7574 5f63 6861 6e6e 656c 733a 2055 6e69  ut_channels: Uni
+00003ae0: 6f6e 5b69 6e74 2c20 7475 706c 652c 2056  on[int, tuple, V
+00003af0: 616c 7565 5370 6163 655d 2c0d 0a20 2020  alueSpace],..   
+00003b00: 2020 2020 206b 6572 6e65 6c5f 7369 7a65       kernel_size
+00003b10: 3a20 556e 696f 6e5b 696e 742c 2056 616c  : Union[int, Val
+00003b20: 7565 5370 6163 655d 2c0d 0a20 2020 2020  ueSpace],..     
+00003b30: 2020 2073 7472 6964 653a 2055 6e69 6f6e     stride: Union
+00003b40: 5b69 6e74 2c20 5661 6c75 6553 7061 6365  [int, ValueSpace
+00003b50: 5d20 3d20 312c 0d0a 2020 2020 2020 2020  ] = 1,..        
+00003b60: 7061 6464 696e 673a 2055 6e69 6f6e 5b73  padding: Union[s
+00003b70: 7472 2c20 696e 742c 2056 616c 7565 5370  tr, int, ValueSp
+00003b80: 6163 655d 203d 2030 2c0d 0a20 2020 2020  ace] = 0,..     
 00003b90: 2020 2064 696c 6174 696f 6e3a 2055 6e69     dilation: Uni
-00003ba0: 6f6e 5b69 6e74 2c20 7475 706c 655d 203d  on[int, tuple] =
-00003bb0: 2031 2c0d 0a20 2020 2020 2020 2067 726f   1,..        gro
-00003bc0: 7570 733a 2069 6e74 203d 2031 2c0d 0a20  ups: int = 1,.. 
-00003bd0: 2020 2020 2020 2062 6961 733a 2062 6f6f         bias: boo
-00003be0: 6c20 3d20 5472 7565 2c0d 0a20 2020 2020  l = True,..     
-00003bf0: 2020 2070 6164 6469 6e67 5f6d 6f64 653a     padding_mode:
-00003c00: 2073 7472 203d 2027 7a65 726f 7327 2c0d   str = 'zeros',.
-00003c10: 0a20 2020 2020 2020 2061 7574 6f5f 7061  .        auto_pa
-00003c20: 6464 696e 673a 2062 6f6f 6c20 3d20 4661  dding: bool = Fa
-00003c30: 6c73 652c 0d0a 2020 2020 2020 2020 2a61  lse,..        *a
-00003c40: 7267 732c 202a 2a6b 7761 7267 730d 0a20  rgs, **kwargs.. 
-00003c50: 2020 2029 3a0d 0a20 2020 2020 2020 2073     ):..        s
-00003c60: 7570 6572 2843 6f6e 7633 642c 2073 656c  uper(Conv3d, sel
-00003c70: 6629 2e5f 5f69 6e69 745f 5f28 0d0a 2020  f).__init__(..  
-00003c80: 2020 2020 2020 2020 2020 696e 5f63 6861            in_cha
-00003c90: 6e6e 656c 732c 206f 7574 5f63 6861 6e6e  nnels, out_chann
-00003ca0: 656c 732c 206b 6572 6e65 6c5f 7369 7a65  els, kernel_size
-00003cb0: 2c20 7374 7269 6465 2c20 7061 6464 696e  , stride, paddin
-00003cc0: 672c 0d0a 2020 2020 2020 2020 2020 2020  g,..            
-00003cd0: 6469 6c61 7469 6f6e 2c20 6772 6f75 7073  dilation, groups
-00003ce0: 2c20 6269 6173 2c20 7061 6464 696e 675f  , bias, padding_
-00003cf0: 6d6f 6465 2c20 6175 746f 5f70 6164 6469  mode, auto_paddi
-00003d00: 6e67 290d 0a0d 0a20 2020 2064 6566 2069  ng)....    def i
-00003d10: 6e69 745f 6f70 7328 0d0a 2020 2020 2020  nit_ops(..      
-00003d20: 2020 7365 6c66 2c20 0d0a 2020 2020 2020    self, ..      
-00003d30: 2020 696e 5f63 6861 6e6e 656c 733a 2069    in_channels: i
-00003d40: 6e74 2c0d 0a20 2020 2020 2020 206f 7574  nt,..        out
-00003d50: 5f63 6861 6e6e 656c 733a 2069 6e74 2c0d  _channels: int,.
-00003d60: 0a20 2020 2020 2020 206b 6572 6e65 6c5f  .        kernel_
-00003d70: 7369 7a65 3a20 5f73 697a 655f 335f 742c  size: _size_3_t,
-00003d80: 0d0a 2020 2020 2020 2020 7374 7269 6465  ..        stride
-00003d90: 3a20 5f73 697a 655f 335f 7420 3d20 312c  : _size_3_t = 1,
-00003da0: 0d0a 2020 2020 2020 2020 7061 6464 696e  ..        paddin
-00003db0: 673a 2055 6e69 6f6e 5b73 7472 2c20 5f73  g: Union[str, _s
-00003dc0: 697a 655f 335f 745d 203d 2030 2c0d 0a20  ize_3_t] = 0,.. 
-00003dd0: 2020 2020 2020 2064 696c 6174 696f 6e3a         dilation:
-00003de0: 205f 7369 7a65 5f33 5f74 203d 2031 2c0d   _size_3_t = 1,.
-00003df0: 0a20 2020 2020 2020 2067 726f 7570 733a  .        groups:
-00003e00: 2069 6e74 203d 2031 2c0d 0a20 2020 2020   int = 1,..     
-00003e10: 2020 2062 6961 733a 2062 6f6f 6c20 3d20     bias: bool = 
-00003e20: 5472 7565 0d0a 2020 2020 293a 0d0a 2020  True..    ):..  
-00003e30: 2020 2020 2020 2727 2747 656e 6572 6174        '''Generat
-00003e40: 6520 436f 6e76 206f 7065 7261 7469 6f6e  e Conv operation
-00003e50: 2727 270d 0a20 2020 2020 2020 2073 656c  '''..        sel
-00003e60: 662e 6b65 726e 656c 5f73 697a 6520 3d20  f.kernel_size = 
-00003e70: 5f74 7269 706c 6528 6b65 726e 656c 5f73  _triple(kernel_s
-00003e80: 697a 6529 0d0a 2020 2020 2020 2020 7365  ize)..        se
-00003e90: 6c66 2e73 7472 6964 6520 3d20 5f74 7269  lf.stride = _tri
-00003ea0: 706c 6528 7374 7269 6465 290d 0a20 2020  ple(stride)..   
-00003eb0: 2020 2020 2073 656c 662e 7061 6464 696e       self.paddin
-00003ec0: 6720 3d20 7061 6464 696e 6720 6966 2069  g = padding if i
-00003ed0: 7369 6e73 7461 6e63 6528 7061 6464 696e  sinstance(paddin
-00003ee0: 672c 2073 7472 2920 656c 7365 205f 7472  g, str) else _tr
-00003ef0: 6970 6c65 2870 6164 6469 6e67 290d 0a20  iple(padding).. 
-00003f00: 2020 2020 2020 2073 656c 662e 6469 6c61         self.dila
-00003f10: 7469 6f6e 203d 205f 7472 6970 6c65 2864  tion = _triple(d
-00003f20: 696c 6174 696f 6e29 0d0a 2020 2020 2020  ilation)..      
-00003f30: 2020 7365 6c66 2e6f 7574 7075 745f 7061    self.output_pa
-00003f40: 6464 696e 6720 3d20 5f74 7269 706c 6528  dding = _triple(
-00003f50: 3029 0d0a 2020 2020 2020 2020 7365 6c66  0)..        self
-00003f60: 2e63 6f6e 7620 3d20 462e 636f 6e76 3364  .conv = F.conv3d
-00003f70: 0d0a 0d0a 0d0a 6966 205f 5f6e 616d 655f  ......if __name_
-00003f80: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
-00003f90: 0d0a 2020 2020 696d 706f 7274 2074 6f72  ..    import tor
-00003fa0: 6368 0d0a 2020 2020 6672 6f6d 2068 7970  ch..    from hyp
-00003fb0: 6572 626f 782e 6d75 7461 746f 7220 696d  erbox.mutator im
-00003fc0: 706f 7274 2052 616e 646f 6d4d 7574 6174  port RandomMutat
-00003fd0: 6f72 0d0a 2020 2020 6f63 203d 2056 616c  or..    oc = Val
-00003fe0: 7565 5370 6163 6528 6361 6e64 6964 6174  ueSpace(candidat
-00003ff0: 6573 3d5b 332c 3130 5d29 0d0a 2020 2020  es=[3,10])..    
-00004000: 6b73 203d 2056 616c 7565 5370 6163 6528  ks = ValueSpace(
-00004010: 6361 6e64 6964 6174 6573 3d5b 332c 352c  candidates=[3,5,
-00004020: 375d 290d 0a20 2020 206f 7020 3d20 436f  7])..    op = Co
-00004030: 6e76 3264 2869 6e5f 6368 616e 6e65 6c73  nv2d(in_channels
-00004040: 3d33 2c20 6f75 745f 6368 616e 6e65 6c73  =3, out_channels
-00004050: 3d6f 632c 206b 6572 6e65 6c5f 7369 7a65  =oc, kernel_size
-00004060: 3d6b 7329 0d0a 2020 2020 726d 203d 2052  =ks)..    rm = R
-00004070: 616e 646f 6d4d 7574 6174 6f72 286f 7029  andomMutator(op)
-00004080: 0d0a 2020 2020 666f 7220 6920 696e 2072  ..    for i in r
-00004090: 616e 6765 2831 3029 3a0d 0a20 2020 2020  ange(10):..     
-000040a0: 2020 2072 6d2e 7265 7365 7428 290d 0a20     rm.reset().. 
-000040b0: 2020 2020 2020 2078 203d 2074 6f72 6368         x = torch
-000040c0: 2e72 616e 6428 322c 332c 382c 3829 0d0a  .rand(2,3,8,8)..
-000040d0: 2020 2020 2020 2020 7920 3d20 6f70 2878          y = op(x
-000040e0: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-000040f0: 2879 2e73 6861 7065 290d 0a              (y.shape)..
+00003ba0: 6f6e 5b69 6e74 2c20 5661 6c75 6553 7061  on[int, ValueSpa
+00003bb0: 6365 5d20 3d20 312c 0d0a 2020 2020 2020  ce] = 1,..      
+00003bc0: 2020 6772 6f75 7073 3a20 556e 696f 6e5b    groups: Union[
+00003bd0: 696e 742c 2056 616c 7565 5370 6163 655d  int, ValueSpace]
+00003be0: 203d 2031 2c0d 0a20 2020 2020 2020 2062   = 1,..        b
+00003bf0: 6961 733a 2062 6f6f 6c20 3d20 5472 7565  ias: bool = True
+00003c00: 2c0d 0a20 2020 2020 2020 2070 6164 6469  ,..        paddi
+00003c10: 6e67 5f6d 6f64 653a 2073 7472 203d 2027  ng_mode: str = '
+00003c20: 7a65 726f 7327 2c0d 0a20 2020 2020 2020  zeros',..       
+00003c30: 2061 7574 6f5f 7061 6464 696e 673a 2062   auto_padding: b
+00003c40: 6f6f 6c20 3d20 4661 6c73 652c 0d0a 2020  ool = False,..  
+00003c50: 2020 2020 2020 6465 7669 6365 3d4e 6f6e        device=Non
+00003c60: 652c 0d0a 2020 2020 2020 2020 6474 7970  e,..        dtyp
+00003c70: 653d 4e6f 6e65 2c0d 0a20 2020 2020 2020  e=None,..       
+00003c80: 202a 2a6b 7761 7267 730d 0a20 2020 2029   **kwargs..    )
+00003c90: 3a0d 0a20 2020 2020 2020 2073 7570 6572  :..        super
+00003ca0: 2843 6f6e 7632 642c 2073 656c 6629 2e5f  (Conv2d, self)._
+00003cb0: 5f69 6e69 745f 5f28 696e 5f63 6861 6e6e  _init__(in_chann
+00003cc0: 656c 732c 206f 7574 5f63 6861 6e6e 656c  els, out_channel
+00003cd0: 732c 206b 6572 6e65 6c5f 7369 7a65 2c20  s, kernel_size, 
+00003ce0: 7374 7269 6465 2c20 7061 6464 696e 672c  stride, padding,
+00003cf0: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
+00003d00: 6c61 7469 6f6e 2c20 6772 6f75 7073 2c20  lation, groups, 
+00003d10: 6269 6173 2c20 7061 6464 696e 675f 6d6f  bias, padding_mo
+00003d20: 6465 2c20 6465 7669 6365 2c20 6474 7970  de, device, dtyp
+00003d30: 652c 2061 7574 6f5f 7061 6464 696e 672c  e, auto_padding,
+00003d40: 202a 2a6b 7761 7267 7329 0d0a 0d0a 2020   **kwargs)....  
+00003d50: 2020 6465 6620 666f 726d 6174 5f61 7267    def format_arg
+00003d60: 7328 0d0a 2020 2020 2020 2020 7365 6c66  s(..        self
+00003d70: 2c0d 0a20 2020 2020 2020 206b 6572 6e65  ,..        kerne
+00003d80: 6c5f 7369 7a65 3a20 5f73 697a 655f 325f  l_size: _size_2_
+00003d90: 742c 0d0a 2020 2020 2020 2020 7374 7269  t,..        stri
+00003da0: 6465 3a20 5f73 697a 655f 325f 7420 3d20  de: _size_2_t = 
+00003db0: 312c 0d0a 2020 2020 2020 2020 7061 6464  1,..        padd
+00003dc0: 696e 673a 2055 6e69 6f6e 5b73 7472 2c20  ing: Union[str, 
+00003dd0: 5f73 697a 655f 325f 745d 203d 2030 2c0d  _size_2_t] = 0,.
+00003de0: 0a20 2020 2020 2020 2064 696c 6174 696f  .        dilatio
+00003df0: 6e3a 205f 7369 7a65 5f32 5f74 203d 2031  n: _size_2_t = 1
+00003e00: 2c0d 0a20 2020 2029 3a0d 0a20 2020 2020  ,..    ):..     
+00003e10: 2020 2027 2727 4765 6e65 7261 7465 2043     '''Generate C
+00003e20: 6f6e 7620 6f70 6572 6174 696f 6e27 2727  onv operation'''
+00003e30: 0d0a 2020 2020 2020 2020 7365 6c66 2e6b  ..        self.k
+00003e40: 6572 6e65 6c5f 7369 7a65 203d 205f 7061  ernel_size = _pa
+00003e50: 6972 286b 6572 6e65 6c5f 7369 7a65 290d  ir(kernel_size).
+00003e60: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00003e70: 7269 6465 203d 205f 7061 6972 2873 7472  ride = _pair(str
+00003e80: 6964 6529 0d0a 2020 2020 2020 2020 7365  ide)..        se
+00003e90: 6c66 2e70 6164 6469 6e67 203d 2070 6164  lf.padding = pad
+00003ea0: 6469 6e67 2069 6620 6973 696e 7374 616e  ding if isinstan
+00003eb0: 6365 2870 6164 6469 6e67 2c20 7374 7229  ce(padding, str)
+00003ec0: 2065 6c73 6520 5f70 6169 7228 7061 6464   else _pair(padd
+00003ed0: 696e 6729 0d0a 2020 2020 2020 2020 7365  ing)..        se
+00003ee0: 6c66 2e64 696c 6174 696f 6e20 3d20 5f70  lf.dilation = _p
+00003ef0: 6169 7228 6469 6c61 7469 6f6e 290d 0a20  air(dilation).. 
+00003f00: 2020 2020 2020 2073 656c 662e 6f75 7470         self.outp
+00003f10: 7574 5f70 6164 6469 6e67 203d 205f 7061  ut_padding = _pa
+00003f20: 6972 2830 290d 0a20 2020 2020 2020 2073  ir(0)..        s
+00003f30: 656c 662e 636f 6e76 203d 2046 2e63 6f6e  elf.conv = F.con
+00003f40: 7632 640d 0a0d 0a0d 0a63 6c61 7373 2043  v2d......class C
+00003f50: 6f6e 7633 6428 4261 7365 436f 6e76 4e64  onv3d(BaseConvNd
+00003f60: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
+00003f70: 6974 5f5f 280d 0a20 2020 2020 2020 2073  it__(..        s
+00003f80: 656c 662c 0d0a 2020 2020 2020 2020 696e  elf,..        in
+00003f90: 5f63 6861 6e6e 656c 733a 2055 6e69 6f6e  _channels: Union
+00003fa0: 5b69 6e74 2c20 5661 6c75 6553 7061 6365  [int, ValueSpace
+00003fb0: 5d2c 0d0a 2020 2020 2020 2020 6f75 745f  ],..        out_
+00003fc0: 6368 616e 6e65 6c73 3a20 556e 696f 6e5b  channels: Union[
+00003fd0: 696e 742c 2056 616c 7565 5370 6163 655d  int, ValueSpace]
+00003fe0: 2c0d 0a20 2020 2020 2020 206b 6572 6e65  ,..        kerne
+00003ff0: 6c5f 7369 7a65 3a20 556e 696f 6e5b 696e  l_size: Union[in
+00004000: 742c 2056 616c 7565 5370 6163 655d 2c0d  t, ValueSpace],.
+00004010: 0a20 2020 2020 2020 2073 7472 6964 653a  .        stride:
+00004020: 2055 6e69 6f6e 5b69 6e74 2c20 5661 6c75   Union[int, Valu
+00004030: 6553 7061 6365 5d20 3d20 312c 0d0a 2020  eSpace] = 1,..  
+00004040: 2020 2020 2020 7061 6464 696e 673a 2055        padding: U
+00004050: 6e69 6f6e 5b69 6e74 2c20 5661 6c75 6553  nion[int, ValueS
+00004060: 7061 6365 5d20 3d20 302c 0d0a 2020 2020  pace] = 0,..    
+00004070: 2020 2020 6469 6c61 7469 6f6e 3a20 556e      dilation: Un
+00004080: 696f 6e5b 696e 742c 2056 616c 7565 5370  ion[int, ValueSp
+00004090: 6163 655d 203d 2031 2c0d 0a20 2020 2020  ace] = 1,..     
+000040a0: 2020 2067 726f 7570 733a 2055 6e69 6f6e     groups: Union
+000040b0: 5b69 6e74 2c20 5661 6c75 6553 7061 6365  [int, ValueSpace
+000040c0: 5d20 3d20 312c 0d0a 2020 2020 2020 2020  ] = 1,..        
+000040d0: 6269 6173 3a20 556e 696f 6e5b 7374 722c  bias: Union[str,
+000040e0: 2056 616c 7565 5370 6163 655d 203d 2054   ValueSpace] = T
+000040f0: 7275 652c 0d0a 2020 2020 2020 2020 7061  rue,..        pa
+00004100: 6464 696e 675f 6d6f 6465 3a20 7374 7220  dding_mode: str 
+00004110: 3d20 277a 6572 6f73 272c 0d0a 2020 2020  = 'zeros',..    
+00004120: 2020 2020 6175 746f 5f70 6164 6469 6e67      auto_padding
+00004130: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
+00004140: 0a20 2020 2020 2020 2064 6576 6963 653d  .        device=
+00004150: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2064  None,..        d
+00004160: 7479 7065 3d4e 6f6e 652c 0d0a 2020 2020  type=None,..    
+00004170: 2020 2020 2a2a 6b77 6172 6773 0d0a 2020      **kwargs..  
+00004180: 2020 293a 0d0a 2020 2020 2020 2020 7375    ):..        su
+00004190: 7065 7228 436f 6e76 3364 2c20 7365 6c66  per(Conv3d, self
+000041a0: 292e 5f5f 696e 6974 5f5f 2869 6e5f 6368  ).__init__(in_ch
+000041b0: 616e 6e65 6c73 2c20 6f75 745f 6368 616e  annels, out_chan
+000041c0: 6e65 6c73 2c20 6b65 726e 656c 5f73 697a  nels, kernel_siz
+000041d0: 652c 2073 7472 6964 652c 2070 6164 6469  e, stride, paddi
+000041e0: 6e67 2c0d 0a20 2020 2020 2020 2020 2020  ng,..           
+000041f0: 2064 696c 6174 696f 6e2c 2067 726f 7570   dilation, group
+00004200: 732c 2062 6961 732c 2070 6164 6469 6e67  s, bias, padding
+00004210: 5f6d 6f64 652c 2064 6576 6963 652c 2064  _mode, device, d
+00004220: 7479 7065 2c20 6175 746f 5f70 6164 6469  type, auto_paddi
+00004230: 6e67 2c20 2a2a 6b77 6172 6773 290d 0a0d  ng, **kwargs)...
+00004240: 0a0d 0a20 2020 2064 6566 2066 6f72 6d61  ...    def forma
+00004250: 745f 6172 6773 280d 0a20 2020 2020 2020  t_args(..       
+00004260: 2073 656c 662c 200d 0a20 2020 2020 2020   self, ..       
+00004270: 206b 6572 6e65 6c5f 7369 7a65 3a20 5f73   kernel_size: _s
+00004280: 697a 655f 335f 742c 0d0a 2020 2020 2020  ize_3_t,..      
+00004290: 2020 7374 7269 6465 3a20 5f73 697a 655f    stride: _size_
+000042a0: 335f 7420 3d20 312c 0d0a 2020 2020 2020  3_t = 1,..      
+000042b0: 2020 7061 6464 696e 673a 2055 6e69 6f6e    padding: Union
+000042c0: 5b73 7472 2c20 5f73 697a 655f 335f 745d  [str, _size_3_t]
+000042d0: 203d 2030 2c0d 0a20 2020 2020 2020 2064   = 0,..        d
+000042e0: 696c 6174 696f 6e3a 205f 7369 7a65 5f33  ilation: _size_3
+000042f0: 5f74 203d 2031 2c0d 0a20 2020 2020 2020  _t = 1,..       
+00004300: 2062 6961 733a 2062 6f6f 6c20 3d20 5472   bias: bool = Tr
+00004310: 7565 0d0a 2020 2020 293a 0d0a 2020 2020  ue..    ):..    
+00004320: 2020 2020 2727 2747 656e 6572 6174 6520      '''Generate 
+00004330: 436f 6e76 206f 7065 7261 7469 6f6e 2727  Conv operation''
+00004340: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+00004350: 6b65 726e 656c 5f73 697a 6520 3d20 5f74  kernel_size = _t
+00004360: 7269 706c 6528 6b65 726e 656c 5f73 697a  riple(kernel_siz
+00004370: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
+00004380: 2e73 7472 6964 6520 3d20 5f74 7269 706c  .stride = _tripl
+00004390: 6528 7374 7269 6465 290d 0a20 2020 2020  e(stride)..     
+000043a0: 2020 2073 656c 662e 7061 6464 696e 6720     self.padding 
+000043b0: 3d20 7061 6464 696e 6720 6966 2069 7369  = padding if isi
+000043c0: 6e73 7461 6e63 6528 7061 6464 696e 672c  nstance(padding,
+000043d0: 2073 7472 2920 656c 7365 205f 7472 6970   str) else _trip
+000043e0: 6c65 2870 6164 6469 6e67 290d 0a20 2020  le(padding)..   
+000043f0: 2020 2020 2073 656c 662e 6469 6c61 7469       self.dilati
+00004400: 6f6e 203d 205f 7472 6970 6c65 2864 696c  on = _triple(dil
+00004410: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+00004420: 7365 6c66 2e6f 7574 7075 745f 7061 6464  self.output_padd
+00004430: 696e 6720 3d20 5f74 7269 706c 6528 3029  ing = _triple(0)
+00004440: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00004450: 6f6e 7620 3d20 462e 636f 6e76 3364 0d0a  onv = F.conv3d..
+00004460: 0d0a 0d0a 6966 205f 5f6e 616d 655f 5f20  ....if __name__ 
+00004470: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0d0a  == '__main__':..
+00004480: 2020 2020 6672 6f6d 2074 696d 6520 696d      from time im
+00004490: 706f 7274 2074 696d 650d 0a20 2020 2069  port time..    i
+000044a0: 6d70 6f72 7420 746f 7263 680d 0a20 2020  mport torch..   
+000044b0: 2066 726f 6d20 6879 7065 7262 6f78 2e6d   from hyperbox.m
+000044c0: 7574 6174 6f72 2069 6d70 6f72 7420 5261  utator import Ra
+000044d0: 6e64 6f6d 4d75 7461 746f 720d 0a20 2020  ndomMutator..   
+000044e0: 2064 6576 6963 6520 3d20 746f 7263 682e   device = torch.
+000044f0: 6465 7669 6365 2827 6375 6461 2720 6966  device('cuda' if
+00004500: 2074 6f72 6368 2e63 7564 612e 6973 5f61   torch.cuda.is_a
+00004510: 7661 696c 6162 6c65 2829 2065 6c73 6520  vailable() else 
+00004520: 2763 7075 2729 0d0a 2020 2020 7374 6570  'cpu')..    step
+00004530: 7320 3d20 3530 0d0a 2020 2020 2320 2320  s = 50..    # # 
+00004540: 3164 0d0a 2020 2020 2320 6f63 203d 2056  1d..    # oc = V
+00004550: 616c 7565 5370 6163 6528 6361 6e64 6964  alueSpace(candid
+00004560: 6174 6573 3d5b 332c 3130 5d29 0d0a 2020  ates=[3,10])..  
+00004570: 2020 2320 6b73 203d 2056 616c 7565 5370    # ks = ValueSp
+00004580: 6163 6528 6361 6e64 6964 6174 6573 3d5b  ace(candidates=[
+00004590: 332c 352c 375d 290d 0a20 2020 2023 206f  3,5,7])..    # o
+000045a0: 7020 3d20 436f 6e76 3164 2869 6e5f 6368  p = Conv1d(in_ch
+000045b0: 616e 6e65 6c73 3d33 2c20 6f75 745f 6368  annels=3, out_ch
+000045c0: 616e 6e65 6c73 3d6f 632c 206b 6572 6e65  annels=oc, kerne
+000045d0: 6c5f 7369 7a65 3d6b 732c 2062 6961 733d  l_size=ks, bias=
+000045e0: 5472 7565 292e 746f 2864 6576 6963 6529  True).to(device)
+000045f0: 0d0a 2020 2020 2320 726d 203d 2052 616e  ..    # rm = Ran
+00004600: 646f 6d4d 7574 6174 6f72 286f 7029 0d0a  domMutator(op)..
+00004610: 2020 2020 2320 7072 696e 7428 272a 272a      # print('*'*
+00004620: 3830 290d 0a20 2020 2023 2078 203d 2074  80)..    # x = t
+00004630: 6f72 6368 2e72 616e 6428 322c 332c 3136  orch.rand(2,3,16
+00004640: 292e 746f 2864 6576 6963 6529 0d0a 2020  ).to(device)..  
+00004650: 2020 2320 7374 6172 7420 3d20 7469 6d65    # start = time
+00004660: 2829 0d0a 2020 2020 2320 666f 7220 6920  ()..    # for i 
+00004670: 696e 2072 616e 6765 2873 7465 7073 293a  in range(steps):
+00004680: 0d0a 2020 2020 2320 2020 2020 726d 2e72  ..    #     rm.r
+00004690: 6573 6574 2829 0d0a 2020 2020 2320 2020  eset()..    #   
+000046a0: 2020 7920 3d20 6f70 2878 290d 0a20 2020    y = op(x)..   
+000046b0: 2023 2020 2020 2023 2070 7269 6e74 2879   #     # print(y
+000046c0: 2e73 6861 7065 290d 0a20 2020 2023 2065  .shape)..    # e
+000046d0: 6e64 203d 2074 696d 6528 290d 0a20 2020  nd = time()..   
+000046e0: 2023 2070 7269 6e74 2866 2274 6573 7469   # print(f"testi
+000046f0: 6e67 2031 6420 7b6f 707d 2c20 636f 7374  ng 1d {op}, cost
+00004700: 207b 656e 642d 7374 6172 743a 2e32 667d   {end-start:.2f}
+00004710: 2073 2229 0d0a 0d0a 2020 2020 2320 3264   s")....    # 2d
+00004720: 0d0a 2020 2020 6f63 203d 2056 616c 7565  ..    oc = Value
+00004730: 5370 6163 6528 6361 6e64 6964 6174 6573  Space(candidates
+00004740: 3d5b 392c 3138 5d29 0d0a 2020 2020 6b73  =[9,18])..    ks
+00004750: 203d 2056 616c 7565 5370 6163 6528 6361   = ValueSpace(ca
+00004760: 6e64 6964 6174 6573 3d5b 332c 352c 375d  ndidates=[3,5,7]
+00004770: 290d 0a20 2020 2067 726f 7570 7320 3d20  )..    groups = 
+00004780: 5661 6c75 6553 7061 6365 2863 616e 6469  ValueSpace(candi
+00004790: 6461 7465 733d 5b31 2c33 5d29 0d0a 2020  dates=[1,3])..  
+000047a0: 2020 6f70 203d 2043 6f6e 7632 6428 696e    op = Conv2d(in
+000047b0: 5f63 6861 6e6e 656c 733d 392c 206f 7574  _channels=9, out
+000047c0: 5f63 6861 6e6e 656c 733d 3336 2c20 6b65  _channels=36, ke
+000047d0: 726e 656c 5f73 697a 653d 6b73 2c20 6772  rnel_size=ks, gr
+000047e0: 6f75 7073 3d67 726f 7570 7329 2e74 6f28  oups=groups).to(
+000047f0: 6465 7669 6365 290d 0a20 2020 2072 6d20  device)..    rm 
+00004800: 3d20 5261 6e64 6f6d 4d75 7461 746f 7228  = RandomMutator(
+00004810: 6f70 290d 0a20 2020 2070 7269 6e74 2827  op)..    print('
+00004820: 2a27 2a38 3029 0d0a 2020 2020 7820 3d20  *'*80)..    x = 
+00004830: 746f 7263 682e 7261 6e64 2832 2c39 2c31  torch.rand(2,9,1
+00004840: 362c 3136 292e 746f 2864 6576 6963 6529  6,16).to(device)
+00004850: 0d0a 2020 2020 7374 6172 7420 3d20 7469  ..    start = ti
+00004860: 6d65 2829 0d0a 2020 2020 666f 7220 6920  me()..    for i 
+00004870: 696e 2072 616e 6765 2873 7465 7073 293a  in range(steps):
+00004880: 0d0a 2020 2020 2020 2020 726d 2e72 6573  ..        rm.res
+00004890: 6574 2829 0d0a 2020 2020 2020 2020 7920  et()..        y 
+000048a0: 3d20 6f70 2878 290d 0a20 2020 2020 2020  = op(x)..       
+000048b0: 2023 2070 7269 6e74 2879 2e73 6861 7065   # print(y.shape
+000048c0: 290d 0a20 2020 2065 6e64 203d 2074 696d  )..    end = tim
+000048d0: 6528 290d 0a20 2020 2070 7269 6e74 2866  e()..    print(f
+000048e0: 2274 6573 7469 6e67 2032 6420 7b6f 707d  "testing 2d {op}
+000048f0: 2c20 636f 7374 207b 656e 642d 7374 6172  , cost {end-star
+00004900: 743a 2e32 667d 2073 2229 0d0a 2020 2020  t:.2f} s")..    
+00004910: 2320 3364 0d0a 2020 2020 6f63 203d 2056  # 3d..    oc = V
+00004920: 616c 7565 5370 6163 6528 6361 6e64 6964  alueSpace(candid
+00004930: 6174 6573 3d5b 332c 3130 5d29 0d0a 2020  ates=[3,10])..  
+00004940: 2020 6b73 203d 2056 616c 7565 5370 6163    ks = ValueSpac
+00004950: 6528 6361 6e64 6964 6174 6573 3d5b 332c  e(candidates=[3,
+00004960: 352c 375d 290d 0a20 2020 206f 7020 3d20  5,7])..    op = 
+00004970: 436f 6e76 3364 2869 6e5f 6368 616e 6e65  Conv3d(in_channe
+00004980: 6c73 3d33 2c20 6f75 745f 6368 616e 6e65  ls=3, out_channe
+00004990: 6c73 3d6f 632c 206b 6572 6e65 6c5f 7369  ls=oc, kernel_si
+000049a0: 7a65 3d6b 7329 2e74 6f28 6465 7669 6365  ze=ks).to(device
+000049b0: 290d 0a20 2020 2072 6d20 3d20 5261 6e64  )..    rm = Rand
+000049c0: 6f6d 4d75 7461 746f 7228 6f70 290d 0a20  omMutator(op).. 
+000049d0: 2020 2070 7269 6e74 2827 2a27 2a38 3029     print('*'*80)
+000049e0: 0d0a 2020 2020 7820 3d20 746f 7263 682e  ..    x = torch.
+000049f0: 7261 6e64 2832 2c33 2c31 362c 3136 2c31  rand(2,3,16,16,1
+00004a00: 3629 2e74 6f28 6465 7669 6365 290d 0a20  6).to(device).. 
+00004a10: 2020 2073 7461 7274 203d 2074 696d 6528     start = time(
+00004a20: 290d 0a20 2020 2066 6f72 2069 2069 6e20  )..    for i in 
+00004a30: 7261 6e67 6528 7374 6570 7329 3a0d 0a20  range(steps):.. 
+00004a40: 2020 2020 2020 2072 6d2e 7265 7365 7428         rm.reset(
+00004a50: 290d 0a20 2020 2020 2020 2079 203d 206f  )..        y = o
+00004a60: 7028 7829 0d0a 2020 2020 2020 2020 2320  p(x)..        # 
+00004a70: 7072 696e 7428 792e 7368 6170 6529 0d0a  print(y.shape)..
+00004a80: 2020 2020 656e 6420 3d20 7469 6d65 2829      end = time()
+00004a90: 0d0a 2020 2020 7072 696e 7428 6622 7465  ..    print(f"te
+00004aa0: 7374 696e 6720 3364 207b 6f70 7d2c 2063  sting 3d {op}, c
+00004ab0: 6f73 7420 7b65 6e64 2d73 7461 7274 3a2e  ost {end-start:.
+00004ac0: 3266 7d20 7322 290d 0a                   2f} s")..
```

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/ops/embedding.py` & `hyperbox-1.4.3/hyperbox/mutables/ops/embedding.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,22 @@
         self.search_embedding_dim = False
         if all([not vs.is_search for vs in self.value_spaces.values()]):
             return False
         if is_searchable(getattr(self.value_spaces, 'embedding_dim', None)):
             self.search_embedding_dim = True
         return True
 
+    @property
+    def params(self):
+        weight = self.weight
+        if self.search_embedding_dim:
+            weight = weight[:, :self.value_spaces['embedding_dim'].value]
+        size = weight.numel()
+        return size
+
 
 if __name__ == "__main__":
     from hyperbox.mutator import RandomMutator
     for i in range(10):
         embed_dim = ValueSpace([10, 20])
         embedding = Embedding(
             10, embed_dim, max_norm=1.0, norm_type=2.0,
```

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/ops/groupnorm.py` & `hyperbox-1.4.3/hyperbox/mutables/ops/groupnorm.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,25 @@
         if not self.is_search:
             x = F.group_norm(input, self.num_groups, self.weight, self.bias, self.eps)
         else:
             n_groups = self.value_spaces['num_groups'].value if self.search_num_groups else self.num_groups
             n_channels = self.value_spaces['num_channels'].value if self.search_num_channels else self.num_channels
             return F.group_norm(input, n_groups, self.weight[:n_channels], self.bias[:n_channels], self.eps)
 
+    @property
+    def params(self):
+        weight = self.weight
+        bias = self.bias
+        if self.search_num_channels:
+            weight = weight[:self.value_spaces['num_channels'].value]
+            bias = bias[:self.value_spaces['num_channels'].value] if bias is not None else None
+        parameters = [weight, bias]
+        params = sum([p.numel() for p in parameters if p is not None])
+        return params
+
 
 if __name__ == '__main__':
     from hyperbox.mutator import RandomMutator
     from hyperbox.mutables.ops import Conv2d
     input = torch.randn(20, 6, 10, 10)
 
     #### no search
```

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/ops/layernorm.py` & `hyperbox-1.4.3/hyperbox/mutables/ops/layernorm.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,25 @@
         self.search_normalized_shape = False
         if all([not vs.is_search for vs in self.value_spaces.values()]):
             return False
         if is_searchable(getattr(self.value_spaces, 'normalized_shape', None)):
             self.search_normalized_shape = True
         return True
 
+    @property
+    def params(self):
+        weight = self.weight
+        bias = self.bias
+        if self.search_normalized_shape:
+            weight = self.weight[:self.value_spaces["normalized_shape"].value]
+            bias = self.bias[:self.value_spaces["normalized_shape"].value] if self.bias is not None else None
+        parameters = [weight, bias]
+        size = sum([p.numel() for p in parameters if p is not None])
+        return size
+
 
 if __name__ == "__main__":
     # NLP Searchable Example
     from hyperbox.mutables.ops import Embedding
     from hyperbox.mutator import RandomMutator
     
     batch, sentence_length, vocab_size = 20, 5, 10000
```

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/ops/linear.py` & `hyperbox-1.4.3/hyperbox/mutables/ops/linear.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/ops/multihead_attention.py` & `hyperbox-1.4.3/hyperbox/mutables/ops/multihead_attention.py`

 * *Files 20% similar despite different names*

```diff
@@ -76,22 +76,84 @@
         max_embed_dim = self.embed_dim
         embed_dim_candidates = sorted(self.value_spaces['embed_dim'].candidates_original)
         
         matrices = {}
         for i in range(len(embed_dim_candidates) - 1):
             dim_small = embed_dim_candidates[i]
 
-            # weiights
-            if self.transform_params_method == 'Large2Small':
+            if self.transform_params_method == 'PoolConv':
+                assert max_embed_dim % dim_small == 0, \
+                    f'embed_dim ({max_embed_dim}) must be divisible by candidate dim ({dim_small})'
+                downsample_ratio = max_embed_dim // dim_small
+                downsample_times = int(math.log2(downsample_ratio))
+                
+                # in_proj_weight
+                param_name = f'in_proj_weight_TM_{max_embed_dim}to{dim_small}'
+                matrices[param_name] = nn.Sequential(
+                    *[nn.Sequential(
+                        # nn.AvgPool2d(2),
+                        nn.Conv2d(1, 1, 3, 2, 1, bias=False)
+                    ) for i in range(downsample_times)],
+                )
+
+                # out_proj_weight
+                param_name = f'out_proj_weight_TM_{max_embed_dim}to{dim_small}'
+                matrices[param_name] = nn.Sequential(
+                    *[nn.Sequential(
+                        # nn.AvgPool2d(2),
+                        nn.Conv2d(1, 1, 3, 2, 1, bias=False)
+                    ) for i in range(downsample_times)],
+                )
+
+                # in_proj_bias
+                if self.in_proj_bias is not None:
+                    param_name = f'in_proj_bias_TM_{max_embed_dim}to{dim_small}'
+                    matrices[param_name] = nn.Sequential(
+                        *[nn.Sequential(
+                            # nn.AvgPool1d(2),
+                            nn.Conv1d(1, 1, 3, 2, 1, bias=False)
+                        ) for i in range(downsample_times)]
+                    )
+                
+                # out_proj_bias
+                if self.out_proj.bias is not None:
+                    param_name = f'out_proj_bias_TM_{max_embed_dim}to{dim_small}'
+                    matrices[param_name] = nn.Sequential(
+                        *[nn.Sequential(
+                            # nn.AvgPool1d(2),
+                            nn.Conv1d(1, 1, 3, 2, 1, bias=False)
+                        ) for i in range(downsample_times)]
+                    )
+
+                # bias_k
+                if self.bias_k is not None:
+                    param_name = f'bias_k_TM_{max_embed_dim}to{dim_small}'
+                    matrices[param_name] = nn.Sequential(
+                        *[nn.Sequential(
+                            # nn.AvgPool1d(2),
+                            nn.Conv1d(1, 1, 3, 2, 1, bias=False)
+                        ) for i in range(downsample_times)]
+                    )
+
+                # bias_v
+                if self.bias_v is not None:
+                    param_name = f'bias_v_TM_{max_embed_dim}to{dim_small}'
+                    matrices[param_name] = nn.Sequential(
+                        *[nn.Sequential(
+                            # nn.AvgPool1d(2),
+                            nn.Conv1d(1, 1, 3, 2, 1, bias=False)
+                        ) for i in range(downsample_times)]
+                    )
+            elif self.transform_params_method == 'Large2Small':
                 # in_proj_weight
                 left_param_name = f'in_proj_weight_left_TM_{max_embed_dim}to{dim_small}'
                 right_param_name = f'in_proj_weight_right_TM_{max_embed_dim}to{dim_small}'
-                matrices[left_param_name] = Parameter(torch.eye(3*dim_small, 3*max_embed_dim))
-                matrices[right_param_name] = Parameter(torch.eye(max_embed_dim, dim_small))               
-                
+                matrices[left_param_name] = Parameter(torch.eye(dim_small, 3*max_embed_dim))
+                matrices[right_param_name] = Parameter(torch.eye(max_embed_dim, 3*dim_small))
+
                 # out_proj_weight
                 left_param_name = f'out_proj_weight_left_TM_{max_embed_dim}to{dim_small}'
                 right_param_name = f'out_proj_weight_right_TM_{max_embed_dim}to{dim_small}'
                 matrices[left_param_name] = Parameter(torch.eye(dim_small, max_embed_dim))
                 matrices[right_param_name] = Parameter(torch.eye(max_embed_dim, dim_small))
 
                 # in_proj_bias
@@ -112,19 +174,19 @@
                 # bias_v
                 if self.bias_v is not None:
                     param_name = f'bias_v_TM_{max_embed_dim}to{dim_small}'
                     matrices[param_name] = Parameter(torch.eye(max_embed_dim, dim_small))
             elif self.transform_params_method == 'TruncatedLinear':
                 # in_proj_weight
                 param_name = f'in_proj_weight_TM_{dim_small}'
-                matrices[param_name] = Parameter(torch.eye(3*dim_small, 3*dim_small))
+                matrices[param_name] = Parameter(torch.eye(dim_small, dim_small))
 
                 # out_proj_weight
                 param_name = f'out_proj_weight_TM_{dim_small}'
-                matrices[param_name] = Parameter(torch.eye(dim_small, max_embed_dim))
+                matrices[param_name] = Parameter(torch.eye(dim_small, dim_small))
 
                 # in_proj_bias
                 if self.in_proj_bias is not None:
                     param_name = f'in_proj_bias_TM_{dim_small}'
                     matrices[param_name] = Parameter(torch.eye(3*dim_small, 3*dim_small))
 
                 # out_proj_bias
@@ -140,16 +202,19 @@
                 # bias_v
                 if self.bias_v is not None:
                     param_name = f'bias_v_TM_{dim_small}'
                     matrices[param_name] = Parameter(torch.eye(dim_small, dim_small))
             else:
                 raise NotImplementedError
                 
-        for name, param in matrices.items():
-            self.register_parameter(name, param)
+        for name, val in matrices.items():
+            if isinstance(val, Parameter):
+                self.register_parameter(name, val)
+            elif isinstance(val, nn.Module):
+                self.add_module(name, val)
 
     def forward(
         self,
         query: Tensor, # (BatchSize, TargetSeqLength, EmbedDim) if batch_first is True else (TargetSeqLength, BatchSize, EmbedDim)
         key: Tensor,   # (BatchSize, SourceSeqLength, EmbedDim) if batch_first is True else (SourceSeqLength, BatchSize, EmbedDim) 
         value: Tensor, # (BatchSize, SourceSeqLength, EmbedDim) if batch_first is True else (SourceSeqLength, BatchSize, EmbedDim) 
         key_padding_mask: Optional[Tensor] = None, # require a mask of shape (BatchSize, SourceSeqLength). 
@@ -169,16 +234,15 @@
                 query, key, value, self.embed_dim, self.num_heads,
                 self.in_proj_weight, self.in_proj_bias,
                 self.bias_k, self.bias_v, self.add_zero_attn,
                 self.dropout, self.out_proj.weight, self.out_proj.bias,
                 training=self.training,
                 key_padding_mask=key_padding_mask, need_weights=need_weights,
                 attn_mask=attn_mask)
-        else:
-            
+        else:            
             if self.search_num_heads:
                 num_heads = self.value_spaces['num_heads'].value
             else:
                 num_heads = self.num_heads
             if self.search_embed_dim:
                 embed_dim = self.value_spaces['embed_dim'].value
             else:
@@ -197,20 +261,39 @@
             return attn_output.transpose(1, 0), attn_output_weights
         else:
             return attn_output, attn_output_weights
 
     def transform_params(self, embed_dim):
         if embed_dim == self.embed_dim:
             return self.in_proj_weight, self.in_proj_bias, self.bias_k, self.bias_v, self.out_proj.weight, self.out_proj.bias
-        if self.transform_params_method == 'Large2Small':
+        if self.transform_params_method == 'PoolConv':
+            in_proj_weight = getattr(
+                self, f'in_proj_weight_TM_{self.embed_dim}to{embed_dim}'
+                )(self.in_proj_weight.unsqueeze(0).unsqueeze(0)).squeeze(0).squeeze(0)
+            out_proj_weight = getattr(
+                self, f'out_proj_weight_TM_{self.embed_dim}to{embed_dim}'
+                )(self.out_proj.weight.unsqueeze(0).unsqueeze(0)).squeeze(0).squeeze(0)
+            in_proj_bias = getattr(
+                self, f'in_proj_bias_TM_{self.embed_dim}to{embed_dim}'
+                )(self.in_proj_bias.unsqueeze(0)).squeeze(0) if self.in_proj_bias is not None else None
+            out_proj_bias = getattr(
+                self, f'out_proj_bias_TM_{self.embed_dim}to{embed_dim}'
+                )(self.out_proj.bias.unsqueeze(0)).squeeze(0) if self.out_proj.bias is not None else None
+            bias_k = getattr(
+                self, f'bias_k_TM_{self.embed_dim}to{embed_dim}'
+                )(self.bias_k.unsqueeze(0)).squeeze(0) if self.bias_k is not None else None
+            bias_v = getattr(
+                self, f'bias_v_TM_{self.embed_dim}to{embed_dim}'
+                )(self.bias_v.unsqueeze(0)).squeeze(0) if self.bias_v is not None else None
+        elif self.transform_params_method == 'Large2Small':
             # weights
             in_proj_weight = self.param_transform_via_TM(
                 self.in_proj_weight,
                 L_transform_matrix=getattr(self, f'in_proj_weight_left_TM_{self.embed_dim}to{embed_dim}'),
-                R_transform_matrix=getattr(self, f'in_proj_weight_right_TM_{self.embed_dim}to{embed_dim}'))
+                R_transform_matrix=getattr(self, f'in_proj_weight_right_TM_{self.embed_dim}to{embed_dim}')).T
             out_proj_weight = self.param_transform_via_TM(
                 self.out_proj.weight,
                 L_transform_matrix=getattr(self, f'out_proj_weight_left_TM_{self.embed_dim}to{embed_dim}'),
                 R_transform_matrix=getattr(self, f'out_proj_weight_right_TM_{self.embed_dim}to{embed_dim}'))
 
             # biases
             in_proj_bias = self.param_transform_via_TM(
@@ -281,44 +364,104 @@
             constant_(self.in_proj_bias, 0.)
             constant_(self.out_proj.bias, 0.)
         if self.bias_k is not None:
             xavier_normal_(self.bias_k)
         if self.bias_v is not None:
             xavier_normal_(self.bias_v)
 
+    @property
+    def params(self):
+        in_proj_weight = self.in_proj_weight
+        in_proj_bias = self.in_proj_bias
+        out_proj_weight = self.out_proj.weight
+        out_proj_bias = self.out_proj.bias
+        bias_k = self.bias_k
+        bias_v = self.bias_v
+        if self.search_embed_dim:
+            embed_dim = self.value_spaces['embed_dim'].value
+            in_proj_weight = in_proj_weight[:3 * embed_dim, :embed_dim]
+            in_proj_bias = in_proj_bias[:3 * embed_dim] if in_proj_bias is not None else None
+            out_proj_weight = out_proj_weight[:embed_dim, :embed_dim]
+            out_proj_bias = out_proj_bias[:embed_dim] if out_proj_bias is not None else None
+            bias_k = bias_k[:, :, :embed_dim] if bias_k is not None else None
+            bias_v = bias_v[:, :, :embed_dim] if bias_v is not None else None
+        parameters = [in_proj_weight, in_proj_bias, out_proj_weight, out_proj_bias, bias_k, bias_v]
+        size = sum([p.numel() for p in parameters if p is not None])
+        return size
+        
 
 if __name__ == '__main__':
     import timeit
+    from time import time
     from hyperbox.mutables.ops import Linear
     from hyperbox.networks.base_nas_network import BaseNASNetwork
     from hyperbox.mutator import RandomMutator
     
     class Net(BaseNASNetwork):
         def __init__(self, dim_in, dims, heads, transform_params_method='TruncatedLinear'):
             super().__init__()
             self.linear = Linear(dim_in, dims)
-            self.mha = MultiheadAttention(dims, heads, 0.1, True)
+            self.mha = MultiheadAttention(dims, heads, 0.1, True,
+                                          transform_params_method=transform_params_method)
+            self.linear_time = []
+            self.mha_time = []
         def forward(self, x):
+            start = time()
             x = self.linear(x)
+            end = time()
+            self.linear_time.append(end-start)
+            
+            start = time()
             y = self.mha(x, x, x)
+            end = time()
+            self.mha_time.append(end-start)
             return y[0]
 
-    for tpm in ['TruncatedLinear', 'Large2Small', 'disbale']:
-        print(f"...")
+    for tpm in [
+            'disable', 
+            'Large2Small', 
+            'PoolConv', 
+            'TruncatedLinear'
+        ]:
+        print(f"testing {tpm}...")
         dims = ValueSpace([256, 512, 1024])
         heads = ValueSpace([4, 8, 16])
-        device = 'mps'
+        # device = 'mps'
+        device = 'cuda' if torch.cuda.is_available() else 'cpu'
         dim_in = 128
         net = Net(dim_in, dims, heads, tpm).to(device)
+        total_params = sum(p.numel() for p in net.parameters())
+        if tpm == 'disable':
+            TM_params = 0
+        else:
+            TM_params = sum(p.numel() for name, p in net.named_parameters() if 'TM' in name)
+        print(f"Testing {tpm}: Total params: {total_params}, TM params: {TM_params} ({TM_params/total_params:.2%})")
         rm = RandomMutator(net)
-        x = torch.rand(2, 10, dim_in).to(device)
-        
-        for i in range(10):
+        x = torch.rand(16, 512, dim_in).to(device)
+
+        steps = 100
+        start = time()
+        reset_times = []
+        fw_times = []
+        bw_times = []
+        for i in range(steps):
+            start1 = time()
             rm.reset()
+            end1 = time()
+            reset_times.append(end1-start1)
+            start2 = time()
             y = net(x)
-            # print(net.arch)
-            # print(y[0].shape)
-
-        def test_forward():
-            net(x)
-        t = timeit.timeit(test_forward, number=200, globals=globals())
-        print(f"Testing {tpm}: Time taken about {t:.6f} seconds")
+            end2 = time()
+            fw_times.append(end2-start2)
+            start3 = time()
+            loss = y.sum()
+            loss.backward()
+            end3 = time()
+            bw_times.append(end3-start3)
+        end = time()
+        print(f"Testing {tpm}: Time taken about {(end-start)/(steps-5):.6f} seconds")
+        print(f"\treset time: {sum(reset_times[5:])/(steps-5):.6f}")
+        print(f"\tforward time: {sum(fw_times[5:])/(steps-5):.6f}")
+        print(f"\t\tlinear time: {sum(net.linear_time[5:])/(steps-5):.6f}")
+        print(f"\t\tmha time: {sum(net.mha_time[5:])/(steps-5):.6f}")
+        print(f"\tbackward time: {sum(bw_times[5:])/(steps-5):.6f}")
+        print('*'*20)
```

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/ops/utils.py` & `hyperbox-1.4.3/hyperbox/mutables/ops/utils.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutables/spaces.py` & `hyperbox-1.4.3/hyperbox/mutables/spaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,24 @@
     @property
     def max_value(self):
         try:
             value = max(self.candidates_original)
             return value
         except Expection as e:
             logger.warning(str(e))
+            logger.warning("The candidates cannot be compared to get max value, return the last item instead.")
+            return self.candidates_original[-1]
+
+    @property
+    def min_value(self):
+        try:
+            value = min(self.candidates_original)
+            return value
+        except Expection as e:
+            logger.warning(str(e))
             logger.warning("The candidates cannot be compared to get max value, return the first item instead.")
             return self.candidates_original[0]
 
     def forward(self):
         logger.warning(f'You should not run forward of {self.__class__.__name__} directly.')
         return self.value
```

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/__init__.py` & `hyperbox-1.4.3/hyperbox/mutator/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/base_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/base_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/darts_multiple_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/darts_multiple_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/darts_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/darts_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/default_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/default_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/ea_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/ea_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/enas_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/enas_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/evolution_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/evolution_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/fairnas_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/fairnas_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/fewshot_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/fewshot_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/fixed_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/fixed_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/hete_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/hete_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/onehot_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/onehot_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/proxyless_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/proxyless_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/random_multiple_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/random_multiple_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/random_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/random_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/repnas_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/repnas_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/sequential_mutator.py` & `hyperbox-1.4.3/hyperbox/mutator/sequential_mutator.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/mutator/utils.py` & `hyperbox-1.4.3/hyperbox/mutator/utils.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/base_nas_network.py` & `hyperbox-1.4.3/hyperbox/networks/base_nas_network.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,10 +197,16 @@
     def load_from_ckpt(self, ckpt):
         '''load from the checkpoint of model
         ckpt includes `state_dict` of network, optimizer, and mutator in `BaseModel`.
         '''
         to_copy_weight = extract_net_from_ckpt(ckpt)
         self.load_state_dict(to_copy_weight)
 
-    def to_pipeline(self):
+    def to_pipeline_layers(self):
         '''convert to pipeline network'''
-        raise NotImplementedError
+        layers = []
+        for name, m in self.named_children():
+            if isinstance(m, nn.Sequential):
+                layers.append(*m)
+            else:
+                layers.append(m)
+        return m
```

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/bnnas/bn_blocks.py` & `hyperbox-1.4.3/hyperbox/networks/bnnas/bn_blocks.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/bnnas/bn_net.py` & `hyperbox-1.4.3/hyperbox/networks/bnnas/bn_net.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/bnnas/ea_search.py` & `hyperbox-1.4.3/hyperbox/networks/bnnas/ea_search.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/darts/darts_network.py` & `hyperbox-1.4.3/hyperbox/networks/darts/darts_network.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/darts/darts_ops.py` & `hyperbox-1.4.3/hyperbox/networks/darts/darts_ops.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/enas/enas_network.py` & `hyperbox-1.4.3/hyperbox/networks/enas/enas_network.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/enas/enas_ops.py` & `hyperbox-1.4.3/hyperbox/networks/enas/enas_ops.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/gpt/gpt2.py` & `hyperbox-1.4.3/hyperbox/networks/gpt/gpt2.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/mobilenet/mobile3d_net.py` & `hyperbox-1.4.3/hyperbox/networks/mobilenet/mobile3d_net.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/mobilenet/mobile3d_ops.py` & `hyperbox-1.4.3/hyperbox/networks/mobilenet/mobile3d_ops.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/mobilenet/mobile_net.py` & `hyperbox-1.4.3/hyperbox/networks/mobilenet/mobile_net.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/mobilenet/mobile_ops.py` & `hyperbox-1.4.3/hyperbox/networks/mobilenet/mobile_ops.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/mobilenet/mobile_utils.py` & `hyperbox-1.4.3/hyperbox/networks/mobilenet/mobile_utils.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench101/base_ops.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench101/base_ops.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/db_gen.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/db_gen.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/graph_util.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/graph_util.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/model.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/model.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench101/db_gen/query.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench101/db_gen/query.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench101/graph_util.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench101/graph_util.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench101/model_spec.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench101/model_spec.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench101/nasbench101.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench101/nasbench101.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench201/db_gen/db_gen.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench201/db_gen/db_gen.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench201/db_gen/model.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench201/db_gen/model.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench201/db_gen/query.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench201/db_gen/query.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench201/nasbench201.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench201/nasbench201.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench301/nasbench301_network.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench301/nasbench301_network.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench301/utils.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench301/utils.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/nasbench_mbnet/network.py` & `hyperbox-1.4.3/hyperbox/networks/nasbench_mbnet/network.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/network_ema.py` & `hyperbox-1.4.3/hyperbox/networks/network_ema.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/pytorch_modules.py` & `hyperbox-1.4.3/hyperbox/networks/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/repnas/rep_ops.py` & `hyperbox-1.4.3/hyperbox/networks/repnas/rep_ops.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/repnas/repnas_spos.py` & `hyperbox-1.4.3/hyperbox/networks/repnas/repnas_spos.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/repnas/utils.py` & `hyperbox-1.4.3/hyperbox/networks/repnas/utils.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/resnet/resnet.py` & `hyperbox-1.4.3/hyperbox/networks/resnet/resnet.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/rnn/genotypes.py` & `hyperbox-1.4.3/hyperbox/networks/rnn/genotypes.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/rnn/rnn.py` & `hyperbox-1.4.3/hyperbox/networks/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/rnn/utils.py` & `hyperbox-1.4.3/hyperbox/networks/rnn/utils.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/spos/shuffle_blocks.py` & `hyperbox-1.4.3/hyperbox/networks/spos/shuffle_blocks.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/spos/spos_net.py` & `hyperbox-1.4.3/hyperbox/networks/spos/spos_net.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/utils.py` & `hyperbox-1.4.3/hyperbox/networks/utils.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/networks/vit/vit.py` & `hyperbox-1.4.3/hyperbox/networks/vit/vit.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         dropout: float = 0., # dropout rate
         suffix: str = '', # suffix for the name of the module
         mask= None, # mask for the search space (mutables)
     ):
         super().__init__()
         self.mask = mask
         hidden_dim_list = keepPositiveList([int(r*hidden_dim) for r in search_ratio])
-        hidden_dim_list = spaces.ValueSpace(hidden_dim_list, key=f"{suffix}_hidden_dim", mask=self.mask)
+        hidden_dim_list = spaces.ValueSpace(hidden_dim_list, key=f"{suffix}_hidden_dim", mask=self.mask) if len(hidden_dim_list) > 1 else hidden_dim_list[0]
         self.net = nn.Sequential(
             ops.Linear(dim, hidden_dim_list),
             nn.GELU(),
             nn.Dropout(dropout),
             ops.Linear(hidden_dim_list, dim),
             nn.Dropout(dropout)
         )
@@ -81,33 +81,37 @@
         mask: dict = None, # mask for the search space (mutables)
     ):
         super().__init__()
         self.mask = mask
         self.heads_list = keepPositiveList([int(r*heads) for r in search_ratio])
         self.dim_head_list = keepPositiveList([int(r*dim_head) for r in search_ratio])
         self.scale_list = [dh**-0.5 for dh in self.dim_head_list]
-        
+
         self.inner_dim_list = []
         self.heads_idx_map = {}
         self.dim_head_idx_map = {}
         count = 0
         for h_idx, h in enumerate(self.heads_list):
             for d_idx, d in enumerate(self.dim_head_list):
                 inner_dim = h * d
                 self.inner_dim_list.append(inner_dim)
                 self.heads_idx_map[count] = h_idx
                 self.dim_head_idx_map[count] = d_idx
                 count += 1
-        self.inner_dim_list = spaces.ValueSpace(self.inner_dim_list, key=f"{suffix}_inner_dim", mask=self.mask)
+        self.inner_dim_list = spaces.ValueSpace(self.inner_dim_list, key=f"{suffix}_inner_dim", mask=self.mask) \
+            if len(self.inner_dim_list) > 1 else self.inner_dim_list[0]
         
         self.attend = nn.Softmax(dim = -1)
         self.dropout = nn.Dropout(dropout)
 
-        qkv_dim_list = [x*3 for x in self.inner_dim_list.candidates_original]
-        qkv_dim_list = spaces.ValueSpace(qkv_dim_list, key=f"{suffix}_inner_dim", mask=self.mask) # coupled with self.inner_dim_list
+        if isinstance(self.inner_dim_list, spaces.ValueSpace):
+            qkv_dim_list = [x*3 for x in self.inner_dim_list.candidates_original]
+            qkv_dim_list = spaces.ValueSpace(qkv_dim_list, key=f"{suffix}_inner_dim", mask=self.mask) # coupled with self.inner_dim_list
+        else:
+            qkv_dim_list = self.inner_dim_list * 3
         self.to_qkv = ops.Linear(dim, qkv_dim_list, bias = False)
 
         self.to_out = nn.Sequential(
             ops.Linear(self.inner_dim_list, dim),
             nn.Dropout(dropout)
         )
 
@@ -122,27 +126,33 @@
 
         out = torch.matmul(attn, v)
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
     @property
     def heads(self):
-        idx = self.inner_dim_list.index
-        if idx is None:
-            idx = self.inner_dim_list.mask.float().argmax().item()
-        idx = self.heads_idx_map[idx]
-        return self.heads_list[idx]
+        if isinstance(self.inner_dim_list, spaces.ValueSpace):
+            idx = self.inner_dim_list.index
+            if idx is None:
+                idx = self.inner_dim_list.mask.float().argmax().item()
+            idx = self.heads_idx_map[idx]
+            return self.heads_list[idx]
+        else:
+            return self.heads_list[0]
     
     @property
     def scale(self):
-        idx = self.inner_dim_list.index
-        if idx is None:
-            idx = self.inner_dim_list.mask.float().argmax().item()
-        idx = self.dim_head_idx_map[idx]
-        return self.scale_list[idx]
+        if isinstance(self.inner_dim_list, spaces.ValueSpace):
+            idx = self.inner_dim_list.index
+            if idx is None:
+                idx = self.inner_dim_list.mask.float().argmax().item()
+            idx = self.dim_head_idx_map[idx]
+            return self.scale_list[idx]
+        else:
+            return self.scale_list[0]
 
     @property
     def dim_head(self):
         idx = self.inner_dim_list.index
         if idx is None:
             idx = self.inner_dim_list.mask.float().argmax().item()
         idx = self.dim_head_idx_map[idx]
@@ -182,14 +192,23 @@
         cls_tokens = repeat(self.cls_token, '1 1 d -> b 1 d', b = b)
         x = torch.cat((cls_tokens, x), dim=1)
         x += self.pos_embedding[:, :(n + 1)]
         x = self.dropout(x)
         return x
 
 
+class ResidualBlock(nn.Module):
+    def __init__(self, block):
+        super().__init__()
+        self.block = block
+
+    def forward(self, x):
+        return self.block(x) + x
+
+
 class VitBlock(nn.Module):
     def __init__(
         self,
         dim: int, # dimension of the model
         heads: int, # number of heads
         dim_head: int, # dimension of each head
         mlp_dim: int, # dimension of the feedforward layer
@@ -200,24 +219,24 @@
     ):
         super().__init__()
         self.search_ratio = search_ratio
         self.mask = mask
         self.suffix = suffix
         attKey = f"att_{suffix}"
         ffKey = f"ff_{suffix}"
-        self.attn = PreNorm(dim, Attention(
+        self.attn = ResidualBlock(PreNorm(dim, Attention(
             dim, heads = heads, dim_head = dim_head, search_ratio=self.search_ratio,
-            dropout = dropout, suffix = attKey, mask = self.mask))
-        self.ff = PreNorm(dim, FeedForward(
+            dropout = dropout, suffix = attKey, mask = self.mask)))
+        self.ff = ResidualBlock(PreNorm(dim, FeedForward(
             dim, mlp_dim, search_ratio=self.search_ratio, dropout = dropout,
-            suffix = ffKey, mask = self.mask))
+            suffix = ffKey, mask = self.mask)))
 
     def forward(self, x):
-        x = self.attn(x) + x
-        x = self.ff(x) + x
+        x = self.attn(x)
+        x = self.ff(x)
         return x
 
 
 class VitClsHead(nn.Module):
     def __init__(
         self,
         pool: str, # 'cls' or 'mean'
@@ -262,27 +281,27 @@
         mask: dict = None, # mask for the search space (mutables)
     ):
         super().__init__(mask = mask)
         self.to_search_path = to_search_depth
         
         self.vit_embed = VitEmbedding(image_size, patch_size, channels, dim, emb_dropout)
 
-        if self.to_search_path:
-            runtime_depth = [v for v in range(1, depth + 1)]    
-            self.run_depth = spaces.ValueSpace(runtime_depth, key='run_depth', mask=self.mask)
-
         vit_blocks = [
             VitBlock(
                 dim=dim, heads=heads, dim_head=dim_head, mlp_dim=mlp_dim,
                 search_ratio=search_ratio, dropout=dropout, suffix=i, mask=self.mask
             ) for i in range(depth)]
         self.vit_blocks = nn.Sequential(*vit_blocks)
 
         self.vit_cls_head = VitClsHead(pool, dim, num_classes)
 
+        if self.to_search_path:
+            runtime_depth = [v for v in range(1, depth + 1)]    
+            self.run_depth = spaces.ValueSpace(runtime_depth, key='run_depth', mask=self.mask)
+
     def forward(self, x):
         out = self.vit_embed(x)
         if self.to_search_path:
             vit_blocks = list(self.vit_blocks.children())
             runtime_depth = self.run_depth.value
             vit_blocks = vit_blocks[:runtime_depth]
             vit_blocks = nn.Sequential(*vit_blocks)
```

### Comparing `hyperbox-1.4.2b0/hyperbox/optimizers/lamb.py` & `hyperbox-1.4.3/hyperbox/optimizers/lamb.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/optimizers/sam.py` & `hyperbox-1.4.3/hyperbox/optimizers/sam.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/run.py` & `hyperbox-1.4.3/hyperbox/run.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/schedulers/warmup_scheduler.py` & `hyperbox-1.4.3/hyperbox/schedulers/warmup_scheduler.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/train.py` & `hyperbox-1.4.3/hyperbox/train.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/utils/average_meter.py` & `hyperbox-1.4.3/hyperbox/utils/average_meter.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/utils/calc_model_size.py` & `hyperbox-1.4.3/hyperbox/utils/calc_model_size.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,45 +30,95 @@
     m.module_used = torch.tensor([1])
 
 
 def count_FG_convNd(m, _, y):
     cin = m.value_spaces['in_channels'].value if m.search_in_channel else m.in_channels
     kernel_size = m.value_spaces['kernel_size'].value if m.search_kernel_size else m.kernel_size
     if isinstance(kernel_size, int):
-        dim = int(m.conv_dim[0])
+        dim = int(m.conv_dim)
         kernel_ops = kernel_size**dim
     elif isinstance(kernel_size, (list, tuple)):
         kernel_ops = torch.prod(torch.Tensor(kernel_size))
     ops_per_element = kernel_ops
     groups = m.value_spaces['groups'].value if m.search_groups else m.groups
     output_elements = y.nelement()
-    total_ops = cin * output_elements * ops_per_element // groups  # cout x oW x oH
+    total_ops = torch.div(cin * output_elements * ops_per_element, groups)
     m.total_ops = torch.Tensor([int(total_ops)])
     m.module_used = torch.tensor([1])
 
 
 def count_FG_linear(m, _, __):
     in_features = m.value_spaces['in_features'].value if m.search_in_features \
         else m.in_features
     out_features = m.value_spaces['out_features'].value if m.search_out_features \
         else m.out_features
     total_ops = in_features * out_features
     m.total_ops = torch.Tensor([int(total_ops)])
     m.module_used = torch.tensor([1])
 
+# Todo: add more FG ops
+# def count_FG_Embedding(m, _, __):
+#     num_embeddings = m.value_spaces['num_embeddings'].value if m.search_num_embeddings \
+#         else m.num_embeddings
+#     embedding_dim = m.value_spaces['embedding_dim'].value if m.search_embedding_dim \
+#         else m.embedding_dim
+#     total_ops = num_embeddings * embedding_dim
+#     m.total_ops = torch.Tensor([int(total_ops)])
+#     m.module_used = torch.tensor([1])
+
+
+# def count_FG_GroupNorm(m, _, __):
+#     num_channels = m.value_spaces['num_channels'].value if m.search_num_channels \
+#         else m.num_channels
+#     num_groups = m.value_spaces['num_groups'].value if m.search_num_groups \
+#         else m.num_groups
+#     total_ops = num_channels * num_groups
+#     m.total_ops = torch.Tensor([int(total_ops)])
+#     m.module_used = torch.tensor([1])
+
+
+# def count_FG_LayerNorm(m, _, __):
+#     normalized_shape = m.value_spaces['normalized_shape'].value if m.search_normalized_shape \
+#         else m.normalized_shape
+#     total_ops = torch.prod(torch.Tensor(normalized_shape))
+#     m.total_ops = torch.Tensor([int(total_ops)])
+#     m.module_used = torch.tensor([1])
+
+
+# def count_FG_MultiheadAttention(m, _, __):
+#     total_ops = 0
+#     if m.search_in_features:
+#         in_features = m.value_spaces['in_features'].value
+#         total_ops += in_features
+#     if m.search_out_features:
+#         out_features = m.value_spaces['out_features'].value
+#         total_ops += out_features
+#     if m.search_num_heads:
+#         num_heads = m.value_spaces['num_heads'].value
+#         total_ops += num_heads
+#     if m.search_dropout:
+#         dropout = m.value_spaces['dropout'].value
+#         total_ops += dropout
+#     m.total_ops = torch.Tensor([int(total_ops)])
+#     m.module_used = torch.tensor([1])
+
 
 register_hooks = {
     nn.Conv1d: count_convNd,
     nn.Conv2d: count_convNd,
     nn.Conv3d: count_convNd,
     nn.Linear: count_linear,
     hyperbox.mutables.ops.conv.Conv1d: count_FG_convNd,
     hyperbox.mutables.ops.conv.Conv2d: count_FG_convNd,
     hyperbox.mutables.ops.conv.Conv3d: count_FG_convNd,
     hyperbox.mutables.ops.linear.Linear: count_FG_linear,
+    # hyperbox.mutables.ops.embedding.Embedding: count_FG_Embedding,
+    # hyperbox.mutables.ops.GroupNorm: count_FG_GroupNorm,
+    # hyperbox.mutables.ops.LayerNorm: count_FG_LayerNorm,
+    # hyperbox.mutables.ops.MultiheadAttention: count_FG_MultiheadAttention,
 }
 
 
 def flops_size_counter(_model, input_size, convert=True, verbose=False):
     '''Calculate the flops and size of the given model
     Args:
         _model: nn.Module
```

### Comparing `hyperbox-1.4.2b0/hyperbox/utils/logger.py` & `hyperbox-1.4.3/hyperbox/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/utils/metrics.py` & `hyperbox-1.4.3/hyperbox/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/utils/utils.py` & `hyperbox-1.4.3/hyperbox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/utils/visualize_darts_cell.py` & `hyperbox-1.4.3/hyperbox/utils/visualize_darts_cell.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox/utils/visualize_mbconv_net.py` & `hyperbox-1.4.3/hyperbox/utils/visualize_mbconv_net.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/hyperbox.egg-info/SOURCES.txt` & `hyperbox-1.4.3/hyperbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/setup.cfg` & `hyperbox-1.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/setup.py` & `hyperbox-1.4.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     required = f.read().splitlines()
 for module in required:
     if not module.startswith('#'):
         required_modules.append(module)
 
 setup(
     name="hyperbox",  # you should change "src" to your project name
-    version="1.4.2.b",
+    version="1.4.3",
     description="Hyperbox: An easy-to-use NAS framework.",
     author="marsggbo",
     url="https://github.com/marsggbo/hyperbox",
     # replace with your own github project link
     install_requires=required_modules,
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `hyperbox-1.4.2b0/tests/helpers/module_available.py` & `hyperbox-1.4.3/tests/helpers/module_available.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/tests/helpers/runif.py` & `hyperbox-1.4.3/tests/helpers/runif.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/tests/smoke/test_commands.py` & `hyperbox-1.4.3/tests/smoke/test_commands.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/tests/smoke/test_mixed_precision.py` & `hyperbox-1.4.3/tests/smoke/test_mixed_precision.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/tests/smoke/test_sweeps.py` & `hyperbox-1.4.3/tests/smoke/test_sweeps.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/tests/smoke/test_wandb.py` & `hyperbox-1.4.3/tests/smoke/test_wandb.py`

 * *Files identical despite different names*

### Comparing `hyperbox-1.4.2b0/tests/unit/test_sth.py` & `hyperbox-1.4.3/tests/unit/test_sth.py`

 * *Files identical despite different names*

