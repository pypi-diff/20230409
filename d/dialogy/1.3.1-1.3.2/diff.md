# Comparing `tmp/dialogy-1.3.1.tar.gz` & `tmp/dialogy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialogy-1.3.1.tar", max compression
+gzip compressed data, was "dialogy-1.3.2.tar", max compression
```

## Comparing `dialogy-1.3.1.tar` & `dialogy-1.3.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1069 2023-03-31 08:50:13.735186 dialogy-1.3.1/LICENSE.md
--rw-r--r--   0        0        0        0 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/__init__.py
--rw-r--r--   0        0        0      183 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/base/__init__.py
--rw-r--r--   0        0        0     4949 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/base/entity_extractor/__init__.py
--rw-r--r--   0        0        0     9794 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/base/input/__init__.py
--rw-r--r--   0        0        0     4595 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/base/output/__init__.py
--rw-r--r--   0        0        0    15185 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/base/plugin/__init__.py
--rw-r--r--   0        0        0     3908 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/cli/__init__.py
--rw-r--r--   0        0        0     2587 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/cli/project.py
--rw-r--r--   0        0        0     1865 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/cli/workflow.py
--rw-r--r--   0        0        0     4676 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/constants/__init__.py
--rw-r--r--   0        0        0     1203 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/__init__.py
--rw-r--r--   0        0        0     3995 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/address_parser/__init__.py
--rw-r--r--   0        0        0     1406 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/address_parser/mapmyindia.py
--rw-r--r--   0        0        0     4978 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/address_parser/maps.py
--rw-r--r--   0        0        0        0 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/calibration/__init__.py
--rw-r--r--   0        0        0     8825 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/calibration/xgb.py
--rw-r--r--   0        0        0     3746 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/canonicalization/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/classification/__init__.py
--rw-r--r--   0        0        0    11821 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/classification/mlp.py
--rw-r--r--   0        0        0     1142 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/classification/retain_intent.py
--rw-r--r--   0        0        0       58 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/classification/tokenizers.py
--rw-r--r--   0        0        0    13953 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/classification/xlmr.py
--rw-r--r--   0        0        0     7633 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/combine_date_time/__init__.py
--rw-r--r--   0        0        0    39284 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/duckling_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/error_recovery/__init__.py
--rw-r--r--   0        0        0    20312 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/error_recovery/error_recovery.py
--rw-r--r--   0        0        0    12300 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/intent_entity_mutator/__init__.py
--rw-r--r--   0        0        0      744 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
--rw-r--r--   0        0        0      797 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/intent_entity_mutator/const.py
--rw-r--r--   0        0        0      313 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/intent_entity_mutator/registry.py
--rw-r--r--   0        0        0     1740 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/lb_plugin/__init__.py
--rw-r--r--   0        0        0    14080 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/list_entity_plugin/__init__.py
--rw-r--r--   0        0        0    11480 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/list_search_plugin/__init__.py
--rw-r--r--   0        0        0     4841 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/list_search_plugin/sample_config.yaml
--rw-r--r--   0        0        0     4656 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/merge_asr_output/__init__.py
--rw-r--r--   0        0        0     1565 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/oos_filter/__init__.py
--rw-r--r--   0        0        0     4204 2023-03-31 08:50:13.735186 dialogy-1.3.1/dialogy/plugins/text/qc_plugin/__init__.py
--rw-r--r--   0        0        0      833 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/plugins/text/slot_filler/__init__.py
--rw-r--r--   0        0        0     4111 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/plugins/text/slot_filler/rule_slot_filler.py
--rw-r--r--   0        0        0        0 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/plugins/text/voting/__init__.py
--rw-r--r--   0        0        0     1862 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/__init__.py
--rw-r--r--   0        0        0      170 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/__init__.py
--rw-r--r--   0        0        0      914 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/address/__init__.py
--rw-r--r--   0        0        0     1811 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/amount_of_money/__init__.py
--rw-r--r--   0        0        0     7163 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/base_entity/__init__.py
--rw-r--r--   0        0        0     2264 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/credit_card_number/__init__.py
--rw-r--r--   0        0        0     3637 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/deserialize/__init__.py
--rw-r--r--   0        0        0     4317 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/duration/__init__.py
--rw-r--r--   0        0        0      601 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/keyword/__init__.py
--rw-r--r--   0        0        0     4698 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/numerical/__init__.py
--rw-r--r--   0        0        0     2271 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/people/__init__.py
--rw-r--r--   0        0        0      910 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/pincode/__init__.py
--rw-r--r--   0        0        0    13534 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/time/__init__.py
--rw-r--r--   0        0        0     8803 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/entity/time_interval/__init__.py
--rw-r--r--   0        0        0     8893 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/intent/__init__.py
--rw-r--r--   0        0        0      154 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/signal/__init__.py
--rw-r--r--   0        0        0      194 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/signal/signal.py
--rw-r--r--   0        0        0      991 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/slots/__init__.py
--rw-r--r--   0        0        0      191 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/types/utterances/__init__.py
--rw-r--r--   0        0        0      638 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/utils/__init__.py
--rw-r--r--   0        0        0     2180 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/utils/datetime.py
--rw-r--r--   0        0        0     3437 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/utils/file_handler.py
--rw-r--r--   0        0        0      808 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/utils/logger.py
--rw-r--r--   0        0        0     2687 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/utils/misc.py
--rw-r--r--   0        0        0      584 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/utils/naive_lang_detect.py
--rw-r--r--   0        0        0     8236 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/utils/normalize_utterance.py
--rw-r--r--   0        0        0     3605 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/utils/temperature_scaling.py
--rw-r--r--   0        0        0       47 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/workflow/__init__.py
--rw-r--r--   0        0        0     6795 2023-03-31 08:50:13.739186 dialogy-1.3.1/dialogy/workflow/workflow.py
--rw-r--r--   0        0        0     1400 2023-03-31 08:50:33.843249 dialogy-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 dialogy-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-05 07:41:49.636805 dialogy-1.3.2/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/__init__.py
+-rw-r--r--   0        0        0      183 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/base/__init__.py
+-rw-r--r--   0        0        0     4949 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/base/entity_extractor/__init__.py
+-rw-r--r--   0        0        0     9794 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/base/input/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/base/output/__init__.py
+-rw-r--r--   0        0        0    15185 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/base/plugin/__init__.py
+-rw-r--r--   0        0        0     3908 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/cli/__init__.py
+-rw-r--r--   0        0        0     2587 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/cli/project.py
+-rw-r--r--   0        0        0     1865 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/cli/workflow.py
+-rw-r--r--   0        0        0     4676 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/constants/__init__.py
+-rw-r--r--   0        0        0     1203 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/__init__.py
+-rw-r--r--   0        0        0     3995 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/address_parser/__init__.py
+-rw-r--r--   0        0        0     1406 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/address_parser/mapmyindia.py
+-rw-r--r--   0        0        0     4978 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/address_parser/maps.py
+-rw-r--r--   0        0        0        0 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/calibration/__init__.py
+-rw-r--r--   0        0        0     8825 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/calibration/xgb.py
+-rw-r--r--   0        0        0     3746 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/canonicalization/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/classification/__init__.py
+-rw-r--r--   0        0        0    11821 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/classification/mlp.py
+-rw-r--r--   0        0        0     1142 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/classification/retain_intent.py
+-rw-r--r--   0        0        0       58 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/classification/tokenizers.py
+-rw-r--r--   0        0        0    13953 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/classification/xlmr.py
+-rw-r--r--   0        0        0     7633 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/combine_date_time/__init__.py
+-rw-r--r--   0        0        0    39284 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/duckling_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/error_recovery/__init__.py
+-rw-r--r--   0        0        0    20312 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/error_recovery/error_recovery.py
+-rw-r--r--   0        0        0    12300 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/intent_entity_mutator/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
+-rw-r--r--   0        0        0      797 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/intent_entity_mutator/const.py
+-rw-r--r--   0        0        0      313 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/intent_entity_mutator/registry.py
+-rw-r--r--   0        0        0     1740 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/lb_plugin/__init__.py
+-rw-r--r--   0        0        0    14080 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/list_entity_plugin/__init__.py
+-rw-r--r--   0        0        0    11480 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/list_search_plugin/__init__.py
+-rw-r--r--   0        0        0     4841 2023-04-05 07:41:49.636805 dialogy-1.3.2/dialogy/plugins/text/list_search_plugin/sample_config.yaml
+-rw-r--r--   0        0        0     4656 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/plugins/text/merge_asr_output/__init__.py
+-rw-r--r--   0        0        0     1565 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/plugins/text/oos_filter/__init__.py
+-rw-r--r--   0        0        0     4204 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/plugins/text/qc_plugin/__init__.py
+-rw-r--r--   0        0        0      833 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/plugins/text/slot_filler/__init__.py
+-rw-r--r--   0        0        0     4111 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/plugins/text/slot_filler/rule_slot_filler.py
+-rw-r--r--   0        0        0        0 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/plugins/text/voting/__init__.py
+-rw-r--r--   0        0        0     1862 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/__init__.py
+-rw-r--r--   0        0        0      914 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/address/__init__.py
+-rw-r--r--   0        0        0     1811 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/amount_of_money/__init__.py
+-rw-r--r--   0        0        0     7163 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/base_entity/__init__.py
+-rw-r--r--   0        0        0     2264 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/credit_card_number/__init__.py
+-rw-r--r--   0        0        0     3637 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/deserialize/__init__.py
+-rw-r--r--   0        0        0     4317 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/duration/__init__.py
+-rw-r--r--   0        0        0      601 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/keyword/__init__.py
+-rw-r--r--   0        0        0     4698 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/numerical/__init__.py
+-rw-r--r--   0        0        0     2271 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/people/__init__.py
+-rw-r--r--   0        0        0      910 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/pincode/__init__.py
+-rw-r--r--   0        0        0    13534 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/time/__init__.py
+-rw-r--r--   0        0        0     8803 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/entity/time_interval/__init__.py
+-rw-r--r--   0        0        0     8893 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/intent/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/signal/__init__.py
+-rw-r--r--   0        0        0      194 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/signal/signal.py
+-rw-r--r--   0        0        0      991 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/slots/__init__.py
+-rw-r--r--   0        0        0      191 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/types/utterances/__init__.py
+-rw-r--r--   0        0        0      638 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/utils/__init__.py
+-rw-r--r--   0        0        0     2180 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/utils/datetime.py
+-rw-r--r--   0        0        0     3437 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/utils/file_handler.py
+-rw-r--r--   0        0        0      808 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/utils/logger.py
+-rw-r--r--   0        0        0     2687 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/utils/misc.py
+-rw-r--r--   0        0        0      584 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/utils/naive_lang_detect.py
+-rw-r--r--   0        0        0     8236 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/utils/normalize_utterance.py
+-rw-r--r--   0        0        0     3605 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/utils/temperature_scaling.py
+-rw-r--r--   0        0        0       47 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/workflow/__init__.py
+-rw-r--r--   0        0        0     6795 2023-04-05 07:41:49.640805 dialogy-1.3.2/dialogy/workflow/workflow.py
+-rw-r--r--   0        0        0     1400 2023-04-05 07:42:07.269000 dialogy-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 dialogy-1.3.2/PKG-INFO
```

### Comparing `dialogy-1.3.1/LICENSE.md` & `dialogy-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/base/entity_extractor/__init__.py` & `dialogy-1.3.2/dialogy/base/entity_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/base/input/__init__.py` & `dialogy-1.3.2/dialogy/base/input/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/base/output/__init__.py` & `dialogy-1.3.2/dialogy/base/output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/base/plugin/__init__.py` & `dialogy-1.3.2/dialogy/base/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/cli/__init__.py` & `dialogy-1.3.2/dialogy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/cli/project.py` & `dialogy-1.3.2/dialogy/cli/project.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/cli/workflow.py` & `dialogy-1.3.2/dialogy/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/constants/__init__.py` & `dialogy-1.3.2/dialogy/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/__init__.py` & `dialogy-1.3.2/dialogy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/address_parser/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/address_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/address_parser/mapmyindia.py` & `dialogy-1.3.2/dialogy/plugins/text/address_parser/mapmyindia.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/address_parser/maps.py` & `dialogy-1.3.2/dialogy/plugins/text/address_parser/maps.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/calibration/xgb.py` & `dialogy-1.3.2/dialogy/plugins/text/calibration/xgb.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/canonicalization/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/canonicalization/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/classification/mlp.py` & `dialogy-1.3.2/dialogy/plugins/text/classification/mlp.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/classification/retain_intent.py` & `dialogy-1.3.2/dialogy/plugins/text/classification/retain_intent.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/classification/xlmr.py` & `dialogy-1.3.2/dialogy/plugins/text/classification/xlmr.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/combine_date_time/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/combine_date_time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/duckling_plugin/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/duckling_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/error_recovery/error_recovery.py` & `dialogy-1.3.2/dialogy/plugins/text/error_recovery/error_recovery.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/intent_entity_mutator/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/intent_entity_mutator/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py` & `dialogy-1.3.2/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     ) > 0.5:  # consider it as a number only if a number is present in more than 50% of the transcripts
         return False
     return True
 
 
 def contain_digits(ner_input: List[str], threshold: int = 5) -> bool:
     first_alternative = ner_input[0]
-    return sum(c.isdigit() for c in first_alternative) >= threshold
+    return sum(c.isdigit() for c in first_alternative) < threshold
```

### Comparing `dialogy-1.3.1/dialogy/plugins/text/intent_entity_mutator/const.py` & `dialogy-1.3.2/dialogy/plugins/text/intent_entity_mutator/const.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/lb_plugin/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/lb_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/list_entity_plugin/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/list_entity_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/list_search_plugin/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/list_search_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/list_search_plugin/sample_config.yaml` & `dialogy-1.3.2/dialogy/plugins/text/list_search_plugin/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/merge_asr_output/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/merge_asr_output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/oos_filter/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/oos_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/qc_plugin/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/qc_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/slot_filler/__init__.py` & `dialogy-1.3.2/dialogy/plugins/text/slot_filler/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/plugins/text/slot_filler/rule_slot_filler.py` & `dialogy-1.3.2/dialogy/plugins/text/slot_filler/rule_slot_filler.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/__init__.py` & `dialogy-1.3.2/dialogy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/address/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/address/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/amount_of_money/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/amount_of_money/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/base_entity/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/base_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/credit_card_number/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/credit_card_number/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/deserialize/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/deserialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/duration/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/keyword/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/numerical/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/people/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/people/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/pincode/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/pincode/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/time/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/entity/time_interval/__init__.py` & `dialogy-1.3.2/dialogy/types/entity/time_interval/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/intent/__init__.py` & `dialogy-1.3.2/dialogy/types/intent/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/types/slots/__init__.py` & `dialogy-1.3.2/dialogy/types/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/utils/__init__.py` & `dialogy-1.3.2/dialogy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/utils/datetime.py` & `dialogy-1.3.2/dialogy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/utils/file_handler.py` & `dialogy-1.3.2/dialogy/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/utils/logger.py` & `dialogy-1.3.2/dialogy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/utils/misc.py` & `dialogy-1.3.2/dialogy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/utils/naive_lang_detect.py` & `dialogy-1.3.2/dialogy/utils/naive_lang_detect.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/utils/normalize_utterance.py` & `dialogy-1.3.2/dialogy/utils/normalize_utterance.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/utils/temperature_scaling.py` & `dialogy-1.3.2/dialogy/utils/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/dialogy/workflow/workflow.py` & `dialogy-1.3.2/dialogy/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.3.1/pyproject.toml` & `dialogy-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialogy"
-version = "1.3.1"
+version = "1.3.2"
 description = "Dialogy is a library for building and managing SLU applications."
 authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/skit-ai/dialogy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `dialogy-1.3.1/PKG-INFO` & `dialogy-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialogy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Dialogy is a library for building and managing SLU applications.
 Home-page: https://github.com/skit-ai/dialogy
 License: MIT
 Author: Amresh Venugopal
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

