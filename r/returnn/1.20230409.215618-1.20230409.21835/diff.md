# Comparing `tmp/returnn-1.20230409.215618.tar.gz` & `tmp/returnn-1.20230409.21835.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230409.215618.tar", last modified: Sun Apr  9 20:20:29 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230409.21835.tar", last modified: Sun Apr  9 00:34:28 2023, max compression
```

## Comparing `returnn-1.20230409.215618.tar` & `returnn-1.20230409.21835.tar`

### file list

```diff
@@ -1,410 +1,410 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63018 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-09 20:20:06.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-09 20:20:09.000000 returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25061 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36530 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    94908 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   154928 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36628 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   150268 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69478 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19899 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   148678 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   582337 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18948 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25786 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144495 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/py-to-pickle.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187447 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:20:29.000000 returnn-1.20230409.215618/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-09 20:20:04.000000 returnn-1.20230409.215618/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63018 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24201 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36530 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93069 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155711 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36628 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150268 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69478 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19899 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148678 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   582337 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292822 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23698 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144495 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/py-to-pickle.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187447 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230409.215618/.gitignore` & `returnn-1.20230409.21835/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/.gitmodules` & `returnn-1.20230409.21835/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/CHANGELOG.md` & `returnn-1.20230409.21835/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/CODEOWNERS` & `returnn-1.20230409.21835/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/CONTRIBUTING.md` & `returnn-1.20230409.21835/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/LICENSE` & `returnn-1.20230409.21835/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/MANIFEST.in` & `returnn-1.20230409.21835/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/PKG-INFO` & `returnn-1.20230409.21835/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230409.215618
+Version: 1.20230409.21835
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230409.215618/README.rst` & `returnn-1.20230409.21835/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/__init__.py` & `returnn-1.20230409.21835/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/12AX.cluster_map` & `returnn-1.20230409.21835/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-fwd.config` & `returnn-1.20230409.21835/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-horovod-mpi.py` & `returnn-1.20230409.21835/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230409.21835/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-hyper-param-tuning.config` & `returnn-1.20230409.21835/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-iter-dataset.py` & `returnn-1.20230409.21835/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-list-devices.py` & `returnn-1.20230409.21835/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-lua-torch-layer.config` & `returnn-1.20230409.21835/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230409.21835/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-returnn-as-framework.py` & `returnn-1.20230409.21835/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-rf.config` & `returnn-1.20230409.21835/demos/demo-rf.config`

 * *Files 7% similar despite different names*

```diff
@@ -45,18 +45,17 @@
 
 def get_model(**_kwargs):
     return Model()
 
 def train_step(*, model: Model, extern_data, **_kwargs):
     data = extern_data["data"]
     logits = model(data)
-    logits_packed, pack_dim = rf.pack(logits, dims=(batch_dim, time_dim), enforce_sorted=False)
     targets = extern_data["classes"]
-    targets_packed, _ = rf.pack(targets, dims=(batch_dim, time_dim), enforce_sorted=False, out_dim=pack_dim)
-    loss = rf.cross_entropy(estimated=logits_packed, estimated_type="logits", target=targets_packed, axis=out_dim)
+    # TODO: use flattening on logits/targets
+    loss = rf.cross_entropy(estimated=logits, estimated_type="logits", target=targets, axis=out_dim)
     loss.mark_as_loss(name="ce")
 
 
 # training
 optimizer = {"class": "adam"}
 
 learning_rate = 0.01
```

### Comparing `returnn-1.20230409.215618/demos/demo-rhn-enwik8.config` & `returnn-1.20230409.21835/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-sprint-interface.py` & `returnn-1.20230409.21835/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-att-copy.config` & `returnn-1.20230409.21835/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-attention.config` & `returnn-1.20230409.21835/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-enc-dec.config` & `returnn-1.20230409.21835/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230409.21835/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230409.21835/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230409.21835/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230409.21835/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230409.21835/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-rec-self-att.config` & `returnn-1.20230409.21835/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230409.21835/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230409.21835/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-torch.config` & `returnn-1.20230409.21835/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/demo.sh` & `returnn-1.20230409.21835/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/README.txt` & `returnn-1.20230409.21835/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/config_demo` & `returnn-1.20230409.21835/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230409.21835/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/config_real` & `returnn-1.20230409.21835/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230409.21835/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/decode.py` & `returnn-1.20230409.21835/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230409.21835/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230409.21835/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230409.21835/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230409.21835/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230409.21835/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230409.21835/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230409.21835/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/__init__.py` & `returnn-1.20230409.21835/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/__main__.py` & `returnn-1.20230409.21835/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/__old_mod_loader__.py` & `returnn-1.20230409.21835/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/__setup__.py` & `returnn-1.20230409.21835/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/config.py` & `returnn-1.20230409.21835/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/audio.py` & `returnn-1.20230409.21835/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/basic.py` & `returnn-1.20230409.21835/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/bundle_file.py` & `returnn-1.20230409.21835/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/cached.py` & `returnn-1.20230409.21835/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/cached2.py` & `returnn-1.20230409.21835/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/generating.py` & `returnn-1.20230409.21835/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/hdf.py` & `returnn-1.20230409.21835/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/lm.py` & `returnn-1.20230409.21835/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/map.py` & `returnn-1.20230409.21835/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/meta.py` & `returnn-1.20230409.21835/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/multi_proc.py` & `returnn-1.20230409.21835/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/normalization_data.py` & `returnn-1.20230409.21835/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/numpy_dump.py` & `returnn-1.20230409.21835/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/raw_wav.py` & `returnn-1.20230409.21835/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/sprint.py` & `returnn-1.20230409.21835/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/stereo.py` & `returnn-1.20230409.21835/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230409.21835/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/datasets/util/vocabulary.py` & `returnn-1.20230409.21835/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/engine/base.py` & `returnn-1.20230409.21835/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/engine/batch.py` & `returnn-1.20230409.21835/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/graph_editor/edit.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/graph_editor/select.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/graph_editor/transform.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/extern/graph_editor/util.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/__init__.py` & `returnn-1.20230409.21835/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/_backend.py` & `returnn-1.20230409.21835/returnn/frontend/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,23 +123,14 @@
         backend = get_backend_by_raw_tensor_type(type(raw_tensor))
         existing_shape = backend.get_known_shape_raw(raw_tensor)
         assert all(dim is not None for dim in existing_shape)
         assert len(shape) == len(existing_shape)
         assert all(dim is None or dim == existing_shape[i] for i, dim in enumerate(shape))
 
     @staticmethod
-    def get_new_dim_raw(raw_tensor: T, axis: int) -> Dim:
-        """
-        :param raw_tensor:
-        :param axis:
-        :return: dim tag of axis
-        """
-        raise NotImplementedError
-
-    @staticmethod
     def fill_raw(shape: Union[Sequence[Union[int, T]], T], value: Union[Any, T]) -> T:
         """
         :param shape: shape
         :param value: scalar value to fill
         :return: raw tensor filled with value everywhere
         """
         raise NotImplementedError
@@ -616,29 +607,14 @@
         out: Optional[Tensor] = None,
     ) -> Tensor:
         """
         random. See `rf.random` for details.
         """
         raise NotImplementedError
 
-    @staticmethod
-    def masked_select(
-        tensor: Tensor, *, mask: Tensor, dims: Sequence[Dim], out_dim: Optional[Dim] = None
-    ) -> Tuple[Tensor, Dim]:
-        """
-        :param tensor:
-        :param mask:
-        :param dims: the order of the dims defines the format. those dims should be exactly the dims of the mask.
-        :param out_dim:
-        :return: tensor where all dims in mask/dims are removed and replaced by a new dim.
-            the new dim is also returned.
-            if mask==True for all elements, the returned tensor would be simply the flattened input tensor.
-        """
-        raise NotImplementedError
-
 
 # We use a global instance, and we modify __class__ inplace,
 # such that any reference to this can be updated.
 # This is exposed to the user as `returnn.frontend`.
 # The __class__ assignment is done in `select_engine`.
 # Use object.__new__ because we disallow creating instances of Frontend.
 global_backend = object.__new__(Backend)
```

### Comparing `returnn-1.20230409.215618/returnn/frontend/_numpy_backend.py` & `returnn-1.20230409.21835/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/_utils.py` & `returnn-1.20230409.21835/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/const.py` & `returnn-1.20230409.21835/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/dims.py` & `returnn-1.20230409.21835/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/dtype.py` & `returnn-1.20230409.21835/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/init.py` & `returnn-1.20230409.21835/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/linear.py` & `returnn-1.20230409.21835/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/loss.py` & `returnn-1.20230409.21835/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/math_.py` & `returnn-1.20230409.21835/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/matmul.py` & `returnn-1.20230409.21835/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/module.py` & `returnn-1.20230409.21835/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/parameter.py` & `returnn-1.20230409.21835/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/rand.py` & `returnn-1.20230409.21835/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/reduce.py` & `returnn-1.20230409.21835/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/run_ctx.py` & `returnn-1.20230409.21835/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/state.py` & `returnn-1.20230409.21835/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/frontend/types.py` & `returnn-1.20230409.21835/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/import_/common.py` & `returnn-1.20230409.21835/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/import_/git.py` & `returnn-1.20230409.21835/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/import_/import_.py` & `returnn-1.20230409.21835/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/learning_rate_control.py` & `returnn-1.20230409.21835/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/log.py` & `returnn-1.20230409.21835/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/native_op.cpp` & `returnn-1.20230409.21835/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/native_op.py` & `returnn-1.20230409.21835/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/pretrain.py` & `returnn-1.20230409.21835/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/sprint/cache.py` & `returnn-1.20230409.21835/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/sprint/control.py` & `returnn-1.20230409.21835/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/sprint/error_signals.py` & `returnn-1.20230409.21835/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/sprint/extern_interface.py` & `returnn-1.20230409.21835/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/sprint/interface.py` & `returnn-1.20230409.21835/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tensor/_dim_extra.py` & `returnn-1.20230409.21835/returnn/tensor/_dim_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Backwards-compatible functions and attribs for the old ``Dim`` class,
 or just rarely used attribs, such that we can save memory for the common case.
 """
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Union, Tuple, Sequence, Dict, List
+from typing import TYPE_CHECKING, Optional, Union, Tuple, Dict, List
 
 from returnn.util.basic import Entity
 from returnn.util import basic as util
 
 if TYPE_CHECKING:
     # Those are only used for TensorFlow, or they are deprecated.
     from returnn.tf.util.data import BatchInfo, ControlFlowContext
@@ -686,49 +686,14 @@
                 batch_dim_axis=0,
                 batch=self.batch,
                 beam=beam,
                 control_flow_ctx=self.control_flow_ctx,
             )
         self.dyn_size_ext.placeholder = dyn_size
 
-    def get_mask(self: Dim, *, dim_order: Optional[Sequence[Dim]] = None) -> _t.Tensor:
-        """
-        :param dim_order: if given, the dims of the mask will be in this order.
-            This can be useful if the mask is broadcasted against some other tensor.
-        :return: if need_masking(), the corresponding mask.
-            If this is e.g. the time-dim T of shape [B], then the mask will be of shape [B,T].
-            The mask could be used with :func:`masked_select` (``boolean_mask``) or ``where``.
-        """
-        import returnn.frontend as rf
-
-        assert self.dyn_size_ext and self.dyn_size_ext.raw_tensor is not None
-        # noinspection PyProtectedMember
-        backend = self.dyn_size_ext._raw_backend
-
-        max_idx = rf.reduce(
-            self.dyn_size_ext,
-            axis=self.dyn_size_ext.dims,
-            mode="max",
-            # Masking here is not always possible, e.g. if we have
-            # tag = Dim{'self-att-keys'['time:var:extern_data:classes'[B]]}
-            use_time_mask=False,
-        )
-        # We use the assumption that self.placeholder.shape[axis] == max_idx.
-        # size_ext might have invalid (zero) sizes
-        # when it itself has some padding, e.g. when its own shape is dynamic.
-        # A zero size can lead to problems in some cases, e.g. in SoftmaxOverSpatialLayer,
-        # when everything is masked to -inf, it results in nan,
-        # and this likely produces nan in backprop or elsewhere.
-        # Thus, mask size_ext itself, and set the padded values to 1.
-        # This assumes that max_idx >= 1.
-        size_ext = self.dyn_size_ext.copy_masked(max_idx)
-        idx_range = backend.range_over_dim(self)
-        seq_mask = rf.compare(idx_range, "<", size_ext, allow_broadcast_all_sources=True, dim_order=dim_order)
-        return seq_mask
-
     def is_batch_dim(self):
         """
         :return: whether this dim tag is of kind batch
         :rtype: bool
         """
         return self.kind == DimTypes.Batch
```

### Comparing `returnn-1.20230409.215618/returnn/tensor/_tensor_extra.py` & `returnn-1.20230409.21835/returnn/tensor/_tensor_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -2657,14 +2657,16 @@
         :param int|None axis:
         :return: seq mask of shape ((batch,time) or (time,batch)) + (1,)s for remaining dims
           if BT or TB major, and axis is T or None.
           In general compatible to placeholder, i.e. same ndim, with broadcast dims.
           We assert here that the axis is dynamic (:func:`is_axis_dynamic`), i.e. we have the size.
         :rtype: tf.Tensor
         """
+        import returnn.frontend as rf
+
         if axis is None:
             assert self.time_dim_axis is not None
             axis = self.time_dim_axis
         if axis < 0:
             assert axis + self.batch_ndim > 0
             axis += self.batch_ndim
         assert 0 <= axis < self.batch_ndim
@@ -2686,34 +2688,39 @@
                 seq_mask = backend.sequence_mask_raw(size, batch_major=axis >= self.batch_dim_axis)  # (B,T) or (T,B)
                 shape = [1] * self.batch_ndim  # type: List[Union[int,_t.RawTensorType]]
                 shape[self.batch_dim_axis] = self.get_batch_dim()
                 shape[axis] = tag.get_dim_value()
                 seq_mask = backend.reshape_raw(seq_mask, shape)
                 assert seq_mask.get_shape().ndims == self.batch_ndim
             else:  # size is something unusual, not just [B], but e.g. [B,S] or so
+                max_idx = rf.reduce(
+                    tag.dyn_size_ext,
+                    axis=tag.dyn_size_ext.dims,
+                    mode="max",
+                    # Masking here is not always possible, e.g. if we have
+                    # tag = Dim{'self-att-keys'['time:var:extern_data:classes'[B]]}
+                    use_time_mask=False,
+                ).raw_tensor
+                # We use the assumption that self.placeholder.shape[axis] == max_idx.
+                # size_ext might have invalid (zero) sizes
+                # when it itself has some padding, e.g. when its own shape is dynamic.
+                # A zero size can lead to problems in some cases, e.g. in SoftmaxOverSpatialLayer,
+                # when everything is masked to -inf, it results in nan,
+                # and this likely produces nan in backprop or elsewhere.
+                # Thus, mask size_ext itself, and set the padded values to 1.
+                # This assumes that max_idx >= 1.
+                size_ext = tag.dyn_size_ext.copy_masked(max_idx)
+                idx_range = backend.range_over_dim(tag)
                 seq_mask = (
-                    self.get_sequence_mask_tensor(axis)
+                    rf.compare(idx_range, "<", size_ext, allow_broadcast_all_sources=True, dim_order=self.dims)
                     .copy_compatible_to(self, check_dtype=False, check_sparse=False)
                     .raw_tensor
                 )
         return seq_mask
 
-    def get_sequence_mask_tensor(self: Tensor, axis: int) -> Tensor:
-        """
-        :param axis:
-        :return: mask
-        """
-        if axis < 0:
-            assert axis + self.batch_ndim > 0
-            axis += self.batch_ndim
-        assert 0 <= axis < self.batch_ndim
-        assert axis != self.batch_dim_axis
-        tag: Dim = self.dim_tags[axis]
-        return tag.get_mask(dim_order=self.dims)
-
     def get_sequence_lengths_broadcast(self, axis=None):
         """
         :param int|None axis:
         :return: seq len of some shape which is broadcastable to self.placeholder.
           Note that this is not always possible, e.g. when the seq len has shape [B]
           but the tensor has just shape [T]. We currently throw an error then.
         :rtype: tf.Tensor
@@ -2760,15 +2767,15 @@
                 dims.remove(dim_)
             n_ = rf.reduce_sum(dim.dyn_size_ext, axis=dim.dyn_size_ext.dims)
             n *= n_
         return n
 
     def copy_masked(self: Tensor, mask_value) -> Tensor:
         """
-        :param float|int|tf.Tensor|Tensor mask_value:
+        :param float|int|tf.Tensor mask_value:
         """
         assert self.placeholder is not None
         if not any(dim.need_masking() for dim in self.dims):
             return self.copy()
         assert self._raw_backend.is_tensorflow  # not implemented otherwise for now
         from returnn.tf.util.basic import mask_dyn_seq_len_nd
```

### Comparing `returnn-1.20230409.215618/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230409.21835/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230409.21835/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230409.21835/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tensor/dim.py` & `returnn-1.20230409.21835/returnn/tensor/dim.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,14 @@
             self.capacity = capacity or dimension
             self.size = dimension
             self.dyn_size_ext = None
         elif isinstance(dimension, _t.Tensor):
             self.capacity = capacity
             self.size = None
             self.dyn_size_ext = dimension.copy()
-        else:
-            raise TypeError(f"unexpected dimension type: {type(dimension)}")
         if not name and not description and self.dyn_size_ext:
             name = self.dyn_size_ext.name
         self.name = name or description
         self._extra = None
 
         if kwargs:
             self._handle_extra_kwargs(**kwargs)
```

### Comparing `returnn-1.20230409.215618/returnn/tensor/marked_dim.py` & `returnn-1.20230409.21835/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tensor/tensor.py` & `returnn-1.20230409.21835/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tensor/tensor_dict.py` & `returnn-1.20230409.21835/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/compat.py` & `returnn-1.20230409.21835/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/data_pipeline.py` & `returnn-1.20230409.21835/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/distributed.py` & `returnn-1.20230409.21835/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/engine.py` & `returnn-1.20230409.21835/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230409.21835/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/horovod.py` & `returnn-1.20230409.21835/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230409.21835/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/layers/base.py` & `returnn-1.20230409.21835/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/layers/basic.py` & `returnn-1.20230409.21835/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/layers/rec.py` & `returnn-1.20230409.21835/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/layers/segmental_model.py` & `returnn-1.20230409.21835/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/layers/signal_processing.py` & `returnn-1.20230409.21835/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/native_op.py` & `returnn-1.20230409.21835/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/network.py` & `returnn-1.20230409.21835/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/sprint.py` & `returnn-1.20230409.21835/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/updater.py` & `returnn-1.20230409.21835/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/util/basic.py` & `returnn-1.20230409.21835/returnn/tf/util/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import threading
 import numpy
 import tensorflow as tf
 from tensorflow.python.client import device_lib
 from tensorflow.python.ops import init_ops
 from returnn.util import basic as util
 from returnn.util.basic import NotSpecified, NativeCodeCompiler
-from returnn.tensor import Tensor
 import returnn.tf.compat as tf_compat
 
 # noinspection PyUnresolvedReferences
 from .data import Data, SearchBeam, Dim, DimensionTag
 
 try:
     from tensorflow.python.ops.control_flow_v2_func_graphs import ControlFlowFuncGraph
@@ -257,23 +256,20 @@
         if v != pad_value:
             del d[k]
     d[dim] = pad_value
 
 
 def mask_dyn_seq_len_nd(x, pad_value, axes):
     """
-    :param Tensor x:
-    :param float|int|tf.Tensor|Tensor pad_value:
+    :param Data x:
+    :param float|int|tf.Tensor pad_value:
     :param list[int]|tuple[int] axes:
     :return: masked x
     :rtype: tf.Tensor
     """
-    if isinstance(pad_value, Tensor):
-        assert pad_value.dims == ()
-        pad_value = pad_value.placeholder
     # Filter out some axes which should not be used for masking.
     axes_ = []
     for axis in axes:
         tag = x.dim_tags[axis]
         assert tag.dyn_size_ext
         # It only makes sense to apply for this axis if the dyn size dims are all existing in x itself.
         # E.g. if the dyn_size_ext shape is [B] but the shape of x is just [T] (without B),
```

### Comparing `returnn-1.20230409.215618/returnn/tf/util/data.py` & `returnn-1.20230409.21835/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/util/ken_lm.py` & `returnn-1.20230409.21835/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/tf/util/open_fst.py` & `returnn-1.20230409.21835/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/torch/data/pipeline.py` & `returnn-1.20230409.21835/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230409.21835/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/torch/data/tensor_utils.py` & `returnn-1.20230409.21835/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/torch/engine.py` & `returnn-1.20230409.21835/returnn/torch/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,14 @@
         if isinstance(model, rf.Module):
             self._pt_model = rf_module_to_pt_module(model)
         elif isinstance(model, torch.nn.Module):
             self._pt_model = model
         else:
             raise TypeError(f"get_model returned {model} of type {type(model)}, expected rf.Module or torch.nn.Module")
         assert isinstance(self._pt_model, torch.nn.Module)
-        print("Model:", self._pt_model, file=log.v4)
 
         if checkpoint_state is not None:
             self._pt_model.load_state_dict(checkpoint_state["model"])
         preload_from_files = self.config.typed_value("preload_from_files", {})
         if preload_from_files:
             # see `preload_from_files` in tf engine and `returnn.tf.network.CustomCheckpointLoader`
             is_training = self.config.value("task", "train") == "train"
```

### Comparing `returnn-1.20230409.215618/returnn/torch/frontend/_backend.py` & `returnn-1.20230409.21835/returnn/torch/frontend/_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,23 +104,14 @@
     def get_known_shape_raw(raw_tensor: torch.Tensor) -> Tuple[Optional[int]]:
         """
         :return: shape of raw tensor; here for PyTorch the full shape is always known
         """
         return tuple(raw_tensor.size())
 
     @staticmethod
-    def get_new_dim_raw(raw_tensor: torch.Tensor, axis: int) -> Dim:
-        """
-        :param raw_tensor:
-        :param axis:
-        :return: new Dim object
-        """
-        return Dim(raw_tensor.size(axis))
-
-    @staticmethod
     def expand_dims_raw(raw_tensor: torch.Tensor, axis: int) -> torch.Tensor:
         """
         :param raw_tensor:
         :param axis: e.g. 1
         :return: raw tensor with new axis
         """
         return raw_tensor.unsqueeze(axis)
@@ -616,44 +607,7 @@
                     "maxval": maxval,
                     "seed": seed,
                     "static": static,
                     "out": out_,
                 }
             )
         return out
-
-    @staticmethod
-    def masked_select(
-        tensor: Tensor, *, mask: Tensor, dims: Sequence[Dim], out_dim: Optional[Dim] = None
-    ) -> Tuple[Tensor, Dim]:
-        """
-        :param tensor:
-        :param mask:
-        :param dims: the order of the dims defines the format. those dims should be exactly the dims of the mask.
-        :param out_dim:
-        :return: tensor where all dims in mask/dims are removed and replaced by a new dim.
-            the new dim is also returned.
-            if mask==True for all elements, the returned tensor would be simply the flattened input tensor.
-        """
-        assert mask.dtype == "bool"
-        assert set(mask.dims) == set(dims)
-        assert set(mask.dims).issubset(set(tensor.dims))
-        remaining_dims = [d for d in tensor.dims if d not in mask.dims]
-        tensor_templ = tensor.copy_template_new_dim_tags(tuple(dims) + tuple(remaining_dims))
-        tensor = tensor.copy_compatible_to(tensor_templ, add_dims=False)
-        mask = mask.copy_compatible_to(tensor_templ, check_dtype=False, check_sparse=False)
-        out_raw = torch.masked_select(tensor.raw_tensor, mask.raw_tensor)
-        remaining_shape = [d.get_dim_value() for d in remaining_dims]
-        remaining_num_elements = numpy.prod(remaining_shape) if remaining_shape else 1
-        assert out_raw.numel() % remaining_num_elements == 0
-        flattened_num_elements = out_raw.numel() // remaining_num_elements
-        out_raw = out_raw.resize(flattened_num_elements, *remaining_shape)
-        if not out_dim:
-            out_dim = TorchBackend.get_new_dim_raw(out_raw, 0)
-        out = Tensor(
-            "masked_select",
-            dims=(out_dim,) + tuple(remaining_dims),
-            dtype=tensor.dtype,
-            sparse_dim=tensor.sparse_dim,
-            raw_tensor=out_raw,
-        )
-        return out, out_dim
```

### Comparing `returnn-1.20230409.215618/returnn/torch/frontend/_rand.py` & `returnn-1.20230409.21835/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/torch/frontend/bridge.py` & `returnn-1.20230409.21835/returnn/torch/frontend/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,14 @@
             assert isinstance(pt_param, torch.nn.Parameter)
             self.register_parameter(name, pt_param)
 
         for name, rf_mod in rf_module.named_children():
             pt_mod = rf_module_to_pt_module(rf_mod)
             self.add_module(name, pt_mod)
 
-    def _get_name(self):
-        return self._rf_module.__class__.__name__ + "[RF→PT]"
-
     @property
     def rf_module(self) -> rf.Module:
         """RF module"""
         return self._rf_module
 
     def forward(self, *args, **kwargs):
         """forward"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `returnn-1.20230409.215618/returnn/torch/updater.py` & `returnn-1.20230409.21835/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/basic.py` & `returnn-1.20230409.21835/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/better_exchook.py` & `returnn-1.20230409.21835/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/bpe.py` & `returnn-1.20230409.21835/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/debug.py` & `returnn-1.20230409.21835/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/debug_helpers.py` & `returnn-1.20230409.21835/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/fsa.py` & `returnn-1.20230409.21835/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230409.21835/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/pprint.py` & `returnn-1.20230409.21835/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/py-to-pickle.cpp` & `returnn-1.20230409.21835/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/sig_proc.py` & `returnn-1.20230409.21835/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn/util/task_system.py` & `returnn-1.20230409.21835/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/returnn.egg-info/PKG-INFO` & `returnn-1.20230409.21835/returnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230409.215618
+Version: 1.20230409.21835
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230409.215618/returnn.egg-info/SOURCES.txt` & `returnn-1.20230409.21835/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/setup.py` & `returnn-1.20230409.21835/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/DummySprintExec.py` & `returnn-1.20230409.21835/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230409.21835/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230409.21835/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230409.21835/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/_set_num_threads1.py` & `returnn-1.20230409.21835/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/_setup_test_env.py` & `returnn-1.20230409.21835/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/bpe-unicode-demo.codes` & `returnn-1.20230409.21835/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/bpe-unicode-demo.vocab` & `returnn-1.20230409.21835/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/lexicon_opt.isyms` & `returnn-1.20230409.21835/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/lexicon_opt.jpg` & `returnn-1.20230409.21835/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/lint_common.py` & `returnn-1.20230409.21835/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/pycharm-inspect.py` & `returnn-1.20230409.21835/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/pylint.py` & `returnn-1.20230409.21835/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/returnn-as-framework.py` & `returnn-1.20230409.21835/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/rf_utils.py` & `returnn-1.20230409.21835/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/spelling.dic` & `returnn-1.20230409.21835/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_Config.py` & `returnn-1.20230409.21835/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_Dataset.py` & `returnn-1.20230409.21835/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_Fsa.py` & `returnn-1.20230409.21835/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_GeneratingDataset.py` & `returnn-1.20230409.21835/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_HDFDataset.py` & `returnn-1.20230409.21835/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_LearningRateControl.py` & `returnn-1.20230409.21835/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_Log.py` & `returnn-1.20230409.21835/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_MultiProcDataset.py` & `returnn-1.20230409.21835/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_PTDataset.py` & `returnn-1.20230409.21835/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_Pretrain.py` & `returnn-1.20230409.21835/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_ResNet.py` & `returnn-1.20230409.21835/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_SprintDataset.py` & `returnn-1.20230409.21835/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_SprintInterface.py` & `returnn-1.20230409.21835/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TFEngine.py` & `returnn-1.20230409.21835/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TFNativeOp.py` & `returnn-1.20230409.21835/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TFNetworkLayer.py` & `returnn-1.20230409.21835/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230409.21835/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230409.21835/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TFUpdater.py` & `returnn-1.20230409.21835/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TFUtil.py` & `returnn-1.20230409.21835/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TF_determinism.py` & `returnn-1.20230409.21835/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TaskSystem.py` & `returnn-1.20230409.21835/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230409.21835/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_TranslationDataset.py` & `returnn-1.20230409.21835/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_Util.py` & `returnn-1.20230409.21835/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_demos.py` & `returnn-1.20230409.21835/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_fork_exec.py` & `returnn-1.20230409.21835/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_hdf_dump.py` & `returnn-1.20230409.21835/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_rf_base.py` & `returnn-1.20230409.21835/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_tensor.py` & `returnn-1.20230409.21835/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_tools.py` & `returnn-1.20230409.21835/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_torch_frontend.py` & `returnn-1.20230409.21835/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tests/test_torch_internal_frontend.py` & `returnn-1.20230409.21835/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/analyze-dataset-batches.py` & `returnn-1.20230409.21835/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/bliss-collect-seq-lens.py` & `returnn-1.20230409.21835/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/bliss-dump-text.py` & `returnn-1.20230409.21835/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/bliss-get-segment-names.py` & `returnn-1.20230409.21835/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/bliss-to-ogg-zip.py` & `returnn-1.20230409.21835/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/bpe-create-lexicon.py` & `returnn-1.20230409.21835/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/calculate-word-error-rate.py` & `returnn-1.20230409.21835/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/cleanup-old-models.py` & `returnn-1.20230409.21835/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/collect-orth-symbols.py` & `returnn-1.20230409.21835/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/collect-words.py` & `returnn-1.20230409.21835/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/compile_native_op.py` & `returnn-1.20230409.21835/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/compile_tf_graph.py` & `returnn-1.20230409.21835/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/debug-dump-search-scores.py` & `returnn-1.20230409.21835/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/debug-plot-search-scores.py` & `returnn-1.20230409.21835/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/dump-dataset-raw-strings.py` & `returnn-1.20230409.21835/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/dump-dataset.py` & `returnn-1.20230409.21835/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/dump-forward-stats.py` & `returnn-1.20230409.21835/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/dump-forward.py` & `returnn-1.20230409.21835/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/dump-network-json.py` & `returnn-1.20230409.21835/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/dump-pickle.py` & `returnn-1.20230409.21835/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230409.21835/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/get-attention-weights.py` & `returnn-1.20230409.21835/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/get-best-model-epoch.py` & `returnn-1.20230409.21835/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/hdf_dump.py` & `returnn-1.20230409.21835/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230409.21835/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/import-blocks-mt-model.py` & `returnn-1.20230409.21835/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/import-t2t-mt-model.py` & `returnn-1.20230409.21835/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/Makefile` & `returnn-1.20230409.21835/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/README.md` & `returnn-1.20230409.21835/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/example/README.md` & `returnn-1.20230409.21835/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230409.21835/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/file.h` & `returnn-1.20230409.21835/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230409.21835/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230409.21835/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/main.cc` & `returnn-1.20230409.21835/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230409.21835/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230409.21835/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230409.21835/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/tf_avg_checkpoints.py` & `returnn-1.20230409.21835/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/tf_inspect_checkpoint.py` & `returnn-1.20230409.21835/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.215618/tools/tf_inspect_summary_log.py` & `returnn-1.20230409.21835/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

