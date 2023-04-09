# Comparing `tmp/ckip-transformers-0.3.3.tar.gz` & `tmp/ckip-transformers-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckip-transformers-0.3.3.tar", last modified: Sun Apr  9 05:38:25 2023, max compression
+gzip compressed data, was "ckip-transformers-0.3.4.tar", last modified: Sun Apr  9 13:02:50 2023, max compression
```

## Comparing `ckip-transformers-0.3.3.tar` & `ckip-transformers-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:38:25.973787 ckip-transformers-0.3.3/
--rw-r--r--   0 emfo       (501) staff       (20)    35149 2021-02-01 06:02:22.000000 ckip-transformers-0.3.3/LICENSE
--rw-r--r--   0 emfo       (501) staff       (20)       26 2021-02-01 06:53:21.000000 ckip-transformers-0.3.3/MANIFEST.in
--rw-r--r--   0 emfo       (501) staff       (20)    25418 2023-04-09 05:38:25.973934 ckip-transformers-0.3.3/PKG-INFO
--rw-r--r--   0 emfo       (501) staff       (20)    24484 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/README.rst
-drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:38:25.972128 ckip-transformers-0.3.3/ckip_transformers/
--rw-r--r--   0 emfo       (501) staff       (20)      403 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/ckip_transformers/__init__.py
-drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:38:25.973636 ckip-transformers-0.3.3/ckip_transformers/nlp/
--rw-r--r--   0 emfo       (501) staff       (20)      298 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/ckip_transformers/nlp/__init__.py
--rw-r--r--   0 emfo       (501) staff       (20)    12460 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/ckip_transformers/nlp/driver.py
--rw-r--r--   0 emfo       (501) staff       (20)     9620 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/ckip_transformers/nlp/util.py
-drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:38:25.973055 ckip-transformers-0.3.3/ckip_transformers.egg-info/
--rw-r--r--   0 emfo       (501) staff       (20)    25418 2023-04-09 05:38:25.000000 ckip-transformers-0.3.3/ckip_transformers.egg-info/PKG-INFO
--rw-r--r--   0 emfo       (501) staff       (20)      394 2023-04-09 05:38:25.000000 ckip-transformers-0.3.3/ckip_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 emfo       (501) staff       (20)        1 2023-04-09 05:38:25.000000 ckip-transformers-0.3.3/ckip_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 emfo       (501) staff       (20)       44 2023-04-09 05:38:25.000000 ckip-transformers-0.3.3/ckip_transformers.egg-info/requires.txt
--rw-r--r--   0 emfo       (501) staff       (20)       18 2023-04-09 05:38:25.000000 ckip-transformers-0.3.3/ckip_transformers.egg-info/top_level.txt
--rw-r--r--   0 emfo       (501) staff       (20)       57 2021-06-16 06:01:27.000000 ckip-transformers-0.3.3/pyproject.toml
--rw-r--r--   0 emfo       (501) staff       (20)       80 2023-04-09 05:38:25.974388 ckip-transformers-0.3.3/setup.cfg
--rw-r--r--   0 emfo       (501) staff       (20)     1944 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/setup.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 13:02:50.828004 ckip-transformers-0.3.4/
+-rw-r--r--   0 emfo       (501) staff       (20)    35149 2021-02-01 06:02:22.000000 ckip-transformers-0.3.4/LICENSE
+-rw-r--r--   0 emfo       (501) staff       (20)       26 2021-02-01 06:53:21.000000 ckip-transformers-0.3.4/MANIFEST.in
+-rw-r--r--   0 emfo       (501) staff       (20)    25603 2023-04-09 13:02:50.828234 ckip-transformers-0.3.4/PKG-INFO
+-rw-r--r--   0 emfo       (501) staff       (20)    24669 2023-04-09 13:02:33.000000 ckip-transformers-0.3.4/README.rst
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 13:02:50.825924 ckip-transformers-0.3.4/ckip_transformers/
+-rw-r--r--   0 emfo       (501) staff       (20)      403 2023-04-09 13:02:33.000000 ckip-transformers-0.3.4/ckip_transformers/__init__.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 13:02:50.827489 ckip-transformers-0.3.4/ckip_transformers/nlp/
+-rw-r--r--   0 emfo       (501) staff       (20)      298 2023-04-09 05:37:58.000000 ckip-transformers-0.3.4/ckip_transformers/nlp/__init__.py
+-rw-r--r--   0 emfo       (501) staff       (20)    12460 2023-04-09 05:37:58.000000 ckip-transformers-0.3.4/ckip_transformers/nlp/driver.py
+-rw-r--r--   0 emfo       (501) staff       (20)     9620 2023-04-09 05:37:58.000000 ckip-transformers-0.3.4/ckip_transformers/nlp/util.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 13:02:50.826573 ckip-transformers-0.3.4/ckip_transformers.egg-info/
+-rw-r--r--   0 emfo       (501) staff       (20)    25603 2023-04-09 13:02:50.000000 ckip-transformers-0.3.4/ckip_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 emfo       (501) staff       (20)      394 2023-04-09 13:02:50.000000 ckip-transformers-0.3.4/ckip_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 emfo       (501) staff       (20)        1 2023-04-09 13:02:50.000000 ckip-transformers-0.3.4/ckip_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 emfo       (501) staff       (20)       44 2023-04-09 13:02:50.000000 ckip-transformers-0.3.4/ckip_transformers.egg-info/requires.txt
+-rw-r--r--   0 emfo       (501) staff       (20)       18 2023-04-09 13:02:50.000000 ckip-transformers-0.3.4/ckip_transformers.egg-info/top_level.txt
+-rw-r--r--   0 emfo       (501) staff       (20)       57 2021-06-16 06:01:27.000000 ckip-transformers-0.3.4/pyproject.toml
+-rw-r--r--   0 emfo       (501) staff       (20)       80 2023-04-09 13:02:50.832044 ckip-transformers-0.3.4/setup.cfg
+-rw-r--r--   0 emfo       (501) staff       (20)     1944 2023-04-09 05:37:58.000000 ckip-transformers-0.3.4/setup.py
```

### Comparing `ckip-transformers-0.3.3/LICENSE` & `ckip-transformers-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ckip-transformers-0.3.3/PKG-INFO` & `ckip-transformers-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ckip-transformers
-Version: 0.3.3
+Version: 0.3.4
 Summary: CKIP Transformers
 Home-page: https://ckip-transformers.readthedocs.io
 Author: Mu Yang
 Author-email: emfomy@gmail.com
 License: GPL-3.0
-Download-URL: https://ckip-transformers.readthedocs.io/tarball/0.3.3
+Download-URL: https://ckip-transformers.readthedocs.io/tarball/0.3.4
 Platform: linux_x86_64
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -115,14 +115,15 @@
 | 您可於 https://huggingface.co/ckiplab/ 下載預訓練的模型。
 
 - Language Models
    * `ALBERT Tiny <https://huggingface.co/ckiplab/albert-tiny-chinese>`_: ``ckiplab/albert-tiny-chinese``
    * `ALBERT Base <https://huggingface.co/ckiplab/albert-base-chinese>`_: ``ckiplab/albert-base-chinese``
    * `BERT Tiny <https://huggingface.co/ckiplab/bert-tiny-chinese>`_: ``ckiplab/bert-tiny-chinese``
    * `BERT Base <https://huggingface.co/ckiplab/bert-base-chinese>`_: ``ckiplab/bert-base-chinese``
+   * `GPT2 Tiny <https://huggingface.co/ckiplab/gpt2-tiny-chinese>`_: ``ckiplab/gpt2-tiny-chinese``
    * `GPT2 Base <https://huggingface.co/ckiplab/gpt2-base-chinese>`_: ``ckiplab/gpt2-base-chinese``
 
 - NLP Task Models
    * `ALBERT Tiny — Word Segmentation <https://huggingface.co/ckiplab/albert-tiny-chinese-ws>`_: ``ckiplab/albert-tiny-chinese-ws``
    * `ALBERT Tiny — Part-of-Speech Tagging <https://huggingface.co/ckiplab/albert-tiny-chinese-pos>`_: ``ckiplab/albert-tiny-chinese-pos``
    * `ALBERT Tiny — Named-Entity Recognition <https://huggingface.co/ckiplab/albert-tiny-chinese-ner>`_: ``ckiplab/albert-tiny-chinese-ner``
    * `ALBERT Base — Word Segmentation <https://huggingface.co/ckiplab/albert-base-chinese-ws>`_: ``ckiplab/albert-base-chinese-ws``
@@ -205,14 +206,15 @@
 ================================  ===========  ===========  ========  ==========  =========
 Model                             #Parameters  Perplexity†  WS (F1)‡  POS (ACC)‡  NER (F1)‡
 ================================  ===========  ===========  ========  ==========  =========
 ckiplab/albert-tiny-chinese         4M          4.80        96.66%    94.48%      71.17%
 ckiplab/albert-base-chinese        11M          2.65        97.33%    95.30%      79.47%
 ckiplab/bert-tiny-chinese          12M          8.07        96.98%    95.11%      74.21%
 ckiplab/bert-base-chinese         102M          1.88        97.60%    95.67%      81.18%
+ckiplab/gpt2-tiny-chinese           4M         16.94        --        --          --
 ckiplab/gpt2-base-chinese         102M          8.36        --        --          --
 --------------------------------  -----------  -----------  --------  ----------  ---------
 
 --------------------------------  -----------  -----------  --------  ----------  ---------
 voidful/albert_chinese_tiny         4M         74.93        --        --          --
 voidful/albert_chinese_base        11M         22.34        --        --          --
 bert-base-chinese                 102M          2.53        --        --          --
```

### Comparing `ckip-transformers-0.3.3/README.rst` & `ckip-transformers-0.3.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 | 您可於 https://huggingface.co/ckiplab/ 下載預訓練的模型。
 
 - Language Models
    * `ALBERT Tiny <https://huggingface.co/ckiplab/albert-tiny-chinese>`_: ``ckiplab/albert-tiny-chinese``
    * `ALBERT Base <https://huggingface.co/ckiplab/albert-base-chinese>`_: ``ckiplab/albert-base-chinese``
    * `BERT Tiny <https://huggingface.co/ckiplab/bert-tiny-chinese>`_: ``ckiplab/bert-tiny-chinese``
    * `BERT Base <https://huggingface.co/ckiplab/bert-base-chinese>`_: ``ckiplab/bert-base-chinese``
+   * `GPT2 Tiny <https://huggingface.co/ckiplab/gpt2-tiny-chinese>`_: ``ckiplab/gpt2-tiny-chinese``
    * `GPT2 Base <https://huggingface.co/ckiplab/gpt2-base-chinese>`_: ``ckiplab/gpt2-base-chinese``
 
 - NLP Task Models
    * `ALBERT Tiny — Word Segmentation <https://huggingface.co/ckiplab/albert-tiny-chinese-ws>`_: ``ckiplab/albert-tiny-chinese-ws``
    * `ALBERT Tiny — Part-of-Speech Tagging <https://huggingface.co/ckiplab/albert-tiny-chinese-pos>`_: ``ckiplab/albert-tiny-chinese-pos``
    * `ALBERT Tiny — Named-Entity Recognition <https://huggingface.co/ckiplab/albert-tiny-chinese-ner>`_: ``ckiplab/albert-tiny-chinese-ner``
    * `ALBERT Base — Word Segmentation <https://huggingface.co/ckiplab/albert-base-chinese-ws>`_: ``ckiplab/albert-base-chinese-ws``
@@ -180,14 +181,15 @@
 ================================  ===========  ===========  ========  ==========  =========
 Model                             #Parameters  Perplexity†  WS (F1)‡  POS (ACC)‡  NER (F1)‡
 ================================  ===========  ===========  ========  ==========  =========
 ckiplab/albert-tiny-chinese         4M          4.80        96.66%    94.48%      71.17%
 ckiplab/albert-base-chinese        11M          2.65        97.33%    95.30%      79.47%
 ckiplab/bert-tiny-chinese          12M          8.07        96.98%    95.11%      74.21%
 ckiplab/bert-base-chinese         102M          1.88        97.60%    95.67%      81.18%
+ckiplab/gpt2-tiny-chinese           4M         16.94        --        --          --
 ckiplab/gpt2-base-chinese         102M          8.36        --        --          --
 --------------------------------  -----------  -----------  --------  ----------  ---------
 
 --------------------------------  -----------  -----------  --------  ----------  ---------
 voidful/albert_chinese_tiny         4M         74.93        --        --          --
 voidful/albert_chinese_base        11M         22.34        --        --          --
 bert-base-chinese                 102M          2.53        --        --          --
```

### Comparing `ckip-transformers-0.3.3/ckip_transformers/nlp/driver.py` & `ckip-transformers-0.3.4/ckip_transformers/nlp/driver.py`

 * *Files identical despite different names*

### Comparing `ckip-transformers-0.3.3/ckip_transformers/nlp/util.py` & `ckip-transformers-0.3.4/ckip_transformers/nlp/util.py`

 * *Files identical despite different names*

### Comparing `ckip-transformers-0.3.3/ckip_transformers.egg-info/PKG-INFO` & `ckip-transformers-0.3.4/ckip_transformers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ckip-transformers
-Version: 0.3.3
+Version: 0.3.4
 Summary: CKIP Transformers
 Home-page: https://ckip-transformers.readthedocs.io
 Author: Mu Yang
 Author-email: emfomy@gmail.com
 License: GPL-3.0
-Download-URL: https://ckip-transformers.readthedocs.io/tarball/0.3.3
+Download-URL: https://ckip-transformers.readthedocs.io/tarball/0.3.4
 Platform: linux_x86_64
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -115,14 +115,15 @@
 | 您可於 https://huggingface.co/ckiplab/ 下載預訓練的模型。
 
 - Language Models
    * `ALBERT Tiny <https://huggingface.co/ckiplab/albert-tiny-chinese>`_: ``ckiplab/albert-tiny-chinese``
    * `ALBERT Base <https://huggingface.co/ckiplab/albert-base-chinese>`_: ``ckiplab/albert-base-chinese``
    * `BERT Tiny <https://huggingface.co/ckiplab/bert-tiny-chinese>`_: ``ckiplab/bert-tiny-chinese``
    * `BERT Base <https://huggingface.co/ckiplab/bert-base-chinese>`_: ``ckiplab/bert-base-chinese``
+   * `GPT2 Tiny <https://huggingface.co/ckiplab/gpt2-tiny-chinese>`_: ``ckiplab/gpt2-tiny-chinese``
    * `GPT2 Base <https://huggingface.co/ckiplab/gpt2-base-chinese>`_: ``ckiplab/gpt2-base-chinese``
 
 - NLP Task Models
    * `ALBERT Tiny — Word Segmentation <https://huggingface.co/ckiplab/albert-tiny-chinese-ws>`_: ``ckiplab/albert-tiny-chinese-ws``
    * `ALBERT Tiny — Part-of-Speech Tagging <https://huggingface.co/ckiplab/albert-tiny-chinese-pos>`_: ``ckiplab/albert-tiny-chinese-pos``
    * `ALBERT Tiny — Named-Entity Recognition <https://huggingface.co/ckiplab/albert-tiny-chinese-ner>`_: ``ckiplab/albert-tiny-chinese-ner``
    * `ALBERT Base — Word Segmentation <https://huggingface.co/ckiplab/albert-base-chinese-ws>`_: ``ckiplab/albert-base-chinese-ws``
@@ -205,14 +206,15 @@
 ================================  ===========  ===========  ========  ==========  =========
 Model                             #Parameters  Perplexity†  WS (F1)‡  POS (ACC)‡  NER (F1)‡
 ================================  ===========  ===========  ========  ==========  =========
 ckiplab/albert-tiny-chinese         4M          4.80        96.66%    94.48%      71.17%
 ckiplab/albert-base-chinese        11M          2.65        97.33%    95.30%      79.47%
 ckiplab/bert-tiny-chinese          12M          8.07        96.98%    95.11%      74.21%
 ckiplab/bert-base-chinese         102M          1.88        97.60%    95.67%      81.18%
+ckiplab/gpt2-tiny-chinese           4M         16.94        --        --          --
 ckiplab/gpt2-base-chinese         102M          8.36        --        --          --
 --------------------------------  -----------  -----------  --------  ----------  ---------
 
 --------------------------------  -----------  -----------  --------  ----------  ---------
 voidful/albert_chinese_tiny         4M         74.93        --        --          --
 voidful/albert_chinese_base        11M         22.34        --        --          --
 bert-base-chinese                 102M          2.53        --        --          --
```

### Comparing `ckip-transformers-0.3.3/setup.py` & `ckip-transformers-0.3.4/setup.py`

 * *Files identical despite different names*

