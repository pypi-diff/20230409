# Comparing `tmp/so_vits_svc_fork-3.1.5.tar.gz` & `tmp/so_vits_svc_fork-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.1.5.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.1.6.tar", max compression
```

## Comparing `so_vits_svc_fork-3.1.5.tar` & `so_vits_svc_fork-3.1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-09 10:47:25.913718 so_vits_svc_fork-3.1.5/LICENSE
--rw-r--r--   0        0        0    17988 2023-04-09 10:47:25.913718 so_vits_svc_fork-3.1.5/README.md
--rw-r--r--   0        0        0     3113 2023-04-09 10:47:27.061730 so_vits_svc_fork-3.1.5/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-09 10:47:27.013730 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22637 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1275 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2712 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2826 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7259 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    24381 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    22944 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0      731 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     5854 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1627 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1377 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1438 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2997 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4614 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4693 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    14776 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13081 2023-04-09 10:47:25.917719 so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    19957 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.1.5/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-09 15:42:33.495442 so_vits_svc_fork-3.1.6/LICENSE
+-rw-r--r--   0        0        0    17988 2023-04-09 15:42:33.495442 so_vits_svc_fork-3.1.6/README.md
+-rw-r--r--   0        0        0     3113 2023-04-09 15:42:34.563462 so_vits_svc_fork-3.1.6/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-09 15:42:34.515461 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22637 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1275 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2712 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2826 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7259 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    24381 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    22944 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0      731 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     5854 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1627 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1377 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1438 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2997 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4614 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4693 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    16186 2023-04-09 15:42:33.499442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13081 2023-04-09 15:42:33.503442 so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    19957 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.1.6/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.1.5/LICENSE` & `so_vits_svc_fork-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/README.md` & `so_vits_svc_fork-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/pyproject.toml` & `so_vits_svc_fork-3.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.1.5"
+version = "3.1.6"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import math
 import warnings
 from logging import getLogger
 from pathlib import Path
 from typing import Any
 
 import lightning.pytorch as pl
 import torch
@@ -65,33 +64,34 @@
     hparams = utils.get_backup_hparams(config_path, model_path)
     utils.ensure_pretrained_model(model_path, hparams.model.get("type_", "hifi-gan"))
 
     datamodule = VCDataModule(hparams)
     trainer = pl.Trainer(
         logger=TensorBoardLogger(model_path),
         # profiler="simple",
+        val_check_interval=hparams.train.eval_interval,
         max_epochs=hparams.train.epochs,
-        check_val_every_n_epoch=math.ceil(
-            hparams.train.eval_interval
-            / len(datamodule.train_dataset)
-            * hparams.train.batch_size
-        ),
+        check_val_every_n_epoch=None,
         precision=16
         if hparams.train.fp16_run
         else "bf16"
         if hparams.train.get("bf16_run", False)
         else 32,
     )
     model = VitsLightning(reset_optimizer=reset_optimizer, **hparams)
     trainer.fit(model, datamodule=datamodule)
 
 
 class VitsLightning(pl.LightningModule):
     def on_train_start(self) -> None:
-        self.load(False)
+        self.set_current_epoch(self._temp_epoch)
+        total_batch_idx = self._temp_epoch * len(self.trainer.train_dataloader)
+        self.set_total_batch_idx(total_batch_idx)
+        global_step = total_batch_idx * self.optimizers_count
+        self.set_global_step(global_step)
 
         # check if using tpu
         if isinstance(self.trainer.accelerator, TPUAccelerator):
             # patch torch.stft to use cpu
             LOG.warning("Using TPU. Patching torch.stft to use cpu.")
 
             def stft(
@@ -136,14 +136,30 @@
             global_step
         )
         self.trainer.fit_loop.epoch_loop.automatic_optimization.optim_progress.optimizer.step.total.completed = (
             global_step
         )
         assert self.global_step == global_step, f"{self.global_step} != {global_step}"
 
+    def set_total_batch_idx(self, total_batch_idx: int):
+        LOG.info(f"Setting total batch idx to {total_batch_idx}")
+        self.trainer.fit_loop.epoch_loop.batch_progress.total.ready = (
+            total_batch_idx + 1
+        )
+        self.trainer.fit_loop.epoch_loop.batch_progress.total.completed = (
+            total_batch_idx
+        )
+        assert (
+            self.total_batch_idx == total_batch_idx + 1
+        ), f"{self.total_batch_idx} != {total_batch_idx + 1}"
+
+    @property
+    def total_batch_idx(self) -> int:
+        return self.trainer.fit_loop.epoch_loop.total_batch_idx + 1
+
     def load(self, reset_optimizer: bool = False):
         latest_g_path = utils.latest_checkpoint_path(self.hparams.model_dir, "G_*.pth")
         latest_d_path = utils.latest_checkpoint_path(self.hparams.model_dir, "D_*.pth")
         if latest_g_path is not None and latest_d_path is not None:
             try:
                 _, _, _, epoch = utils.load_checkpoint(
                     latest_g_path,
@@ -153,20 +169,17 @@
                 )
                 _, _, _, epoch = utils.load_checkpoint(
                     latest_d_path,
                     self.net_d,
                     self.optim_d,
                     reset_optimizer,
                 )
-                self.set_current_epoch(epoch)
-                global_step = epoch * len(self.trainer.train_dataloader)
-                self.set_global_step(global_step)
-                assert self.current_epoch == epoch, f"{self.current_epoch} != {epoch}"
-                self.scheduler_g.last_epoch = self.current_epoch - 1
-                self.scheduler_d.last_epoch = self.current_epoch - 1
+                self._temp_epoch = epoch
+                self.scheduler_g.last_epoch = epoch - 1
+                self.scheduler_d.last_epoch = epoch - 1
             except Exception as e:
                 raise RuntimeError("Failed to load checkpoint") from e
         else:
             LOG.warning("No checkpoint found. Start from scratch.")
 
     def __init__(self, reset_optimizer: bool = False, **hparams: Any):
         super().__init__()
@@ -194,41 +207,59 @@
         )
         self.scheduler_g = torch.optim.lr_scheduler.ExponentialLR(
             self.optim_g, gamma=self.hparams.train.lr_decay
         )
         self.scheduler_d = torch.optim.lr_scheduler.ExponentialLR(
             self.optim_d, gamma=self.hparams.train.lr_decay
         )
+        self.optimizers_count = 2
+        self.load(reset_optimizer)
 
     def configure_optimizers(self):
         return [self.optim_g, self.optim_d], [self.scheduler_g, self.scheduler_d]
 
     def log_image_dict(
         self, image_dict: dict[str, Any], dataformats: str = "HWC"
     ) -> None:
         if not isinstance(self.logger, TensorBoardLogger):
             warnings.warn("Image logging is only supported with TensorBoardLogger.")
             return
         writer: SummaryWriter = self.logger.experiment
         for k, v in image_dict.items():
             try:
-                writer.add_image(k, v, self.global_step, dataformats=dataformats)
+                writer.add_image(k, v, self.total_batch_idx, dataformats=dataformats)
             except Exception as e:
                 warnings.warn(f"Failed to log image {k}: {e}")
 
     def log_audio_dict(self, audio_dict: dict[str, Any]) -> None:
         if not isinstance(self.logger, TensorBoardLogger):
             warnings.warn("Audio logging is only supported with TensorBoardLogger.")
             return
         writer: SummaryWriter = self.logger.experiment
         for k, v in audio_dict.items():
             writer.add_audio(
-                k, v, self.global_step, sample_rate=self.hparams.data.sampling_rate
+                k,
+                v,
+                self.trainer.fit_loop.total_batch_idx,
+                sample_rate=self.hparams.data.sampling_rate,
             )
 
+    def log_dict_(self, log_dict: dict[str, Any], **kwargs) -> None:
+        if not isinstance(self.logger, TensorBoardLogger):
+            warnings.warn("Logging is only supported with TensorBoardLogger.")
+            return
+        writer: SummaryWriter = self.logger.experiment
+        for k, v in log_dict.items():
+            writer.add_scalar(k, v, self.total_batch_idx)
+        kwargs["logger"] = False
+        self.log_dict(log_dict, **kwargs)
+
+    def log_(self, key: str, value: Any, **kwargs) -> None:
+        self.log_dict_({key: value}, **kwargs)
+
     def training_step(self, batch: dict[str, torch.Tensor], batch_idx: int) -> None:
         self.net_g.train()
         self.net_d.train()
 
         # get optims
         optim_g, optim_d = self.optimizers()
 
@@ -278,29 +309,31 @@
                 from .modules.decoders.mb_istft import PQMF, subband_stft_loss
 
                 y_mb = PQMF(y.device, self.hparams.model.subbands).analysis(y)
                 loss_subband = subband_stft_loss(self.hparams, y_mb, y_hat_mb)
             loss_gen_all += loss_subband
 
         # log loss
-        self.log("grad_norm_g", commons.clip_grad_value_(self.net_g.parameters(), None))
-        self.log("lr", self.optim_g.param_groups[0]["lr"])
-        self.log_dict(
+        self.log_(
+            "grad_norm_g", commons.clip_grad_value_(self.net_g.parameters(), None)
+        )
+        self.log_("lr", self.optim_g.param_groups[0]["lr"])
+        self.log_dict_(
             {
                 "loss/g/total": loss_gen_all,
                 "loss/g/fm": loss_fm,
                 "loss/g/mel": loss_mel,
                 "loss/g/kl": loss_kl,
                 "loss/g/lf0": loss_lf0,
             },
             prog_bar=True,
         )
         if self.hparams.model.get("type_") == "mb-istft":
-            self.log("loss/g/subband", loss_subband)
-        if self.global_step % self.hparams.train.log_interval == 0:
+            self.log_("loss/g/subband", loss_subband)
+        if self.total_batch_idx % self.hparams.train.log_interval == 0:
             self.log_image_dict(
                 {
                     "slice/mel_org": utils.plot_spectrogram_to_numpy(
                         y_mel[0].data.cpu().numpy()
                     ),
                     "slice/mel_gen": utils.plot_spectrogram_to_numpy(
                         y_hat_mel[0].data.cpu().numpy()
@@ -334,16 +367,18 @@
         with autocast(enabled=False):
             loss_disc, losses_disc_r, losses_disc_g = discriminator_loss(
                 y_d_hat_r, y_d_hat_g
             )
             loss_disc_all = loss_disc
 
         # log loss
-        self.log("loss/d/total", loss_disc_all, prog_bar=True)
-        self.log("grad_norm_d", commons.clip_grad_value_(self.net_d.parameters(), None))
+        self.log_("loss/d/total", loss_disc_all, prog_bar=True)
+        self.log_(
+            "grad_norm_d", commons.clip_grad_value_(self.net_d.parameters(), None)
+        )
 
         # optimizer
         self.manual_backward(loss_disc_all)
         optim_d.step()
         optim_d.zero_grad()
         self.untoggle_optimizer(optim_d)
 
@@ -360,27 +395,29 @@
                 {
                     "gen/mel": utils.plot_spectrogram_to_numpy(
                         y_hat_mel[0].cpu().numpy()
                     ),
                     "gt/mel": utils.plot_spectrogram_to_numpy(mel[0].cpu().numpy()),
                 }
             )
+            if self.current_epoch == 0:
+                return
             utils.save_checkpoint(
                 self.net_g,
                 self.optim_g,
                 self.hparams.train.learning_rate,
-                self.current_epoch,
-                Path(self.hparams.model_dir) / f"G_{self.global_step}.pth",
+                self.current_epoch + 1,  # prioritize prevention of undervaluation
+                Path(self.hparams.model_dir) / f"G_{self.total_batch_idx}.pth",
             )
             utils.save_checkpoint(
                 self.net_d,
                 self.optim_d,
                 self.hparams.train.learning_rate,
-                self.current_epoch,
-                Path(self.hparams.model_dir) / f"D_{self.global_step}.pth",
+                self.current_epoch + 1,
+                Path(self.hparams.model_dir) / f"D_{self.total_batch_idx}.pth",
             )
             keep_ckpts = self.hparams.train.get("keep_ckpts", 0)
             if keep_ckpts > 0:
                 utils.clean_checkpoints(
                     path_to_models=self.hparams.model_dir,
                     n_ckpts_to_keep=keep_ckpts,
                     sort_by_time=True,
```

### Comparing `so_vits_svc_fork-3.1.5/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.1.6/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.5/PKG-INFO` & `so_vits_svc_fork-3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.1.5
+Version: 3.1.6
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.1.5 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.1.6 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

