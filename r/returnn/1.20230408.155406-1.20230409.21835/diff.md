# Comparing `tmp/returnn-1.20230408.155406.tar.gz` & `tmp/returnn-1.20230409.21835.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230408.155406.tar", last modified: Sat Apr  8 14:26:43 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230409.21835.tar", last modified: Sun Apr  9 00:34:28 2023, max compression
```

## Comparing `returnn-1.20230408.155406.tar` & `returnn-1.20230409.21835.tar`

### file list

```diff
@@ -1,410 +1,410 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63018 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-08 14:26:27.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-08 14:26:29.000000 returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36530 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92010 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   154243 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36628 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   150268 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69478 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19601 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   148678 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   582337 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   292822 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22395 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144495 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/py-to-pickle.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187447 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:26:43.000000 returnn-1.20230408.155406/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-08 14:26:26.000000 returnn-1.20230408.155406/tools/tf_inspect_summary_log.py
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

### Comparing `returnn-1.20230408.155406/.gitignore` & `returnn-1.20230409.21835/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/.gitmodules` & `returnn-1.20230409.21835/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/CHANGELOG.md` & `returnn-1.20230409.21835/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/CODEOWNERS` & `returnn-1.20230409.21835/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/CONTRIBUTING.md` & `returnn-1.20230409.21835/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/LICENSE` & `returnn-1.20230409.21835/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/MANIFEST.in` & `returnn-1.20230409.21835/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/PKG-INFO` & `returnn-1.20230409.21835/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230408.155406
+Version: 1.20230409.21835
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230408.155406/README.rst` & `returnn-1.20230409.21835/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/__init__.py` & `returnn-1.20230409.21835/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/12AX.cluster_map` & `returnn-1.20230409.21835/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-fwd.config` & `returnn-1.20230409.21835/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-horovod-mpi.py` & `returnn-1.20230409.21835/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230409.21835/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-hyper-param-tuning.config` & `returnn-1.20230409.21835/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-iter-dataset.py` & `returnn-1.20230409.21835/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-list-devices.py` & `returnn-1.20230409.21835/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-lua-torch-layer.config` & `returnn-1.20230409.21835/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230409.21835/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-returnn-as-framework.py` & `returnn-1.20230409.21835/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-rf.config` & `returnn-1.20230409.21835/demos/demo-rf.config`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 def get_model(**_kwargs):
     return Model()
 
 def train_step(*, model: Model, extern_data, **_kwargs):
     data = extern_data["data"]
     logits = model(data)
     targets = extern_data["classes"]
+    # TODO: use flattening on logits/targets
     loss = rf.cross_entropy(estimated=logits, estimated_type="logits", target=targets, axis=out_dim)
     loss.mark_as_loss(name="ce")
 
 
 # training
 optimizer = {"class": "adam"}
```

### Comparing `returnn-1.20230408.155406/demos/demo-rhn-enwik8.config` & `returnn-1.20230409.21835/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-sprint-interface.py` & `returnn-1.20230409.21835/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-att-copy.config` & `returnn-1.20230409.21835/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-attention.config` & `returnn-1.20230409.21835/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-enc-dec.config` & `returnn-1.20230409.21835/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230409.21835/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230409.21835/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230409.21835/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230409.21835/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230409.21835/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-rec-self-att.config` & `returnn-1.20230409.21835/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230409.21835/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230409.21835/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo-torch.config` & `returnn-1.20230409.21835/demos/demo-torch.config`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     data = extern_data["data"]
     logits = model(data.raw_tensor)
     logits_packed = torch.nn.utils.rnn.pack_padded_sequence(
         logits, data.dims[1].dyn_size_ext.raw_tensor, batch_first=True, enforce_sorted=False)
     targets = extern_data["classes"]
     targets_packed = torch.nn.utils.rnn.pack_padded_sequence(
         targets.raw_tensor, data.dims[1].dyn_size_ext.raw_tensor, batch_first=True, enforce_sorted=False)
-    loss = nn.CrossEntropyLoss()(logits_packed.data, targets_packed.data.long())
+    loss = nn.CrossEntropyLoss(reduction='none')(logits_packed.data, targets_packed.data.long())
     rf.get_run_ctx().mark_as_loss(name="cross_entropy", loss=loss)
 
 
 # training
 optimizer = {"class": "adam"}
 
 learning_rate = 0.01
```

### Comparing `returnn-1.20230408.155406/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230409.21835/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/demo.sh` & `returnn-1.20230409.21835/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/README.txt` & `returnn-1.20230409.21835/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/config_demo` & `returnn-1.20230409.21835/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230409.21835/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/config_real` & `returnn-1.20230409.21835/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230409.21835/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/decode.py` & `returnn-1.20230409.21835/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230409.21835/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230409.21835/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230409.21835/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230409.21835/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230409.21835/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230409.21835/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230409.21835/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/__init__.py` & `returnn-1.20230409.21835/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/__main__.py` & `returnn-1.20230409.21835/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/__old_mod_loader__.py` & `returnn-1.20230409.21835/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/__setup__.py` & `returnn-1.20230409.21835/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/config.py` & `returnn-1.20230409.21835/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/audio.py` & `returnn-1.20230409.21835/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/basic.py` & `returnn-1.20230409.21835/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/bundle_file.py` & `returnn-1.20230409.21835/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/cached.py` & `returnn-1.20230409.21835/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/cached2.py` & `returnn-1.20230409.21835/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/generating.py` & `returnn-1.20230409.21835/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/hdf.py` & `returnn-1.20230409.21835/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/lm.py` & `returnn-1.20230409.21835/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/map.py` & `returnn-1.20230409.21835/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/meta.py` & `returnn-1.20230409.21835/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/multi_proc.py` & `returnn-1.20230409.21835/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/normalization_data.py` & `returnn-1.20230409.21835/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/numpy_dump.py` & `returnn-1.20230409.21835/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/raw_wav.py` & `returnn-1.20230409.21835/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/sprint.py` & `returnn-1.20230409.21835/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/stereo.py` & `returnn-1.20230409.21835/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230409.21835/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/datasets/util/vocabulary.py` & `returnn-1.20230409.21835/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/engine/base.py` & `returnn-1.20230409.21835/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/engine/batch.py` & `returnn-1.20230409.21835/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/graph_editor/edit.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/graph_editor/select.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/graph_editor/transform.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/extern/graph_editor/util.py` & `returnn-1.20230409.21835/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/__init__.py` & `returnn-1.20230409.21835/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/_backend.py` & `returnn-1.20230409.21835/returnn/frontend/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,37 @@
         :param dim: the new dim for shape[axis]
         :return: shape[axis] expands to dim.
             in PyTorch or other frameworks which support custom strides,
             this is an efficient view and not a copy.
         """
         raise NotImplementedError
 
+    @staticmethod
+    def cast_raw(raw_tensor: T, dtype: str) -> T:
+        """
+        :param raw_tensor:
+        :param dtype: e.g. "float32"
+        :return: raw tensor with dtype casted
+        """
+        raise NotImplementedError
+
+    @staticmethod
+    def cast(tensor: Tensor, dtype: str) -> Tensor:
+        """
+        :param tensor:
+        :param dtype: e.g. "float32"
+        :return: tensor with dtype casted
+        """
+        # Default implementation using cast_raw.
+        res = tensor.copy_template()
+        res.dtype = dtype
+        # noinspection PyProtectedMember
+        res.raw_tensor = tensor._raw_backend.cast_raw(tensor.raw_tensor, dtype)
+        return res
+
     # Restrict the possible activation function names,
     # to not get unexpected behavior,
     # or unwanted incompatibilities.
     _AllowedActivationFuncs = {
         "exp",
         "expm1",
         "log",
@@ -284,14 +307,21 @@
         :param targets: probabilities, i.e. normalized, can also be sparse
         :param axis: class labels dim over which softmax is computed
         :return: cross entropy (same Dims as 'logits' but without 'axis')
         """
         raise NotImplementedError
 
     @staticmethod
+    def have_sequence_mask_raw() -> bool:
+        """
+        :return: whether we have a sequence_mask_raw implementation
+        """
+        return False
+
+    @staticmethod
     def sequence_mask_raw(lengths: T, *, batch_major: bool = True) -> T:
         """
         Like tf.sequence_mask().
 
         :param lengths: shape (batch,)
         :param batch_major:
         :return: tensor mask of shape (batch,maxlen) if batch_major else (maxlen,batch) of type bool
@@ -305,15 +335,15 @@
         Default implementation for eager-based frameworks:
         Do nothing, tensors do not have a name.
 
         :param name:
         :return: context manager
         """
         # Default implementation for eager-based frameworks
-        pass  # nothing to do
+        yield  # nothing to do
 
     @staticmethod
     @contextlib.contextmanager
     def control_dependencies_raw(dependencies: Sequence[Any]) -> Any:
         """
         Default implementation for eager-based frameworks:
         Do nothing, we expect that the dependencies are already executed.
```

### Comparing `returnn-1.20230408.155406/returnn/frontend/_numpy_backend.py` & `returnn-1.20230409.21835/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/_utils.py` & `returnn-1.20230409.21835/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/array_.py` & `returnn-1.20230409.21835/returnn/frontend/array_.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from returnn.tensor import Tensor, Dim
 import returnn.frontend as rf
 from ._backend import Backend, global_backend, get_backend_by_raw_tensor_type
 from .types import RawTensorTypes
 
 T = TypeVar("T")
 
-__all__ = ["convert_to_tensor", "constant", "gather"]
+__all__ = ["convert_to_tensor", "constant", "cast", "gather"]
 
 
 def convert_to_tensor(
     value: Union[Tensor, T, RawTensorTypes],
     *,
     dims: Sequence[Dim] = None,
     dtype: Optional[str] = None,
@@ -73,14 +73,24 @@
             dtype = value_backend.get_dtype_name_raw(value)
     return _backend.convert_to_tensor(value=value, dims=dims, dtype=dtype, sparse_dim=sparse_dim)
 
 
 constant = convert_to_tensor  # alias for some older code
 
 
+def cast(tensor: Tensor, dtype: str) -> Tensor:
+    """
+    :param tensor:
+    :param dtype:
+    :return: tensor with the same data, but with a different dtype
+    """
+    # noinspection PyProtectedMember
+    return tensor._raw_backend.cast(tensor, dtype=dtype)
+
+
 # noinspection PyUnusedLocal
 def gather(
     source: Tensor,
     *,
     indices: Union[Tensor, int],
     axis: Dim,
     clip_to_valid: bool = False,
```

### Comparing `returnn-1.20230408.155406/returnn/frontend/const.py` & `returnn-1.20230409.21835/returnn/frontend/const.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import returnn.frontend as rf
 
 
 __all__ = ["full", "constant", "fill", "zeros", "ones"]
 
 
 def full(
-    dims: Sequence[Dim], fill_value: RawTensorTypes, *, dtype: Optional[str] = None, sparse_dim: Optional[Dim] = None
+    *, dims: Sequence[Dim], fill_value: RawTensorTypes, dtype: Optional[str] = None, sparse_dim: Optional[Dim] = None
 ) -> Tensor:
     """
     full
 
     https://data-apis.org/array-api/latest/API_specification/generated/array_api.full.html
 
     :param dims: shape
@@ -42,15 +42,15 @@
 fill = full  # alias for TF users
 
 
 def zeros(dims: Sequence[Dim], *, dtype: Optional[str] = None, sparse_dim: Optional[Dim] = None) -> Tensor:
     """
     zeros. float by default.
     """
-    return full(dims, 0, dtype=dtype or rf.get_default_float_dtype(), sparse_dim=sparse_dim)
+    return full(dims=dims, fill_value=0, dtype=dtype or rf.get_default_float_dtype(), sparse_dim=sparse_dim)
 
 
 def ones(dims: Sequence[Dim], *, dtype: Optional[str] = None, sparse_dim: Optional[Dim] = None) -> Tensor:
     """
     ones. float by default.
     """
-    return full(dims, 1, dtype=dtype or rf.get_default_float_dtype(), sparse_dim=sparse_dim)
+    return full(dims=dims, fill_value=1, dtype=dtype or rf.get_default_float_dtype(), sparse_dim=sparse_dim)
```

### Comparing `returnn-1.20230408.155406/returnn/frontend/dims.py` & `returnn-1.20230409.21835/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/dtype.py` & `returnn-1.20230409.21835/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/init.py` & `returnn-1.20230409.21835/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/linear.py` & `returnn-1.20230409.21835/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/loss.py` & `returnn-1.20230409.21835/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/math_.py` & `returnn-1.20230409.21835/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/matmul.py` & `returnn-1.20230409.21835/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/module.py` & `returnn-1.20230409.21835/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/parameter.py` & `returnn-1.20230409.21835/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/rand.py` & `returnn-1.20230409.21835/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/reduce.py` & `returnn-1.20230409.21835/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/run_ctx.py` & `returnn-1.20230409.21835/returnn/frontend/run_ctx.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,32 +115,26 @@
           This can also avoid issues with inf/nan in some cases.
           If False, it will mask the loss to 0 in the padded frames and accumulate over that.
           Typically, setting this to True (default) is both more efficient and better.
         :param bool use_normalized_loss: the loss used in optimization will be normalized.
           E.g. if the overall normalization is sum(loss)/sum(num_frames), this is also what the optimizer will use,
           otherwise the optimizer will just use sum(loss).
         :param custom_inv_norm_factor:
-          The standard norm factor is 1/sum(target_seq_len) if the target has a time-axis,
-          or 1/sum(output_seq_len) if there is no target and the output has a time-axis,
+          The standard inv norm factor is sum(target_seq_len) if the target has a time-axis,
+          or sum(output_seq_len) if there is no target and the output has a time-axis,
           or 1 otherwise. (See :func:`Loss.init` for details.)
           This is used for proper normalization of accumulated loss/error per epoch
           and also proper normalization per batch for reporting,
           no matter if use_normalized_loss is True or False.
           If you want to change this norm factor, you can set this.
-          Basically, for all reporting, it uses sum(loss) * sum(custom_inv_norm_factor).
+          Basically, for all reporting, it uses sum(loss) / sum(custom_inv_norm_factor).
         """
         assert self.stage == "train_step"
         if not isinstance(loss, Tensor):
             assert isinstance(loss, _backend.global_backend.RawTensorType)
-            assert _backend.global_backend.get_ndim_raw(loss) == 0, (
-                f"mark_as_loss(<loss with shape {_backend.global_backend.get_known_shape_raw(loss)}>, {name!r}):"
-                " Only scalar raw losses are supported,"
-                " because we cannot know whether there are any dynamic dims which might require padding."
-                " Explicitly convert to a Tensor first and specify dim tags."
-            )
             loss = rf.convert_to_tensor(loss)
         assert name not in self.losses
         self.losses[name] = Loss(
             loss=loss,
             name=name,
             scale=scale,
             as_error=as_error,
@@ -216,39 +210,60 @@
     """
 
     loss: Tensor
     name: str
 
     scale: float = 1.0
     as_error: bool = False
-    use_normalized_loss: bool = False
+    use_normalized_loss: bool = False  # for the gradient / total loss
     use_flatten_frames: bool = True
     custom_inv_norm_factor: Optional[Tensor] = None
 
+    _summed_loss_cached: Optional[Tensor] = None
+    _mean_loss_cached: Optional[Tensor] = None
+
     def get_summed_loss(self) -> Tensor:
         """
         :return: sum of loss (scalar)
         """
         if not self.loss.dims:
             return self.loss
-        return rf.reduce_sum(self.loss, axis=self.loss.dims)
+        if self._summed_loss_cached is not None:
+            return self._summed_loss_cached
+        if self._mean_loss_cached is not None:
+            return self._mean_loss_cached / self.get_inv_norm_factor()
+        self._summed_loss_cached = rf.reduce_sum(self.loss, axis=self.loss.dims)
+        return self._summed_loss_cached
 
     def get_mean_loss(self) -> Tensor:
         """
         :return: sum of loss (scalar)
         """
+        if self._mean_loss_cached is not None:
+            return self._mean_loss_cached
         if self.custom_inv_norm_factor:
-            return self.get_summed_loss() * self.custom_inv_norm_factor
+            loss = self.get_summed_loss()
+            loss /= rf.cast(self.custom_inv_norm_factor, dtype=loss.dtype)
+            return loss
         if not self.loss.dims:
             return self.loss
-        return rf.reduce_mean(self.loss, axis=self.loss.dims)
+        self._mean_loss_cached = rf.reduce_mean(self.loss, axis=self.loss.dims)
+        return self._mean_loss_cached
+
+    def get_inv_norm_factor(self) -> Union[int, Tensor]:
+        """
+        :return: inverse norm factor (scalar)
+        """
+        if self.custom_inv_norm_factor:
+            return self.custom_inv_norm_factor
+        return self.loss.num_elements()
 
     def get_scaled_reduced_loss(self) -> Tensor:
         """
-        :return: scaled reduced loss (scalar), as it is supposed to be used for calculating the
+        :return: scaled reduced loss (scalar), as it is supposed to be used for calculating the train gradient
         """
         if self.use_normalized_loss:
             loss = self.get_mean_loss()
         else:
             loss = self.get_summed_loss()
         return loss * self.scale
```

### Comparing `returnn-1.20230408.155406/returnn/frontend/state.py` & `returnn-1.20230409.21835/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/frontend/types.py` & `returnn-1.20230409.21835/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/import_/common.py` & `returnn-1.20230409.21835/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/import_/git.py` & `returnn-1.20230409.21835/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/import_/import_.py` & `returnn-1.20230409.21835/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/learning_rate_control.py` & `returnn-1.20230409.21835/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/log.py` & `returnn-1.20230409.21835/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/native_op.cpp` & `returnn-1.20230409.21835/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/native_op.py` & `returnn-1.20230409.21835/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/pretrain.py` & `returnn-1.20230409.21835/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/sprint/cache.py` & `returnn-1.20230409.21835/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/sprint/control.py` & `returnn-1.20230409.21835/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/sprint/error_signals.py` & `returnn-1.20230409.21835/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/sprint/extern_interface.py` & `returnn-1.20230409.21835/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/sprint/interface.py` & `returnn-1.20230409.21835/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tensor/_dim_extra.py` & `returnn-1.20230409.21835/returnn/tensor/_dim_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -743,15 +743,19 @@
         return not self.is_dynamic()
 
     def need_masking(self):
         """
         :return: whether dim is static or dynamic but with scalar dyn_size_ext
         """
         if self.is_static():
+            if self.capacity is not None:
+                return self.size < self.capacity
             return False
+        if self.capacity is not None:
+            return True
         if not self.dyn_size_ext:
             return True  # unknown
         return self.dyn_size_ext.batch_ndim > 0
 
     def can_be_used_as_dim(self):
         """
         :return: whether this can be used as a dim in :class:`Data`, i.e. it is not special
@@ -1514,45 +1518,68 @@
         """
         Infers the dim this axis should have if unbroadcasted.
         If `self.src_data` has a placeholder, will use the shape from there.
         Otherwise, uses `self.dimension` (if static) or `self.dyn_size` (if dynamic).
 
         :return: max(size or dyn_size)
         """
+        res = self.get_dim_value_tensor()
+        if isinstance(res, _t.Tensor):
+            assert res.dims == ()
+            return res.raw_tensor
+        assert isinstance(res, int)
+        return res
+
+    def get_dim_value_tensor(self) -> Union[int, _t.Tensor]:
+        """
+        Infers the dim this axis should have if unbroadcasted.
+        If `self.src_data` has a placeholder, will use the shape from there.
+        Otherwise, uses `self.dimension` (if static) or `self.dyn_size` (if dynamic).
+
+        :return: max(size or dyn_size)
+        """
         import returnn.frontend as rf
 
         if self.dimension is not None:
             return self.dimension
         if self.dyn_size_ext and self.dyn_size_ext.placeholder is not None:  # fast path
             if self.dyn_size_ext.batch_ndim > 0:
                 return rf.reduce_max(
                     self.dyn_size_ext,
                     axis=self.dyn_size_ext.dim_tags,
                     # Masking is not always possible here, e.g.
                     # self = Dim{'self-att-keys'['time:var:extern_data:classes'[B]]}.
                     use_time_mask=False,
-                ).raw_tensor
-            return self.dyn_size_ext.placeholder
+                )
+            return self.dyn_size_ext
         if self.is_batch_dim():
+            res = None
             if self._extra and self._extra.src_data:
-                return self._extra.src_data.get_batch_dim()
-            if self.batch:
-                return self.batch.dim
+                res = self._extra.src_data.get_batch_dim()
+            elif self.batch:
+                res = self.batch.dim
+            if isinstance(res, int):
+                return res
+            if res is not None:
+                return _t.Tensor("batch", dims=(), dtype=rf.get_default_array_index_dtype(), raw_tensor=res)
         if (
             self._extra
             and self._extra.src_data is not None
             and self._extra.src_axis is not None
             and self._extra.src_data.placeholder is not None
         ):
-            return self._extra.src_data.get_dim(self._extra.src_axis)
+            res = self._extra.src_data.get_dim(self._extra.src_axis)
+            if isinstance(res, int):
+                return res
+            return _t.Tensor("batch", dims=(), dtype=rf.get_default_array_index_dtype(), raw_tensor=res)
         self.complete_dyn_size()
         if self.dyn_size_ext and self.dyn_size_ext.placeholder is not None:
             if self.dyn_size_ext.batch_ndim > 0:
-                return rf.reduce_max(self.dyn_size_ext, axis=self.dyn_size_ext.dim_tags).raw_tensor
-            return self.dyn_size_ext.placeholder
+                return rf.reduce_max(self.dyn_size_ext, axis=self.dyn_size_ext.dim_tags)
+            return self.dyn_size_ext
         raise Exception("%s: need placeholder, self.dimension or self.dyn_size for dim value" % self)
 
     def axis_split_info(self):
         """
         :return: axis split info. see :func:`get_param_axes_split_info` and usage (e.g. pretraining)
         :rtype: list[int|None]
         """
```

### Comparing `returnn-1.20230408.155406/returnn/tensor/_tensor_extra.py` & `returnn-1.20230409.21835/returnn/tensor/_tensor_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -2672,15 +2672,19 @@
         assert 0 <= axis < self.batch_ndim
         assert axis != self.batch_dim_axis
         tag: Dim = self.dim_tags[axis]
         assert tag.dyn_size_ext and tag.dyn_size_ext.raw_tensor is not None
         backend = tag.dyn_size_ext._raw_backend
         assert set(tag.dyn_size_ext.dim_tags).issubset(self.dim_tags)  # https://github.com/rwth-i6/returnn/issues/721
         with backend.name_scope_raw("get_sequence_mask_broadcast"):
-            if tag.dyn_size_ext.have_batch_axis() and tag.dyn_size_ext.batch_ndim == 1:  # just [B]
+            if (
+                backend.have_sequence_mask_raw()
+                and tag.dyn_size_ext.have_batch_axis()
+                and tag.dyn_size_ext.batch_ndim == 1
+            ):  # just [B]
                 # This is the common case where the size is of shape [B].
                 # We make use of sequence_mask or sequence_mask_time_major in that case,
                 # which is optimized by caching.
                 size = tag.dyn_size
                 seq_mask = backend.sequence_mask_raw(size, batch_major=axis >= self.batch_dim_axis)  # (B,T) or (T,B)
                 shape = [1] * self.batch_ndim  # type: List[Union[int,_t.RawTensorType]]
                 shape[self.batch_dim_axis] = self.get_batch_dim()
@@ -2729,19 +2733,53 @@
             axis += self.batch_ndim
         assert 0 <= axis < self.batch_ndim
         assert axis != self.batch_dim_axis
         tag = self.dim_tags[axis]
         assert tag.dyn_size_ext
         return tag.dyn_size_ext.copy_compatible_to(self, check_dtype=False, check_sparse=False).placeholder
 
+    def num_elements(self: Tensor) -> Union[int, Tensor]:
+        """
+        :return: number of elements in this tensor, i.e. prod(self.shape)
+        :rtype: tf.Tensor
+        """
+        if all(dim.is_static() for dim in self.dims):
+            n = 1
+            for dim in self.dims:
+                n *= dim.dimension
+            return n
+
+        import returnn.frontend as rf
+
+        n = 1
+        dims = list(self.dims)
+        dims.sort(key=lambda dim: -dim.dyn_size_ext.batch_ndim if dim.dyn_size_ext else 0)
+        while dims:
+            dim = dims.pop(0)
+            if dim.is_static():
+                n *= dim.dimension
+                continue
+            # E.g. dyn_size_ext is shape [B], and self has shape [B,T].
+            # Due to the sorting of dims above, dims will be [T,B], and we will first process T.
+            # We want to sum over dyn_size_ext, but then we need to remove the other dims it covers.
+            for dim_ in dim.dyn_size_ext.dims:
+                assert dim_ in dims  # num elements not really well-defined then
+                assert not dim_.need_masking()  # not implemented
+                dims.remove(dim_)
+            n_ = rf.reduce_sum(dim.dyn_size_ext, axis=dim.dyn_size_ext.dims)
+            n *= n_
+        return n
+
     def copy_masked(self: Tensor, mask_value) -> Tensor:
         """
         :param float|int|tf.Tensor mask_value:
         """
         assert self.placeholder is not None
+        if not any(dim.need_masking() for dim in self.dims):
+            return self.copy()
         assert self._raw_backend.is_tensorflow  # not implemented otherwise for now
         from returnn.tf.util.basic import mask_dyn_seq_len_nd
 
         dyn_axes = [axis for axis, dim in enumerate(self.dim_tags) if not dim.is_batch_dim() and dim.dimension is None]
         res = self.copy()
         res.placeholder = mask_dyn_seq_len_nd(self, pad_value=mask_value, axes=dyn_axes)
         return res
```

### Comparing `returnn-1.20230408.155406/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230409.21835/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230409.21835/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230409.21835/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tensor/dim.py` & `returnn-1.20230409.21835/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tensor/marked_dim.py` & `returnn-1.20230409.21835/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tensor/tensor.py` & `returnn-1.20230409.21835/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tensor/tensor_dict.py` & `returnn-1.20230409.21835/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/compat.py` & `returnn-1.20230409.21835/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/data_pipeline.py` & `returnn-1.20230409.21835/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/distributed.py` & `returnn-1.20230409.21835/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/engine.py` & `returnn-1.20230409.21835/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,19 @@
 
     @staticmethod
     def transpose_raw(raw_tensor: Layer, perm: Sequence[int]) -> Layer:
         """transpose_raw is a no-op in this backend"""
         return raw_tensor
 
     @staticmethod
+    def cast(tensor: Tensor, dtype: str) -> Tensor:
+        """cast"""
+        return rfl.make_layer({"class": "cast", "from": tensor, "dtype": dtype}, name="cast")
+
+    @staticmethod
     def activation(tensor: Tensor, func: str) -> Tensor:
         """activation"""
         return rfl.make_layer({"class": "activation", "activation": func, "from": tensor}, name=func)
 
     @staticmethod
     def activation_raw(raw_tensor: Layer, func: str) -> Layer:
         """activation"""
@@ -169,19 +174,14 @@
             )
         else:  # dense targets
             assert axis in targets.dims and axis in logits.dims
             log_probs = rf.log_softmax(logits, axis=axis)
             return -rf.matmul(targets, log_probs, reduce=axis)
 
     @staticmethod
-    def sequence_mask_raw(lengths: Layer, *, batch_major: bool = True) -> Layer:
-        """sequence mask"""
-        raise NotImplementedError  # TODO
-
-    @staticmethod
     def create_parameter_raw(tensor: rf.Parameter) -> Layer:
         """create parameter"""
         return rfl.make_layer(
             {"class": "variable", "shape": tensor.dims, "dtype": tensor.dtype}, name=tensor.name, existing_tensor=tensor
         ).raw_tensor
 
     @staticmethod
```

### Comparing `returnn-1.20230408.155406/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230409.21835/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230409.21835/returnn/tf/frontend_low_level/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,19 @@
         :return: shape[axis] expands to dim
         """
         assert raw_tensor.shape.as_list()[axis] == 1
         with tf_util.same_control_flow_ctx(raw_tensor):
             return tf.tile(raw_tensor, [1] * axis + [dim] + [1] * (raw_tensor.shape.ndims - axis - 1))
 
     @staticmethod
+    def cast_raw(raw_tensor: tf.Tensor, dtype: str) -> tf.Tensor:
+        """cast"""
+        return tf.cast(raw_tensor, dtype)
+
+    @staticmethod
     def activation_raw(raw_tensor: tf.Tensor, func: str) -> tf.Tensor:
         """
         :param raw_tensor:
         :param func: e.g. "tanh"
         :return: raw tensor after activation
         """
         assert func in Backend._AllowedActivationFuncs
@@ -209,14 +214,21 @@
         elif hasattr(tf, func):
             f = getattr(tf, func)
         else:
             raise ValueError(f"unknown activation function {func!r}")
         return f(raw_tensor)
 
     @staticmethod
+    def have_sequence_mask_raw() -> bool:
+        """
+        :return: whether we have sequence_mask
+        """
+        return True
+
+    @staticmethod
     def sequence_mask_raw(lengths: tf.Tensor, *, batch_major: bool = True) -> tf.Tensor:
         """
         Wraps around tf.sequence_mask().
         It will cache the value inside the passed object so that we don't recompute it multiple times.
 
         :param lengths: shape (batch,)
         :param batch_major:
```

### Comparing `returnn-1.20230408.155406/returnn/tf/horovod.py` & `returnn-1.20230409.21835/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230409.21835/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/layers/base.py` & `returnn-1.20230409.21835/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/layers/basic.py` & `returnn-1.20230409.21835/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/layers/rec.py` & `returnn-1.20230409.21835/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/layers/segmental_model.py` & `returnn-1.20230409.21835/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/layers/signal_processing.py` & `returnn-1.20230409.21835/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/native_op.py` & `returnn-1.20230409.21835/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/network.py` & `returnn-1.20230409.21835/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/sprint.py` & `returnn-1.20230409.21835/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/updater.py` & `returnn-1.20230409.21835/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/util/basic.py` & `returnn-1.20230409.21835/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/util/data.py` & `returnn-1.20230409.21835/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/util/ken_lm.py` & `returnn-1.20230409.21835/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/tf/util/open_fst.py` & `returnn-1.20230409.21835/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/torch/data/pipeline.py` & `returnn-1.20230409.21835/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230409.21835/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/torch/data/tensor_utils.py` & `returnn-1.20230409.21835/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/torch/engine.py` & `returnn-1.20230409.21835/returnn/torch/engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -137,42 +137,52 @@
         train one (sub)epoch
         """
         print("start", self.get_epoch_str(), "with learning rate", self.learning_rate, "...", file=log.v4)
 
         self._pt_model.train()
 
         accumulated_losses_dict = NumbersDict()
+        accumulated_inv_norm_factors_dict = NumbersDict()
         step_idx = 0
         for data in self._train_dataloader:
             self._run_step(data)
 
             train_ctx = rf.get_run_ctx()
-            losses_dict = train_ctx.losses
             total_loss = train_ctx.total_loss()
+            losses_dict = NumbersDict(
+                {
+                    name: float(loss.get_summed_loss().raw_tensor.detach().cpu().numpy())
+                    for name, loss in train_ctx.losses.items()
+                }
+            )
+            inv_norm_factors_dict = NumbersDict(
+                {name: float(_to_raw(loss.get_inv_norm_factor())) for name, loss in train_ctx.losses.items()}
+            )
 
             self._updater.get_optimizer().zero_grad()
             total_loss.raw_tensor.backward()
             self._updater.get_optimizer().step()
 
-            losses_dict = {
-                "train_loss_" + name: float(loss.loss.raw_tensor.detach().cpu().numpy())
-                for name, loss in losses_dict.items()
-            }
-            accumulated_losses_dict += NumbersDict(losses_dict)
-            print("step %i, loss: %f" % (step_idx, total_loss.raw_tensor.detach().cpu().numpy()), file=log.v4)
+            accumulated_losses_dict += losses_dict
+            accumulated_inv_norm_factors_dict += inv_norm_factors_dict
+            print(f"step {step_idx}, loss: {dict(losses_dict / inv_norm_factors_dict)}", file=log.v4)
 
             step_idx += 1
             self._train_step += 1
 
         print("Trained %i steps" % step_idx)
 
-        accumulated_losses_dict = accumulated_losses_dict / step_idx
-        self.learning_rate_control.set_epoch_error(self.epoch, dict(accumulated_losses_dict))
+        accumulated_losses_dict = accumulated_losses_dict / accumulated_inv_norm_factors_dict
+        self.learning_rate_control.set_epoch_error(
+            self.epoch, {f"train_loss_{k}": v for k, v in accumulated_losses_dict.items()}
+        )
         self.learning_rate_control.save()
 
+        print(f"Total train loss: {dict(accumulated_losses_dict)}", file=log.v3)
+
         if self.epoch % self._save_model_epoch_interval == 0 or self.epoch == self._final_epoch:
             self._save_model()
             self._save_optimizer()
 
         self.eval_model()
 
     def eval_model(self):
@@ -182,46 +192,48 @@
         self._pt_model.eval()
 
         for dataset_name, dataset in self.eval_datasets.items():
             print(f"Evaluating dataset {dataset_name!r}'", file=log.v3)
 
             data_loader = self._eval_dataloaders[dataset_name]
 
-            accumulated_loss = 0.0
             accumulated_losses_dict = NumbersDict()
+            accumulated_inv_norm_factors_dict = NumbersDict()
             step_idx = 0
 
             with torch.no_grad():
                 for data in data_loader:
 
                     self._run_step(data)
                     train_ctx = rf.get_run_ctx()
-                    losses_dict = train_ctx.losses
-                    total_loss = train_ctx.total_loss()
-
-                    total_loss = total_loss.raw_tensor.detach().cpu().numpy()
-                    losses_dict = {
-                        dataset_name + "_loss_" + name: float(loss.loss.raw_tensor.detach().cpu().numpy())
-                        for name, loss in losses_dict.items()
-                    }
-                    print("step %i, loss: %f" % (step_idx, total_loss), file=log.v4)
 
-                    accumulated_loss += total_loss
-                    accumulated_losses_dict += NumbersDict(losses_dict)
+                    losses_dict = NumbersDict(
+                        {
+                            name: float(loss.get_summed_loss().raw_tensor.detach().cpu().numpy())
+                            for name, loss in train_ctx.losses.items()
+                        }
+                    )
+                    inv_norm_factors_dict = NumbersDict(
+                        {name: float(_to_raw(loss.get_inv_norm_factor())) for name, loss in train_ctx.losses.items()}
+                    )
+
+                    accumulated_losses_dict += losses_dict
+                    accumulated_inv_norm_factors_dict += inv_norm_factors_dict
+                    print(f"step {step_idx}, loss: {dict(losses_dict / inv_norm_factors_dict)}", file=log.v4)
                     step_idx += 1
 
-            assert step_idx > 0, "No data in dataset '{}'.".format(dataset_name)
-            accumulated_loss = accumulated_loss / step_idx
-            accumulated_losses_dict = accumulated_losses_dict / step_idx
+            assert step_idx > 0, f"No data in dataset {dataset_name!r}."
+            accumulated_losses_dict = accumulated_losses_dict / accumulated_inv_norm_factors_dict
 
-            self.learning_rate_control.set_epoch_error(self.epoch, dict(accumulated_losses_dict))
-
-            print("Total loss for '{}': {:.6}".format(dataset_name, accumulated_loss), file=log.v3)
+            self.learning_rate_control.set_epoch_error(
+                self.epoch, {f"{dataset_name}_loss_{k}": v for k, v in accumulated_losses_dict.items()}
+            )
+            self.learning_rate_control.save()
 
-        self.learning_rate_control.save()
+            print(f"Total loss for {dataset_name!r}: {dict(accumulated_losses_dict)}", file=log.v3)
 
     def _create_data_loader(self, dataset: Dataset) -> DataLoader2:
         """
         :param dataset: RETURNN dataset
         :return: PyTorch data loader created from given RETURNN dataset
         """
         # Make sure that _dataset_reset does not keep a ref to `self`,
@@ -400,7 +412,15 @@
         """
         filename = self.get_epoch_model_filename() + ".opt" + util.get_model_filename_postfix()
         directory = os.path.dirname(filename)
         if directory and not os.path.exists(directory):
             os.makedirs(directory, exist_ok=True)
 
         self._updater.save_optimizer(filename)
+
+
+def _to_raw(n: Union[int, float, Tensor]):
+    if isinstance(n, (int, float)):
+        return n
+    if isinstance(n, Tensor):
+        return n.raw_tensor.detach().cpu().numpy()
+    raise TypeError(f"Unexpected {n} of type {type(n)}")
```

### Comparing `returnn-1.20230408.155406/returnn/torch/frontend/_backend.py` & `returnn-1.20230409.21835/returnn/torch/frontend/_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,14 +113,19 @@
         :param raw_tensor:
         :param axis: e.g. 1
         :return: raw tensor with new axis
         """
         return raw_tensor.unsqueeze(axis)
 
     @staticmethod
+    def cast_raw(raw_tensor: torch.Tensor, dtype: str) -> torch.Tensor:
+        """cast"""
+        return raw_tensor.to(dtype=TorchBackend.as_dtype_raw(dtype))
+
+    @staticmethod
     def activation_raw(raw_tensor: torch.Tensor, func: str) -> torch.Tensor:
         """
         :param raw_tensor:
         :param func: e.g. "tanh"
         :return: raw tensor after activation
         """
         assert func in Backend._AllowedActivationFuncs
@@ -408,33 +413,58 @@
         result_dims = common_dims + a_unique_dims + b_unique_dims
 
         result_tensor = Tensor(name="dot", dims=result_dims, raw_tensor=raw_result, dtype=a.dtype)
 
         return result_tensor
 
     @staticmethod
+    def range_over_dim(dim: Dim) -> Tensor[torch.Tensor]:
+        """
+        :param dim:
+        :return: tensor with shape [dim]
+        """
+        out = Tensor(
+            "range",
+            dims=[dim],
+            sparse_dim=dim,
+            dtype=dim.dyn_size_ext.dtype if dim.dyn_size_ext else rf.get_default_array_index_dtype(),
+        )
+        out.raw_tensor = torch.arange(dim.get_dim_value())
+        return out
+
+    @staticmethod
     def reduce(
         source: Tensor[torch.Tensor],
         *,
         mode: str,
         axis: Union[Dim, Sequence[Dim]],
         use_time_mask: bool = NotSpecified,
     ) -> Tensor[torch.Tensor]:
         """reduce"""
         assert mode in Backend._AllowedReduceModes
         if isinstance(axis, Dim):
-            assert not axis.need_masking()  # not implemented
-        else:
-            assert all(not dim.need_masking() for dim in axis)  # not implemented
+            axis = [axis]
+        assert all(isinstance(dim, Dim) for dim in axis)
+        if use_time_mask is not False and any(dim.need_masking() for dim in axis):
+            source = source.copy()
+            dtype = source.raw_tensor.dtype
+            if mode == "max":
+                mask_value = torch.finfo(dtype).min if dtype.is_floating_point else torch.iinfo(dtype).min
+            elif mode == "min":
+                mask_value = torch.finfo(dtype).max if dtype.is_floating_point else torch.iinfo(dtype).max
+            elif mode == "sum":
+                mask_value = 0
+            else:
+                raise NotImplementedError(f"reduce_{mode} not implemented with masking on tensor {source!r}.")
+            for i, dim in enumerate(axis):
+                if dim.need_masking():
+                    mask = source.get_sequence_mask_broadcast(axis=i)
+                    source.raw_tensor = torch.where(mask, source.raw_tensor, mask_value)
         func = getattr(torch, mode)
-        raw_dims = (
-            [source.get_axis_from_description(axis)]
-            if isinstance(axis, Dim)
-            else [source.get_axis_from_description(dim) for dim in axis]
-        )
+        raw_dims = [source.get_axis_from_description(dim) for dim in axis]
         res_dims = [dim for i, dim in enumerate(source.dims) if i not in raw_dims]
         if not res_dims:
             raw_result = func(source.raw_tensor)
         elif len(raw_dims) == 1:
             raw_result = func(source.raw_tensor, dim=raw_dims[0])
             if mode in ["max", "min"]:
                 # result is a tuple (values, indices). https://pytorch.org/docs/stable/generated/torch.max.html
```

### Comparing `returnn-1.20230408.155406/returnn/torch/frontend/_rand.py` & `returnn-1.20230409.21835/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/torch/frontend/bridge.py` & `returnn-1.20230409.21835/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/torch/updater.py` & `returnn-1.20230409.21835/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/basic.py` & `returnn-1.20230409.21835/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/better_exchook.py` & `returnn-1.20230409.21835/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/bpe.py` & `returnn-1.20230409.21835/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/debug.py` & `returnn-1.20230409.21835/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/debug_helpers.py` & `returnn-1.20230409.21835/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/fsa.py` & `returnn-1.20230409.21835/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230409.21835/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/pprint.py` & `returnn-1.20230409.21835/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/py-to-pickle.cpp` & `returnn-1.20230409.21835/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/sig_proc.py` & `returnn-1.20230409.21835/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn/util/task_system.py` & `returnn-1.20230409.21835/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/returnn.egg-info/PKG-INFO` & `returnn-1.20230409.21835/returnn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230408.155406
+Version: 1.20230409.21835
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230408.155406/returnn.egg-info/SOURCES.txt` & `returnn-1.20230409.21835/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/setup.py` & `returnn-1.20230409.21835/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/DummySprintExec.py` & `returnn-1.20230409.21835/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230409.21835/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230409.21835/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230409.21835/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/_set_num_threads1.py` & `returnn-1.20230409.21835/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/_setup_test_env.py` & `returnn-1.20230409.21835/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/bpe-unicode-demo.codes` & `returnn-1.20230409.21835/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/bpe-unicode-demo.vocab` & `returnn-1.20230409.21835/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/lexicon_opt.isyms` & `returnn-1.20230409.21835/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/lexicon_opt.jpg` & `returnn-1.20230409.21835/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/lint_common.py` & `returnn-1.20230409.21835/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/pycharm-inspect.py` & `returnn-1.20230409.21835/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/pylint.py` & `returnn-1.20230409.21835/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/returnn-as-framework.py` & `returnn-1.20230409.21835/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/rf_utils.py` & `returnn-1.20230409.21835/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/spelling.dic` & `returnn-1.20230409.21835/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_Config.py` & `returnn-1.20230409.21835/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_Dataset.py` & `returnn-1.20230409.21835/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_Fsa.py` & `returnn-1.20230409.21835/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_GeneratingDataset.py` & `returnn-1.20230409.21835/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_HDFDataset.py` & `returnn-1.20230409.21835/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_LearningRateControl.py` & `returnn-1.20230409.21835/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_Log.py` & `returnn-1.20230409.21835/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_MultiProcDataset.py` & `returnn-1.20230409.21835/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_PTDataset.py` & `returnn-1.20230409.21835/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_Pretrain.py` & `returnn-1.20230409.21835/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_ResNet.py` & `returnn-1.20230409.21835/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_SprintDataset.py` & `returnn-1.20230409.21835/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_SprintInterface.py` & `returnn-1.20230409.21835/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TFEngine.py` & `returnn-1.20230409.21835/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TFNativeOp.py` & `returnn-1.20230409.21835/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TFNetworkLayer.py` & `returnn-1.20230409.21835/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230409.21835/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230409.21835/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TFUpdater.py` & `returnn-1.20230409.21835/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TFUtil.py` & `returnn-1.20230409.21835/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TF_determinism.py` & `returnn-1.20230409.21835/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TaskSystem.py` & `returnn-1.20230409.21835/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230409.21835/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_TranslationDataset.py` & `returnn-1.20230409.21835/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_Util.py` & `returnn-1.20230409.21835/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_demos.py` & `returnn-1.20230409.21835/tests/test_demos.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,14 +135,21 @@
 @unittest.skipIf(not torch, "no PyTorch")
 def test_demo_torch_task12ax():
     cleanup_tmp_models("demos/demo-torch.config")
     run(py, "rnn.py", "demos/demo-torch.config", print_stdout=True)
     # TODO also check FER. So far this is not properly reported. https://github.com/rwth-i6/returnn/issues/1120
 
 
+@unittest.skipIf(not torch, "no PyTorch")
+def test_demo_rf_torch_task12ax():
+    cleanup_tmp_models("demos/demo-rf.config")
+    run(py, "rnn.py", "demos/demo-rf.config", print_stdout=True)
+    # TODO also check FER. So far this is not properly reported. https://github.com/rwth-i6/returnn/issues/1120
+
+
 def test_demo_iter_dataset_task12ax():
     # there should be no actual TF dependency, we just iterate the dataset
     cleanup_tmp_models("demos/demo-tf-vanilla-lstm.12ax.config")
     # pick any 12ax config for the dataset test
     out = run(py, "demos/demo-iter-dataset.py", "demos/demo-tf-vanilla-lstm.12ax.config")
     assert_in("Epoch 5.", out.splitlines())
```

### Comparing `returnn-1.20230408.155406/tests/test_fork_exec.py` & `returnn-1.20230409.21835/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_hdf_dump.py` & `returnn-1.20230409.21835/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_rf_base.py` & `returnn-1.20230409.21835/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_tensor.py` & `returnn-1.20230409.21835/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_tools.py` & `returnn-1.20230409.21835/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_torch_frontend.py` & `returnn-1.20230409.21835/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tests/test_torch_internal_frontend.py` & `returnn-1.20230409.21835/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/analyze-dataset-batches.py` & `returnn-1.20230409.21835/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/bliss-collect-seq-lens.py` & `returnn-1.20230409.21835/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/bliss-dump-text.py` & `returnn-1.20230409.21835/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/bliss-get-segment-names.py` & `returnn-1.20230409.21835/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/bliss-to-ogg-zip.py` & `returnn-1.20230409.21835/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/bpe-create-lexicon.py` & `returnn-1.20230409.21835/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/calculate-word-error-rate.py` & `returnn-1.20230409.21835/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/cleanup-old-models.py` & `returnn-1.20230409.21835/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/collect-orth-symbols.py` & `returnn-1.20230409.21835/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/collect-words.py` & `returnn-1.20230409.21835/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/compile_native_op.py` & `returnn-1.20230409.21835/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/compile_tf_graph.py` & `returnn-1.20230409.21835/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/debug-dump-search-scores.py` & `returnn-1.20230409.21835/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/debug-plot-search-scores.py` & `returnn-1.20230409.21835/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/dump-dataset-raw-strings.py` & `returnn-1.20230409.21835/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/dump-dataset.py` & `returnn-1.20230409.21835/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/dump-forward-stats.py` & `returnn-1.20230409.21835/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/dump-forward.py` & `returnn-1.20230409.21835/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/dump-network-json.py` & `returnn-1.20230409.21835/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/dump-pickle.py` & `returnn-1.20230409.21835/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230409.21835/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/get-attention-weights.py` & `returnn-1.20230409.21835/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/get-best-model-epoch.py` & `returnn-1.20230409.21835/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/hdf_dump.py` & `returnn-1.20230409.21835/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230409.21835/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/import-blocks-mt-model.py` & `returnn-1.20230409.21835/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/import-t2t-mt-model.py` & `returnn-1.20230409.21835/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/Makefile` & `returnn-1.20230409.21835/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/README.md` & `returnn-1.20230409.21835/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/example/README.md` & `returnn-1.20230409.21835/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230409.21835/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/file.h` & `returnn-1.20230409.21835/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230409.21835/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230409.21835/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/main.cc` & `returnn-1.20230409.21835/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230409.21835/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230409.21835/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230409.21835/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/tf_avg_checkpoints.py` & `returnn-1.20230409.21835/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/tf_inspect_checkpoint.py` & `returnn-1.20230409.21835/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230408.155406/tools/tf_inspect_summary_log.py` & `returnn-1.20230409.21835/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

